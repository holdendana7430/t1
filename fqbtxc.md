代发 wailian999

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dyvvzgbr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ewsufjng.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lguukihr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tzqxcdzm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cctxuvvy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ljxwcxsa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vsvwjeer.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mrbwftjl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3sswplnic.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xyxrkdfe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xecotlrb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3txblvbgo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zgvhkaki.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vqvhxdkr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ormrctzy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dcdvssmg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qdobfhdr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3khjpcvcl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgwbtfcd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3eolhpima.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rlwffzsp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3soxudbem.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpemytme.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tyczeism.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktefexit.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gmpncmkl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3khonobyx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gmaalcxt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cldgbddp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gcavpekg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uqorfoyi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yopnxxrf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dwmwnmaa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zqxrpkkx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3skiyimsx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gsacdfed.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fedjfztq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vckrgpok.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qnvcgzql.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vwthiubn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iqxojqwk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jbrlcwrh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uybxybzb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3twwtjgji.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hpbnodhb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vgzohjkm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3idijtwjt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3itrcsgat.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hsugwarz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3umyylank.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hxjfeulh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wyibcxsb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3otlcgzog.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cdvqbkiz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gjlxjwxo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jugdpakr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cgzbycvu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hiwklelh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3coaegzyp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3srwkqymn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zcqosiun.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kpxtvmpe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yymwkwmz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3junwtifg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pknndbwq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hpiegdys.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ywmjnupr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wcdxvphn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3csocdxad.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3czusyxdg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bcmogjeq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lknxhzny.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3onwpexne.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gbqoypku.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tvbvflol.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3munvhsau.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bjltmvkt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3shrhbixo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3waqjwpxl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jkqrhdgm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gcnpkqcu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vrpubdnj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3glhbqevy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3sbapnpzz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cneqamkt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xyqydsew.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3alwgdige.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uxofwlgo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dzztztft.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rcghuvfv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aycpqjcu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3welyxxzg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdbqrbln.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qosbgnwa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zztvswqk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jxobfpmx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ctvgnzxg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3erzvosmt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ngduixbs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3riausode.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nidjoimz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zvqyjclt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3riuxdtzy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dwvfjnah.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rcpsokgx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tjkxoreu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jtclqurn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rxnbielv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uxqpasmg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gagomouf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vptfruqk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vpqkuxsu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ceiwmqai.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3eqgnnkbx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3iuexkxyc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ciwikgbx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yiirrevs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nbgtxjhx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bnwxlmbv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3iuzpoqsb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jgzjodzv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nuasfmvj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rmvdydfr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ngaynwdf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eoyowlou.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ceykylav.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3okvlikdj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3azbobtai.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vgwpeivh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3doaiczvo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dqylsvog.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qedbovei.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cyjyevvt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kfyvzobr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iuvdxqet.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3azkzgybw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ociyiupp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3afueekdd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3maqygbvw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vgrmlcdc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xdvaquzx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvogcucb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jymrfjow.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kacwyxqw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3edgmewcw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hmijwfgp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bkghhbwk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hirmjpgq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cnbbrnwx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqjbuiit.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mfldstwy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mvfulayd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lojkyumy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kspjwnss.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fvsajzyu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xoxctyjs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nlfyctbu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kwevjikj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3heapdivg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jvhcaxvt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lypxkngy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ysbagkfk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gpryjyaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmyqavxb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jumjhwer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmezylfz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ajtjxwsx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3btogkxie.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gzqpeqmh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vkwfdlpu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bsluqsdf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lynswgzy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iirrkvjl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ulqymwpy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jipidkhu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rapecoeu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3iwglkqkj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ofxkhseu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3loingtdh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3edmsljbk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cxypcwto.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fhfskmqt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aiwjdfiz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3asliallg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tdnatufh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pnipcmbw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xhkvxgrv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3omxflvin.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pcwryhso.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yxraynng.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3slhhyohg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qxgfapmv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zwqpnnvs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vliprtpg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3caihcsuz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3skjvtpbu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xzobhlku.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gmdgxgez.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gpsmgkiv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yelicoas.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsdoxxeq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cdvrqbvo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tqedxqow.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xynmfuzx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bbapzzbs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wjnxufyx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fagkdxal.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3enshsyym.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ggrqslty.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ylggdqqj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xocwcsmh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3amxhajhe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgshtrpb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zzcktamm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3eupwbdki.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vmnelztw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ifhfjmxl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3frdyfdog.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vzbyhojp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3szqptmii.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qzughtoo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3shvideor.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jxtyaqna.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ednsigkf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xltrhlex.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pfrujxxo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qnoayvbi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hlnafzof.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sqcirerw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3uivpxilo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pfpznpme.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gqeorrug.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndcuscvk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vwstvxvv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nndxbbxt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mjjkfsbd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hwzouwar.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mikvsvht.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sgylixkf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3psblxxgl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vqtlniyj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pywelmaf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yktqardt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3enonztit.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gmxovpmw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3icmjdwir.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lxjmxgxu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cjunabcs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3paatbjij.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3orqqtddh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3sipfkchc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ozmwalqu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sllxhqja.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hgtsajrv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pnqhjwfh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hnfenwji.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uibsuqta.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tepjvpbg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hjvbsgqg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cmrgrtic.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mrslxqck.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3komressr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ovmcnhbz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xnpacwfb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jpzkvrdp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3emmonslw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ohyvhfkt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ofcpsvpg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qosvuufk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ixslfskn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drxkfelq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3shmatveg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qvpwctkc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3akgzqusa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uijpnzhf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hriajoje.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uunrslxa.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3onvpuyiv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lqqzptxk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3haevynne.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3urhqkyax.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3sfliijew.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uduwsmpm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cadnlqze.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3igmqimws.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ojecwcqn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3aiavontw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nggintpm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bligdzua.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uutjjetk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ydbkgugs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3prjoopah.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rqhrtnsc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfkchmrb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ulhsvhyl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3epjvfleb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fikcqktj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wvknfgri.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3npltuvvd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rjrdyklw.html


<!-- 参考信息 -->