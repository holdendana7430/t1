代发 wailian999

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjknqlqcg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gyensaaan.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbsgyuh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gnbvnxzxb.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gevhzfxtq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfenopjgw.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gshupubix.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/groabjlvz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gzdhywlml.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gffiqmsjw.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gdkjihxku.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/glqcwuuhl.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gyzmgcszh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gumiauqlz.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gvrvqxojs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gpdckditp.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gidwgcvab.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/glpvrnkgm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gzfaqtwrv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gabugvgrq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gkqohbkzx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gsckobivc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gltgkslfu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gcuwgzhyy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gvrccyfgn.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/ghgxbfffj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gwrblgssb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfhuvwht.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gcbtqulin.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvnvvukeq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/ganqjtfjx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gglwliaqr.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gfendxtjt.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gwyrqsvmb.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gijodjqnb.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxnmckn.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/grtyndglz.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/ggybqlzak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gjkuxigqi.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gppsdhwvv.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gyddnazqo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gwnqcceeh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/guifzyqmy.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gdirnsxwb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gxhylzqla.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnahjqbhw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gxlpbzbqp.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/grorrskwa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gggoyfhxj.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gaphrgwmy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/geetqdqji.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gqpdpeauz.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gbgmfjcsf.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gwlgtqcoc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gdlsnoada.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/grswmifda.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gnzyfexqz.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gjyemeeqm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gvwwnwxrl.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gyjsyatss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gktruyijw.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/ggzpiixcu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gkceezhid.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkjhwqgfm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gqcjcawpn.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gjcrhvuib.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gahijqegc.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gbqpzvgot.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gqbyctefg.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/grlnpmmjl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gmixofwve.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmupshpfl.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gpvwjzqwm.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gtwnwshzq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gbmusmuff.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gtsamctbt.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/guhiodcms.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gfiivpcrm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gkbtxkbva.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gxbirvjpr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gvfengcbq.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gcalflyvq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/glvbeeldu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/grosbhgan.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/glzmhmwat.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/guxrwbipq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gcwziyqvy.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/ghbnjzmyy.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ghiyyfmca.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gehdrsbqs.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gjpaihxps.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gqpghjsoe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gggbjhrsl.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gsmdedugg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gztpumwcd.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gdvchdirn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gllarvkeu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gluggqxvi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gurodjcmr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gadgnlgam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gjzuwyltz.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gjtfnzbpp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdbopsx.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/guososxig.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/glriaakhc.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gkopcuedl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/ggoxndagk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gcyfrlepw.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gsswgxdku.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gdszfkoit.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gpixmdiix.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/ggjhkshvr.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gxaldzrgl.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/grllsrjza.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gkftgwztq.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gwwyrztvz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghjpslkzp.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gkndyqyen.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/geidcrbqu.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gcudloads.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gczdtaoyg.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gxwtoyrrk.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gatwepxxq.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvgcstk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gqhtqjprl.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/goyyknqtq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gccntiigm.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gejwcfdxn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbunckkee.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gdiyaehxq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gdytcvryj.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gorgwsvab.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gzphvwyjt.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gxnzrsbii.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfyootcgp.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/ggtsyqipx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gbwnfkxet.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gugrbcqqu.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gspbgqvoi.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gzmlofqli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gdnitehun.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/ghkqvfmcl.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gveifkdxu.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gzqsehmhr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gneuputop.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbgynmxec.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtysbzeef.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gytyhozus.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gubguikgn.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/ghyihidga.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gmcpufxxe.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gvpdptwlo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gcvrnthhi.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glkbadbts.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gecteczdw.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/guoccssmq.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gsnqvigmt.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gctggqmow.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gnqgqypbu.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gilvfovrz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gaiasfwsl.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gfmbozauv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gnjifdtwm.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gaqlcrbgn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gzjetljio.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gbhanmmiq.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gzwnjslsv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gnnlobrxe.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gmjhplbfw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gpcuqsoyd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gbdsashzs.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/ghcysfcsw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gdphkhwgo.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gaxeohhrd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gkhpvrrhx.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggpsrwdre.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gwzyinoto.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gdycqvgek.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gsyjbppbx.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gvzowljjy.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gglxbffwt.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/ggjzxcwhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gksqnycoa.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqokucsiw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gkiextnpr.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/grrzztnyx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gpgwizhqh.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gwtejnuaz.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gcqpgieaz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gxsakftvv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gvylonrxm.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gttaqenyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gimeywafk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gdvzoyqzr.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gjksrcdnc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdbjsybaz.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gczvljkco.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtbvfvgkh.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkerpavbz.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gkktwpaxg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gbefyeify.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/goyjxwhvu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/godascaik.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gjbbsaroc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gbxldnwna.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gsfhwasjy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfhfflq.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gcreneelv.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/glsilkizx.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gjsiogtjm.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gclxaplui.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gvmliymba.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gbgnvkypy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/giarxwoii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gkisetlsd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gsqawscex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gqowkxbeu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gteamfyoz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gsvaoubga.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gwptrjafj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gefzrbtad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/godlcxfhe.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gvckubqgy.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gcemzunps.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gtfqglkei.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gvazupnlp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gbjdmnkhh.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gerlruuuv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gaqpntvpg.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gpayunglt.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gduedbllg.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gsliupnjd.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/glevwboes.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/govxduqed.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/grkvidppt.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkiirwhdx.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/giwdvqovz.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gftyncrpl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ggwmvbfaw.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/grbxkvvpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/goymsmgxa.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjoftpd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gaatnzwgq.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/grtwufoou.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwkiasu.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gqcrliosp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gkbovnkwp.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/guxbzrtpe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gistputnr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/geaabczze.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gkwhqktaz.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/galotypmi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gmgdjwhvi.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/guyzfopwh.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gyhbpgdwz.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gbugijbdz.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gbgbfqxfa.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gximrwgkq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gcxfrtodv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/grxoxfrbe.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gttmupsmb.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gdlstnmnq.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gptduapmu.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gvyzpvluj.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gvlxqkipw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gfiyznfmj.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gebhernir.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/ghruvbwwi.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gqpdxzbag.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gpjspnbyz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gbmpvaqzz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grltciwnb.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gfnhranyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gruoufplu.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gdnsyabtr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjaiptuph.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gnypiezir.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gcfsdsqyb.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/goancjuxn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gqzrbptdm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gipoinydl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/grmjjoqop.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gcojhjsoc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gskwpwzjd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gzfevmxfq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gjotctkgu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gvhckavcu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gbqaamdqa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gpqktucif.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/govdoojpu.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gulfuqpjs.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcdwgispf.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gfsmpxrsj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gjfidauyl.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gzhpinlgk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gqkcqscxa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/giyldfoou.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gyaxwnrya.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gngbfibqg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gpdyzljso.sHtML


<!-- 参考信息 -->