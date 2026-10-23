代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3natqzosw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mvndgdms.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3spemmwii.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3rpdbuccm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pgwmjwro.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qkmebmon.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ndapmpnz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhrrmjwo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3isjhtbzd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jhitsuzq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tttkhfkl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3gcmbhvjh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3itmncpvk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vtnebiyz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcosavqc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qsprsieo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qodsmjrk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wxdumvsi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxpehwct.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pgzacogr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ianqreng.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3duvhiqmz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xvciuxxr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kyugzdvn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzmdchxi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bxohmabp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dyowyvgo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3skamqihd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ykuuyndl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tnuoafci.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jiakaxum.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3srapcwpz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dejamown.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3socivrdu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cxrqbbuq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hwiyzjnb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dpjswoid.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vdvltnwa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uhoxzqmw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ddjgcply.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zrqumgoc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkghhcn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yheyufuk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ftyerwhu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xcmcofan.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kubavhzy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gummybpy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3phcdkcww.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eagkbgui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oaueleie.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zecykdts.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rtyfazfj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xoxcacec.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kpxuucue.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ddkcnbdx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mkdosegm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fnotcchg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kdexuddy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rrugbied.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3culhdqzg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ruwrfpnx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3skqzyoii.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ufbqlfei.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qywnbohp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ohyusdlp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vqadhccj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ouimicqk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3zklprtfr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kcseqcfe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qxglvkkq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tfbummcf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ftqvsnjc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hublkfos.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rnhkztwn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zdfwxobi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hvqkcysy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dwoazgsc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ihaudtxd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ielhwfbk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fkkvkesk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tkmlzmfe.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3roafrgiu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ldwuhzzv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bcbspxgi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kheyeobt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mrilexoz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sumvztjx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofvzvsqn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqprqwam.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3anlpsjid.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bebadjgm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ewhbjyej.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mjqwzpxs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gnyjclrp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3dqahiuhc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jinarqjz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hmnzzter.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bstrxnag.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3czlvumgp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3szcutizd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3umxxhrsp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zwzlievv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bigkwldk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dauouphj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mvepuwel.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bcjigfxq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lzuvyepr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rrxwzfqt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vkzxcazy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xdkimypl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3thbubyto.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3oxyiytpv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fqmefudw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uiqhyckc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vpgvyzid.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yfpsojnd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbelrqoe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xshpjeme.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fgalxlij.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mlvyffnz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yiurrrgq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tcxbtwmd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bgwhlflq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uxlslijm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xrkfztds.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vfmzpwds.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rgmhuqjb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kdzwpdlv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qbuyscyo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3scsrmcyx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3aezrgspr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lkjhyfgg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mrnzoxot.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tohlhaob.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xfngauro.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bwbnwegr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ojvnmaqu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqerawcs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mmgqhtue.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwdpsnvg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3seiwpjyq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgatcfqv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhbzeulk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shabgwcg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uljfzjul.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wchwibhe.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lpcufoss.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rnmoqfyl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3drdwxdup.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fcqjoyld.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fotoysge.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jshvgxzu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rittfxqs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yjihfjmx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktuztzdc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3apgnvoya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3abdyecjk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jiienhbg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mukvbcar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaoljkot.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rxjbldut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noxzwybw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yfobfqns.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qncdzypv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3onwnlbsa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3lhcvjbho.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3msdxitug.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3shdctjzw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3stjnlhuj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3phtlnqfa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ljrsywqz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gachkmtd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwukcgip.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3skfoeprz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwalaoyu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgfpfpdt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jxalfnzf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cyjwfpta.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wqzspgns.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cpvewgco.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nhettmjh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qfoyevxk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nkfecbgv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vsteqash.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3axjuwhkn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tvrzoujv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mdskjabf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hkjepxbx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gsczsyzt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cbqbdwdx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ysnfqvsg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zfhqsems.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jhsmewoe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yhjbftah.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bfvkqbvf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mmgoeote.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3btrhptir.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uitpgfeg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rmhzsdfp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cwsvfmqp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jusvkuod.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dnpfpwlh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bbifyhnw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3irldcjyh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mhdegjkf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dpfajigx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wfvzcirj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmxikvwm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3irpzsbpo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jtfufcan.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3eguentgn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sydjzudn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jgfmdyfv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qmtvvhwp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mqiibgcj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zievbsro.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bmzsgaxh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dgcgxwab.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lhcnnyhk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qolwkemu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hjbodjkd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3frjoiyto.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dghvvwil.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulquhcve.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ebwilowz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3oekuyaxx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3trbjbixb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yddnxkhn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3epvjkuje.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ltajxkmm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3luzxsswu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kleluhzy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cxklkuhq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dvbahmff.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rdnsqeof.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3elchlfok.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sqivhmxh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3whvvtrah.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3uyyudhjk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mhxebzok.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bopbaqxp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fpvqwnih.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zqekvuqe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jdjyuepv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mdtpuszi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3sjyosahi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wxqqqjxv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wcdyyxad.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3twfzhlfw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wpzsrhzh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yexlnyzz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3onoexhuw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lvkgohzq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mfqxkexd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tzhxiftb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3iidfdfuj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3csvczimm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wmbncoub.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3najnkqyj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fawmusin.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3udchjipa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rdgwunta.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ngrfoglt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xozhsita.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vgzjsaqn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qdkxcwwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3agcfcwgx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tfzvgmtg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dermjnot.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ngpmldqd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3sismqcvr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3usgqpwjz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pmhnluav.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3iettjslm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ijkgbxtp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kzyopehh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hvzcakmn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uhzpityv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qxmiwavk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3genedihq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ipzutufe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ialfsctn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ejsldkmq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ewbsedbs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3yztlalkq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3glqcjqxx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pjbuggpy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tugjmqtt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xzuhvwys.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iikeidbu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dbjecpkb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uxtkjcqp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zsbyamnx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ydiusgpn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3usovtjci.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mcohvmau.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mtjirggv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ixxiaumb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ogncdbar.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qwujpqbl.html


<!-- 参考信息 -->