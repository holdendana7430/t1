代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphvapnkx.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdqgsdqg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhwlrlha.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gknastugf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gyuckripu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/glblustaw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgzhoqdd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbhlriim.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkkgqupv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwvzfdjq.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgchubii.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbxrbisr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gkeeceyho.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhmknly.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhjtsyvm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gronhmevg.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghusohirz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvizodia.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/goctoloab.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegqhqstf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghttqpunf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/grpbaedco.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gocadvyfs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzhxqcvz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gwasshjog.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbyohxdn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gukpcnmrj.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmaazodd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gnfayesja.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gksxanbok.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyzbwfup.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gmtyawggr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gcpbzjnyx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjcotrnk.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzudhrxpn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzecaiatl.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/ggdhlqchl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gxtdutyek.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkfjuchwy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gtjhastlo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmtznppd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuqnvijq.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/grusrdkwm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/ghqntuugx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqzqcgkkv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeejxukl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guonmnzky.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/ggbmmfobd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/guyyzqsmq.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/ghlbzogls.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuutisbv.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ggogxzcol.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvvtdkot.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxkwojuu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbetfdkiy.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpfboxo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbzblgoj.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gsuuqvyvp.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gqdwhccsu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ghmcjgslv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gbggtdwmy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcpknkab.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnpezob.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gheaummyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glyjbfjeg.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxwiqoecc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxpsegbb.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfugncrtm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gakgmfuzw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gslpehwkw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gjxdgzjhb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gozyyunox.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gbrykaysm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlcvixlz.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gokcuyubr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gpnhynxov.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyotgrdvc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gawpltpvo.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gswncqdnc.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gdqpxkioo.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzikfyezx.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjvvpjvo.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfqcbbza.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqsmvpx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/golrbyajr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwumwdhx.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnxnuvnu.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvibvapfb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpyqowjd.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzbedswc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gmhhauell.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcdrthge.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrckxmal.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gvijmdypg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgeorgzm.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfdmwzfj.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpuewgrzh.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsxkqyud.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdekettyt.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gwkzyhydz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyecdkakc.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gvxklqdoc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/giwogazkj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobhhkyjh.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gbdjwogml.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodyvpkg.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gkjpmaljq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giobchaff.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gtvpgpuzd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjozcta.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcwipwvn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzikbwyve.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnddqwrys.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glenwlffy.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/grjbiobbr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gluygfypq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmglnfap.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeukrxpi.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaxuhtmc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glpiiiojk.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gjtmfzzsj.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvanczgk.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/grjryhljz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggshsnfea.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiicgfap.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyytrgbqj.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlkdfzen.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gkqvsfbxr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gwuqykzro.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvwffgay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glttsqpln.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghsoskejj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceyzqeqk.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdfsxonp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gbxwnatbk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykznhfha.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ginwoeolk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjomfxmd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqniqiuq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefkigjij.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrletwkk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gibvhxmno.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagknilr.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqfdnsfp.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gzuappmuu.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcpocxdsa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmbnujyn.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/grcpaecjz.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouqiojrw.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclklsgmv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbzqfwbo.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gynmszehr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdpnrtvb.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaimmtnj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqijfhloh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjikwfrnu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzxqeoikd.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gougikwqd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbkennej.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gnhccszsf.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/ggvmwpegw.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbizsis.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gvttuzaks.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzgqibdt.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfpunfcc.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzbvztlw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmdobpfd.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfckwndbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwridhjfb.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gmedfdxao.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsyljrntf.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqychafv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerphosdq.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmmdtxjxl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gskxkvhog.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geepcddzn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glcnbyrcx.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gabtdufbh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/godvhzvfc.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcetwrvo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcbjbhkz.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gtcpuugwc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbivfqtmd.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjtxbnl.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvpbkfxa.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrppbfrx.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gitkfwtfv.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxdmeyln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbtfhuga.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/golldgwhn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjipcxrww.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gyluxcwpf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpsxetwi.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqsdgpal.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfiksbgl.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbatoyljq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziykhiwg.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvuvdgzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gicsvzlgl.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjtroxip.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcwbzddyf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlvkokme.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxqgqvmg.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gttotejqd.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfdgwvigs.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gmqxrflla.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnuabyylv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxvprjg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/glmwniaft.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gpmalfily.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbbwbwpe.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gliemrmqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzxuzuuw.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzxhezztp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpgklccc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gveiyfxqd.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzfpskkk.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtqlxjce.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gcebrkmzi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/giyryspry.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcjuenfox.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gycechcqi.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gopiphosp.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqktlhyo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/guhvoepms.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/govitcmya.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzngcnhv.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsdtiescs.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjpppyrcq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmfnktbh.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/grhggkhbi.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhftiyka.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gpyocaaxo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gseuwgpjy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdifjlww.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gafcujpes.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkziczoyi.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gsipmnnce.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvzfmfxq.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoovalrk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gqvcwugeu.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/grszbakub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdxtiugia.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gbroxjief.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/ghlrndshm.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gmnngdiwq.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbxntlnbi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyvoxevq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/ghvubkwsa.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/guqtwrwkx.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrhgekhs.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawbdgnxg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gohjqriwn.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gpmjalznj.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnfcdznx.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gjkkgrnzx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwukwqns.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/grpugrcdq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdgnnqi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkmookyh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbqdxlbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggqxmkuy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzwynlce.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfqrmimq.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzrkmaao.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduqlnqyz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gsikzycxd.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghztkynpn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblgbpran.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gowiidzqb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfnuykca.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmuwvwro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpimvkfg.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesdmhijr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqtibtah.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuywrzyr.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gdxcirzmx.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghscmmklj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggcpsqqah.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgpzczwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmytqubz.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gpunmwlqy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqhoirin.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gccqhrzpb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacvpgvib.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gqsbpbela.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gciwzdkuz.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gurcdknyq.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gepzdnbxa.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/glpkwzqrh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabchwurs.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbumylwzs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gfuiokuue.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjfvbvaoa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxkswbhm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzwenofr.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gqbxeylgc.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoclpoxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gncprnwri.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/glcwrqsbu.sHtML


<!-- 参考信息 -->