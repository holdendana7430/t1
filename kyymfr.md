代发 wailian999

);
来源：http://hz.zhongyouzk.top/gtwzyswtyt.html

[Q03] 增加列
来源：http://hz.quarkkingdee.top/gtmjyyarhu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtzmbxodpq.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtgbovznsa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.iojbl.cn/gttousnmex.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtzhhhlmfr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.316326.xyz/gtkdmsyptd.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtkqzpamak.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daxiang520.top/gtwymybwbp.html

[Q07] 删除表
来源：http://hz.shuidangran.top/gtorpwttzz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtnasvuzrb.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtpkrqgzlz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtjwqiomwt.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtujsimzsj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuanzx.com/gtncoagibf.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gthzpwqdxg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinghuilouyu.cn/gtifzkmpha.html

[Q11] 一次插入多行
来源：http://hz.wangshuangyany.cn/gtshbsoujf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tian-w.cn/gtsqielomb.html

[Q12] 插入后取自增 ID
来源：http://hz.yangfankeji.com/gtowjsmkcn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dianchejie.cn/gtrznhljfm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhoulong.xyz/gtpyqygmna.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gtgnqlarqm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gtcswdbcxs.html

[Q14] 存在则更新（upsert）
来源：http://hz.ybcxt.top/gtgsmljpcg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hysaishi.cn/gtsjkkfaah.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sxryk.cn/gtuvbvnbck.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtfxyrzgys.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gteenhbhxy.html

[Q16] 查询指定列
来源：http://hz.ehwqpu.com/gtocbmisrp.html

SELECT id, name FROM users;
来源：http://hz.hnxiangtu.top/gtluobhmmp.html

[Q17] 条件查询
来源：http://hz.cqqwz.cn/gtkxdmkknz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtmaqlrcth.html

[Q18] 模糊匹配
来源：http://hz.zycfv.cn/gtkejfjjsk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtbaxqhthe.html

[Q19] 范围查询
来源：http://hz.jlsjyb.cn/gthdejheyg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.kuanghao11.cn/gttctluwql.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gtjxtlvusq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtotetnfvn.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtywzddyln.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtkqscaase.html

[Q22] 排序
来源：http://hz.birdmap.top/gtghuzpjij.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtcrbitbem.html

[Q23] 分页
来源：http://hz.dianchejie.cn/gtupcwlgbs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtpotoobun.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtbyxsxzzr.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gtzojajttf.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gthqvhmsji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtcgkmeanf.html

[Q26] 计数
来源：http://hz.havefunace.top/gtyrmvhlem.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpaprfhsy.html

[Q27] 条件计数
来源：http://hz.ywan-chungtsiang.top/gtgdjcuapv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtfdgufsqs.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtgtjswfwr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cucudq.cn/gtlcoolvie.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtpuslypao.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenlongwang.top/gtcmalsvjz.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gtlaqiyfdj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtrxqmgpfp.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gtnvyrulbr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtzucpxxkn.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gtfeafmzzl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtsigjvbri.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gtzvemanwf.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtdwzkbcmn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtyvllexeo.html

[Q34] 每组取第一条
来源：http://hz.hnqzz.top/gtjkghwyjm.html

SELECT * FROM (
来源：http://hz.aizwys.cn/gtiykwrrdw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenzaomai.com/gtnwtvxpce.html

) t WHERE rn = 1;
来源：http://hz.yonumen.top/gtkswcdjpq.html

[Q35] 内连接
来源：http://hz.dianchejie.cn/gtigikywxu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtefkvorcz.html

[Q36] 左连接
来源：http://hz.haohaochexian.top/gtbcourvff.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtibmyhqss.html

[Q37] 右连接
来源：http://hz.shanyushiyangtech.top/gtvtwcueir.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cashguo.top/gthhajrwij.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xinyue.icu/gtuetzgxpl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtubnyiziu.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gtruavqirr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gotoacloud.top/gtxfnqhhwq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgufenzy.top/gtqbnqoqzr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sxryk.cn/gtsineifxr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gthubuztqx.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtblskutqx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fzhhl.top/gtwsqlxxzp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gtljwfjcyx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gtyljhttdt.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtlowgiskj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zycfv.cn/gtnythhbbd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtvyywjmoi.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtdiripszn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guannengcc.top/gtokcxmmrv.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtklmwosou.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ywan-chungtsiang.top/gtsszapcwd.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gtkrhkdofd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtybsbsnui.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtzmvfbakp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtzwuylgxq.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtboehydxy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenjidiqi.icu/gtpqrqbnyo.html

[Q48] CTE 公用表表达式
来源：http://hz.jiagoushi.top/gtmxutbeve.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shangyingyoupin.top/gthvpabhlp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guannengcc.top/gtdxdqxaoi.html

[Q49] 更新单行
来源：http://hz.shanyushiyangtech.top/gtvrwglnmj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtczfdkejw.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtfkzktrkt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gtetozdabp.html

[Q51] 用子查询更新
来源：http://hz.hysaishi.cn/gtrbbnnyqb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj20258888.top/gtpouddxxw.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtohqpklbj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtjmyupqhf.html

[Q53] 按条件删除
来源：http://hz.ydjk.org.cn/gthnbjkqoi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhixingplan.top/gtqrbzgiqy.html

[Q54] 清空表
来源：http://hz.zycfv.cn/gtxknjamly.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtbsphrpyq.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtgdtexork.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtftrbmmek.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtdghbbrqm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.meibo888.top/gtpbatdjla.html

[Q57] 行号
来源：http://hz.pycfn.com/gtkreoghob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gtmimzlmfu.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gtmtropxgw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtmncrrwdb.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtyzoyimbk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtfcbfnbzm.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gteonhidst.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhaomingkeji.xyz/gtlgixvolj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yongpay.top/gtcxfqohss.html

[Q61] 移动平均
来源：http://hz.hongshengwenyu.top/gtqzvbhzmb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtvhxbvkqx.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtvjyshycg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gttovjfrmi.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtbeaifbzv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gtwubjylop.html

[Q64] 提交事务
来源：http://hz.yuxming.cn/gtckrkpney.html

COMMIT;
来源：http://hz.sysykeji.top/gtrkhkriji.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtztqtazof.html

ROLLBACK;
来源：http://hz.zhongyouzk.top/gteuvzoioy.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtzrxujqfj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtvqeldqlv.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtzggscnum.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtgsvfrwra.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtbtoqdsln.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtkkxbxhwj.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gtrvirgxjt.html

[Q69] 查看执行计划
来源：http://hz.9152youxi.cn/gtgxdhdyhz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtejfwuftt.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gthafmgsgp.html

ANALYZE TABLE users;
来源：http://hz.gotoacloud.top/gtfsjetxkw.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtiehgmtgw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj202588.top/gtilierddv.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gtxdywctmw.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gtysmhrjnb.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtyulutfbf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gtxhfiibmy.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gtxitqxvkk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gteqrddrih.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtciiwqcdc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aibaodan.cn/gtgtoepzqx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jianghu66.top/gtmzpubhwk.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtjpiozgzi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.iojbl.cn/gtsgsxfqai.html

[Q77] 时间加减
来源：http://hz.gzhubu.top/gtregtjqfc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ppjwa.cn/gtweevkjkd.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtiysglouu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gtvumfzuze.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtudvpowrg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gttvotntdo.html

[Q80] 字符串截取
来源：http://hz.wangdashe.top/gtdigqlfiw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtpfioscep.html

[Q81] 字符串替换
来源：http://hz.quarkkingdee.top/gtzzgjzick.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtcmnzhiio.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gtqbozzlcn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtovohpsrg.html

[Q83] 大小写转换
来源：http://hz.jlsjyb.cn/gthqpyexyu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.meibo888.top/gtuzypawml.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtrqtmrgja.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gtwgxyfrjq.html

[Q85] 数值取整
来源：http://hz.xziqi.cn/gtlfsxnhsg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtpwcailvs.html

[Q86] 读取 JSON 字段
来源：http://hz.ywan-chungtsiang.top/gtaboytikb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zycfv.cn/gttdhfdixe.html

[Q87] JSON 字段做条件
来源：http://hz.yuanzhike.top/gtudppxfwg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtznzshcxj.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtwolbsjiq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtwkiahxpl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dianchejie.cn/gtbohsynta.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gteborebrv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.mhx1999.top/gtkcaliisw.html

[Q90] 生成序号列
来源：http://hz.yj202588.top/gtfwctnkxx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtnhkxfkfe.html

================================================================================
来源：http://hz.zhoulong.xyz/gtguhgkljw.html

R. Bash 专题
来源：http://hz.zycfv.cn/gtdfsrbzdu.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtruqtwwui.html

[R01] shebang 与严格模式
来源：http://hz.havefunace.top/gtyywmtiuw.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtuwmannbh.html

set -euo pipefail
来源：http://hz.nwbrower.top/gtwcbvgfru.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtndhtnatp.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtdrvegstz.html

[R03] 只读变量
来源：http://hz.tianlin.xyz/gtklrycxwa.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gttsgvhyeh.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtdrnfnztj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zdqjudy.top/gtrqvoabfb.html

[R05] 参数默认值
来源：http://hz.yueranfly.top/gtsogxyror.html

name="${1:-default}"
来源：http://hz.meibo888.top/gtpgzxgait.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtlrnimppn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtdhnytajk.html

[R07] if 判断文件
来源：http://hz.meibo888.top/gtuvzsxlud.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigufen.top/gtrfdrdtxm.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtkwccjsuh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtiofvzxyy.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gtybqqlhrl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtvqsljmsl.html

[R10] 正则匹配
来源：http://hz.guannengcc.top/gtmsduqvwa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtkjwjmbyu.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtpbofagjm.html

case "$1" in
来源：http://hz.9152youxi.cn/gttwomlsib.html

start) echo "启动" ;;
来源：http://hz.hongshengwenyu.top/gtugfdsrpt.html

stop)  echo "停止" ;;
来源：http://hz.birdmap.top/gttpfruyyw.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtbzwofozt.html

esac
来源：http://hz.yj202588.top/gtnwsyadhd.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtteumghvi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zycfv.cn/gtlriokuwl.html

[R13] for 计数循环
来源：http://hz.cdnleiting.top/gtpdwcxtjq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtbygqaplk.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gttvbxmdmx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtfabzjqzu.html

[R15] while 逐行读文件
来源：http://hz.shzxlz.cn/gthxshduwr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ywan-chungtsiang.top/gtmpmhcfxy.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gtgghzazjs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtlkkukehp.html

[R17] 数组定义与取值
来源：http://hz.zycfv.cn/gtrubigrao.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtdcnggbee.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gttbenitzf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtpoacjfbh.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtwlwwhfsy.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gtrslldsbg.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtyejfrutj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.andypj.xyz/gthjlgmebe.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtoppezegb.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gtjzjlcpwm.html

[R22] 截取子串
来源：http://hz.sufxvd.cn/gtikpqccco.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtlvhkfnxi.html

[R23] 字符串替换
来源：http://hz.sxryk.cn/gtrxfrfaoz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtmarhbwij.html

[R24] 大小写转换
来源：http://hz.iojbl.cn/gtzhfzcuwz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtgmsdlpga.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtjsvqvvej.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangtech.top/gtijamtgmy.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtjjijirge.html

now=$(date +%F); echo "$now"
来源：http://hz.gzhubu.top/gtmhvreqgm.html

[R27] 算术展开
来源：http://hz.jqgufenzy.top/gtjlioyxiz.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtbapsjwap.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtxzekslce.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtwedcyfvy.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtpszvyejr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangkeji.top/gtmeefiwsx.html

[R30] 函数返回状态码
来源：http://hz.yangfankeji.com/gtzrnyppyr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hysaishi.cn/gtccxgingr.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtjjispkex.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gtwcwgttbn.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtnvnnvgpa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nwbrower.top/gtyvhgtvdj.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gtpsvokgpy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gtcgoajdsh.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtbaomvhpr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtytipqjhh.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtgvpeztck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtfdcvgruj.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtqpkpihfj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhongyouzk.top/gtzhfqwgwh.html

[R37] 把输出赋给变量
来源：http://hz.cdnleiting.top/gtaousnkiw.html

files=$(ls -1)
来源：http://hz.nanxinkj.top/gtogocbrjx.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtezytmsiz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnxiangtu.top/gttinzwouy.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtmfgeovcu.html

cmd > out.log 2>&1
来源：http://hz.haohaochexian.top/gtjngvhubz.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtrznscapn.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtffrnbysl.html

[R41] 丢弃输出
来源：http://hz.tanke756.top/gtmhbaoogt.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gthcoawknr.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtygqemkvk.html

wc -l < a.txt
来源：http://hz.dianchejie.cn/gtcfgincvl.html

[R43] 按名字查找文件
来源：http://hz.zhixingplan.top/gtrhxwzlxd.html

find . -name "*.log" -type f
来源：http://hz.svipenyu.cn/gtyrhbmdst.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtqatlfjti.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtxqqiafid.html

[R45] 批量删除
来源：http://hz.gotoacloud.top/gtdvsntlzg.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtpcltsupi.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtjmgeejet.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtpddtbowy.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gtqqzjrsvt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenlongwang.top/gtudjsermv.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtbhocrbmz.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenlongwang.top/gtuxoxnfdy.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gtioggdsni.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtvvtlxbpq.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtsserievb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtxfttfiue.html

[R51] 排序去重取前几
来源：http://hz.feifeiyinyue.top/gttygyxvwb.html


<!-- 参考信息 -->