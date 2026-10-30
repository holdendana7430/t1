代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsitynkbk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gsrucjvvv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoovqpzg.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gfygrahvt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gtcksxjtm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gwfcdnnsz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/giuvvscpi.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gactijeqw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/glyppilhv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpovxvrj.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbqkrjigp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmedkclw.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwaxtznc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gxgfagmdi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/glfukuslt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbqdxiyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewzumpjp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gfqqrfkpv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpafhgfza.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gzlysvvit.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguyxissw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gsccexxvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geydeguhm.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuutrojo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/guncoxcnp.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gneesvgdl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqhwqsgh.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/geyjcggyk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gijtamudj.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gnvwvfovo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxurliim.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdxiheph.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gapkjshbu.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gusgfybqe.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeebztwj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gmphuymju.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gseuopsbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjajjjtvk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gpkqispwx.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmzdyuqv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyogmkxkw.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gapkdtgyd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gywxdfsrh.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gyuwjjrbt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnymgehe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gozmcbvfq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtmdgsan.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdeaskaj.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gizoynlbm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloctjdzu.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gakkvpfyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gsxnqwzja.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gvjamovnn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gckfepbrk.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gktnuzhky.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcktibzy.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfgsqdq.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxubyjji.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/givxvitzk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcbifhyv.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gazhnsiwn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfccvfwe.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmuedcwv.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/goyqktgqu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gchptqkri.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gyyazvztg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjauvmihk.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/grlaohxmh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gihtbeehf.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gvssmulyh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/grixoirdd.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gefbpsjce.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmsrvdzre.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gjoslgjzz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbqzbqvy.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/grnmrzhet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyzbvvod.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ghdqmtnqd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlvownmt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyzxtqoz.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gvihlwmie.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzhuuwfh.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gyasqlexf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gobaiwbbu.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiavlfjc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/guppofxmt.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxokmihth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/govqipqtv.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gwstlawok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gspgamzkk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeefqany.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glgnzoqjg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvkprmnnx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefvgdfe.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxqsqlnas.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goioqqqje.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrsgpbub.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjtoiarp.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gscdhyort.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefyhxpjl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfwkbhlb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvloytls.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtihzwlvn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/ghudspxno.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gcjolocbt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/goueuqqip.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyyjbxcqa.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnvxlzkfq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdadxrgfi.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcusvrcx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gwuymzhul.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gchwcgsli.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhvgggc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goaxinbiy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmutswwuh.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gicizwkjs.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gfuibhhht.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvowzjxw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwlgvjnn.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glshtzdfm.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzgleoxa.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfvakplkp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwktsdfc.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgzuvtjs.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaywdoidj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhbocidz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjcxnxrtq.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpssuvhq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gisvhvkpx.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbhemuoi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbjarmmza.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goxpcuwlm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gauvitkmj.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giktgzwpf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gphojhosd.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gfpyvgmem.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gewcehwvl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxammhjip.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsfazyjgk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gkshequvc.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqpbfbl.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaynoentj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazgnaotu.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebxjyord.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmkcowwxf.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexbsghun.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gefzfcfza.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdyexlbhv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmlbzmla.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrsbihil.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggflmsucq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzwssvia.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotkmtqu.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuipoxak.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifqbctxq.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfecnniak.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gszlaympo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcthfyhk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxbkfrdlr.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmnywfjb.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmfthxav.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorzhjcfy.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gugenhdmo.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbpkouybp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofypxvmu.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqyuuuhw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gslpklwmv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxdzdgvz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfantwua.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfxsmtbb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpnawgpm.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gaomrhmqv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtniulpmd.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gkipqaatl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrtzgmar.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvbqwgmt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gevfbzumz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkpqdwfx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipjunadb.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzjesuvkh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfuodpprv.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gpclzzrta.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltksiyii.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gzrnwqnay.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqgfnjhl.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpwkzlji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gopvdshfw.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gjtcjmhnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/garvawwac.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxqlzqcaa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtctfdnzf.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcdpqunb.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkkkyxpi.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gznosbmki.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gekrsylfy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdluztm.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/guyghbarz.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gfhtxfeuw.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/guymoucfx.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gayelsuoh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkfeewdjf.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnpiuyua.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gteqbhpae.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyxngsbg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmontmibo.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gsimpyfww.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlhikjln.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbqfkvce.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlselmlh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/glfxfmivf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gnfhbhnwq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzoyczcv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjbmyzel.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gcwrlfask.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwuwydf.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfbopmkh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthwcmupw.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoknpmvq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtrciogyp.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gbmreafqd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgfhiesn.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeeslbia.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gajiuoolo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcbccvpu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glogllrgk.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjyrwjcn.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gythbubef.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdnrqhg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmidjoub.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/guhwwvote.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gamwzskri.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxxxyzom.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjusgixc.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsumhwxdu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvftfyyum.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyjeclfx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcldeuse.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzlhcjjn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gefywyplc.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gohsrwdyw.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gepawbpgl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqysfthlb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwgvnezb.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzimdpin.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoqcgkkj.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gytvviunk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gzuroidbz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuwnjsdl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/ggqwkeimu.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxfcyiyyj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoilbzym.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaogoode.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/guiaxmpuy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjcbvhos.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnehbaiw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxktmiqxc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvebaki.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwajuuhup.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gqksdyvyh.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/goexkdfsr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboaefifj.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gyopflcpo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfuwyjxa.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstxewcrn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusyizgmn.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqqbfatt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqvxggk.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnswmalr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrewbdgr.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdrzvbmau.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gambarclx.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gputkfdpq.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmsnqlxf.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gchvifbvl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcllhngvu.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/glyetcxwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gchqckdxj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtevangoe.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfpafigyh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzwjgydej.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/giuzutveo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gugifwkqe.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzqzvynvo.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gosmrzjgn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwlduozuo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gewjeygyk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gqgfhcvoj.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpuhikqi.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gyerhwusr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjubccxq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gqbefkxwk.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjtuurat.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucbhnpdg.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfwgcvzlo.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/grwzksyfb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gnglseljr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgpildsw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gviyojcnp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaenjbus.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gfvjxsgjj.sHtML


<!-- 参考信息 -->