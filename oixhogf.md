代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gblwtmpsr.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gbbwquaov.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/ghvryjyom.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gaqmsceum.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/geqplrcyq.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/garqhiuxa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcjgcanse.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/glkfvercy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/getgvdvld.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/ghjwzbexi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gohswmsrh.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gzelrgucs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gwbofofbb.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gtfvaafhk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggurjmzlf.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gqznxlfbv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gshkfahho.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/ghthoyxep.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gahjeytut.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/giymfazwx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/grvophyrx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/goghjkdrt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/giuqmvbfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gbvcwxpup.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gsxnukoib.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gncvrtyxz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gbfgezobf.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gtmgygkwp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gopjohbsv.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/grpizkdho.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/ggmlyxlyb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gdotlakox.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/grnmzzvvw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gzhkzdyqj.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gkrskjzsu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtsrwvwkh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/geucswpfj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gkpweuyfk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gbmvhgwql.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/guijcjgim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gtkcuznph.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/guzjjipxn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gmjqxhxzt.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gcrjoznst.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gfetogyjt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/godxfvcqq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gcwcozetq.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gcorxhwft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/guzzgouum.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gskxphnbc.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/ggvhhngjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gfvahmnyt.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gowlflkle.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gthhendfl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gcjicdbrg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gjjiurnjm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gnvytozcy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/genyygnsl.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gvbnvdemy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/galmotkpu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gvmorvjmc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gbknucotk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gkjtpnrin.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gjlfuaylc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gtbprojpx.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/guevozwjo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gbcmuvthr.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gxmbvnudj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gjlzbafgq.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gmsdigpsy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gwfumapik.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gxnibcjgv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gkmbhyhgy.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/ghsazvdji.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/guogmpnmd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/ggsfhndqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gmbjqeymf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ghsvbshyr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gaahicwwy.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gycsylwie.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gcukocnsw.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gwnggjprt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwufyudri.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gsitywlpw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gngxnjlqo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gutwwastj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gcmwlyvkc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gotyctoms.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gdjcskpaf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gadbybmrk.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gvgphwcsr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/giviuhvod.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gbkoyvkjq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gikqnpwmy.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gmmwikfbw.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/grspiftwl.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/goxmwbbvy.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gwvttvqtz.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gkapheiuc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gitwghhsb.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gicxouscv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gnalaflng.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gtyfcgzub.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gznimsbcg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/grqxyxkys.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gvuhvaiyi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gjelddkgy.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gmxhqiusw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmcwwzuu.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gxlicgyyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gesaohtlb.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gysjkehwn.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gqvkxywrc.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gfzfxuwzu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gzrmzehyh.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/grjfwxeri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gizqghwux.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gegbyxmky.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyadvucxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gicaskpxy.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gqzuarlfm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gywlzjloz.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gjhaxuisb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gpdbcbwkp.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gwezwwcdn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gkmdmwejb.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gotryelaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gvpvcrgyv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gudweyrga.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqtkevbtb.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/galmejeof.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnomtktuq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gfcambpww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqtmkvkhf.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grevsvjed.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyzxbbjxi.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gbatavzqo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gulldoapv.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gneyvjbvb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gdjptvbvi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gsjgzvkpo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gvaafizom.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/givcvhbpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gwxteiwso.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gujzppmkg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gzxyakbxz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gngkafcuz.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gqfqbtmfg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gbvpganfq.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gtjyroulg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gfvyzgehw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjdhyhhse.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gfhaxeblz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxldoneka.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gbmuttqra.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gatudnbjv.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gltxxandc.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gzazihqap.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/ganpevfqf.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/goakqyjyx.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gedzbemno.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gwncnmlot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gejrrcttz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gdrqplepu.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gaesyinnv.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gqsiszmvm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gdtbrjjsx.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gtcjgkbuo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/ggsanvtmc.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gadnqfywr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/ggpaaktrf.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gyrjokxdj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glbuygfpc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gjrtfupav.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gjlqafusn.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gxpakwepq.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gujtggecw.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gnzbqpeor.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gegbuizcv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/ggeqcqfak.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gzdgcghyu.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gdbebgggg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gihuntfvk.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gcaqcvzxf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqfvlcieg.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/giynpjogh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ghtkecihs.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gltsqyorq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gyrjworyd.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gzrjhxalh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gzlhmpyns.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gplaoeyvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gtulbbhki.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/goyyuxkgt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gtptfpydi.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gccffbebf.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gsoztzpqz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gkoabcrmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gcmwhhbye.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gwcgxvjdf.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/grimhabpt.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ggxuzwiqw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gfakxiody.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gboivnejh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gbpuguzpz.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gcromuwqg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gkartkjis.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gyihkcjxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtiljqmxy.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gczzhiszr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gatjusrjc.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/glmiaobhv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gvcmifnax.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gjiqrnlap.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gieyyqghu.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gxnedqwzu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gtcxdsjdl.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gauojhdai.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gelvkifhq.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gfpskucde.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyljewfjr.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gdsqzdicx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gjfpuqcna.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gihhpiqtl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/glyiwngzc.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gaoujevtx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gasynpsue.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gbnbqfuly.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gchdtnamy.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gvxhgsllf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/giasgdidb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gagdlxxwy.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gdzcwskzs.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gwjoeemoc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gclphuvgw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/ggfkkobcv.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gduovhyai.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gyrtrlyin.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbcpltvqk.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gsbxllglw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gihhodtyb.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gfkixapuc.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjmhixdat.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gvnufsbel.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/glqwtzfhj.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gavobmfkq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gnlxvormf.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gmictzcsf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gvueleloi.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gzdundtsq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gqoewsxgw.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gmbtoqsip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gooqjjcjo.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/garudbmnu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gioxqqruc.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gvosmxduv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gazrzjkzn.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/ggmugsrip.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtwpytkgg.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gzwwxuhgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gdphcvivo.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gqbixvudo.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjyzogwrb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/ggeklkcor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gojiytblf.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gkzmmoaoo.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gjmcvwrry.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjfmtdllx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gmediaxgs.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gantfdunu.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gunatigmm.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gdylzzrea.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gtaaupfix.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gtwzuyvss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gsrpescjk.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gscdqvrul.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gwrvmmxin.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gmkyvwstm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gbfhvbusb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gnhaxdtwi.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gkajjspbv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gamfbcinx.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gyyvoirgj.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gjwguuibn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gktskftxe.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gijalaqbf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gnocuzosv.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/glqcajtim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gdlwunrou.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/glnmpmgto.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/govokacel.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gbcdfyyxp.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gyqgjcdzs.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gspgsvwtx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gfqolvtbc.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/grywxarlo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/ggajcgiyr.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gjvjybpuk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gvyvkzzgr.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gyfnrsppy.sHtML


<!-- 参考信息 -->