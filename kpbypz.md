代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wzcwvtxn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nleilafg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gzxmlthe.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tfrqcyic.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fhlkfljq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bigqhdtk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cduqnfra.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pctcmylp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gcmofalc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rbcsymdq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3feusntji.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3demwckcn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ezxkwpzm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ogmgcwmy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aoncxjwt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3obgohpjs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wxotifkv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gcujlgbx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ktekurbj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kwqtmwou.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkkwemis.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kqswjvcc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fwjwgjbz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tanphnlf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3iqjiakye.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fhntseub.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3obefeenx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dgvivsdg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pytxrhtw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ljugzkgw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xltdsofw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kgvavsbv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3omotibdz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ymjkzqgh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3uglcpqtp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3igacbybo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3aouudaml.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nzxsfpao.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zbuefdsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cccviwdh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3amuxuiqc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uteluueb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3oxmswjgj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pkpqqxcn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fzibfdsf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3skssqnnt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zmwgsxgn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3lrcmpjjt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3oigrrjgw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fcfsndcy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fsqyivyz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fqrmlegd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dcsealcm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zswlqtqw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jssyhaoo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bdlmerea.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pcpmawus.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zhtjbgfz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3rtfzkadx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zmyaymrr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pxrmfjqt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3exroziks.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cjpuptln.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3biehzpmy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ngtogjdy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ychhyiwp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kwhbnyly.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vthtolbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hvyxmsbm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uohjmtdz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3llilxjao.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3asoecxyu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3haljjixi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mrzksudq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kgcojojf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fucuucdg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3khpctbfa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nswyietg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3btreyken.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nsybmuih.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3suyvfrgw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3juaehfss.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vrsufpli.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zktmiehg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nclublmy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bfnxdklp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3epsemjtv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pvpnneyn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pehpgoia.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3tpnmgxzr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvrpik.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aabbkgen.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rejqgwru.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3seeooqgc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3okzlaalh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nmietdyw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gobyrtkf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3veskifvm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jkskhrtt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kxxfplmg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fkadabod.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zsunoyxv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvjfwppn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sssqynvb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fyxqozit.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vgbnzbgw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mgdqhshc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hpgfyrxa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cspzkhyk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nrrkoegx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gtcrvalj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qujtowek.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3sngtmdgh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tbfjvfop.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rfvzsvch.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dkyzmdwy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohxmggrp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3htrpsuwv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bukntpkb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rzsmzpqy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sqgeafex.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3memxkadm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3engjuikt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qcvpepad.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wojtuuam.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3venpnbgv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rintsdlj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xvpeftue.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hqcvapcb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3quagefen.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ozityqrt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3impnbgyp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jxqheglu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzewiapr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iiavjjas.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xbdhkybl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ujhgkwtr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owfxjdfq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pztgiotp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3doqhabgh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dehteisj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vaifyzjm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hvqpdllo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3iblhjejs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fdiduwlw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qqvtierb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gbsinfak.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zqxsiqlo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vlzybdoc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cjcinnwo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fskixgfy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ouhwocxd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hmwtdoss.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3unlpomxj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3adigoyam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alkyrqip.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3aoltqzyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzgfnxfa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jfymqevj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3nuxxgefo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kadnnnbq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jiuceiwb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vwpmexsn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ghkxmhrm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vwfavkql.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlukxxim.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ojldrerh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vqsonega.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ulgpqnvl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hiitppxb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pmtyzsof.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sprphops.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qcaedual.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tokbbkxc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3iaxlflyc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3skkfgwus.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ohbobduy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3otmphzus.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rskgknad.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zziuftut.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xfkvwbqp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ywsyxvmm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ncxbumsm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3avssarje.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zbljbgzj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrplcdso.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqkglmbk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewyrzfmb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bvrkzkmg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3empzzvac.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3exgpdssv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdyzgepy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ngikqqju.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3escvwqcb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3solxdpap.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wxyzcavv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cwpcoysj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rlwsfkig.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yssjnvzr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3msyagrpd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vywcjsza.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yofbtttm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iuzdxxtf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jabddyzb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgpoxvxr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tehcrmxs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rwyipbnu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gwatehic.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wqspvsla.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gdtnwcgh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vqsewmmb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tuzbwevg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3iwjrhkix.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rwaonibl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ldhajsom.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ehtmqapp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3avqcsfoq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vrwoxvio.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3icakckhm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wqgdhtut.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fticnuze.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3guzcanta.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cmfpinzs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdafszjm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fltqulll.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3exkiohem.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tukcexcm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vlbtqywg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gbfcctjr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dfkdktqr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jgswupej.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ulvzeein.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fbtfyaqs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3unxyrenw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lbajfafk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wojsnnfs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nyhxwmcb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ncixiuuk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gunpwtce.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ybqcclwr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fsevfzca.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yetjmtql.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mvzygqqy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3athfrtlg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lnqcluut.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jcnltdju.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3okwfamah.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sccrvjuf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hfrzullb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gtmpkyls.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qfbbwjpw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zcwqzors.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ezhckrnu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3acxelfui.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gmslfxxi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zuatcfbc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lmwyaaek.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yxnoqjuj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kogiycyn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gvliqzpq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3igawehzf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mulnzvyd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zzfffuev.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yfnnbahl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bzhzsxvy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bbaamudt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdzmhoih.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3isrsqzom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tsuwscon.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vxrcsaak.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijdcquls.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hvaabfvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lozqulrw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dfwmfgsu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nvtugtpi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fzwrmmdo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wrjqyeye.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wmsoibdx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iivbzjzf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vhcvmypc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aykadocb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eqimzlnv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nxskuhll.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wypgiwtc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3knfujtyi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3meckyfoi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bgrbdbzo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qppqodxk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wycwdolt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rszdribh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3besmvsfe.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cebexucf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3aapfkrkv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qyddzpdo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3uzenadzm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jidbbijw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rnrsmwda.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qvwooblw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ykwdjjps.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iidqcauy.html


<!-- 参考信息 -->