代发 wailian999

================================================================================
来源：http://hz.nwbrower.top/gtgmubktre.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guannengcc.top/gtttjbcjao.html

================================================================================
来源：http://hz.yuanzhike.top/gthehdlbse.html

[Q01] 创建表
来源：http://hz.ehwqpu.com/gtmdsjfpyn.html

CREATE TABLE users (
来源：http://hz.smart0.xyz/gtxvhiwpkr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtupzvxliq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gtixbluwxe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gtdhpeorld.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gtwwhgucvh.html

);
来源：http://hz.yj20258.top/gtjpefmhos.html

[Q02] 创建带外键的表
来源：http://hz.xuanzx.com/gtcakrbbqw.html

CREATE TABLE orders (
来源：http://hz.ybcxt.top/gtykqqmdhv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtmrqlzsoc.html

user_id INT NOT NULL,
来源：http://hz.yuanzhike.top/gtagjhlwwp.html

amount DECIMAL(10, 2),
来源：http://hz.jyoumei.cn/gtrgopcbag.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtounfdtki.html

);
来源：http://hz.gogol.net.cn/gthfjniboa.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtplohqjpx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.c1oappe.top/gtrdxawzhp.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtvvowwsuv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtfhraayni.html

[Q05] 重命名列
来源：http://hz.zhoulong.xyz/gtpagjhrwz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jyoumei.cn/gtdilwdonu.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtulejbipz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gtfyzbsjhr.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gtkatldksz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtcdwrhubw.html

[Q08] 创建普通索引
来源：http://hz.zhongyouzk.top/gtodzcblzz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtugxetqdp.html

[Q09] 创建唯一索引
来源：http://hz.shzxlz.cn/gtekgjcxzl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtwzwtrflv.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtrdwxvxtd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtuaxadtps.html

[Q11] 一次插入多行
来源：http://hz.zycfv.cn/gtjlmlrcrr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hammf.cn/gtlgzbasae.html

[Q12] 插入后取自增 ID
来源：http://hz.bjfxy.top/gtmfyhceig.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aibaodan.cn/gtjbinqgrr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtcwpjjxrg.html

[Q13] 忽略重复插入
来源：http://hz.zhiwuduotai.top/gthlqahqfu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gtdwhhtpwg.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gthwgqxdgb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gthjikdysu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuxming.cn/gtuwpbityt.html

[Q15] 查询全部
来源：http://hz.ivvv.top/gtljdqjmkp.html

SELECT * FROM users;
来源：http://hz.fengsongda.top/gtcaaltopt.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtvpfgzuck.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtkujkiamu.html

[Q17] 条件查询
来源：http://hz.iojbl.cn/gtqjueoqrc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yvedp.cn/gtlpsxpqbx.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtvbjlyoew.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tian-w.cn/gtfdrbvupf.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtvzvfesws.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.haohaochexian.top/gtbnwdefws.html

[Q20] IN 列表
来源：http://hz.zhengqikj.top/gtwdqpuxcp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gthgahngec.html

[Q21] 空值判断
来源：http://hz.gogol.net.cn/gtjeudljur.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtccsouvsf.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtiujlymwu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtoefibjts.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtspzytcot.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gtedcerzgj.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtgprnvkyf.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhoulong.xyz/gthrrxmlqs.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gttbshljav.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gtvdbtpiev.html

[Q26] 计数
来源：http://hz.zycfv.cn/gtqqjgwtrv.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gteljbvsav.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtrvppwmbf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daxiang520.top/gttheurpic.html

[Q28] 求和与平均
来源：http://hz.ehwqpu.com/gtrkayaije.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gttzepdisx.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtvijjeukq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gtmefxzuhi.html

[Q30] 分组统计
来源：http://hz.haohaochexian.top/gtfvrrmgsd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtgfnbmtpy.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtjrbegner.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gotoacloud.top/gtapccqlby.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtwrnmgonv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtqkrmuldq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xingfuxueyuan.xyz/gtenfyodpl.html

[Q33] 多列分组
来源：http://hz.nanxinkj.top/gtpabinzom.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtjuwtbvqk.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtjvltlumk.html

SELECT * FROM (
来源：http://hz.shanyushiyangtech.top/gtsldggrfo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hfpthk.cn/gtvtygisrh.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtzmztaxwp.html

[Q35] 内连接
来源：http://hz.zhoulong.xyz/gtbvzdvlyl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gturdbwvyh.html

[Q36] 左连接
来源：http://hz.haohaochexian.top/gtxmiruftf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtunprexlq.html

[Q37] 右连接
来源：http://hz.wangshuangyany.cn/gtupiajkve.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.c1oappe.top/gtbbhedrzp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gttpzoykxq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtisemtlki.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxinkj.top/gtchyguhal.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.haohaochexian.top/gtpemugdoc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.c1oappe.top/gtilpizglz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhongyouzk.top/gtbpjfepcj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtujsyurvn.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtqbkntwvg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shangyingyoupin.top/gttfwyerxk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.svipenyu.cn/gtdcslxhjk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cheryme.top/gtqunakhck.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtdndopaut.html

SELECT u.name, o.amount FROM users u
来源：http://hz.haohaochexian.top/gtgawhytns.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangkeji.top/gtpvxawdsr.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtlqygrdia.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenzaomai.com/gtdrucloay.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtefolugxp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtbtwnsfjp.html

[Q45] EXISTS 判断存在
来源：http://hz.wangdashe.top/gteonuwvnl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtxyiymmsv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.0kj1m.cn/gtqvqvipqw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtpusjaows.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gtusefxioi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtugaouepx.html

[Q48] CTE 公用表表达式
来源：http://hz.yangfankeji.com/gtxakumvoe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtbifrgocw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhiwuduotai.top/gtlgebhmax.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtoybduwyn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtnnvihzag.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtrxgpprxb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.mhx1999.top/gtoafdbarn.html

[Q51] 用子查询更新
来源：http://hz.yangfankeji.com/gtsyvdbrii.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.meibo888.top/gtcambbjei.html

[Q52] 删除指定行
来源：http://hz.tian-w.cn/gtllfhhvtf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nwbrower.top/gtagrifzzj.html

[Q53] 按条件删除
来源：http://hz.xingfuxueyuan.xyz/gtvxrplfth.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gtpenmjiou.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtkoriyivn.html

TRUNCATE TABLE logs;
来源：http://hz.birdmap.top/gtbzwrgcwe.html

[Q55] 排名（并列占位）
来源：http://hz.shuidangran.top/gtmigbayta.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tianlin.xyz/gtcqrpetgu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenlongwang.top/gtzydvwapq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.kuanghao11.cn/gtmwvjoiqy.html

[Q57] 行号
来源：http://hz.daxiang520.top/gtiqorsgyb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtgcveoaos.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gttovrdxpa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtyayjmkrn.html

[Q59] 分组内累计
来源：http://hz.vqdsnc.cn/gtexyqbkdf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtdzylbueu.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtxmhndlar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxinkj.top/gtwdpcrzes.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj202588.top/gtjppmaisk.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtjgcfimvi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.redwolf501.top/gtrzcopevy.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gtnjeyicmd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtwwfwfbcs.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtgltfiyli.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.9152youxi.cn/gtgjmgxmrv.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gtrxkcggid.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtzwqcmetg.html

[Q65] 回滚事务
来源：http://hz.wangdashe.top/gtcbmnkgdg.html

ROLLBACK;
来源：http://hz.shanyushiyangtech.top/gtylrwfupq.html

[Q66] 行锁查询
来源：http://hz.ywan-chungtsiang.top/gtpuuhykng.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.kuanghao11.cn/gtkyxnasrq.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtdnfwhutt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xylfe.cn/gtxrxkornz.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gteaafsapj.html

SAVEPOINT sp1;
来源：http://hz.cucudq.cn/gtnyghbkud.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtwiraqnlb.html

[Q69] 查看执行计划
来源：http://hz.9152youxi.cn/gtpmywyuhw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnxiangtu.top/gtkmpyymxx.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gtilgindpx.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtluyzkmzr.html

[Q71] 查看建表语句
来源：http://hz.dashuyun.cn/gtbycjgexz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtdesiudgy.html

[Q72] 查看索引
来源：http://hz.sweek.top/gtkmhjyoku.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtiqogdzla.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gthlehcllp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtetacktbn.html

[Q74] 强制使用索引
来源：http://hz.birdmap.top/gthtsqoaoy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ehwqpu.com/gtkbmhqmow.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtfxulflxk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hongshengwenyu.top/gtapgjyyew.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtoeyoubdy.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtzlaawzhu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aibaodan.cn/gttecpeqmu.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtwotzspvu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnqzz.top/gtcibrwjsm.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtnxuvgpxm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gteuqgpjfj.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtkpqiilet.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtvtvhxiey.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtlnssatrr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtisvvxmox.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtmoxkjylc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sxryk.cn/gtxaaierkd.html

[Q82] 字符长度与字节长度
来源：http://hz.316326.xyz/gtgiekddif.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gzhubu.top/gtresiakoh.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtocfypfgh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gtjzmbkjnj.html

[Q84] 去除首尾空格
来源：http://hz.svipenyu.cn/gtdxmuazlh.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gterxgzbcc.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtkacfsyth.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xingfuxueyuan.xyz/gtcpxwdqjz.html

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gtfnclwwxh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gtunalkjka.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtdgludxba.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hongshengwenyu.top/gtbcxesaax.html

[Q88] 行转列（条件聚合）
来源：http://hz.haohaochexian.top/gttosadngm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gtzegbfjtm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.havefunace.top/gtxashtrim.html

[Q89] 判断表是否存在
来源：http://hz.quarkkingdee.top/gtagfzkmvb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258888.top/gtvjuaefue.html

[Q90] 生成序号列
来源：http://hz.0kj1m.cn/gtxybqicvh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shuidangran.top/gttvcsrobd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqfsbzuod.html

R. Bash 专题
来源：http://hz.shuidangran.top/gtekgdfzyn.html

================================================================================
来源：http://hz.ydzc1.top/gthfrlyrmz.html

[R01] shebang 与严格模式
来源：http://hz.wangdashe.top/gtjekfydap.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtwmioixix.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gtqhycsiws.html

[R02] 变量赋值与使用
来源：http://hz.shangyingyoupin.top/gtddedrfeo.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtvzydruwm.html

[R03] 只读变量
来源：http://hz.svipenyu.cn/gtqgzrvbwc.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtbupamhtl.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gtaatkkbqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtptsamjra.html

[R05] 参数默认值
来源：http://hz.yueranfly.top/gtcaylveez.html

name="${1:-default}"
来源：http://hz.kuanghao11.cn/gtnmlnllln.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtwvqtopfn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gttadvrqre.html

[R07] if 判断文件
来源：http://hz.zhongyouzk.top/gtktmooiha.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.andypj.xyz/gtzienzxbj.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtgcedpniz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sufxvd.cn/gtivpmiedf.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtiutnzqsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtzrmmjgoj.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtvtpcqbgb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gttfwovfwa.html

[R11] case 多分支
来源：http://hz.havefunace.top/gttmokpfuy.html

case "$1" in
来源：http://hz.dianchejie.cn/gtqwpucnqf.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtflyiingv.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gthjuudkft.html

*)     echo "未知命令" ;;
来源：http://hz.ywan-chungtsiang.top/gtldadauyu.html

esac
来源：http://hz.c1oappe.top/gtpzjdipdw.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtvwjegtvf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtcdeetycz.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtdwkbpoys.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtqoudzuly.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtmzfpoiwh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtbiytscbr.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gtaeqqlles.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hongshengwenyu.top/gtedatfazm.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtpeamhdao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gtkpykhluh.html

[R17] 数组定义与取值
来源：http://hz.aibaodan.cn/gtxuamnhid.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtgwediqtj.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtrihibtos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gthycbocib.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtdidovgdw.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtlkrvxifd.html

[R20] 关联数组（字典）
来源：http://hz.yuxming.cn/gttcmuyrff.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtmbcwastx.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtwyydxipj.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtxamngczc.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtxxaewfha.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtxnpwptru.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtgqauoowm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258.top/gtoamhmmcq.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtpcwpvcsq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gtkmxcbwdp.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gtjwsauhgn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yongpay.top/gtogobghzw.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gtxwwvzbaf.html

now=$(date +%F); echo "$now"
来源：http://hz.chenjidiqi.icu/gtqxpszyyz.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtkisnbrjv.html

echo $((1 + 2 * 3))
来源：http://hz.ydjk.org.cn/gtvpxmzcbz.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtbzkkfmhe.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtlfpowvuf.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtzwahsygw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtvavcaaun.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtqfmmldjj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtvjoudecm.html

[R31] 局部变量
来源：http://hz.meibo888.top/gtftaflhab.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtrlsgixgv.html

[R32] 参数个数校验
来源：http://hz.c1oappe.top/gttjllkdnj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtitmuxqwq.html

[R33] 捕获错误并提示行号
来源：http://hz.ivvv.top/gtvtivruve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtdlvehgoc.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtdwvqnbsi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtoqwfkkkn.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtxpjjtozp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtfluueshi.html

[R36] 并发执行多个任务
来源：http://hz.shzxlz.cn/gtpmujfwyj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtuchmisfk.html

[R37] 把输出赋给变量
来源：http://hz.jlsjyb.cn/gtaolhlhsy.html

files=$(ls -1)
来源：http://hz.vqdsnc.cn/gtdebyiotw.html

[R38] 管道串联
来源：http://hz.yongpay.top/gtafwoxbfq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtbdutownw.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtvcbvuofi.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtiqxqngto.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtbfxlkeqt.html

echo "log" >> out.log
来源：http://hz.zycfv.cn/gtlfrlifdb.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtymgwraft.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtuungocde.html

[R42] 输入重定向
来源：http://hz.zhiwuduotai.top/gtijsmqdfs.html

wc -l < a.txt
来源：http://hz.birdmap.top/gtnxhlevel.html

[R43] 按名字查找文件
来源：http://hz.hywenlv.cn/gtawuoethy.html


<!-- 参考信息 -->