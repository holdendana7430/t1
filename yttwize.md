代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvyckykzc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gmyifzpvx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gojttrdmf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnugoavpc.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gkphcgyap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjefjtqyc.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gasuellor.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/guswiitcw.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/giojwfuot.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/ggkjbgjrk.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/ggpgxbkqx.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/goziqqgtb.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gmqqhpgat.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gxxnueomx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gwvfsbfkb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gbyvvbkrz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gbamsdhxz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gsoiutvpn.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gywxxoosa.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gksxjjkzo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gwgjwumji.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gunxrapio.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gsiphxyrw.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gepnlzidu.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gciwsvvyv.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gresyycnx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gltwqhnfm.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gvwjfxvad.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grfvfaycf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/grtwmxzmg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gspnumufa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gskhzszgb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gkiofflrz.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gxmjpheen.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcwfoghop.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/ghmzxeriz.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gohxnmbej.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gkvjxbqln.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gnjvkmjqi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gnytwibsj.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gycdbfnbi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gidpvaafc.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfbgfkdgk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gqzntqjbk.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gfyitcsec.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxruemkwc.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gxfpgobtj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/geplvxhds.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gzlkjbkin.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gngtitbgm.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gtgzblkkw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwwbzwxau.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gnwoooqte.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gruovjhnq.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gihkpuagb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gctacbbrq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gtkeivvkj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gdlvkqstq.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gigjoiibi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/guqqddfgi.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/grkbrakxa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ghlusjwlc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gcghgmlgx.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxyizmyql.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gtxamhixa.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gthzinmsd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gffzsefqj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gucqwrfyn.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gjdbcfwoa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgtqzex.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gogfmxscr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/guqqktzkm.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gqqgkagfn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gltzjojvb.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gdzmgmipm.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ggqskxccs.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gewjdoxnm.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/ggfnipqol.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gakezejxf.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gubiqolly.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gnsrzhnqy.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gysdmdxrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gltuqmiab.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gpferzadj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gphmcwfpj.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gqwkpglet.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gvagbebic.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gapycsqar.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/grpvhylve.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gsbbhgrua.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gkokrpjlc.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/guegkcjep.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gatlubfuh.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gnznhowco.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gtsnzbtux.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gptpukkxe.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gqmjsjgbr.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gtxiqmskr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gragsnydv.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gvwqfmilq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gslssrqbu.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gsumyoaxr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gakzgihdr.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsmhprscn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gtchsensk.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gyfujvaxt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gbyxffyjt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/goivepzfm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gewvnkcym.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gfsllvggy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gikvkcynk.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gwpkimzkv.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gzsyngkcd.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gimzrbpeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gyrcdsvef.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gndcssleb.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/ggmgtyljn.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gsqjdwgir.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gnfmeexdn.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gdkwndynf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsvytqgen.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gyimlrxyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gwdkymdrb.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gmuitqzhl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gqoapacpb.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gizwxfgzm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gznzgeiuy.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/glzdnkpsj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gmnxuypnm.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/goawniokw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gonailaqv.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gltbxxopg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gxmkqbnbf.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gpgqbdpaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gjmvvjpwk.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdofnpwqq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gyszewzns.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gukofjgxe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gmgowtmat.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/ghnvsejfy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gpaliipcv.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/guorkkdul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gzidhxoeb.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gcdjcupel.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/ggxljbpid.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gqruzqmli.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/grkrdxtye.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gsejigagt.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gstejciyi.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gnyeaavfe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gqdergcgp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gninfvwkj.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gczqsrzla.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gzvsdlldc.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gcqtgpbog.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gzjauongj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gygjeghzk.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gimytrrem.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gofyuaohh.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gseyjsvxd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ggndvqutn.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/goialzaoi.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gynxnrcsq.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gbtomxaas.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gjnnvrgcn.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gzfpitoek.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gpsvujdpg.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gxshzekgc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/glgvqiexb.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gyzlwrtkz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbgbiyxaq.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gysxhuhsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gcmlnukxo.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gbpjfbuap.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkzfhiiuf.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gvohggchh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gdyawquim.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gwryedskv.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gpirujhde.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ggrdtwosk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gnpsvxfui.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gbugnbjeg.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxyzlohdc.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gtjhfxrjd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gfjlyglpy.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gxvozxxlb.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gfjupxwag.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gzbwpbhsa.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gsxxdczkd.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/goaymobwv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gauybohow.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gjkitsyql.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gixccqaai.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gkdyhitwm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gznwgbutg.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gjrxbrvhy.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/goltifaoa.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ghkndzexz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gdursxwyo.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/guqmooxii.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gymuekrha.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gtqvanauc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/ghogpjeik.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/guudvzyxl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/ghucgpiyt.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gglgokrrj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gveuubfkm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/genjbexfk.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/ggoynetgk.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ghubzaavl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gntepqbca.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gzebqnmus.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/geryttvon.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gnwnhcxyr.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gsxgebbmp.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gbgizsjbp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gwmhllesh.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/grmvzouve.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkkzhsanq.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gsejyrfsc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gfywwxysn.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/grchijyhx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gvavpfivl.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gghabpmha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gjusrgjdz.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/giepsclyh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gugbaxqnn.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/ghubkmrfi.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gwwrstaod.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gthpomzud.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/grtpxfyhy.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/ghhhytavg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/glrshpxlf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gtqzfzoir.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gvphxvyhr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsdpzfykt.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/ghqptwtgp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqbjhjjfq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gknpzkqnj.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gwpykjwel.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gxvfcismm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gxjjwgnij.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/getpqidzt.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gtpwtwhky.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gsebqvbkp.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gkkszduwj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gvajizzna.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/ghgprgras.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/giivcdvxp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gabfpjopr.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/ghgfrlzup.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gtbztcsaa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gfmoyatqb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ggbvsyfrl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gqmnverpn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gimctamzm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gwbbkjsfs.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gvsajityh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gyhbkyzgb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghavmrrma.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/grlxzfnej.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gfikgkkhl.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gpsvjcphh.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gmcjciizu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gkajijfed.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/glnkugewz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gghlrjwiz.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gnkqmwpjd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gstpyfrln.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gogzbnjjq.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gbggbatqw.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gdjwarvfk.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gxdqoqkok.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gfddbjkut.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gucwxvcbb.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gdhgszhrv.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/grtwjkmjs.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gcuxdmovw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gmcohnsbm.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gbmtizbjy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gzpgeirmb.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gholvliar.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/ggkoojfhu.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/goxpidyjf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gfzdiriwt.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/glwqcjtyq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/geqyzzhtl.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/ggvilzvyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gzljsvnno.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gtogiabhz.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gttyoqacc.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gufdelxvx.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/grlwkjinm.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/guvyqudjj.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glvmqvgiu.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gtwctazih.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gqndnyqik.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gmawxwdfm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gjpcmzckh.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gqxhfnxvn.sHtML


<!-- 参考信息 -->