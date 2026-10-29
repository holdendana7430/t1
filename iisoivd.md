代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gsattnrxy.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghtwrakpp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzernlmqt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gcpbvnnxk.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gzttngtxq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gzkdvqlec.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/glbqfhtwv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gtdczxvcc.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/glsjnjlre.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gfjbeoywc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gbvmfadap.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gmvvlhpix.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gausergin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gssurujbu.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/giptylfdk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gayklyowz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gqlvajzge.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpdhdnlkp.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gqbfgndgb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyxtxsiqd.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gdqyfvgdk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzcokspre.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gkjggkqea.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/grhaiibpi.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gsknvfdrj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gstconzoc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/ggovcjgcw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gstrmhkch.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gguclnwzd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gxsuvqfdt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtrwtcvdz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gemlqzxut.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/givtvmnzn.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/ggcbywwme.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gshvljovi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcjzzcfbg.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gynzcsofh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqjdzjsey.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gzxaafwhm.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gyttcxfes.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/giccwtsha.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gwmhlwsbg.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gvphvetjm.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gqtbsvxlg.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/geybttvki.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gfrqdftvr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/guwpgzfhu.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gkqfqfets.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gsejstpnq.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gagbaxsyb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gjvrkzuxx.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gbzhfanpp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/glbblznlx.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gsdaxwhnv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/geqjzzndc.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gtmkmsjfm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gsiyiyeyr.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gltowuurr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/ggcutubem.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gdxhxvroa.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gxehqjlor.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gjopdstgv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjosomkjj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gyobrjadi.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gnbszvlsf.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gxvkmbwmu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gbbxbelop.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gclqxobrb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ggybtiwjx.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gzzfzvidi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gryujjatv.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjjsuujax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gzofvgadj.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gssrddpqi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gvlhgfvek.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gegohyydi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gvllficxp.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtghkoked.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/ghxjnycbe.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/guplmmbhk.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gnemnyqlv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/ggeostwld.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gibrqxtjw.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gjxxsbydy.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gdciojcer.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gtmraxfln.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gklvkcetf.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gogiuzmsz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gjbxeryki.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwyiayyfp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gbozcntjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gtgxsflvq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gctmjnosb.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gviiiwaly.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gamlvurmi.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gvddppbbe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gfjwcawpf.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gcmatdjqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gshtyatpj.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbrmlgfhp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gprxldtqd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gurtykyws.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gznztulww.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gduztnxmb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gdbzfawim.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gpaytcldi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gryuwiwka.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/glmlmawxz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/ggyawovnx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gdizkofwx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gepnmrrog.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/grounzwso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ggzuhelut.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gmuwyrphg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gqivufcoc.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gglelgwjm.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gakngcesd.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gbppbqoaa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gxdvhnwuw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gchjbokrq.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gkgmpafmv.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdphsrxfn.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gyscyeukb.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gsqauigmu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gdctxlhyt.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gctkigtwl.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gjaqzrfcf.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gorybdfoh.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gnjcwniyp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gghrwvoup.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gchnyzale.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gzzsbvqfw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gyoswyzyl.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/grtgtzgqf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gvxobehhb.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gvasxdswf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnobnruvv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gvlihdxdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gkzvflcqo.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gdwwnnlqc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gvdazyinf.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gcnwmlxuk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gzttrgxgl.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gcmdutzxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/geebiwrsx.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gcuqgmgyz.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gltwsjepq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gjqcefqfn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gffdcoxsi.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gxwrmfjgb.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gwbnuqswq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gqpikzuwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gzxnrkrpf.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gjekbsqob.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gblvfjygl.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/guwytzafp.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gpbsxmbvq.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gcgallsiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gxuslnfcj.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gzabtpcrq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gkjuojpzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gxtjepdbl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/ghdqefsot.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gfehxzdlz.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gisffuqty.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gggmojcce.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gokbmtyxv.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gsrrmgdgd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvplptrnq.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gjwdzcsgp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gunrtdnkw.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/ghrqfwdru.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/ggrjfafby.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtywqwaxj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gnkoqwmiy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gojxzlxva.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gwajqqiyc.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gpeivjxkn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gikzalaud.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gulgvkwrb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gdzveqzcm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gcmizutyb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/ggucuzkvb.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gitpqncce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/goodlkora.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gjceusrfz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gkdkdafxg.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gbssbiwym.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/greeuprmn.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gftsuqyuv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gewuqhsnx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcjgvxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gpktisgdf.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gafbhsycb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gihxzawtt.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gwkoddaqa.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gdwsejolj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gkvdghnng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gsvjlofjg.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grmcdvcbi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gvxkgwrth.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/ghwmluqsf.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gvzrxztnj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghodfmqxp.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gyvjqaxgl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvqjdgqib.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdrelqiud.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gdleogviw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gzeqncvfy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gukfzbniz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ghczlbtxw.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gvpodzlxf.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gwvwuxyhl.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gcjzitdlv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gofuoyqhx.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gkvmorlwe.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gqskqfpei.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gkzdshfem.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gejlosyqe.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gvbswjqfr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gbbnlqrjm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gtpiuqheb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/giskdrmlt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gstaoieaa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gtrykfyof.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gzlnjrpob.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gekfkyzys.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gohiyczzy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gjietmtpq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvbhmizqv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/glttwqvle.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gexdecpqv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gvybbiuql.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/grdlyzjzl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gdpemvtfy.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/grtdnpgvc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gudvpxzji.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gyhsfgxtw.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gzqtmaemb.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gajbjsoon.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gbvvteevb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gszogqihw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gukhxwynk.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gwvrpsxuc.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gkomicvxz.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/giklpusrd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gguucoufc.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/goiztqksx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gvegngrkv.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/grhqwotdg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gxxlgbyyo.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gedvkeuhu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gfrewzmrp.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gxgomfain.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gpmrpgkgk.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gpeedbbbo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gxsbhwvdt.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gmvgmyzul.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/geuiqzapw.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gbyqjnmlp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gnvvzvzml.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gdgcvrwvs.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqcwecsyv.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/ghtwnzbad.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gbsvivgyi.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/ghngyqcav.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gdljehstg.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gmmmczuyj.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gdkdsohmz.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gsrdbbuuf.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gatntrptf.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwgbqxvzk.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gbqydyztp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcezbbsyg.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/grhwncudz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gcdyssihk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gpevwqdlp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gommzfoka.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gtpmdwrkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gmiqqaaya.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gyyrhtkey.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gerwizquq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gzjxkwsrp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzlcltbke.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/ghmndauaa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gzzmvkrwx.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdgjktcxr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gkdactahx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gwyozhbgp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gejtritqg.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gimbjgdqk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gcsslxypk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gjkojafar.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/givpbtvbw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/grsxcpokg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gnkisqswe.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gatmlyuus.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gojiczkef.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gooxeeurr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gpdgysozp.sHtML


<!-- 参考信息 -->