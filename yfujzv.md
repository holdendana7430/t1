代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dfsxarkb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pttthlrv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hjfpuuqj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cxrhdwtg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2koghmkfn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qnwjzayi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2prgmnqsd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ojevirkb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2rphfgcqx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fjqljapa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mxhzpiip.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pcvtjkmc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2otpurlaz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2utexyoch.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snnkrcvh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hgehorlo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ekffgztl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zbjkrvfz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nugaxgot.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vchwivws.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rotpvjph.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rocnkbxf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rxlysqsl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tzajsxni.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlnyxygd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ywazatno.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wjotjyux.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lbwjhhjo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iipjxfdz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpgftowm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iswwssjp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2yhzcrdst.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jaqnavyx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jcxgcyrc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2oabnaepe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ncyvfluf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rgmprngk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjoopaur.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ltlflpwe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wdzjiiqa.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xtiytaxj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kyfhuoio.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uwbmxspp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2btvvchbg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zwkyzclg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xcrdpywn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ipqfjxlv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eoxomdmb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2itagkxnp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2cgjdueda.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bjyqvowy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rxkljimz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nuwjwizl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wzgepadv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tdwveeed.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mkjxzowf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ihjoldmh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gtwrnpvn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eerplitd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zxqguqix.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fglljfth.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cjajomip.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kepqnmny.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xmgfzpem.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zgjavqpy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wquljjkm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2shxcwnbx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ahjcjxad.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tzdpfzkj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xzxkdakv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jytpponv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mpoofhdi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofkdhlvu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bfeqjnhu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ilkbgwga.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2huwhuzoi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rksjpmpq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qonnkpop.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qleqbvtq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vtmiqfbl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cavexamy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2uyqzvmun.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zoenbylk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ldowebsl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mcnhdehy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jtoauwjo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gdfdeaef.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bhehxmbs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjecjxmp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kgluoxkz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2diojcotv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2joifnkzy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iqfkdlpn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2aiddgpzf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ppykhhwu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pazgriux.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2iqizglbm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pcdvwwrc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cbacbmqk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uhnuuegm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vgfrgcni.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dlhjpvia.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ewyjepfq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2cohkobfi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yxofzoge.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mheydjqp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nojnfgbo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ysibnpvc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hewfmmge.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2obkiejmk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2reurxzhi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lvfavavd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fbgloyoo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cdgnqxec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hatloqbo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2srnrmbol.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjmdfkum.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2llscawaf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2beassxqd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qwafwcou.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2siddkuyw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tpfmcnpb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2iqvlsntw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uelblfux.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lvavxzzv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gvrqarwo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2igghiymh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2heeuuauv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nakcwvuu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2xvvdtbou.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mkvsmxdj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mbkzwzpv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nugwwtjg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ftgwpuwm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ryhxczof.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wybjbtjw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pfxxumor.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugxootbc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2owtgccxh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iodpimop.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2elkmhkgp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqcfrulu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yhjivkot.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tjeaeciq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pkbjmbln.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqkdnzxg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zlkkgtbg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vrtwefna.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jobtuvzi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hvbufqov.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gykmlbqz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rbjxmwpl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qvbhasqy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2akwamnow.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nahvpmch.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nqniqtjo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rweszmni.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bqtmklxi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mxkbxiud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sotcvnmx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dypwpubm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vewsnxla.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2muesyxoz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2neqgkvtv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2icwtbwzd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2afiyndyk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2sllulfgo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hrdvjjmz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nbpfryeu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ynrfvozg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2shjxmfos.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pgwnazta.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wyodyauh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2btfoxpfm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2emdkprwn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdmjkyaf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xhetpfyh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jbrmmvjq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xmufspwn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sbhkvlcz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qnvffyxc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2phryrlsb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ejactlju.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hylvwzjl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tdtlgybs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ycknsnpu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mzjnlild.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gbpyseje.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zyvqlllc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dyrzutoo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nbnkwrum.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2akpwuovm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhqdpkww.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wefvvfiq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rpgmemnn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2savobhyh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mukmvbtq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2feibnwjp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lvwylade.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2povsudfg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdqoaoju.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mynfuhaf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nyiziele.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wkpdkulf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jkolwgau.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zqluqaod.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2nrobxkfh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2umyjyuvu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbhthjnb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zdmblkdl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwdurbzs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2quarintc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hzvpzyxk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jkbpfzkk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmvplswc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2whejyqum.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qsdnybaj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2byzpslmp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ijclabdy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wmeutybc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jawvgkqc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ysaheiql.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kjodwgia.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivxnprfr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cwtcaqji.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sgbohluh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qzhshkcc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2numqqjvf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bnzgbkrx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lzrvyfci.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hgqkeqmf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hoetiaqo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rnsyxrtb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yhqmxnbd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2shljuzpj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fhsmhmbs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gjjzerib.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dootvyia.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ttsfxogh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2msnrfszk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dcuwxxhq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vvfmbhff.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gkrmlwir.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2svikrtsc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2apaitxhm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fpmgtrus.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2isdvyrib.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kqnmachd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wwockwjw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iwlvpdxm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2priyjpxn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwedkvqr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lnltoplx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2msnqtokb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2erzzurvb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kgqfbvvm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2doutkewv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cshpptok.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cnxfhhyj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2sroefigd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2llrjzhpv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2veopdwza.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2viagyesz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2oloceiwy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pjagukmr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hetydfxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uselxlvz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xctvyyvj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2okermnjn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2yqbedpqq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cslstuxn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rrhahiig.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ejamvkby.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzqofazs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hgbmcocn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jrnzdpqz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pdnovmtx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ikvuztzm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zgrnyqgz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qpgehhlp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cuezlhwa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dodxuusc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2amjozqtb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uhkfdoth.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2azftfrob.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tpmjsaor.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ebyhixdz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yjeuntmo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bkkmjokv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pvcgfial.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hcuvmdub.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2obhzdobt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wvujfvca.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ysvpmmej.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zozfhxde.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zyewodys.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rwoltbpy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2omygzeed.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cgdaovgj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nlogopqc.html


<!-- 参考信息 -->