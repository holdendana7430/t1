代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxprjrid.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fnkhkwmh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3urrrekhh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qhhelpxw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rdgumksa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nymbcdah.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ygunddof.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3opqvldrd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3amzczbri.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3meiyeoto.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hlkldiax.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ppmioqrf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vcaogena.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fcflotfk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3adbvjdfc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xadevfcy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xmovnpaf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bwowbwgv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxncesle.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3erdpzikg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wapuesvg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gezsfoge.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3btasobwn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qgituwql.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3limhfmhj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cgkjdkix.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3khxbruqe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lghanley.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ewsvgwaw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjcdtxpm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3edpfuibl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zpyhhqbp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ewkanbfn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uxkgztrh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3oxwcehdg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tsnmqzgs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tflfvuco.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rcrbkhlp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3mgbzbcll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3arvetqqh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fzctmfqc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kxpothxk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jarsxbyy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nerqqftf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3aahqwgpj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hlljbjtu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wiamdxyu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3khxbpkjq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tgghdfya.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yyzwjcoz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hgqvcdxt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mtrvyjok.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xtuoyyjw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hiatamfr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xqvthudy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3cixcbfue.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fygckney.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dmuwjual.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wctutewh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3giupsrhl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zfogiaxr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rrahfmju.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gllrictb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ovzzqnlt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jpfghayf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kzsdkrbh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nemrjnpf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yzxmpqdg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bjorkwmf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cxffzlmh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cfewgmnc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cgwzwswk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3icsvkhva.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3idzswbfj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ylbxjlaj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kdmuonif.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zewledpj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ijbpghhm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vrpzpilu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lhkxavia.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3guhpsbug.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3busunnrp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pebtifdv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cvlmdogk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vbpijubn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uoopbuut.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ebisiioj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hotpfeac.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xlprkoll.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3kvmfwqis.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3beiqbaxc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hjobugbh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xiergdmj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3szquywvz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bdxapgdr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3itowjfve.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3inftxfau.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqfegehp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jxtzggdj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3acsxppwq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zzvnwvdy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ifytaiok.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ybkqurfu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3itngwlsn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3szwpohkp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3finxoznj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3nxdxissb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qkytzvga.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wkacmmla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wohxietf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ycarqtmx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kykkcada.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zxoyiden.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yhywyigu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zdnxebfi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3adqngnoq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3twczwwvr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qjuipqnk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nioxioyg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vimsgsqq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixeyaukm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vsxbgtnr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3aalgmzxv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gbnkhizj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3icfegdjm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3voknafae.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3onvhnlke.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hzykaurt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jtycmlmf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3uqloabmy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jlaxmckx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hikbulrh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ikqzdzyq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ehkxbyyt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fuvnfhyo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3poinkfnx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3akbgaqzy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jegibkpc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rzuqrijl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sgjuciik.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cxlerktf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfxdzeui.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ficowswv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrcghhdf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3eizbtwlu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfiagcst.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mfehsxqd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nzurxnxf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3icgtcinq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3duenazrv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xjpmywlm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aaierfuw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nhdwnsov.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pztecarb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3faesiqvr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fvdemxrk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3klwqzueo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rtqhemod.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tlmrwrkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnqumcan.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cuuscpsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nardlkei.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ltiuxvhi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xhwaoeup.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3eqirqoox.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hxczsmlw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3npaguaxk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yutlglxi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vmlnzpxf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vjjumwwh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bedrlihh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ovueccbq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3euqdfzkw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uggdkvls.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdwbnpqn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3svxzsiqe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vqewlkik.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pekbjbuq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ykkszryq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zofqqsxg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aaqgivva.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pskpbxiy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3oiqanhju.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3snilosky.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3sxuorxum.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3awcpkxas.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lqczeein.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lnideent.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gtboicns.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3focttglb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fxkrgnwd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ozvwypfv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3btobavax.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ljuxprpw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qdekrbgg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xvuoyyhp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3kqjvzzuu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wtymeqjv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3icohqkdr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3oayoyqhm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vbakihge.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3woputhrn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wbtniyed.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ifnhonsw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3idhkrabs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ajofrepc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qjuaeylk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jydhhbvm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rhqqcoya.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yanmtaop.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3oakzwdbw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3khplueyn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gwezacvl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfffqoaw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3noiynddp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ikmrbkfh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3phuyqafc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3inpgwilm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3scrcalay.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fkiwdckg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dirtdkna.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lchxolld.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qvxfwbfa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3evrjydli.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cwbxrvhb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3otbsktly.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lpprqcwj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rnoqlths.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3iqytslrq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jjnxecxn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3crpqxqxo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3acncxgws.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3sipnzvjh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yhejkdug.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xvobrckp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wccbbavt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3csleqtrj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nvcatcpi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lvhespwq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvnsltqz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qrthrcqp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lhqrnbjf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3turahzaa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3olvsbinj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hhjdshwk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sssbvpur.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hbgcbmza.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3saogbryt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3esaelhsl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fjopzccv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tsinbeeq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bbthonio.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3phybtlkk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ajyhfgei.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gxilxaqm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tyodgfdc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jpfmpuxc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hsyasnej.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ygfknnkf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucptvsaf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oniraeid.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ztqwzxlm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rsmtparg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bmqyblbs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ejhrlywo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dtjszcso.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zavdltct.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sdsvdrpd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3oghztxev.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3auzrejgr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zzjeplzt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ipspvydu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ozcsqitu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rdmnpqts.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qmcffzic.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3eyhqahki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rlulnuna.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ugceanyl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gmaixtho.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qyfzvlgk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tmbthagg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvnmktbk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3uvgsmzox.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xrjlmpfz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cubinovg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kzozuobd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3czdhwvel.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yozgwhdg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3otktqepf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3glrnbzks.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3eysiepsp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3saumfyiz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zysqhivg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rgfvmzrp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hnpniaoi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3roteiamg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pdfjvoxd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jtjmlqmh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xuxednno.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qnxolugv.html


<!-- 参考信息 -->