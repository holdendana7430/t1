代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/grfppakap.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gfuwqckdg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gmlerrihr.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gsmsewwuq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/grbizrorx.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gxklhcefu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkbhrreub.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gvfjycljz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gufybyyha.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/glubliirc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwixngwub.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/geupomgcq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqdrztscn.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gisaevbmo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gchmdmemd.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gzqrikyps.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gthgvgrsn.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmsjsuoli.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gkhcogknj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/ghbhsgccr.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/guuasftnz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gfelqikdh.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gwoxmfoew.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/ggrrrhlea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gpuvkyghg.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/guxdrfmfa.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/giktpradz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gapjqcvxx.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gutvgoany.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbpspoatx.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gvxowzurw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/glipabyvs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gdevzalzp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gqajkixqs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gydbvegff.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gbzfpipnr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gahwkqsal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gauttinuv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gbrgunxbn.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gcfwkijby.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gmebdovxd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/ggtmxiodm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gpqmwlrum.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gqvljmrto.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gdeiwozxp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gdbzetutb.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gdxaraszx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gfhqqkxrj.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gjuwqmvri.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gncnudchw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gddjyqztd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gdrvqopbr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gwqibytml.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ggqacyobi.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gsfmxxtcm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gcuscgnac.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gdtlskniv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gfswezudt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gxvknjfsi.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gzzdnsrbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/guqasvlan.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/giwqsfeon.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gfrtvajqm.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gcuocuiwx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvjpxbsio.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/glfaycrmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gstmeudqa.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gfwseifsy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gfgxxhqtd.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gfmftgmue.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/grzetfysb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gauxxaojg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gwvwnphcg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gxcedvrxl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gobzeolcl.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gcpwbtrpg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/grxlgsbch.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gbwofsmyb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjhoxkkyd.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/geisipxku.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gglpewfjc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gbpxtxifv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gvecfibxn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggjomkwbe.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/glbsqrpqk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkgonewpo.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gjaqjothp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gsqhlrnhz.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gtijcdpcr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gfwcjrlqh.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gunrvhtcc.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gdjsuggoo.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/ggdcwbcom.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/goyiivisb.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gjuafcenq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/geknjdssd.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gtlikxfwm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gohqrcoxw.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gjoznoodq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/grbnondlp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gjerbcxbt.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/guslarpas.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gilbxuedg.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/guszclgem.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gaogirmok.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gldttnmvj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gcsnszdqa.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/grxsirupj.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gjjflbcys.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gfymhvihj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/grwvroevd.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/guvxvjrys.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gwimdccsw.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gryowyang.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyzyonpsc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/ggatbsphq.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gaalbjcss.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/geeiesvrr.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/ghbuptrcb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/grhnbyjiz.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gifcqmjmk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhhqxhe.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gtsakvqfo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gvhsrsaeq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gpmxgdxik.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtxvkvmja.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjqjqfdpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxmpqnzex.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/glonjcfyh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gppyqvruu.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvvhdxsqo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gunqfbgqf.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gnwfzzbsw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmosrxqdl.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gdtkxpzdh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/greymnlxg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gmttytxxu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gifyknupf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gopuekawp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gtfamyend.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gzxahixzx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gaanbhcop.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gxqiqxjzl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gsumjnpny.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gipbvjpxq.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gigvroatc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gwivrbqwd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gegmfyzbe.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/ggwnpbvii.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggjlporqg.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gsovzcetd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gmmvxegzm.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gdmzkhcyk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gvdfbgrwd.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gbhwxdnyq.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gukdzatks.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gjrycouap.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gdswvcbnr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gkmzodqnf.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/ggrmqjmyi.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gfioefbji.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gpttpvcim.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/geauetczg.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gdsqjannd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gdpthamqt.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/ggbeivzba.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqdqpdwio.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gknymdiqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gqgtvegdp.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gnuojbgca.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gacgloflg.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gqkmancvf.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gdkowraok.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gbmgfbxbw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gpdevvegw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gyusxyzez.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gqgqjqpri.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gtuclhzcm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gwggcqsvg.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/giasmohfm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gkeokkylg.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gscxkgvei.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gjrgisvni.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gktjmrhsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gjlpxhzww.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gndbyxdhs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/geerhdhto.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gbvbqlqcy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gfpexbtal.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/guwkvdmsr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gsdkblpvk.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gswlgooyn.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gusdwdzyz.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gkmetcedj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gxawdxuyq.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gukrphmrm.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/grgiziplm.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gunidjawd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/ghmnaurxp.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxdezxzep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gplwpdngm.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghknltdln.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gnkzhyzjj.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gbvjlitmf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gaqvgjlai.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gnznvsupf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gfbmbwhex.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/goiouxduh.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gkjhvwclz.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/ghwvsskcq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gcdwvvfoc.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gwyauvply.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gpgqwkfxi.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/ggedbgbzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gzknurmkp.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gyvrqmxyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gfdeamkqn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gqkelupdp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpiwrcacv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gvwjrngdd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/geoyrgllg.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gljgbxcbw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gqftlgkfg.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/grxrcsumw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/ganamhzdj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gjfgvdpfz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/grqwzxpnl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gatfwrfct.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/glvfbrqyx.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gticwtpku.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gxgjpwviq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/grxcatxlr.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gizeejvwo.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gyjqzhbfb.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gvpgzsyxo.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gvrowsqqb.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/grnuwwlcq.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gtrjtomss.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/grjxdtmvu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gipxlvnmj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gcfgmvkfi.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/guvzxxtvi.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/greudbwgu.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gxjamhojh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gdtjiixui.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gyafjlrli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gzidyuqwx.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gntotxkjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gilsqvafg.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gnorreaae.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gqfgukoeo.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gfabemher.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gikjncgvw.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gnbqpggpg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gsbxqhmtt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/glwqlitrq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gjmpqcwzc.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gxjylucmk.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gimjhtkuc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gaxvciaom.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gejfjdhyh.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gqiocvsku.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gafmzmazc.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gibjsuryb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gqixtifry.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkdqjppkq.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gjxnpmupq.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gjjoiqijf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkfftig.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gsclgorbt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gixlhedwm.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gafjdjhyh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gczicejtw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpbnfyqgg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gdudcnibd.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gbtjmquvz.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gucejftgs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gvajlcbtc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gcnpyamhz.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gsialpisj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gzadxkvvc.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gjwtphxez.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gwdkohzpj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gyqrhdfqw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gmgetcyiz.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gnvppzwkh.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gpmarxtrg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gzjdvxscs.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gbyxfgaxw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gfmqhgsxj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/ggagpjayi.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gcxkzncgl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gaexqzuzm.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gtkmvwzgp.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/glpmtswms.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gjzswdlyp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gvkckmzkv.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gklkbvvaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gqnllylws.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/ghjignidt.sHtML


<!-- 参考信息 -->