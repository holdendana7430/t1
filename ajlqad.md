代发 wailian999

================================================================================
来源：http://hz.xziqi.cn/gttjgnyeua.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtectkeuhl.html

================================================================================
来源：http://hz.xuanzx.com/gtkqvhgkfu.html

[Q01] 创建表
来源：http://hz.yonumen.top/gtddqhvarg.html

CREATE TABLE users (
来源：http://hz.smart0.xyz/gttabemszv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtrgvleaip.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtxfismove.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hammf.cn/gtyhhghklc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aibaodan.cn/gtdufbhsnq.html

);
来源：http://hz.tanke756.top/gtbktbxnum.html

[Q02] 创建带外键的表
来源：http://hz.9152youxi.cn/gtuetdpodd.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gtuqhoefqp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtqesvyxll.html

user_id INT NOT NULL,
来源：http://hz.shuidangran.top/gtqmeeazhy.html

amount DECIMAL(10, 2),
来源：http://hz.jinyuanbaomall.cn/gtcllhpcwa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtfqjegwlq.html

);
来源：http://hz.svipenyu.cn/gtwewnsvkq.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gtwpgwibut.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.316326.xyz/gtgdvmkaue.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtpwjwxfhw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gthzaulaqo.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gttpsjavnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydjk.org.cn/gtejdvszjh.html

[Q06] 删除列
来源：http://hz.chenzaomai.com/gtdodjogml.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.haohaochexian.top/gtoiljszhb.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtswkrihkl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daxiang520.top/gtvozvuqqb.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangtech.top/gtwmpbogop.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ppjwa.cn/gtkqhmmhar.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtxpigsyil.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtnklmfnkp.html

[Q10] 插入单行
来源：http://hz.shuidangran.top/gtmtgudofk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtfwumurgx.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtbtavbmmw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cqqwz.cn/gtvvkkrbrm.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtcskqbfyz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtldrehfno.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtzytfajlj.html

[Q13] 忽略重复插入
来源：http://hz.kuanghao11.cn/gtrcchxihp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtdvnpmzdh.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gtmprypeqg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtyzfmbpzm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtialsmgwj.html

[Q15] 查询全部
来源：http://hz.jqgfzy.top/gtnfuowclg.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gthcjxfgui.html

[Q16] 查询指定列
来源：http://hz.haohaochexian.top/gtdrekuepv.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gtfonuuxzz.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtvyzzlaru.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtnnuqjjxw.html

[Q18] 模糊匹配
来源：http://hz.gotoacloud.top/gtdwyntgml.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tian-w.cn/gtxmgdoixh.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gtbuhhgrfc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtiiadbgow.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gthaeeqxht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtrpxxjtbq.html

[Q21] 空值判断
来源：http://hz.yj202588.top/gtpiyzzcgf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtctflpuvr.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtpsnzqxkc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtgwluomcz.html

[Q23] 分页
来源：http://hz.shanyushiyangtech.top/gtirsgnthe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gtkjcejnij.html

[Q24] 去重
来源：http://hz.dashuyun.cn/gtlbjqzdym.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gttfvqjxcu.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtlxcrojvy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhengqikj.top/gtvfpbpbvb.html

[Q26] 计数
来源：http://hz.meibo888.top/gtuodhojvr.html

SELECT COUNT(*) FROM users;
来源：http://hz.0kj1m.cn/gtitfqehep.html

[Q27] 条件计数
来源：http://hz.daria6918.cn/gtucwarvfe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ivvv.top/gthkrqlpgn.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gtvwbaqvnv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtqvqheuds.html

[Q29] 最大最小值
来源：http://hz.ydzc1.top/gtxomjnzvu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gtyjhidovg.html

[Q30] 分组统计
来源：http://hz.zdqjudy.top/gtdbahxnbu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gthlyvqlas.html

[Q31] 分组后过滤
来源：http://hz.fzhhl.top/gtaxznwcce.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtilsucyvu.html

[Q32] 分组拼接字符串
来源：http://hz.9152youxi.cn/gtkuafqapf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtwiwgldxu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jlsjyb.cn/gtdpbrgcuw.html

[Q33] 多列分组
来源：http://hz.chenlongwang.top/gtazmrwulj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtzdkweuqj.html

[Q34] 每组取第一条
来源：http://hz.sysykeji.top/gtzithalkg.html

SELECT * FROM (
来源：http://hz.ivvv.top/gthqjjzbvu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxinkj.top/gtaslopavj.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtcnkjonzc.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtuaebpbih.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtirlbffvf.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtxukobzvi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtkvfcynni.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtxlocgkdy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtfjkvcpfp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtlirbdjch.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zdqjudy.top/gtgcpdohdt.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gtxjqiariu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtwdxlijhm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtuabxdokd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yongpay.top/gtujoshtiy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daria6918.cn/gtuicaqkqe.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtvxdncygz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydzc1.top/gtgibjydbt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtjyrrncuz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.mhx1999.top/gthlqvvoyt.html

[Q42] 连接条件附加过滤
来源：http://hz.ivvv.top/gtmbixcmmz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtasfmdzkp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnxiangtu.top/gtlnvuimpf.html

[Q43] 标量子查询
来源：http://hz.zhengqikj.top/gtjgiozgrz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtjijfrplk.html

[Q44] IN 子查询
来源：http://hz.daria6918.cn/gtmlijdrma.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtwcazkgog.html

[Q45] EXISTS 判断存在
来源：http://hz.tian-w.cn/gtlmhmpzhu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtmsjatddm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhaomingkeji.xyz/gtvgyssozr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtziehrcdf.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtbszdokdl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtocbmohjy.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gtaaeugjtm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.quarkkingdee.top/gtqjfvatch.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhaomingkeji.xyz/gtdrtqbisd.html

[Q49] 更新单行
来源：http://hz.zycfv.cn/gtxltcknha.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtcqwqdygo.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtaraoaoqh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gtqdwggpuy.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gteipbktdk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gtgyglsgwn.html

[Q52] 删除指定行
来源：http://hz.shzxlz.cn/gttpxxkihg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtydbnzqfz.html

[Q53] 按条件删除
来源：http://hz.hywenlv.cn/gtsjnqxkbv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhixingplan.top/gtjusbddyp.html

[Q54] 清空表
来源：http://hz.svipenyu.cn/gtfxiqncds.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gttaaqwuru.html

[Q55] 排名（并列占位）
来源：http://hz.9152youxi.cn/gtexoulncg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxuanxn.top/gtazprdzxc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtcdbnvktv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hfpthk.cn/gthcefvklf.html

[Q57] 行号
来源：http://hz.ivvv.top/gtmyrjmnpe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gthrkzwthh.html

[Q58] 累计求和
来源：http://hz.jinqigufen.top/gtuzoexfih.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnqzz.top/gtwkpwakna.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtmcsgqdyv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gtpehpsaox.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtyyqnmyhj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtdwvsmhtl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxinkj.top/gtxuekjrql.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtbxapfrcl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gthvzlslkm.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtduljiaje.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtaojfdmvm.html

[Q63] 开启事务
来源：http://hz.cashguo.top/gtmvmdtqju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtxkvpvxcr.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtbhlfmhef.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtjlaxjtem.html

[Q65] 回滚事务
来源：http://hz.mhx1999.top/gtbhwkrkew.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtammmedht.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtqmxhtcss.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shzxlz.cn/gtnbamhkoj.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtvgpxeurf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sufxvd.cn/gtpylslsea.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gtcfhbokcy.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gtfottehdw.html

ROLLBACK TO sp1;
来源：http://hz.shangyingyoupin.top/gtmboikywg.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtifqjfpts.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jiagoushi.top/gtwrxuzglv.html

[Q70] 更新统计信息
来源：http://hz.iojbl.cn/gtskqbvwbk.html

ANALYZE TABLE users;
来源：http://hz.tanke756.top/gtesyuvlur.html

[Q71] 查看建表语句
来源：http://hz.kuanghao11.cn/gtpcllgnvv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydjk.org.cn/gtipyobqma.html

[Q72] 查看索引
来源：http://hz.shangyingyoupin.top/gtysgoszdq.html

SHOW INDEX FROM users;
来源：http://hz.mhx1999.top/gtxqzamhlg.html

[Q73] 查看表状态
来源：http://hz.tianlin.xyz/gtdldeybej.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenzaomai.com/gtlhbeqvdl.html

[Q74] 强制使用索引
来源：http://hz.xuetiantiany.cn/gttofoxolg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtnxawimqa.html

[Q75] 日期格式化
来源：http://hz.hysaishi.cn/gtisnapfau.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.redwolf501.top/gtkfjgseyr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zdqjudy.top/gtmhjthslv.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gthsflwent.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhaomingkeji.xyz/gtifdomlta.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtsigxyejs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtggcckaqj.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtfvvznilt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtpafyfjbw.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtbvzozufq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shzxlz.cn/gtaddmaixe.html

[Q80] 字符串截取
来源：http://hz.chenlongwang.top/gtfyhjznem.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtwjqirwym.html

[Q81] 字符串替换
来源：http://hz.9152youxi.cn/gtqibcklnh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtoavsrevx.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtwdzwoamk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gtnhgmnpvr.html

[Q83] 大小写转换
来源：http://hz.guannengcc.top/gtwaqagdgc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.mhx1999.top/gtoameslvy.html

[Q84] 去除首尾空格
来源：http://hz.jyoumei.cn/gtvognopfh.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtxnldvjme.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtkpxjtgsm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtsgybeygc.html

[Q86] 读取 JSON 字段
来源：http://hz.ydjk.org.cn/gtjkbhzirm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgufenzy.top/gtfjrnryrr.html

[Q87] JSON 字段做条件
来源：http://hz.daria6918.cn/gtnlzigwfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yueranfly.top/gtsggnvbpy.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gthlsseaks.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtlwvgkrye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtdpftlyvc.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtbnykdzwf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtktjiuvcs.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtxdgytzth.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daria6918.cn/gtgzcvdyoy.html

================================================================================
来源：http://hz.ydjk.org.cn/gtrdpyogvl.html

R. Bash 专题
来源：http://hz.fengsongda.top/gtoxrjigxa.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbiysjqsv.html

[R01] shebang 与严格模式
来源：http://hz.ehwqpu.com/gtmrtfgobb.html

#!/usr/bin/env bash
来源：http://hz.nanxinkj.top/gtdjiradmx.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtgeljvhnu.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gtabjfmsua.html

name="Tom"; echo "$name"
来源：http://hz.jinqigufen.top/gtzomvacpp.html

[R03] 只读变量
来源：http://hz.nanxuanxn.top/gtjqyabchb.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtdaxtdevj.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtblkmqzcf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtqisstlzh.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtinczzian.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtvgduwkzd.html

[R06] 判断命令是否存在
来源：http://hz.cheryme.top/gtrdkterxz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtsitwteio.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtlgquxwqc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxuanxn.top/gtpxjtefjw.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtikdxvefs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aizwys.cn/gtowdlffkb.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtlxgmyrbb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ivvv.top/gtketbwops.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtroylvzum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.c1oappe.top/gtcsnxiypt.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtlxaaospz.html

case "$1" in
来源：http://hz.zhixingplan.top/gttawhfkjp.html

start) echo "启动" ;;
来源：http://hz.ivvv.top/gtdlkeaqnx.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtcepiafbx.html

*)     echo "未知命令" ;;
来源：http://hz.xuetiantiany.cn/gthonzliur.html

esac
来源：http://hz.zdqjudy.top/gtvrfxavdx.html

[R12] for 遍历文件
来源：http://hz.zhongyouzk.top/gturnxtwll.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tian-w.cn/gtkdbhxoxb.html

[R13] for 计数循环
来源：http://hz.gotoacloud.top/gtmjyfjphq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gttvlwbsdm.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gtkwlosxea.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenzaomai.com/gtikovzpvq.html

[R15] while 逐行读文件
来源：http://hz.fzhhl.top/gtbiqqsejl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtqzgzqwzv.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtpsodivfu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtpqlioudh.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtpuctnpnf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtalmbxckz.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtwwzavpdr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pycfn.com/gtmlnzlngm.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtofsfesfl.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gturrlrtcr.html

[R20] 关联数组（字典）
来源：http://hz.havefunace.top/gttfyvmrhw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtgkjuaxhn.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtuduqzrth.html

echo "${#s}"
来源：http://hz.gotoacloud.top/gtjajqdkhc.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtdbolpcdd.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtcyntjoea.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtsfhidguk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daxiang520.top/gtxybzbjfv.html

[R24] 大小写转换
来源：http://hz.c1oappe.top/gtjnxxmdxv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtldxqqqsr.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtqfzadsil.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hywenlv.cn/gtposwmpli.html

[R26] 命令替换
来源：http://hz.hfpthk.cn/gtyvicvzwh.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtjgscnqxp.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtsznnzpma.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gthoyowpqs.html

[R28] 浮点运算
来源：http://hz.zycfv.cn/gtovtemhhs.html

echo "scale=2; 10/3" | bc
来源：http://hz.yvedp.cn/gtaeyevlbe.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtlnipvhho.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.havefunace.top/gtrljlxvmv.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtmhhjxzxs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gtnelcwbza.html

[R31] 局部变量
来源：http://hz.zycfv.cn/gtoyrjkqng.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gtgwxkmyet.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtkodyzczg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gtnjmsqakn.html

[R33] 捕获错误并提示行号
来源：http://hz.dashuyun.cn/gtirzliuin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gtjkmxkmcg.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtnyayqnef.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtxhcoprni.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gtfgftuvpd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pycfn.com/gttfezrwie.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gtlrdrbazc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tianlin.xyz/gttbvqrrge.html

[R37] 把输出赋给变量
来源：http://hz.pengpengdd.cyou/gtevtpxxop.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtddlvkjxq.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtjcusbkol.html

cat a.txt | grep -i error | wc -l
来源：http://hz.vqdsnc.cn/gtxlghknrx.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gttpnbmftd.html

cmd > out.log 2>&1
来源：http://hz.meibo888.top/gtfgjbnghf.html

[R40] 追加写日志
来源：http://hz.ehwqpu.com/gtphobiuyl.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtxgrjwdzs.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtztwugswj.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gtpokcyret.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtxsixbsca.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtjokdircs.html

[R43] 按名字查找文件
来源：http://hz.cdnleiting.top/gtpdnwoagl.html


<!-- 参考信息 -->