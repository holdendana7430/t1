代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gtutgtupqq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gaohongyu789.top/gthpvdgcoc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xinyue.icu/gtprhlermm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.c1oappe.top/gtroffbpte.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sysykeji.top/gtwnanuukr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shzxlz.cn/gtqkhyffrt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtmcewobgh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xinyue.icu/gtzofhegrl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcpngrawn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gtgiffbunr.html

================================================================================
来源：http://hz.xuanzx.com/gtmlhogjno.html

[Q01] 创建表
来源：http://hz.hysaishi.cn/gtzykcxipp.html

CREATE TABLE users (
来源：http://hz.shangyingyoupin.top/gteoevnzty.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gttfmkclst.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenzaomai.com/gtnkvoccfc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtspuynqyr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtdhfymsql.html

);
来源：http://hz.gogol.net.cn/gtkhrfyfsg.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtupvajnsw.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gtxbsaztep.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtmofyoepz.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtjcnpqgrb.html

amount DECIMAL(10, 2),
来源：http://hz.zhaomingkeji.xyz/gtdvckuerp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtavwsevqj.html

);
来源：http://hz.iojbl.cn/gthkiualga.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gthiynfbay.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zycfv.cn/gttziuilbq.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtaiumpief.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gteggqiaij.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtxqdbgqfd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aibaodan.cn/gtgdhxijuw.html

[Q06] 删除列
来源：http://hz.0kj1m.cn/gthswnilra.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hysaishi.cn/gttmqvsbcm.html

[Q07] 删除表
来源：http://hz.iojbl.cn/gtaqoecnvh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtysuzpeej.html

[Q08] 创建普通索引
来源：http://hz.ydjk.org.cn/gtygbinvfh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtfwanpbkw.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtwibaqlqu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gttaefrimv.html

[Q10] 插入单行
来源：http://hz.jqgufenzy.top/gtaqxfrtcz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gtotkgnnpm.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtulofeubk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gotoacloud.top/gtwzksgnic.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtlmvzimqz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhoulong.xyz/gtzlirgymg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtqypkislk.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtrvtevekj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangtech.top/gtmniosqbi.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtznwkwkvb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtydczmyji.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtzmiwjyoj.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gtbkewuxhd.html

SELECT * FROM users;
来源：http://hz.aizwys.cn/gtloaxwwjz.html

[Q16] 查询指定列
来源：http://hz.ehwqpu.com/gtieaqkkdd.html

SELECT id, name FROM users;
来源：http://hz.ywan-chungtsiang.top/gtpbgptxya.html

[Q17] 条件查询
来源：http://hz.xziqi.cn/gtfzfzmgwb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jyoumei.cn/gtsvfaazub.html

[Q18] 模糊匹配
来源：http://hz.andypj.xyz/gttxyrnils.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgfzy.top/gtjnkrpjlb.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtsuekyflq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtisoywkuc.html

[Q20] IN 列表
来源：http://hz.yongpay.top/gtqxbaapfo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dianchejie.cn/gthbvckihj.html

[Q21] 空值判断
来源：http://hz.jinqigufen.top/gtqqrilakj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtfmjevjsg.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtsjxhjdcy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.mhx1999.top/gtwmnhtblu.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtlqoqsxpm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gttmkfwmrw.html

[Q24] 去重
来源：http://hz.gogol.net.cn/gtsqajctqy.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnqzz.top/gtywlqbtti.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtqlmqihdc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.quarkkingdee.top/gtvekerjuk.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtirqgxwvo.html

SELECT COUNT(*) FROM users;
来源：http://hz.redwolf501.top/gtucyvbmdl.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gtysvgnzhp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gotoacloud.top/gtvksqhnsw.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtjetpnfjp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtmatuuzgn.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtftkxccav.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guannengcc.top/gtakxhnxwr.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtyblugpci.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtrvvtoiiu.html

[Q31] 分组后过滤
来源：http://hz.fzhhl.top/gtmbffgihf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtwgevpgbo.html

[Q32] 分组拼接字符串
来源：http://hz.cashguo.top/gttyedkgoq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtrpfkvejg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.svipenyu.cn/gtzjfukhrs.html

[Q33] 多列分组
来源：http://hz.zycfv.cn/gtnrnhhrvc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigufen.top/gtgnjbxvve.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtdzhlikid.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtotqolawr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtwdrkobil.html

) t WHERE rn = 1;
来源：http://hz.tian-w.cn/gtptuwwmxm.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtgizedahi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtbwpttplr.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtvpgxpxmi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtltfajfcd.html

[Q37] 右连接
来源：http://hz.hywenlv.cn/gtfsmxkhxs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gthnckgbqq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.svipenyu.cn/gtasteyxmp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtjghkyrst.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtuxnnxghq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sweek.top/gtjkqzyxfv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtpneahnkd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hammf.cn/gtqqullsev.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtdxvkckoe.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtpbmtvhnm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtxpsjzkka.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gthfjacjvi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuanzx.com/gtfiuyjxpw.html

[Q42] 连接条件附加过滤
来源：http://hz.jinghuilouyu.cn/gtlxisgide.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtflywdekr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtoarafoqj.html

[Q43] 标量子查询
来源：http://hz.iojbl.cn/gtaflgsmkx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtyreinlvq.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtautvuxyq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cucudq.cn/gtgswlyqaj.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtxkbmudhn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtnvsifbtq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtnfhhdkgj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtxlrstqzz.html

[Q47] 与平均值比较
来源：http://hz.shangyingyoupin.top/gttovoiteq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenzaomai.com/gtriirmpiq.html

[Q48] CTE 公用表表达式
来源：http://hz.zycfv.cn/gtfslohlcb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtblkmutuq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtnonhataw.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtjwblanik.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtrcbvdbwp.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtxqypulrn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gttstywcnw.html

[Q51] 用子查询更新
来源：http://hz.redwolf501.top/gtifxeblkb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydjk.org.cn/gtvqxlnamc.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtaeflxiiu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gotoacloud.top/gtrlabfthb.html

[Q53] 按条件删除
来源：http://hz.zhijiandao.cn/gttldrmngh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtuyeniglt.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtunijepkt.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtvioypdeu.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtlqqbadoc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tanke756.top/gtkfkeutiq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.smart0.xyz/gtyqxyyndp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtbggqfowu.html

[Q57] 行号
来源：http://hz.cucudq.cn/gtexoonsbz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gtrwmvrwgs.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtiqtfvfpt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtiadorujj.html

[Q59] 分组内累计
来源：http://hz.ppjwa.cn/gthwaibamh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gtzrxnearj.html

[Q60] 取上一行 / 下一行
来源：http://hz.cqqwz.cn/gtvzxxwkqb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tanke756.top/gtmtokiisd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gthftgeels.html

[Q61] 移动平均
来源：http://hz.wangdashe.top/gtfflevvdt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtjtigftkf.html

[Q62] 分组占比
来源：http://hz.yangfankeji.com/gtwrifutbc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtjnimykkn.html

[Q63] 开启事务
来源：http://hz.aibaodan.cn/gtgxwayysg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtxsodiiwn.html

[Q64] 提交事务
来源：http://hz.sxryk.cn/gthahvxltw.html

COMMIT;
来源：http://hz.jqgufenzy.top/gtpvswmgxh.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gteruizyyy.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gttndlkbdv.html

[Q66] 行锁查询
来源：http://hz.guannengcc.top/gtbvicdlya.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gtguwzylse.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtfmdawxtn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ybcxt.top/gtmhhakiwz.html

[Q68] 保存点
来源：http://hz.hfpthk.cn/gtkdettipy.html

SAVEPOINT sp1;
来源：http://hz.yongpay.top/gtlwudmhpq.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtpofxisae.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtkuncugyx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhixingplan.top/gtvtawtsbc.html

[Q70] 更新统计信息
来源：http://hz.0kj1m.cn/gtgjtxzcft.html

ANALYZE TABLE users;
来源：http://hz.tianlin.xyz/gtdqompmhv.html

[Q71] 查看建表语句
来源：http://hz.tianlin.xyz/gtelavyrkc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yvedp.cn/gtkuetljco.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtqknngejb.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gticeklzwj.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtdfgyfbda.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.birdmap.top/gtfodfommz.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtfgejpesg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtkfrtvarp.html

[Q75] 日期格式化
来源：http://hz.xuetiantiany.cn/gtqyrtpnea.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtiqtkawrl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.316326.xyz/gtmzfkgqhk.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gtijwcvaiq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtpiarblmd.html

[Q77] 时间加减
来源：http://hz.zhoulong.xyz/gtyyecamuj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sweek.top/gtllikoazx.html

[Q78] 当前时间
来源：http://hz.ywan-chungtsiang.top/gtfooolaqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gtlazjyqlh.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtqfgwonqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sweek.top/gtmdcorqpe.html

[Q80] 字符串截取
来源：http://hz.zhixingplan.top/gtjbrcybqa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtxgthgfwy.html

[Q81] 字符串替换
来源：http://hz.iojbl.cn/gtskwjevml.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtuhwenkms.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gtloccrpxf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigufen.top/gtzfbblyic.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtbrntkdxt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtmjedjmsm.html

[Q84] 去除首尾空格
来源：http://hz.zycfv.cn/gtwxzditun.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnqzz.top/gtibuzkabo.html

[Q85] 数值取整
来源：http://hz.yvedp.cn/gtdglwpvbl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtbtoayqcp.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtyawhfrol.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtliideekq.html

[Q87] JSON 字段做条件
来源：http://hz.zhiwuduotai.top/gtuqgribah.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtklyltjvc.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtwwisiibg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.birdmap.top/gtpzpelbyr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xziqi.cn/gtgkczsqob.html

[Q89] 判断表是否存在
来源：http://hz.jqgfzy.top/gtueqetphx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtxxumavng.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtjghmyelm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ybcxt.top/gtaszgxhuq.html

================================================================================
来源：http://hz.chenzaomai.com/gtkhzzjmaq.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtkjqlrnju.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxvovclbm.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gtqhxsaxeg.html

#!/usr/bin/env bash
来源：http://hz.sweek.top/gtrljvjpmn.html

set -euo pipefail
来源：http://hz.gzhubu.top/gtjgucxmhv.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtrcayqzac.html

name="Tom"; echo "$name"
来源：http://hz.redwolf501.top/gtgjshtuig.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtjkfrhylz.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtsgnzhvrv.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gthqbywiuc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aibaodan.cn/gtllxcyruj.html

[R05] 参数默认值
来源：http://hz.jianghu66.top/gteahloyha.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtoxwzzppi.html

[R06] 判断命令是否存在
来源：http://hz.hysaishi.cn/gtalzxqucz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dashuyun.cn/gtowrtftov.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtxakjdvog.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gttbajohga.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtowozmwgl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cqqwz.cn/gtoestzubh.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtiaxkjuxq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtyabwjixj.html

[R10] 正则匹配
来源：http://hz.c1oappe.top/gtnsazbinl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhengqikj.top/gtjotuysgp.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtgjcybnus.html

case "$1" in
来源：http://hz.yuanzhike.top/gtjdrramnk.html

start) echo "启动" ;;
来源：http://hz.ydzc1.top/gthfvbjozq.html

stop)  echo "停止" ;;
来源：http://hz.sysykeji.top/gtqbndqvvs.html

*)     echo "未知命令" ;;
来源：http://hz.yonumen.top/gtdspguwkb.html

esac
来源：http://hz.hammf.cn/gtdcwxbrvs.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtsxdolqhz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gttlcbfshf.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtwyfvpwoh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gogol.net.cn/gtxzlzmiec.html

[R14] C 风格 for
来源：http://hz.guowangkeji.top/gtyejvnuqr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtxsduzfgz.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtquihgpna.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtccuooudb.html

[R16] until 等待条件
来源：http://hz.gaohongyu789.top/gtxliyikhy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtopopjfrk.html

[R17] 数组定义与取值
来源：http://hz.xinyue.icu/gtxgprfnxm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.52xcode.cn/gtypqrsevp.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtnqwfdaph.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtwkejgrrg.html

[R19] 数组长度
来源：http://hz.feifeiyinyue.top/gtsrojcgpu.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtcaswnvyo.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangkeji.top/gtqnphrgvf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtvhpydxty.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gtticofttn.html

echo "${#s}"
来源：http://hz.tian-w.cn/gthlkrcjbq.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtjhhmsmrr.html

echo "${s:0:5}"
来源：http://hz.sysykeji.top/gtodicnxym.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gtrbhgiqab.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtjocqwotw.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtgfeyxnrt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtuaupuloa.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtswluuoxk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtztgagjkp.html

[R26] 命令替换
来源：http://hz.yuxming.cn/gtbxwrcguc.html

now=$(date +%F); echo "$now"
来源：http://hz.ivvv.top/gtfeducpvy.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtwwsjkczz.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtryfsaaih.html

[R28] 浮点运算
来源：http://hz.zdqjudy.top/gtrsfeludq.html

echo "scale=2; 10/3" | bc
来源：http://hz.jlsjyb.cn/gtevtjqunl.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtnjubonkt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtajuzsavh.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtyyvxjuag.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtyqjlojvp.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtggxqrffd.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gtzbfpbrlu.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtsidpzkpn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtlhqfppdh.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtkrynanqt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtzynvvsou.html

[R34] 退出时清理
来源：http://hz.zhengqikj.top/gtudljoxyk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtsjqzmmdh.html

[R35] 后台执行并等待
来源：http://hz.hnxiangtu.top/gtfdexuyhl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.havefunace.top/gtsdwpskku.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtfizfazgt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ybcxt.top/gtwqwzsidx.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gthamflemr.html

files=$(ls -1)
来源：http://hz.52xcode.cn/gtjfzvvatl.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtflqrvgyx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jyoumei.cn/gtqagtevtb.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtrfibhpre.html


<!-- 参考信息 -->