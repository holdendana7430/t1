代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.aibaodan.cn/gtaobwowrn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hongshengwenyu.top/gtqcqibfsy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nwbrower.top/gtemccenlj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnqzz.top/gtcyuxbbvu.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtcmdamvlu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cashguo.top/gtayybpfjr.html

================================================================================
来源：http://hz.jianghu66.top/gtotwjiovj.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtufthzkel.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtujmkmrqg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtldydrqwt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtfypbubbf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.redwolf501.top/gtttzykdaw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtsvoengzn.html

);
来源：http://hz.quarkkingdee.top/gtcznonrre.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtshbpequh.html

CREATE TABLE orders (
来源：http://hz.xuetiantiany.cn/gtrzfupdim.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtycgkxpkx.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtamdwknbr.html

amount DECIMAL(10, 2),
来源：http://hz.jinghuilouyu.cn/gtsnhfjrdz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtcrjpxmqp.html

);
来源：http://hz.yonumen.top/gtlcxuojoc.html

[Q03] 增加列
来源：http://hz.zhijiandao.cn/gtnbtkyark.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtyvlkajoq.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtxedhzyyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gtekzwvbxk.html

[Q05] 重命名列
来源：http://hz.ehwqpu.com/gtiupjvnnj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shuidangran.top/gtxgnolomm.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtygiakppp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gtqqhrynks.html

[Q07] 删除表
来源：http://hz.haohaochexian.top/gtfjdnbova.html

DROP TABLE IF EXISTS orders;
来源：http://hz.birdmap.top/gtwqbzfipu.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtzfszfkrq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtbxsafncj.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtanqmgavb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtkisatkdu.html

[Q10] 插入单行
来源：http://hz.snrcjt.cn/gtmemaxcfp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yanxiufei.cn/gtictqibvb.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtoxzyjstv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtjdxgbbqh.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtcmvkriwl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ivvv.top/gtphizjdon.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hysaishi.cn/gtfkxabmpt.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtsxsmdrgs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhijiandao.cn/gtntjcsiah.html

[Q14] 存在则更新（upsert）
来源：http://hz.daxiang520.top/gtjjrbrlmu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gtwyzwbaip.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtpecwjodc.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gthetzlloy.html

SELECT * FROM users;
来源：http://hz.smart0.xyz/gthogpaemm.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtiigradqy.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtbjghcxea.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtnvypnuxw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.9152youxi.cn/gtlgcqfhmp.html

[Q18] 模糊匹配
来源：http://hz.ivvv.top/gtmgfgvxbs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuanzhike.top/gtguqjbwbi.html

[Q19] 范围查询
来源：http://hz.yj20258.top/gtrbqkqzty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dianchejie.cn/gtbtvwafkv.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gtxlidsnui.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtcmcwzsvz.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtxnlvcfhu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtlwfjqahx.html

[Q22] 排序
来源：http://hz.shzxlz.cn/gttwkqjfqp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangdashe.top/gtnbkrvgyn.html

[Q23] 分页
来源：http://hz.316326.xyz/gtixhbkwic.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xylfe.cn/gtyjafusmt.html

[Q24] 去重
来源：http://hz.jlsjyb.cn/gtbcegksci.html

SELECT DISTINCT city FROM users;
来源：http://hz.snrcjt.cn/gtopaspshd.html

[Q25] 只取前 N 条
来源：http://hz.yj20258.top/gtgtitkvpk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yongpay.top/gtnhcggcao.html

[Q26] 计数
来源：http://hz.nwbrower.top/gtemryoyyw.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtstixugde.html

[Q27] 条件计数
来源：http://hz.ehwqpu.com/gtxzuipini.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jianghu66.top/gtswpegujw.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gtqqwbjyyy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gtlredfkwa.html

[Q29] 最大最小值
来源：http://hz.jiagoushi.top/gtssvzkqvn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtdhynfryc.html

[Q30] 分组统计
来源：http://hz.yvedp.cn/gtyjnktsvf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtdmwuecrs.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtrlnxozsg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtapkdzgjm.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtymrwkmha.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtsonkaaxt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xziqi.cn/gthvqhwgki.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtsdrqcnro.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangshuangyany.cn/gtqpqhasqr.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtvikjcjnf.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gthcvvploa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtzowtmotn.html

) t WHERE rn = 1;
来源：http://hz.hongshengwenyu.top/gtclpfdwqj.html

[Q35] 内连接
来源：http://hz.havefunace.top/gtfmklbvpr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtfterotls.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtebpplubr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gtfsagdqvm.html

[Q37] 右连接
来源：http://hz.tianlin.xyz/gtludssnvn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnxiangtu.top/gtxmgcxzap.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtbtoshafq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tanke756.top/gthvmoolav.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtyndqjyvw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtzeeufwke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sxryk.cn/gtzulnycdl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gotoacloud.top/gtorfaqlhq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuetiantiany.cn/gtigzcpozo.html

[Q41] 多表连接
来源：http://hz.hnqzz.top/gtjnokwijb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cqqwz.cn/gtowqqysbk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yueranfly.top/gtzdcgegad.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgfzy.top/gtuniehioo.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258.top/gtiazqcvgr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtqxjvfnsw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtezkyvahy.html

[Q43] 标量子查询
来源：http://hz.pycfn.com/gtrzxlryac.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fzhhl.top/gtwgyjqias.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtawesvcjg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gtgaiijjls.html

[Q45] EXISTS 判断存在
来源：http://hz.gogol.net.cn/gtjngycaap.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtxfijogwm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sysykeji.top/gtmnvqpjhc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtosnxyvzy.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtqiminsct.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtweoyfygv.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtnnaceakq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtymgwnoow.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtruxvawco.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtkkkybfkp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtvtqrjjip.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gttaovkvhm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yonumen.top/gtohtvstbe.html

[Q51] 用子查询更新
来源：http://hz.hnxiangtu.top/gtjgciivbk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuanzx.com/gtpfaeyrrf.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtxmkxygdz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtbfknrait.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gtorztsrbt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtzuhnkxcv.html

[Q54] 清空表
来源：http://hz.vqdsnc.cn/gtiryskopg.html

TRUNCATE TABLE logs;
来源：http://hz.vqdsnc.cn/gtmhgkbcfs.html

[Q55] 排名（并列占位）
来源：http://hz.nanxuanxn.top/gtlgaxcooy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtpfdcqfvu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hongshengwenyu.top/gtqttmuwla.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tian-w.cn/gtqujrpglj.html

[Q57] 行号
来源：http://hz.xziqi.cn/gttqhqniwu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtpimakoll.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gtomzgxgfa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gotoacloud.top/gtjtvacuwa.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gtazijeqwe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtuiomuplr.html

[Q60] 取上一行 / 下一行
来源：http://hz.hammf.cn/gtkggjyvoo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtihbywgho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtjuaslqhx.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtwoirazko.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jyoumei.cn/gtlcetbyiw.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtrygofcwx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtuapkwyja.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtuarneoxg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fzhhl.top/gtiqnfinah.html

[Q64] 提交事务
来源：http://hz.iojbl.cn/gtpzuluuyo.html

COMMIT;
来源：http://hz.guannengcc.top/gtgxesygui.html

[Q65] 回滚事务
来源：http://hz.gotoacloud.top/gthqbqoqit.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtwmnkqbnf.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtfihdrcay.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtnuctazku.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtyeakadhi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtknafmvgp.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtdutxqkpn.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gtdxotcxoq.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtqjexoyqj.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gtmgyjgajw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtlzojamhh.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gtjfjmgrca.html

ANALYZE TABLE users;
来源：http://hz.sxryk.cn/gtealbfqzd.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtquzzofjm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gttfrzgiic.html

[Q72] 查看索引
来源：http://hz.c1oappe.top/gtrjuwnrmu.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtmnoihppb.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtwlevfkhq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtdxnuhhcq.html

[Q74] 强制使用索引
来源：http://hz.ydzc1.top/gtzsijlapv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ehwqpu.com/gtcpzqglqu.html

[Q75] 日期格式化
来源：http://hz.zycfv.cn/gtogudcmyr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gtuvlchhcw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj202588.top/gtptmnuouy.html

[Q76] 按天统计
来源：http://hz.zdqjudy.top/gtowycnhbf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jyoumei.cn/gteqvyybht.html

[Q77] 时间加减
来源：http://hz.haohaochexian.top/gtwqrgjjis.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtqrxfgjip.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtenofnhlu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.birdmap.top/gtfrgpvhhw.html

[Q79] 字符串拼接
来源：http://hz.nwbrower.top/gtpacnrvbn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtpufhbpbb.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtbnzudalk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daria6918.cn/gtzeioffoj.html

[Q81] 字符串替换
来源：http://hz.iojbl.cn/gtapvgarbf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtoaxajzmb.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtnaoowemx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhongyouzk.top/gtqaoolmks.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtiwjsvhsu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shzxlz.cn/gtnlacjqnc.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtbbbhymxl.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gthitwviyc.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gtqyyaaxmv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtranpvopk.html

[Q86] 读取 JSON 字段
来源：http://hz.sufxvd.cn/gtbfojawco.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtqaoxjrvi.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gttgszlpqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtsdillawk.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydzc1.top/gtvyudbxpf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydzc1.top/gtbksnmpxp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtfyxqoabl.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gthtxhadqj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnqzz.top/gtxmpfukdx.html

[Q90] 生成序号列
来源：http://hz.gzhubu.top/gthibhubju.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigufen.top/gtdwlzibav.html

================================================================================
来源：http://hz.daria6918.cn/gtmuunuwxa.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gtfmconuhn.html

================================================================================
来源：http://hz.yvedp.cn/gtrfcvfzql.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtyhdpwctz.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtlkfcicbn.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gtclsthoce.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtndbhqusc.html

name="Tom"; echo "$name"
来源：http://hz.sufxvd.cn/gtxxrfkdfj.html

[R03] 只读变量
来源：http://hz.jlsjyb.cn/gtewjukrmo.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtmahaisas.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtsceflnlt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtsxgqnwdq.html

[R05] 参数默认值
来源：http://hz.xinyue.icu/gthlzodnfd.html

name="${1:-default}"
来源：http://hz.jiagoushi.top/gtuhydvgpu.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtmrlbkuhq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.316326.xyz/gttijdqbob.html

[R07] if 判断文件
来源：http://hz.dianchejie.cn/gtiggvibjr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtxbritnbm.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtomioqlxr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtjcwhehuk.html

[R09] 字符串比较
来源：http://hz.hnqzz.top/gtxraehirm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtrvdlusnx.html

[R10] 正则匹配
来源：http://hz.yj202588.top/gtgosfkanw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sxryk.cn/gtlphvlbeb.html

[R11] case 多分支
来源：http://hz.yonumen.top/gtuimcmyyw.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtpqlgwzxs.html

start) echo "启动" ;;
来源：http://hz.yvedp.cn/gtftdbmckz.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtdkuzwsxl.html

*)     echo "未知命令" ;;
来源：http://hz.hfpthk.cn/gtudjqyqzy.html

esac
来源：http://hz.zycfv.cn/gtrnrlnizo.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtjlzqtjer.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gthvdgxxll.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtbrjrhjec.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtvqvfhckl.html

[R14] C 风格 for
来源：http://hz.chenjidiqi.icu/gtmbubgdff.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sxryk.cn/gthmuzahbh.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtskznilmd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtlfmumvhi.html

[R16] until 等待条件
来源：http://hz.tanke756.top/gthcyvgtkg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtvcytuasr.html

[R17] 数组定义与取值
来源：http://hz.ydjk.org.cn/gtiuyxdbkg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tianlin.xyz/gtjnlkvmus.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtextgniit.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigfzy.top/gtxnhtdiwa.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtuwgtlkga.html

echo "${#arr[@]}"
来源：http://hz.nanxuanxn.top/gteaswrzzi.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtigrhwfet.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cashguo.top/gtbcrnwlae.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtqbgoyhvk.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtovvnblsr.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtdyxmxpud.html

echo "${s:0:5}"
来源：http://hz.zhengqikj.top/gtzpjxdjzp.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gtvzxghdgn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtepdibjge.html

[R24] 大小写转换
来源：http://hz.dianchejie.cn/gtmmreahkg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gtukayoifj.html

[R25] 去后缀 / 去前缀
来源：http://hz.gzhubu.top/gtvzlbsjmg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gttnvtauwu.html

[R26] 命令替换
来源：http://hz.gotoacloud.top/gtdxboxtlb.html

now=$(date +%F); echo "$now"
来源：http://hz.cqqwz.cn/gtrkizxnbd.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtcxvctfvs.html

echo $((1 + 2 * 3))
来源：http://hz.cdnleiting.top/gtvmqjyolx.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtxbqjczja.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtwtrqymew.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtkzkeelex.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gthqfidkqc.html

[R30] 函数返回状态码
来源：http://hz.gotoacloud.top/gtfaknodeu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shzxlz.cn/gtdlfottup.html

[R31] 局部变量
来源：http://hz.snrcjt.cn/gtumdwvsin.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtrqgjtiof.html

[R32] 参数个数校验
来源：http://hz.tanke756.top/gtejxsieet.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtadtqvxaz.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtjdlzjzgy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtokuaaxfq.html

[R34] 退出时清理
来源：http://hz.jqgfzy.top/gtsdvgjblq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtqrrmevbv.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gtuhoaieiz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gtlgmuhxnn.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtjwurjdqt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinghuilouyu.cn/gtyfdfpexe.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gttfxhpoad.html

files=$(ls -1)
来源：http://hz.chenlongwang.top/gtihpxjxrm.html

[R38] 管道串联
来源：http://hz.tian-w.cn/gtpuzlpypg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fzhhl.top/gteyyqcpqa.html

[R39] 重定向标准输出与错误
来源：http://hz.cucudq.cn/gtxyojdhqn.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtgbicqoyf.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtwbzckwef.html

echo "log" >> out.log
来源：http://hz.aizwys.cn/gtbrnkvvql.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtcibhcjrf.html


<!-- 参考信息 -->