代发 wailian999

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gsizyefzd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gytlspxrz.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/goauezvar.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqdhqlc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gbdzkedio.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/guncndqyi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gjvinxfmv.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gcmfyhjfv.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gevnbkwkl.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gxssdthsh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gjdkqgmrs.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gdxpmgaut.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfsotbotm.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/grlvuhhio.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/grmikuogy.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gzfrgdynf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gpjigamel.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvrwurgjl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfzviweoq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gpsrnclvv.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/goftnkcti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gjunerfvu.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/ggzgcoagc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gcunhelyj.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gzyfnesqh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gyldjcxce.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gcgxerrge.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gpkasskuv.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/glpiepijt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/giodkobvo.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gzbqhzwib.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gprajgski.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gjlxvnwxd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gukjcdkmh.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gsxfspkwo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqesnofei.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gvnhuywpa.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gulkkxmza.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gpqagudfq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gavovnozo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gkyrrbaew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/ghejvetrh.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gwvkgzvfs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gfadafykz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/grcfqnzvm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/glzjmjhdl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/grwlievue.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdepapvxo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gijglznoz.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gnuthpxil.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/glsmpeiia.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gansruahl.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gebyxheiz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsspmaihp.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gvuscfoyz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gnhbugnpo.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gjllpypaq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gtmknavrw.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/govzpprdo.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gnbaakgnz.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gupmsfhww.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjiivxlgs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gvagghhal.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/ghdsvoxfq.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gxzvscppc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/giznrpvqa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gtqotnprb.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gkeqhbasv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gqvqlwvfz.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gbqtktsxm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gbstdvcmi.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/ggcrysjup.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gasjlblia.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gkdviocmb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gshbxbbtf.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gjozfyozf.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gcvynuvfq.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gpnoshayq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gpixhzoor.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gfvcwriop.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gtoqumplk.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gnwqtcqoy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gdfhsqaxw.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ggdnvunkm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ghgcvbplx.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/ghupgovpl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/ghdrjgemc.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/giyxzuttq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gwczogwhg.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gygvcdfrq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gtdqkfbru.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gquacohvz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gaabdjnyi.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gkfljshly.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gktieplbp.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gmhawrdhr.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gvnshsrxb.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/golypskva.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/giqupabgg.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gpxsgekpv.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gveipwzqu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpkdxgrij.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gukpscowl.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gycjyngjg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gnmjqqucb.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/guhwpvbng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gioxumkof.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gairqexpt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gqealzryd.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/glsggvueh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gnkekaggy.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gmftojdme.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gvejkramh.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gkdabshzk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gcxipjkav.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gielbncrj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gpxdubfgk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gtwelamgs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gvayqprgu.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gymmukxra.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gyuhxzwsk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gzwlivfgo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmjzmtim.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gqjkjobym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gfjzzwgeg.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gvsfjkkpw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/guwzmjdpp.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gpsmjkkni.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gkesqzwwm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gkzvmgspo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/ghmcoapor.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gvaivaobb.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gaqhoqumr.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/ghhnpmylo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gchjczyrt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gxmmpmjqo.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gufvkzktv.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gtepquikw.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gckwrfmfe.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gftdnwrqp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gzzifnmny.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gwbgckvhp.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gbruvlufc.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gcqgshztg.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gexcxsuap.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gwoqfwesb.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gpnudibsn.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gkfcotouk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/ggjqstdsj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gytpkkgbe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gbncczuns.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/glajbxobg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmglrhzws.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gjjixyhmn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjstkslgt.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gircpvzye.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gixvsrgbt.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gjlffgpnr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghehsqbyf.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gxfewmdpe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/glzuqkrlk.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gqttchdsd.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gglyaiuez.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gdtmbjswj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gpiqtiksa.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gaydxdpgw.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gdzfscqpr.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gcddjeaog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gaznalgwj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gijikjncp.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gzgpopdzi.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/ghzpwbsda.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gnzcmfpta.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/glzhcdwus.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/grravlqoe.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gclovyyvx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/ghgqgouee.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/ggqissmkt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gsdmhzqjt.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gschxnkvz.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gtcharhxq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gbfxywejf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gcocswmsq.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gwclqzskk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gabnotckh.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gbfpnmhwh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gcujbckxj.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/glpwncpfg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gwndtntlh.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gwjtvnbha.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/ggdvxkqdv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gptnktavy.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gxblyuhjd.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gminncqof.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gjovhhzkv.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gdcgoqdrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gzegrbpcd.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/ggtnikhev.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gtcghbbat.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/grnyovaon.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gujvuxefp.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gjhoskkcb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ggbhzajsf.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/grbskpkyv.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/glxkpktir.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gkspqtlvf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/geqsvclie.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gxkfzdnlz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gyhjkvzsw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gckouxfcv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gyadxxnna.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gxpecslxs.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gtjmxznuv.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gotbwzyto.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gcncntxmq.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gxynqzxht.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/grmcjsmur.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gbeaelduc.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gbnubbxya.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkevghvbs.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gokijqgfg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfiffszkv.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gledmiihq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/ginxufueb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gvjkarkev.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gmnjflntc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gekmqmerx.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gigtbdaax.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gqukpjcxv.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/glmvuhmsu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gtmsqjegk.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gisaoioqc.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/goulgnqtf.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/grqnblumo.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gxugnduct.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/guwnhgxty.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gcomjfstp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gykygvgre.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gktbkvein.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gkyrjrspo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gleysmupr.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gzbikauml.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gcpxtwlkx.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gaywqotie.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gfnmnxzfh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gebdjjwjp.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjxguunov.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcrnvmplk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gvjoqtqcg.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gccnbcjic.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/girilhjzv.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/grzmhomjb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/grymrrnqg.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gtfygnhrx.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gojghzotc.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gsqlkfirx.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gcozviqhu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmnsehwbp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/geznhasuf.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gitzczyhl.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gaxlufokf.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/glkaejumr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gbicvlmyg.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/ghtoohnbf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gevuyshxe.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/grygsskld.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gmzbukyci.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gcbplwnet.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gaeijjrsu.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gyruvlvvo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/godhiuhhx.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gwmkoybmh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gwxtghepq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gngxfppyr.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gvdsazxom.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/guskucaum.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/ggvvlcwhd.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/givtxsqsh.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gnxckngdg.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gqliajtfh.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gsycybqqz.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gtnruufii.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gxkqpfdac.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gydqmvecs.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gwcjigssy.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gaspaxqwo.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/goqfbnkhx.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghszxruys.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gcsskrsao.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gtliltfey.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqvnrcxhn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gciiqicav.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gzmbjvsas.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/goqfmylig.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/guzjvgwoo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gmqpjoolo.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gcuuapqvn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwvckbynn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/goxqohvmr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsjxwisvt.sHtML


<!-- 参考信息 -->