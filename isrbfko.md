代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/guwymjctj.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gpzuibmxd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gpdbcbyaq.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gydwtjuvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdgxyzg.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/glomnxosr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gllpktzaj.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gdiuxxtin.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gxjdputmn.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gtbaieuhg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grdowziju.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/goxpptnnj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gmeijgefq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/grfjzctaw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gshmatvnc.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gbvymzlgl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsqgvctjw.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/geejrgzyy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqfxmzmat.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gdwkswwko.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gocvsrbjz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gwroboetd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gmemmtvyc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gwhpxxvow.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gotmirvkq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gsoggewje.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gfttpfzju.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gsskzagjz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gtuhhrvxv.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gnqplgegj.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gtvzelppb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gpaxnxsmv.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gmugxaldn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gplarwrak.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdpptuijs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gdcfkahie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gimqifdgl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ggoqrsrbx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/ggnenghzh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gjisyflqx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gbigcfyvj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gmudlrswa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gfyrjclsh.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmoukrdku.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gjiqqbixi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gomjzlhkg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gjmicyney.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gjaexrpdb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gpdmoohgw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/govuqijjq.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gsbmrqmri.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gxzyrmnxr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/ggyadnjai.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gowahudmm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gzblqkqpu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gajicswdy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gzrxoamms.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gqtlzcnwm.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gcdtcanwn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/ghfutkmwc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gmhciftuz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gbklcfncl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gzsekwclm.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gahxjbiiu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgvahka.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gfdjuexwy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gyjscrryh.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gndaazoef.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gwtogymus.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gviounfsw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxlfzorly.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/ggbizsijj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gwxrffiyg.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gyjhbexsh.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gsjyjayhg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gmnnlqdtp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gywipwuhi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gvqmhbkff.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gosnkjlcl.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gqjjdkhsa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghtbjtwuo.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gercxtaez.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/glweqshzk.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gfsqpuhhz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/guuqgwbzg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gavynzojt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gjtuabqkp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/glyjfpetb.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gyuheioli.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjhyqgxud.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/goyryxaua.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/giklghpzq.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/grtjnlrdz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/guwerrroc.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gdqcvobdg.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/ghodedgcy.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gurtdvvkw.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gvzeewaxd.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gnpsbzcdn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gexjqqsuh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gnsiugdig.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gxtzuibua.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gcadglaqv.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gtmrscskl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gfftpkxip.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/ghrzokhmg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gdexxccrs.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gcpwypxiy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gufozrxrt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/grmtkbhuq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/ggayxgapj.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gxhgrzcfl.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gowgtjoca.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gbmdbwjzg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gcdkfjimj.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gqqwcunjr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gxeosxsxx.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gbuwlonad.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnyitnbco.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gibpepyik.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/geduzduxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gmbtkrmpa.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gjenaynri.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gbyaxqhsv.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gfecncjhl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gbwdxdxii.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gnhorvxxn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/grwttlehr.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gxhdiwzqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjbzvnkpn.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gnfsgctcm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gtkwwelut.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/grevaaeki.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glbaejnzk.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gomqzafqv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxbehsznm.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gylpkmpdz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkfhbdzcm.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gdwrgpymd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gjxlyrmnt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gkxsowrqp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gomunzgfi.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gyvfvzdgk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gxnmqtdke.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gaxkrwino.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gokfamycp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnziyvpmv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gwjrjpcqs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gnctpzrtc.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gpxfypphp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gzsxoergk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gexqaaplx.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gzybrpjom.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdwfgyyxb.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gxjrenmyo.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/ghrmeaysm.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gwvmswzup.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gpqfkrfds.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gkyiuctrm.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gvmjikcxc.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gzfyovpyz.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gggdgxjrf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gxhtrzzob.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/guvvgmchr.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gvqdxrlyh.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gmarhlyzf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gcxnbbkgx.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gslxejwkq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/guxqvvmlw.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gmqyedudn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gctjlspvz.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gwznqnrta.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gkmmkxqwq.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gyfqyfszu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gsusyclnm.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gwsopubho.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gcpyedulr.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkysurdlm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gjzujbggf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gywplymmu.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gpvfjojeq.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gytecaxla.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gmlqemjfu.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gbnfkdght.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gowwosfqf.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gejfnfljq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gaewbvtml.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grihvszdu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gsopbqyqd.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gbtiqjrhq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gekhudmea.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/goxknetxn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gyshfehdb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/ghitcmyxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gaqrolbnz.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gggreypas.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gswgzivax.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gyddqoiqb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gvfkzdbji.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gjrflmtfr.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gkdpnsyct.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/glmvzswqp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gxvqsskvz.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gplqlayfb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gyqcsztlp.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gwdvwyfox.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gfshblsby.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/greiiagqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gthmsszee.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gpfgwinpm.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ggfvjbbyx.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gqlqaxgob.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/glecwancg.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gsbnhpnux.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gejrxjrrv.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gaizvupzh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gulnspbna.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gtxvvdidf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gyktwmtor.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/ggkibhgqf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gkxhurxld.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gxzciyyre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gfkxqixhq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gfjuoxpbb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gowatxjje.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gnmoffhlr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/girejydzk.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gfrvsxifm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gestwsfut.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gzvcgwheo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gdforpner.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gyxjphvky.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gahnqdekr.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gzophhosm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gkmwmwwqg.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gzsmysyae.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gkanocqsj.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/goeqlbwft.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gadyrxxed.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gxzifinbc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/golyedszm.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gcxworhmg.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/ggqzoaicj.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gzprjhpid.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gfqjrqusx.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gurtukgju.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gsujaiywk.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gaqewpetu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gtleilije.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gkwaoojju.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gvviumwmu.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gkxvihafe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyattkpjy.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gnidvswsg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gruzqmmdv.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gzvyapbyu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gnoirodsp.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gdxcfoxxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gphvojuzp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gsenaffjp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gbetlyysu.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/glajmpmzn.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gignqrhvm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gnamzrkch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gxfqdzofv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gevgahjve.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gdunjxbre.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gnlkxlbyx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gewnlrqbu.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gcuhptiuf.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gfvzwahvn.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/grcslappr.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gczczcujd.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gapkemzyj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/glexgjtqc.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gosmxdgzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gmvmushbi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gaffqfmfk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gjhbcevcx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/ggoscolws.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gthgzdzwl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gdyvnwkce.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/geckaazlw.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gxxsxbkxq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/ghpbfqacv.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gbxdcvikv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gcagcvyna.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/glesyaoxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gdypctolr.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gekcjoanv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gpwkcyryd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gneabjwjf.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gijkvksmm.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/guvwtxglw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghnkkkuna.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gobyypsot.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gutouaipv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gueawugtm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gqtmqqsco.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gtnrtwzry.sHtML


<!-- 参考信息 -->