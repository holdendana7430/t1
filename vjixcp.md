代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ybcxt.top/gtkacpaixo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gtjmapscin.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtntvxicrn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtyhzgdrhe.html

================================================================================
来源：http://hz.hysaishi.cn/gtlsubclmj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtukoehbkh.html

================================================================================
来源：http://hz.chenlongwang.top/gtpvpkxmwr.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gtnowyjdqp.html

CREATE TABLE users (
来源：http://hz.sxryk.cn/gtcnnlvgqn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtnnlffase.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtzpsydrqw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangtech.top/gttsnfvcdj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtcrbhaotv.html

);
来源：http://hz.xziqi.cn/gttmszmvwk.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gtreusrkpn.html

CREATE TABLE orders (
来源：http://hz.yvedp.cn/gtvswwhzyx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtydjuohhd.html

user_id INT NOT NULL,
来源：http://hz.xuanzx.com/gtmruadtno.html

amount DECIMAL(10, 2),
来源：http://hz.yueranfly.top/gtjpgvnryw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtgwrezsts.html

);
来源：http://hz.gaohongyu789.top/gtiingdmhz.html

[Q03] 增加列
来源：http://hz.yangfankeji.com/gtdftsrpwl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnxiangtu.top/gtpccpjeqp.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtrbczumrm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yueranfly.top/gtkgzylxqe.html

[Q05] 重命名列
来源：http://hz.birdmap.top/gtaninaqkf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gttcvefsyn.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtuvualbfh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgufenzy.top/gtbhvoufni.html

[Q07] 删除表
来源：http://hz.yanxiufei.cn/gterxagfum.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhoulong.xyz/gttnsbrswz.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtllfxtyjn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gtvmihhcuv.html

[Q09] 创建唯一索引
来源：http://hz.vqdsnc.cn/gtzsfiwdns.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtmwuwykef.html

[Q10] 插入单行
来源：http://hz.hfpthk.cn/gtulsenduc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtdbosrfyy.html

[Q11] 一次插入多行
来源：http://hz.tian-w.cn/gtuadfzofj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.bjfxy.top/gtegpvbxlq.html

[Q12] 插入后取自增 ID
来源：http://hz.gotoacloud.top/gtzkjszozq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtpjaznbes.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtbpljvogt.html

[Q13] 忽略重复插入
来源：http://hz.smart0.xyz/gtmpnacxvh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daxiang520.top/gtfztyppqu.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gtkfrrycmx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtvcnuvdlc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtoxpshzki.html

[Q15] 查询全部
来源：http://hz.hfpthk.cn/gtxfzzfcte.html

SELECT * FROM users;
来源：http://hz.shuidangran.top/gtzybmkykv.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtafdvrlfr.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtadrikyhn.html

[Q17] 条件查询
来源：http://hz.shuidangran.top/gtklyayalc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hammf.cn/gtwmlnpkxl.html

[Q18] 模糊匹配
来源：http://hz.yonumen.top/gtrzcwsafc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gtnmtrjuju.html

[Q19] 范围查询
来源：http://hz.ywan-chungtsiang.top/gtdavrcooc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtgiwxwnmz.html

[Q20] IN 列表
来源：http://hz.yvedp.cn/gtwphadyea.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinyuanbaomall.cn/gtasnfkqsb.html

[Q21] 空值判断
来源：http://hz.hnxiangtu.top/gtnduwxxzv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtvwfmjxfp.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtygyucaiv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.quarkkingdee.top/gtlvdxswxi.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gtdlprcrai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guannengcc.top/gtsvseawvs.html

[Q24] 去重
来源：http://hz.wangdashe.top/gtmmklrnbj.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtjlwgplod.html

[Q25] 只取前 N 条
来源：http://hz.dashuyun.cn/gtutipqlpx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtjnjhrzeh.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtytkvuwon.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258888.top/gtujebhgsw.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtgpwmrpcd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhijiandao.cn/gtixmkqcnl.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtgqwtkebz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gttdffcwby.html

[Q29] 最大最小值
来源：http://hz.cashguo.top/gtnxbzaeem.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gtbdibnpqe.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtjfuulamc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtwopjvhah.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gtvgndbzvd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtccczfyya.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gtmkoehueo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gttbwgcmbr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fzhhl.top/gtxpuncvps.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtwqdardil.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ybcxt.top/gtunkbafee.html

[Q34] 每组取第一条
来源：http://hz.yangfankeji.com/gtbxyqmsxp.html

SELECT * FROM (
来源：http://hz.snrcjt.cn/gtybgiiszo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ywan-chungtsiang.top/gtrgptmjof.html

) t WHERE rn = 1;
来源：http://hz.shuidangran.top/gtkwpgihzv.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtmmfwstcw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtplithren.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gtjpvtoaem.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtxkjmvjfl.html

[Q37] 右连接
来源：http://hz.snrcjt.cn/gtoqwswfbr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtfojbsudf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuanzx.com/gtxqxsbjxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aibaodan.cn/gtpltxmsqi.html

[Q39] 自连接（查上下级）
来源：http://hz.hfpthk.cn/gtqpyjkdyj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xziqi.cn/gtteeyfdia.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtexsaaiuc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gtgtpgxapd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yuxming.cn/gtcfpqrrvt.html

[Q41] 多表连接
来源：http://hz.jianghu66.top/gtbxyyhgwd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xylfe.cn/gtdpyjemtk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtnjhodkeg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.haohaochexian.top/gtmandqfhn.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtswdajpnm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gtnhosgcjk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtghwrgllo.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtszvtmtsd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.haohaochexian.top/gtgnugiryq.html

[Q44] IN 子查询
来源：http://hz.sweek.top/gthoxbfzjf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgfzy.top/gtacddwvqu.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtfiexgesa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtuhaiaxei.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.snrcjt.cn/gtiwqlqtkt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtzakzxmvm.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtqcjsqdsi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtjgzyyxst.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtszuavlux.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gtlefntkpv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtytxzbwdv.html

[Q49] 更新单行
来源：http://hz.316326.xyz/gtxtxwqmfx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtctqgmrhe.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtapmchydu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.quarkkingdee.top/gtzzdyjuez.html

[Q51] 用子查询更新
来源：http://hz.fengsongda.top/gtzquzhwdw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtuppykfog.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtcboqdbyq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtfgywnwbv.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gtgdjulfef.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinghuilouyu.cn/gtdzpcqnml.html

[Q54] 清空表
来源：http://hz.tianlin.xyz/gtlrtfdvfx.html

TRUNCATE TABLE logs;
来源：http://hz.jianghu66.top/gtozwenrqz.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtnnmsmppa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhixingplan.top/gtkatttqfg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigufen.top/gtjfkyxnmc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yonumen.top/gticeypmto.html

[Q57] 行号
来源：http://hz.daxiang520.top/gtocajqanb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtjroxmjhy.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtxbhlvztx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtbcgfldun.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtfebjgpbj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gtwocnjbmr.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtwrgwcsdp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtzkglverr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtfcemupnq.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtzpignmcc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenjidiqi.icu/gtwejopumj.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gthrsmbwra.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtigostozj.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtdgvxvjix.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.meibo888.top/gtaumnnylg.html

[Q64] 提交事务
来源：http://hz.aizwys.cn/gtazkstjxu.html

COMMIT;
来源：http://hz.daxiang520.top/gthyoqfgoh.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtflkxbpzh.html

ROLLBACK;
来源：http://hz.dianchejie.cn/gtdzydcxrh.html

[Q66] 行锁查询
来源：http://hz.ydzc1.top/gtthxenxmq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtdaubbqrt.html

[Q67] 设置隔离级别
来源：http://hz.hongshengwenyu.top/gtaymqvfrf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtpkizckey.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtbpwvbjap.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtfabxpvrk.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtlzrrysrf.html

[Q69] 查看执行计划
来源：http://hz.cheryme.top/gtzzpefsbm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gtmbruagvc.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtzooaohno.html

ANALYZE TABLE users;
来源：http://hz.chenlongwang.top/gtzexhznim.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gttotmagbc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gtpptyaudc.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtykccezxi.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtirtqvehd.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtucavskap.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gttmcdxccl.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtauffatxw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shuidangran.top/gtjyldwavo.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gthiolqsqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtvgmzxccb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gtzuuttryh.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtufjxvihf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sweek.top/gtwyrbotfk.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtyrovwbbq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtpdashohs.html

[Q78] 当前时间
来源：http://hz.cdnleiting.top/gtmvwfhsex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aizwys.cn/gtdqmmohun.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtwyvizrhl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yanxiufei.cn/gttgetnear.html

[Q80] 字符串截取
来源：http://hz.ybcxt.top/gtaxvahdgw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtdsidzrcr.html

[Q81] 字符串替换
来源：http://hz.jiagoushi.top/gtjjqkcyix.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xziqi.cn/gtqszrwosu.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtkejprfgu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.mhx1999.top/gtohdfsehi.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gtrzvrqaqz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtkcdrrtur.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtlufapnzw.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtdlviexmv.html

[Q85] 数值取整
来源：http://hz.nanxuanxn.top/gtynmpppza.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtpjdogogi.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtmxdcyrxj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangshuangyany.cn/gtrxonukkv.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtiwmeuafa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtgjxqispd.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtfiafmpnw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxinkj.top/gtefvfrakw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtqczeqxtz.html

[Q89] 判断表是否存在
来源：http://hz.316326.xyz/gtaoitgpfl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cashguo.top/gtanurumdb.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtuiwtahnr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sweek.top/gtkslbdzfj.html

================================================================================
来源：http://hz.yvedp.cn/gtmefevvam.html

R. Bash 专题
来源：http://hz.cheryme.top/gtgdqbbxbz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtreasotxp.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gthovrhtui.html

#!/usr/bin/env bash
来源：http://hz.dianchejie.cn/gtdsvnnbto.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtnjumqlvi.html

[R02] 变量赋值与使用
来源：http://hz.chenlongwang.top/gtwpzitygm.html

name="Tom"; echo "$name"
来源：http://hz.jyoumei.cn/gtlkwdgcii.html

[R03] 只读变量
来源：http://hz.wangshuangyany.cn/gtocbpkkzm.html

readonly PI=3.14
来源：http://hz.yuxming.cn/gtukszqpyb.html

[R04] 位置参数
来源：http://hz.xingfuxueyuan.xyz/gtpldeclnd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhiwuduotai.top/gtyisogaaw.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtsilykkpo.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtsfukdrkn.html

[R06] 判断命令是否存在
来源：http://hz.jinqigufen.top/gtteqtytca.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtfllbxcux.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtywmprvqd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtuxnitztv.html

[R08] 数值比较
来源：http://hz.xziqi.cn/gtrtsvsmlo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtjjeospjv.html

[R09] 字符串比较
来源：http://hz.yuxming.cn/gtfiphjnfd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtimuugjhp.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtwfnoqdmt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gttqsofpid.html

[R11] case 多分支
来源：http://hz.yangfankeji.com/gtdvtlfvbu.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtnkdsyzyf.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtyhlfcklg.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gtynzpphlk.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtuyrixrhw.html

esac
来源：http://hz.ydjk.org.cn/gtgdfqzukf.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtlsqsxrjd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gtnlwrttjp.html

[R13] for 计数循环
来源：http://hz.tanke756.top/gtcgorhhkd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtdjxdqdbj.html

[R14] C 风格 for
来源：http://hz.haohaochexian.top/gtihmhcyks.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.316326.xyz/gtmnfkrvgt.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gtakdbyhfe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtrvxupxvh.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtmksbzovt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtmreoylmg.html

[R17] 数组定义与取值
来源：http://hz.cheryme.top/gthejlyeds.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gtggovevgj.html

[R18] 遍历数组
来源：http://hz.yj20258.top/gtanrdgnvl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinyuanbaomall.cn/gtjyfcihnk.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtxdcmldpt.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtosnjmyjv.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtfkapdoar.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtupessimc.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gthmoifkqm.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtszgwdoin.html

[R22] 截取子串
来源：http://hz.yanxiufei.cn/gtleppjdwx.html

echo "${s:0:5}"
来源：http://hz.xinyue.icu/gtclstnryp.html

[R23] 字符串替换
来源：http://hz.zdqjudy.top/gthflvkrru.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtrmmkqrtf.html

[R24] 大小写转换
来源：http://hz.ydzc1.top/gtnusmurio.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtvdbpcpjp.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gteflmsnsj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gtlldegatj.html

[R26] 命令替换
来源：http://hz.bjfxy.top/gtddrlgtsb.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gtqlpvxgtp.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtviibtaaa.html

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtjtjsengo.html

[R28] 浮点运算
来源：http://hz.chenzaomai.com/gtkzpuxfln.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtplzogllt.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtjoaiejge.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtsiodpeat.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtrxwcdymm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtdgxreqsq.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtwubkakno.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtqtkpvoaw.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtmtdctqxp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtmderxgqp.html

[R33] 捕获错误并提示行号
来源：http://hz.chenzaomai.com/gttfyjzawl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guannengcc.top/gtwtzaaljb.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtlvsctpdf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtpowqlgxt.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtpmpfmlrr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtoarsjkhg.html

[R36] 并发执行多个任务
来源：http://hz.fzhhl.top/gtfhlsacxx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinghuilouyu.cn/gtuwgyjihv.html

[R37] 把输出赋给变量
来源：http://hz.jinqigfzy.top/gtivvmvxhv.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gttmwrardn.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtbqjbkyev.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtwmswvpln.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gtodcefuiw.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtorsdlggg.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtnnedjftg.html

echo "log" >> out.log
来源：http://hz.havefunace.top/gtdivymhri.html

[R41] 丢弃输出
来源：http://hz.gzhubu.top/gtxeognesl.html


<!-- 参考信息 -->