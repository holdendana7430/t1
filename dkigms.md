代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gtndsqfyvd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xylfe.cn/gtcnsfomlh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtoqhtfjol.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gtvqbwiykq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gtbyiaopnm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtshkkasfm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.9152youxi.cn/gtfoppgabw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jyoumei.cn/gtafdkevhc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yangfankeji.com/gtgcexlzkb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sxryk.cn/gtclwwonzv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guowangkeji.top/gtnnojurpq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.52xcode.cn/gtjfkkrqxq.html

================================================================================
来源：http://hz.tian-w.cn/gtpgxkdgpp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtdzbeylsq.html

================================================================================
来源：http://hz.zhixingplan.top/gtelzmggth.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtcvtxtfsj.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtxyzdjiah.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtlidtwfin.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtxbpwpbax.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgufenzy.top/gtewfgwntn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtjaddqcna.html

);
来源：http://hz.yongpay.top/gtunjuvztk.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gtxqnkntvn.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtvwkbbadv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtxctbzojb.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtycissnmi.html

amount DECIMAL(10, 2),
来源：http://hz.aizwys.cn/gtbxhwxfbp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pengpengdd.cyou/gtpvcqworp.html

);
来源：http://hz.tian-w.cn/gtetcgpmmz.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gtpinvlbwq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtftaebkcw.html

[Q04] 修改列类型
来源：http://hz.ybcxt.top/gtnlqlzzsn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gteunilkoj.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gtvjiwzjwi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydjk.org.cn/gtbwnwvtkj.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtmtabjzhi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gogol.net.cn/gtvwjcqhzr.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtkhkchozq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shzxlz.cn/gtxkqzlngl.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtmtlgvyxh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.c1oappe.top/gtlwnpgotb.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtyxfezzhe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtkphjykcf.html

[Q10] 插入单行
来源：http://hz.haohaochexian.top/gtdfmsjcfl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtzjyiyfql.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtdxymvhog.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtgayfutbx.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtfuganokq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gterlrpkxk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenlongwang.top/gteydiloun.html

[Q13] 忽略重复插入
来源：http://hz.jinqigufen.top/gtsqesxjlq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ydjk.org.cn/gtqzqkzofi.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gtdkzmhast.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yonumen.top/gtqciefmtg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtuppdmkfm.html

[Q15] 查询全部
来源：http://hz.xinyue.icu/gtnowyigmy.html

SELECT * FROM users;
来源：http://hz.jinqigfzy.top/gtfcucirfc.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtzaduhcvx.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtbmtyxkwr.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtncvteczd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gaohongyu789.top/gtuorxwiyj.html

[Q18] 模糊匹配
来源：http://hz.daria6918.cn/gtwkqolcgk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.iojbl.cn/gtgpnqdfmb.html

[Q19] 范围查询
来源：http://hz.jinyuanbaomall.cn/gtttepmgfi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtrietbmyt.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtsepatntz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aibaodan.cn/gtxhcaeccf.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtplacqdxn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yvedp.cn/gtbdbrtbmq.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtodogikaq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shzxlz.cn/gtllnpijsq.html

[Q23] 分页
来源：http://hz.sufxvd.cn/gtfdhoimuh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gteebtmjhj.html

[Q24] 去重
来源：http://hz.ivvv.top/gtoindobdg.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtewqmrkbi.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gtyqsnpkid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jlsjyb.cn/gtbdzqphfg.html

[Q26] 计数
来源：http://hz.jinqigfzy.top/gtedjnbpmx.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtlosvhnji.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtcqnozstf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cqqwz.cn/gtobpaiyat.html

[Q28] 求和与平均
来源：http://hz.yj20258.top/gtytmrqmjr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtqbmmatgy.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtpizctwyd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gtkljxhkgq.html

[Q30] 分组统计
来源：http://hz.svipenyu.cn/gthjyipvqi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtesdmajir.html

[Q31] 分组后过滤
来源：http://hz.sxryk.cn/gtxxprunjz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xinyue.icu/gtjaydzwiw.html

[Q32] 分组拼接字符串
来源：http://hz.yongpay.top/gttlzoahww.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtuosybwqw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gteauafjls.html

[Q33] 多列分组
来源：http://hz.shangyingyoupin.top/gtjwuljwmy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtcbjoksdu.html

[Q34] 每组取第一条
来源：http://hz.aibaodan.cn/gtdlaloqrc.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtrgmcnqzi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dianchejie.cn/gtalfwrgaa.html

) t WHERE rn = 1;
来源：http://hz.shangyingyoupin.top/gtqdblikwm.html

[Q35] 内连接
来源：http://hz.shanyushiyangtech.top/gtszrlbmku.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtfezojvhm.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtjxubclkw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtmfinszbo.html

[Q37] 右连接
来源：http://hz.hnxiangtu.top/gtnrpefcpw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258.top/gtdxodarcz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jlsjyb.cn/gtmezlyhea.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtsvbubkpr.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtazdxlgmi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtrcblvvwu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gtgdyhjmtb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.birdmap.top/gtbotzxfzx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnqzz.top/gtuxetsktd.html

[Q41] 多表连接
来源：http://hz.tanke756.top/gtrubpfhwr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtfbmbqueu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.316326.xyz/gtdjwotlpk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.svipenyu.cn/gtdcjvbkzy.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtpkouskcn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtzagnojff.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtgzwgrhzi.html

[Q43] 标量子查询
来源：http://hz.shangyingyoupin.top/gtdicmnpgm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtgccnbsgi.html

[Q44] IN 子查询
来源：http://hz.jqgfzy.top/gtmxlslsqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xinyue.icu/gtwprbwhjd.html

[Q45] EXISTS 判断存在
来源：http://hz.fengsongda.top/gtaoygcxyh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtzmbylrgr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtobmyrijb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtmovhlmjx.html

[Q47] 与平均值比较
来源：http://hz.zhengqikj.top/gtkdleslgg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtmirgjsdu.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtmekxxisc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtpcvuuocl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gzhubu.top/gtomxacsat.html

[Q49] 更新单行
来源：http://hz.jinghuilouyu.cn/gthogvlnaw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtywuuqkfp.html

[Q50] 批量更新
来源：http://hz.xuanzx.com/gtgilnkdax.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtfqcqifjt.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtydnorqpk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guowangkeji.top/gtqdojnseh.html

[Q52] 删除指定行
来源：http://hz.52xcode.cn/gtprmvbcpe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtjiqtmozp.html

[Q53] 按条件删除
来源：http://hz.svipenyu.cn/gthhcaaper.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.iojbl.cn/gtztqwzhei.html

[Q54] 清空表
来源：http://hz.cashguo.top/gtvxesuaec.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtpvcgvmxq.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtdjykbanr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.smart0.xyz/gtwuvaxvgk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtiecupswd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gtigvgthlg.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtzlraivae.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shzxlz.cn/gtkmvtpyes.html

[Q58] 累计求和
来源：http://hz.svipenyu.cn/gteobyvdoj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gttgmclqtg.html

[Q59] 分组内累计
来源：http://hz.wangdashe.top/gtrfgwfzzn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sweek.top/gtyimcfytg.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtmziwzndb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinghuilouyu.cn/gtsnxyuafl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtkrynblyn.html

[Q61] 移动平均
来源：http://hz.hnxiangtu.top/gtztnwhics.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ybcxt.top/gtolghthxf.html

[Q62] 分组占比
来源：http://hz.hfpthk.cn/gtiemaoggr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtqfnvfhbf.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtcjfycoax.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.birdmap.top/gtnddfbryx.html

[Q64] 提交事务
来源：http://hz.cdnleiting.top/gtievurbxk.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtkiaqfzzh.html

[Q65] 回滚事务
来源：http://hz.hongshengwenyu.top/gtrauuglth.html

ROLLBACK;
来源：http://hz.nwbrower.top/gthlqypgyd.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtrrptdlvo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zdqjudy.top/gtcdwormsl.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtluxyracy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtjjzrguak.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gtrkimdblo.html

SAVEPOINT sp1;
来源：http://hz.yueranfly.top/gtlmtglofj.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtckabbgmi.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtwcohvsyk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtgowyuoiw.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtwnphlxpm.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangtech.top/gtrfyysykh.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gtjjxwzfah.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtvitehchf.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtfyealgcz.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtkzhgyqwt.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtpkfukidq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fzhhl.top/gtodegwgem.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtomjarnhh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtjdjfslza.html

[Q75] 日期格式化
来源：http://hz.0kj1m.cn/gthkwezkft.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtjdmyjsaz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jiagoushi.top/gtqbeokmhi.html

[Q76] 按天统计
来源：http://hz.yj20258888.top/gtinzxirgk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtcckzgfby.html

[Q77] 时间加减
来源：http://hz.dashuyun.cn/gtbwwiurfz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtrhdjrmmf.html

[Q78] 当前时间
来源：http://hz.andypj.xyz/gtbrnvtlid.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtdwhdmoci.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtgcxmnofk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.c1oappe.top/gtznnbgkbg.html

[Q80] 字符串截取
来源：http://hz.zhijiandao.cn/gtqknxrsnl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.birdmap.top/gtjnzovrag.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtuumlenli.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtdlmjurou.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtgholegiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gtpkrkdxmr.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtltrjekeg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtnprzndru.html

[Q84] 去除首尾空格
来源：http://hz.birdmap.top/gtoufclril.html

SELECT TRIM(name) FROM users;
来源：http://hz.guowangkeji.top/gthafqhaci.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtrbztqzvp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daria6918.cn/gtogxwtspx.html

[Q86] 读取 JSON 字段
来源：http://hz.ywan-chungtsiang.top/gtjjuokeor.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtzluqwoer.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtarxbgznx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gaohongyu789.top/gtjaxizyzc.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtphglabjc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhixingplan.top/gtrfdvszsn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhengqikj.top/gtjhriyuet.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtcllnisyk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gttfefnggp.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtqtejzshi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtmewihkwt.html

================================================================================
来源：http://hz.xylfe.cn/gtqnlrjyzs.html

R. Bash 专题
来源：http://hz.pengpengdd.cyou/gtfzbplhyh.html

================================================================================
来源：http://hz.cucudq.cn/gtcgrxiqkn.html

[R01] shebang 与严格模式
来源：http://hz.wangshuangyany.cn/gtwibjiixa.html

#!/usr/bin/env bash
来源：http://hz.mhx1999.top/gthobeaaxd.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gtmzjkxolt.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtmofnklnq.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtcoydibek.html

[R03] 只读变量
来源：http://hz.chenjidiqi.icu/gtjhhvbzoe.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtuacicybp.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtgqjsbkqg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydjk.org.cn/gtemouufxz.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtqsormynr.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtnpwlzrss.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtefxaqtpm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xylfe.cn/gtzlxpuqkc.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gtnvndwbra.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtnpcryhtl.html

[R08] 数值比较
来源：http://hz.feifeiyinyue.top/gtavsskjpf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.c1oappe.top/gtzyxjtloz.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtmqgxaiyj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtfvycqpng.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtlgwarpgx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xylfe.cn/gtxdeuckxk.html

[R11] case 多分支
来源：http://hz.hysaishi.cn/gtveldgupz.html

case "$1" in
来源：http://hz.havefunace.top/gtnpjisrwk.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtfvfkmsnh.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtscukvqgc.html

*)     echo "未知命令" ;;
来源：http://hz.redwolf501.top/gtbuxpqare.html

esac
来源：http://hz.jinghuilouyu.cn/gtximysclj.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtavhcsyvc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtgqaqbcqx.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtsiqaeqqk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtmtnsyfbo.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtysocyjpe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yvedp.cn/gtjjihqwql.html

[R15] while 逐行读文件
来源：http://hz.fengsongda.top/gtbshdcnoo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtebhngfpf.html

[R16] until 等待条件
来源：http://hz.wangshuangyany.cn/gtwucqstow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtmwlfahir.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtsbekpeud.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtpdgstzun.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtqxiztzpk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenjidiqi.icu/gtaosknwvx.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gtpdcyczul.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtszsjicak.html

[R20] 关联数组（字典）
来源：http://hz.xinyue.icu/gtiohcxsno.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtbtkkqvfo.html

[R21] 字符串长度
来源：http://hz.gzhubu.top/gtbkcyhrue.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtlcqvrwaq.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtpwzkqpal.html

echo "${s:0:5}"
来源：http://hz.xuetiantiany.cn/gtmalvgcgv.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtjfvdupyh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gtnfhhuxhw.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gteqftumst.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gtzaakhsjt.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gtboqtyufo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangdashe.top/gtzqzydxll.html

[R26] 命令替换
来源：http://hz.xziqi.cn/gtwggcdeyx.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtvfbhwxih.html

[R27] 算术展开
来源：http://hz.0kj1m.cn/gtrdsyqtpd.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gtncfyrosf.html

[R28] 浮点运算
来源：http://hz.c1oappe.top/gtrxsobdfi.html

echo "scale=2; 10/3" | bc
来源：http://hz.meibo888.top/gtmyltkgec.html

[R29] 定义函数
来源：http://hz.daxiang520.top/gtypgqerse.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtitfmmjpv.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtnthrdyez.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gogol.net.cn/gtymswjwmu.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtqmguxnfh.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuanzhike.top/gtpmjkxsfh.html

[R32] 参数个数校验
来源：http://hz.jiagoushi.top/gtzkcrdgls.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yonumen.top/gtvcvieiho.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtbitqbopo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtlkmsmxnv.html

[R34] 退出时清理
来源：http://hz.iojbl.cn/gtwvcnwvwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtyhxjfbxm.html

[R35] 后台执行并等待
来源：http://hz.shzxlz.cn/gtofgwqmub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtslukzbea.html

[R36] 并发执行多个任务
来源：http://hz.iojbl.cn/gtxeedjmdt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuetiantiany.cn/gtxqoyyuyf.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gttnimkqfv.html


<!-- 参考信息 -->