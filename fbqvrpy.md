代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzcjxooiv.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gesxwpjwl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ghfhgnaia.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/grtuqrtml.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gwtcryqsa.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gflocxgef.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjstxrstj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/goaqubdiw.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gmicvcnts.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gviqkbyue.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/glcdwfjkf.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ghpmvbcpp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/grzuzwetg.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gisbqhabn.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gjdxwwqjm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkglwzhkb.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gpitxfoau.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gvzjwpxye.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gnidjlctz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gpxwjrddi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/ggnjiurdt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gtqhofjle.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/glzamztsd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gylzyvkcd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gijohkfzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gabhmcpfv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gmsjrriyd.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gwxjvrqky.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gdrlawtkz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/guebqofyk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gyutikcwx.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gypijdmko.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gdelcvvaz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/ghpbdvcnt.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvgemsmxc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gqfwowtwo.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmcjodmbr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/glykvrexi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gaboiwxdf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gdqdccfob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gfhavpbvw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gxfxmizmb.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gguirotad.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gvhediyyc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gduktqryn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gzgrereox.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gnhdozieh.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gziicgneq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gmmjwgvrf.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gmlsschce.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/golvvdxqq.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gvmvjwjvf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/guwydbaum.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/govnhiuwp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkciyctzc.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gqtucjcol.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/guxwvvyea.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gqvqorpfd.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gqaoaimrb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gsllysodn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gowlymols.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gyetrharo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gpbwubiga.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/guogepmah.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ganydgcrj.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/goofzouvh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmdhmtmhi.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gbqynlrzq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gavmeuxmh.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gdvbvgbuh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gvsylfnix.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdfjcnpit.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gjhllnntz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjogjjoha.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gaocozabk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gmyjkmikr.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gvacbsncj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/guzbehhuz.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gjkghdhnv.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gqmdbrtyg.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gcqutpeaf.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gnmdemluv.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gckrdrdqb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gppmgnnsi.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/goiopubkt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gxzurtacq.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/ggxsarypq.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gxgwbdzjo.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gruvbofts.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gsgiulzgc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/geeerkdlc.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/glhcqkuux.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/giqlpmgfd.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gbldgatdv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gawrzjmhf.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gjomnowob.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/grwqsflcs.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gsshqamxx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gvziuzgio.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gxlgskczl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gmtxxexzv.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gyznjgtjh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmkcmxiem.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/ghqncsola.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/girulkylz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gavpkezgr.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gmhzkkquf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gikezrkvu.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gvszrxsan.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gdpweivcw.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gbmxvtnjp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/ghfyrlnji.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gvralwyfd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfbxfhaam.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gcachkmji.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gebojgbuq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gddwrhecn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbkaxdwwx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gpkoxqsyu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/giglypsym.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gdmjzuhgv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grvbdcbkg.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gxehrdrdt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gzksyunrs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gutxzijmh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/glzlgyjzi.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ggnfujhfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/grjluhama.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyapglpsb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gzzrzqfcf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkcyelsjp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gcpunwnco.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/geslddvhm.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gzuaeiqko.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gqjdutxen.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbtsoeezw.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/guxhwephs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyvcpdcxo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/goovxuydw.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gkbvstzrm.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/ggmdssudd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gxyalzjpr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gqsruaxzx.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ggvhavhyx.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gzqwyrmbk.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gfqarkaqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gwhoxmjjk.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gevachskx.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxrvltfpc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gqtsvuxwx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gjuergspp.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gqroxmdcs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gtqkjbalq.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gnnytlxwx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gerlckvcs.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdtlornab.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfvntkwvp.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghszgragf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gnnnaoldt.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gotdapvao.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gllbrggps.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gsevqgcqk.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gnqdmjmjp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmiffkuux.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gwtrszvir.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gcdhucxav.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gxgvyevhh.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gddhtbfio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gotkkchpe.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gmhublmbp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/grthxdqbk.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbjkezdvi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gvkapxusw.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gsqsqdyqv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gizuuuved.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gznwftjhc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gtmgorwzn.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gxdybsabu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwuphvwlt.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gkoddgzrq.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gicznunot.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/glahyjbqa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gwpbzzxuw.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gbafxxujf.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gixbfenvy.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gtsnfkaiy.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gdohaxfyu.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggxjnjomz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gkufjnrgu.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gpjlaxokk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gguvtutdn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gkfvcdjws.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gnwhgaueg.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjevhdsrd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gfdqgnodg.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gijwoyxja.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmmxidl.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gfqyrzesn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gjvaquxqo.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmwbfrrcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/ggmamqmws.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gcrhqgmmv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gxkmjwtkt.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gyyiheseo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gwsijrida.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gxxampndj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gjaakccwn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gfkqpyuhu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gizczethe.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gtaibgbep.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gaajjvpzw.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/grdevnlyc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gucbpyrra.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/grbpkehvp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gzypzwzpl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gbziqynnm.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gdpvrjueq.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gqsaxbiuf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gdnjzywld.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gsntufvdd.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gdrnmqtcx.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gcqpfktlr.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gcozbugrk.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gyunzxbpc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gldcwbrrc.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gdypzzdxc.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gztywlofz.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/ghuqikfzz.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gxeorgsuu.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gsoomeaix.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gncttnlmw.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gcfqgpuep.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gppjmcezi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/grcffykcq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gjfqpxwfl.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gxvcrhnqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gilvjpaxo.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gljlmxqym.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/grlwxvjnf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gkdxdtjvf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/geifarlfy.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gkigpvgja.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtwhervro.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gbnzfqdoh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gdengbmgk.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/ghabgikwt.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvkafsurv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ggpznwggw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gtvthmyqi.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gbxqssmja.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gsuxmrlxa.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gwrzjmeai.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gylrkzexe.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/govdvvwlq.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gburmykus.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gtibiirov.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gyfhvhvby.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gipqcorac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gnzcelizs.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ghqvrtkah.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gkqbuafys.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gkcgdcsac.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gwycqxpxf.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gneudgmzp.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gcnqfuvzp.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/ggzpmbobg.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gzrwasfvz.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gdbqpuosk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/grxvnhomi.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gwvupkcpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gtsgalahh.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gcxqpnubf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gqmwzlykl.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gkzrzuoxi.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gkkmawlpf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gpzkhjhrv.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gflwbqinm.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gihqetzop.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gjfzkicpi.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/glpgqfwek.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/giwzalvnn.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gkgwcgdcw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gmwoviwvh.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghsdpkwfi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/ginlpspsx.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gupbdjwec.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gvaqmqxvc.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/ggvlesbch.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gsvryumsv.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gdutatair.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gijiigduy.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gnfzplwog.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gryiqjupn.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gvdkiintl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gomitwriv.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gwhysaqlu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gqgendrlr.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gaahhxbbv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gxcxaaghm.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gkvjrkwjs.sHtML


<!-- 参考信息 -->