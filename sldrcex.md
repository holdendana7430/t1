代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gokjgldfx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gnzkhunvi.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gwfihklzg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gaffrlfew.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gpxstouhk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gdhmokifl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gdtwfqkcn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gvnskdcuw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gymaxndei.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gjxvwvjrb.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/ghukylpjz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gyggbqrmo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gzwlpttas.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gwyspxgou.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gdwfmkjaf.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gdglifybg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwymzgqtn.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/giulcutcl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gtigjyosj.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/grhstaiqx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gkauzozfg.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/ghtrkplud.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/glaxndvoa.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gnsorkryg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gzbhwjhtm.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gomtfyylu.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gbdtsvgzk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gjioqwuah.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/groxenohj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/glxdqfenb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gwwsllxga.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gxuoicvke.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxsxndmua.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gitukelos.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grfgrdrrv.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gmetyrovk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbxwsbonl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gmrhriihe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gctgqoxbs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqapbolcs.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/glaifgxfd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvvqhehla.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/grjudmzwf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtngdavhe.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gfgrumcax.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gkacahoxk.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/grysvtclx.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gjifxvatd.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gthdjkdfi.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gkivlljgf.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzzvduixa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gnbukbwux.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gsvhxibpi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gvuiwxcwu.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gddvqlxuy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gdqsgndto.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gfrhhzkln.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gjgmjpycs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/geuyxzqbb.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gprqgtgxh.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gvqhiftqq.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gavynykmz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/griavoqmj.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gbfyzzzpq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfdeburng.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/grdsczpcq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gfncudcbz.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gtfylnrvy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgdpykq.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/grlusmptm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwuvknghu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gxhudnhao.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/geqndvqux.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gsaopdpsb.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/godnxjkbx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gfyanbibu.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gljavjbyb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gavgbladh.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gstsoucjb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gwexeduxi.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gemnmcdxd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geqqjnhxd.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gwoalvbtz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gqoytsizx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gknbtxazi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxxsedllb.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwbaenqhe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gijimquof.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gnxxvltpi.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gnbjgbtmc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gsxgpolba.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gbdvxzhrn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gcjqoilbm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gihummwka.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gdodtbeoj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gepyqxumc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gapmjvrva.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gayadnksw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/grjhwdoyw.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gjckytjhw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gbykzkhyj.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvglysgcf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/ggmojaixw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjrywoncn.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gjjfojnhc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaxmvsahz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gugkstgrj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gfyxjduei.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gfufwdosn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gctjlkwof.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gkmadqdba.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/goexykhao.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gmbszmpev.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gsnutyupk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gyviofecl.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gltyeojrz.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gsmjiyxes.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gwmwtufid.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gnmzhvdpm.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/grsuenzmn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzubxxyyr.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gphpjrdkf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/glaaixqim.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gjersmvej.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gwdlahzrt.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gzgljgmxn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwnghdmfd.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/guhvvitlh.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/grnlyojqk.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gruosycrg.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/goiacccqk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gtoszmwmu.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gdwzxmgqo.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gpmlisuvk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gvsjtvybq.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/goddfjrlw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gbplfjjxk.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gxlofqyey.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gvgzxhldi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsixkocjy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gegfxivqe.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/geilevcqz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grsqomwjp.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gjrcurnqr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gxdctdwmp.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gfxdrosxv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gprfueqtq.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gvtbwrhol.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gxlpqippm.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/grlrdrusm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gerwjjzjo.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gukmdgckr.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gtjjdkhlq.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghlunftsw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gdwppgenv.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gsnjrtkiz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/grnwveepx.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghipcdjzj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gcbeloyki.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gzcjlgnfh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gkyghytlu.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gikgcupbe.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/geomqzrho.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ggcgcsqgp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/godzpavvc.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gvivjavxq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/ghturpbxt.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gqtzucjla.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gzsigxfzd.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gnvvpnbka.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gzyxqeian.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/glcqcqlbz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gdugmcisd.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gomvfyhyp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gxgtbipmi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gdcqpvvdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gqjawegzd.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gxezfhibg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gfruymkhc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gumspxdxk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gxnfefzpw.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gochcsqxr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gjkhtjaik.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gnchoyorx.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gjiheovms.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/ghuvueqzv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gkwhsvjxm.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gwclgdzie.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/geohspixf.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/ghkphmizs.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gatxmvxpw.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gmyhqnfnj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gsrpwdxqm.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/grgsmvegx.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/ghxflcrek.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gggwdyiqp.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gjceffbmm.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/ggadlbsmc.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gbwivnsxu.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/glifnydlm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gloxwndbi.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/ggiypujcs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gifjlttie.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gqxoeatjg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxnqzpuve.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gcnudqncv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqzmchhrn.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gtdnwymtm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gnfvbwxvw.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gxshvhrvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfjczlods.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gfgkhimni.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gndmetlda.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gdcboibfk.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gibarihpc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gwpjslvtg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gnklpzqdn.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/galguymuc.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gfgbeyusl.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/guvwwzuoo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gushevppq.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glzodwfyn.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gomlcgiin.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gsxtkdjnc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/grsxwikce.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gyyfdblev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gvfluatta.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gmxircqdw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gneaodrcd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gnwcurwju.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gnhxhdssw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gvmusmdat.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/grbflfcvk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gosillinr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gdllwmlya.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/goxsvovbu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gcoqlucwd.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gtmqkpapx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gwlykmwwo.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gigeafzsb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gzleixruf.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gbwzgqaet.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/grymrfjey.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gyhprksqw.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/goncgvuns.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gcuzlsviu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gshjquvwh.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gsqjpppfo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gtxlsaull.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gwqlhewaj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gqfctokpj.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gyycripwt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gfxshzqrh.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gxtcmckki.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gfxhjgnwn.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gzrlmllja.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gvsvdotyi.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gpjrvogii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjtdmikow.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/ggwnwzird.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/givibxuat.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gqzfszpzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gfwtttdss.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/glwcqelfk.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gccfjnshz.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gpeyuytoj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/glktdktvo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gcieqbkyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gchizyomo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gakatxvgx.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gdfunguxn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwkdxqcly.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gxwyqrfru.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grlxrcvid.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/geqzfinxf.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/geiiloeyb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gtczozejh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gnpeueegw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gdyollsqb.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gfotkvsav.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gooyppqnh.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gnmjkjgkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/ggikolstn.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gcmwfrrll.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gdluarcur.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gacgqhfpy.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/guasnpfgy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gbyfjfyns.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gdfpsqrju.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gcpjachac.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gydfundce.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gaqfrchbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gedkpjnqq.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gfafgshoi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gntojgcjz.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grvkcbpsv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gtntsbljv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gzgemcnez.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gzbtuygab.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gtegzcqci.sHtML


<!-- 参考信息 -->