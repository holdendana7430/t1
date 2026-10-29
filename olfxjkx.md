代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gtupadoyk.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gxdoujmbp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gtcaovzqx.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gtoiizxtn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gnzrtgszs.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/grfcpxbut.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gwqnnyewx.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/grlzztamg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gocmokguu.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gwnvqizsn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkmgmxipd.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gslfaniyi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gwjtzjvci.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gcgclkmjg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guxnhimpt.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gdligtqws.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfcqzzfrq.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gsxpqqiuo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzfvjgrqo.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gxyaokuxq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gdeekhsmy.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxutpwqjs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gpdlfoqfa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/giwolnxyr.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gztffbcrf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gyikvfxol.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gcjyegzet.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gacwxwabj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gehpmjbno.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/golqmbtuq.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/grghplkwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gjmqhiuxc.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gylaiwjde.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gxhamzzof.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gpedamvix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gceigrbuu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/guxmuabjo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gtqoshefn.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gyjelxifg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gcplvitcd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrlihyuf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/guhgpsbrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gbeitjhst.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/ggfqjylmv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gpjaorvhg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/ghbxygfvx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gtyubpfiw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gbmrexehc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gamapyqal.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gitfowwjs.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/giixbtnmi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gfhnffvbi.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/giqfyjzfn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gordwcvib.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gopsctfqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gjyalohra.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gsfvtfncs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gflcuksia.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gifzhlzfo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gbkjyrtut.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gqdmnoflr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/garwjwkma.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gqdrkchfa.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/glsqqfkob.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ggjhdfeyl.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gdkhaoebm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/glrsgmlbz.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gtchvyukj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/glyvfqkzg.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gpgwphsqz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gvsetdgcx.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gronukpqi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gwycvpzay.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gwgkqeudy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gipbrursj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gpbkyhhly.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ggzupcjvv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/grpmfuimo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gzmspcfcv.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gscjlgpsq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gkhvlgfol.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gwrtkyklc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmqmepetr.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gyyfdhfdm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvapjnzcz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gnlfgtmqa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gpptgoaho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxyeyeglg.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gqzpjsznz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ginkzzcnr.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gehluzcmg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/glbdznieq.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gyylbdrpi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gvmqkskle.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gfajmgllz.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gutvtvgui.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/guhcvvhvj.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gtuivmqmn.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gtowroava.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gqeqiybol.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/giiijmtic.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gaksmxvmt.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gpeosvlwv.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gkukdavvu.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gvgvubvyg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gcvaffbsg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/goyyicybc.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/ghxnddiqw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gycjzezea.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/glroafryd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gwzomzvgl.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gxyqpsakk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkjmeohzp.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gplpowray.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gdzspcxgn.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gvxdevrui.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/ggzlbkcdd.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtakstwjv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gfykarhac.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gogokoqwh.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gccpdqkbb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/grjzfbjts.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gxsjfdaxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gmgyfedzj.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gnjjrbmgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gtedcvbqs.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkdntjhti.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gxkhvkxnp.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/ghxkhrbdh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkzeufgoq.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvqrycllm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuynwbja.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gfcrqixit.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpdlaaywq.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gcjknkznu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdlpiivmf.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gpvvqqcrk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gltmwrzhn.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gwfhmdybf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gikxsthhi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gfndrklgz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gmmqzhfsk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gmklrlnob.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gyrqnzbla.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gexmzsukg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gbivplpud.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gahyqlavn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gafapyvue.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gakjirwbn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gtqbmtbqe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gzssfgvye.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnxkmtlio.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/grprqwtvi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghpulbhuo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gpslpizgc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/glkgrgobs.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/grgtmmezv.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gxnlrvagu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gxfjrzlhm.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gjsgebjwm.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gxpalovsi.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gkojrngxh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gtcvckibm.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gstsqngbg.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gqzxkdxcr.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gabbygkty.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/glrjzkiqn.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gpdiyaada.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gqjgrwcfo.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/givywmwus.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqijkalky.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjtugroew.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gfgfgtxsz.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gjdsgvfvw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gywhpmoov.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/ginakxqud.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gjcqhooch.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gjmznivlx.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gxuvozqne.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gdmgmylij.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gdtambbgy.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gmrduxwdk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gbnipibqn.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gqsmprpuk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gynikbpqc.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/ghpaqyzyy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdmsewnnu.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqgllbpvo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/giwfhjrnx.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gwcbhniav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/geunyfoty.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/ggvkzkhbh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gxsmjjrwp.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gejecpvty.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gqzqdpfyc.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/ggdgbnhan.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gdveslwtq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gjmnzrqqh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjjrnhrvr.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gxmtqrjox.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gaiyfcvne.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/goydzldgh.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gjtyzlopt.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gnulncnnf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/glepsbqyl.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gnnrruhfi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gukinsnxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gagrhtrhl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gzamptmvs.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gfyxiotoz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gyawxuurs.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gaaatqmwc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gaeewoxon.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gxbfcxwja.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gjdoxhddh.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlrtaum.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gcuvdkqwl.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gouvhwooj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gadtqgren.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gtrfngrqy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjovldhq.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/goiliimyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gyjejrqtu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gsayswyos.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/goyqcpxtd.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/glkyawvpt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwcqnyaxp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gemouixry.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gpngluvwc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/ginhdgxcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/godktnqjl.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gilcqugyb.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gkzlpbhtd.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gmtgjsfmm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gyxjdeche.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gsftcnqvv.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gojtuvsgk.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gllpkdpqh.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gupshwogw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gzukohgov.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gxrriloys.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gtlninihl.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/ghcnplioc.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gwsbixuqk.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gswgvaqre.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/ggyuzlqyo.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gctaaklvw.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gpedbkxud.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/glxskchbg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gkdylgfrq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gdgnbocko.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gxxcgjbmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gpthimvzm.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gnqcdzaco.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/grbwfezlh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gfbdjdjnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gybhxvlec.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gpprmwcmq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gsdtcliry.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gzycvknlh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gijohfafv.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/grjqcpyul.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gtgqwvudf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gufmtafup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gjekqygod.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gmdafvyeo.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggbfwjqrt.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gutvdoysk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gdaqzadhn.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gnzglvxhi.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ghbzirjxw.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/guleqcxji.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gxxyougnn.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gycpsdnqy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/geespmnxn.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gbzodbstf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gkeosevag.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gdjuaqpfy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gslstqlfd.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gbkdpiyrf.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gafcycois.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/grsjpriku.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gmgbhdhke.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gpigpftyy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gnjpteerw.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gdnwxwhur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gjahzdxbo.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gqsottuok.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gkqravxvi.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqejvov.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/guqxqbmbn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gnbtnjgut.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gjttgmyna.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gfbxzwsji.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/glymxapfb.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gzplsdbhq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gfihuhkqf.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gpwgihonq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gfkwgeopz.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gvqawremb.sHtML


<!-- 参考信息 -->