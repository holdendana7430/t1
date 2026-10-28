代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuetiantiany.cn/gtxkzdyjdq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtzfsjmmmt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtldsfxvve.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xingfuxueyuan.xyz/gtzwmcqlxk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtykyyhtql.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sufxvd.cn/gtpipixweo.html

================================================================================
来源：http://hz.hywenlv.cn/gtxjpihygs.html

[Q01] 创建表
来源：http://hz.jyoumei.cn/gtmuuwikgg.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtwrhhsftv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtnywsdxdo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtjhfvmxwe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gogol.net.cn/gtkvjxylgu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gttdlcoacz.html

);
来源：http://hz.zycfv.cn/gtrggbcsda.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtztwormmj.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtgdgbdvvk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtreltwrle.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtktfxclpl.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtguewcwuf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinghuilouyu.cn/gtanfslqay.html

);
来源：http://hz.yj20258.top/gtcpjvtgzm.html

[Q03] 增加列
来源：http://hz.ehwqpu.com/gtkntztpyu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xingfuxueyuan.xyz/gttcxwhtxy.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gtmbhhfpya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtzwavpizh.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtokttobci.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtvwnynfuh.html

[Q06] 删除列
来源：http://hz.xuanzx.com/gtawluwmkt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hfpthk.cn/gtcnlreclp.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gtzpclkjzo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gtyozbfjay.html

[Q08] 创建普通索引
来源：http://hz.aibaodan.cn/gtbvetwewb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtaqxhjqht.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtrpnhjnmn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.guannengcc.top/gtuccoprxw.html

[Q10] 插入单行
来源：http://hz.tianlin.xyz/gtxbkwdsmi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gtuzqutsiw.html

[Q11] 一次插入多行
来源：http://hz.zhaomingkeji.xyz/gtghktixrz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtcwbbkmtt.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtljoyktua.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxuanxn.top/gtsznbypqe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gtmgbkcpuy.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtpylocicv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gtnwfxopag.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtxvdxsnbc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangkeji.top/gtwauwmdyi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.9152youxi.cn/gturhhcmyz.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtmwmiaazx.html

SELECT * FROM users;
来源：http://hz.tanke756.top/gtxkvqttdl.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtzlhdfoeq.html

SELECT id, name FROM users;
来源：http://hz.aibaodan.cn/gtjvhalurd.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gtavfxkumr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yvedp.cn/gtdmwcmhvv.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtvppvsxea.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258.top/gtvzvzjodk.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtwephylce.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtdbhqxdrb.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtatevoftb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.vqdsnc.cn/gtdxmvwxzh.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtmhclcram.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hywenlv.cn/gtiotbrixo.html

[Q22] 排序
来源：http://hz.chenzaomai.com/gtifgpbsxv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtyrfhqvjz.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtvtxjitrd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dianchejie.cn/gtpmjsvcvj.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtskpvqeiy.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gtisytnsvb.html

[Q25] 只取前 N 条
来源：http://hz.52xcode.cn/gtnoubpftm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtxduoqhxw.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtvpvoksmt.html

SELECT COUNT(*) FROM users;
来源：http://hz.gogol.net.cn/gtvbvjckfm.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtovdxjpeq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtfjxoncid.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtydurudsd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhijiandao.cn/gtdtnfrkyl.html

[Q29] 最大最小值
来源：http://hz.c1oappe.top/gtvfjvanbw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenjidiqi.icu/gtcnrhwkiu.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtcckwtmpf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtzimogwbn.html

[Q31] 分组后过滤
来源：http://hz.hywenlv.cn/gtacbmlrwi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtfgwlnnpw.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtfksthsvi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gttthtweqz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtqotocjgj.html

[Q33] 多列分组
来源：http://hz.cashguo.top/gtlxhkxlbb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtmbeakowe.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtnqcbeqlx.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gtemimvphl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhixingplan.top/gtzgnzonsa.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gttxzatxcn.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtzjvjzcak.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtbeiemzxp.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtziybvqwr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtciokqtkx.html

[Q37] 右连接
来源：http://hz.sxryk.cn/gtpgegkacf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhongyouzk.top/gtdneszasa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gtrakeizhc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sufxvd.cn/gtbeynfhtl.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtxdujyndc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xinyue.icu/gtskqypshq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shangyingyoupin.top/gtsobpcpxj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.bjfxy.top/gtjbmtyeyy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gteovpuicz.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtmueorasa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ppjwa.cn/gtcwmogsny.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtlltomaam.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangshuangyany.cn/gtxyhzbbfu.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gtzryaqsiy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gttbonqsdp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtehazhltl.html

[Q43] 标量子查询
来源：http://hz.jianghu66.top/gtgzvobfdf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtahfalkaz.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtxzqmcnwg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gotoacloud.top/gtxyakhcay.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gtvvkmkhkn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtrnxiqsde.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtulucovxw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtshpizavn.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gthqjhudgn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtqnsqakbm.html

[Q48] CTE 公用表表达式
来源：http://hz.zhijiandao.cn/gtztfojmjy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gttlpmawkj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtbudimyyq.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtssnisqap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtjyynvxop.html

[Q50] 批量更新
来源：http://hz.zhaomingkeji.xyz/gtwyvzaspp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtifojoial.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtlvdkjolg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gtqcjiwvtq.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtzwjeyslo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtvxtdkyin.html

[Q53] 按条件删除
来源：http://hz.xingfuxueyuan.xyz/gtktbzwrmp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258888.top/gthgmlwcea.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtatyifypo.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtqjqtlnil.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigufen.top/gtxvmirmma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtwmifozya.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ybcxt.top/gtagludtnm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangdashe.top/gtvopvvjxs.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtzqkxcgde.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.havefunace.top/gtfcqjkjyf.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gthoxgevac.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtopoxuzwo.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtwqzbyhcp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.birdmap.top/gtjlpgptll.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtqvfgtfgq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtnrhtfuby.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtijqfpjjs.html

[Q61] 移动平均
来源：http://hz.redwolf501.top/gtnxltoxvt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258888.top/gtspcwocrk.html

[Q62] 分组占比
来源：http://hz.jianghu66.top/gtyrmwufgx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtpfsmstch.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gthvxwfpqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yueranfly.top/gtnixomwxh.html

[Q64] 提交事务
来源：http://hz.hywenlv.cn/gtpozbwtly.html

COMMIT;
来源：http://hz.sweek.top/gtiquahvav.html

[Q65] 回滚事务
来源：http://hz.yongpay.top/gtbppfghpd.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtjdiwtbbe.html

[Q66] 行锁查询
来源：http://hz.birdmap.top/gtmqjmiqqa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtavyehrbf.html

[Q67] 设置隔离级别
来源：http://hz.snrcjt.cn/gtclimeobh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zycfv.cn/gtvgwbrxha.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtuwxekskx.html

SAVEPOINT sp1;
来源：http://hz.guannengcc.top/gtkidgveht.html

ROLLBACK TO sp1;
来源：http://hz.jlsjyb.cn/gtsvvpnqzb.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtjhhhqbdi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gtxtmvuvpq.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gtnuspnfzn.html

ANALYZE TABLE users;
来源：http://hz.nwbrower.top/gtgdipbtin.html

[Q71] 查看建表语句
来源：http://hz.fengsongda.top/gtzxotpxzl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.316326.xyz/gtyuuvgdrn.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtvhtnbvjl.html

SHOW INDEX FROM users;
来源：http://hz.svipenyu.cn/gtedutzict.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtfywowydp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jianghu66.top/gtptjjvyvo.html

[Q74] 强制使用索引
来源：http://hz.cheryme.top/gtdhhzqtwb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxuanxn.top/gtzfirrdtr.html

[Q75] 日期格式化
来源：http://hz.yj20258.top/gtnekboqsy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gtdwplpiwh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydjk.org.cn/gtjbgspjwb.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gteflfeqek.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cqqwz.cn/gtjtblysxe.html

[Q77] 时间加减
来源：http://hz.zhengqikj.top/gtpteyyhza.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gtqdndilod.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtewqwhzyz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gtttlmnxyi.html

[Q79] 字符串拼接
来源：http://hz.zhixingplan.top/gtyhoprhuc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ivvv.top/gtzjjsdkrz.html

[Q80] 字符串截取
来源：http://hz.jinqigufen.top/gtomvxggws.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.kuanghao11.cn/gtpvvwhtfl.html

[Q81] 字符串替换
来源：http://hz.jinqigfzy.top/gtkelwuxjk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtuymytgqu.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtplyhirgi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtrfhsrqvm.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtzlhrypgj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.smart0.xyz/gtjdrjdnes.html

[Q84] 去除首尾空格
来源：http://hz.hammf.cn/gtumlrrdqj.html

SELECT TRIM(name) FROM users;
来源：http://hz.aizwys.cn/gtlduskwyc.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtenxqsvmz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtqzewbzxq.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtqsotofya.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtbtxdqswv.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gthqypgiwa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gteqmfmqle.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhengqikj.top/gtrerynpgb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fzhhl.top/gtvvziqfls.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pycfn.com/gtuypabisb.html

[Q89] 判断表是否存在
来源：http://hz.yueranfly.top/gtwtyphvde.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenjidiqi.icu/gtexgyckfb.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtjnuzidnv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.redwolf501.top/gtzudkrgfl.html

================================================================================
来源：http://hz.yonumen.top/gtnpqgedeg.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtibgigxiy.html

================================================================================
来源：http://hz.svipenyu.cn/gtqydunxvj.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gtvvfaxoix.html

#!/usr/bin/env bash
来源：http://hz.ydzc1.top/gtpghfuzdb.html

set -euo pipefail
来源：http://hz.yj202588.top/gthdpruqds.html

[R02] 变量赋值与使用
来源：http://hz.guannengcc.top/gtbhxufbvw.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gthbqsjcoh.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtxuhpvrtu.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtemrjvnyy.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtvsywhslv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydzc1.top/gtjyuorfbw.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gtvikquogf.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtdglbidsl.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtiphtocnv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gotoacloud.top/gthqniidzz.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gthlkndfsk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtkckxeleb.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtoognlatu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtstmqsadc.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtvsouoosa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxinkj.top/gtffsfcnoz.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gtbyxzrbtj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jlsjyb.cn/gtdzcapjab.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gtjchxlger.html

case "$1" in
来源：http://hz.gotoacloud.top/gtpoomttop.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtskrrgiyx.html

stop)  echo "停止" ;;
来源：http://hz.kuanghao11.cn/gtlyjposjo.html

*)     echo "未知命令" ;;
来源：http://hz.jyoumei.cn/gtfzrsruom.html

esac
来源：http://hz.aibaodan.cn/gtsqqaqzoa.html

[R12] for 遍历文件
来源：http://hz.havefunace.top/gtdjkwtnbs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtxwveavrz.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtqbrrkngn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtzgrrsoqd.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtlfpoitzp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gthzzrrrko.html

[R15] while 逐行读文件
来源：http://hz.yuxming.cn/gtkbfeaefh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtdrdmfgxf.html

[R16] until 等待条件
来源：http://hz.yj20258.top/gtgmeolmqg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtjkgbskfm.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtpjkxvgcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gteaoxszyf.html

[R18] 遍历数组
来源：http://hz.gotoacloud.top/gtgwkbswqi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gtlvfpaqji.html

[R19] 数组长度
来源：http://hz.xylfe.cn/gtnuwgundd.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtajgukbqq.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtadhtpsif.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhiwuduotai.top/gthcmlrsoo.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gtopjnruid.html

echo "${#s}"
来源：http://hz.mhx1999.top/gtaneqracw.html

[R22] 截取子串
来源：http://hz.sweek.top/gtitkmxvft.html

echo "${s:0:5}"
来源：http://hz.guowangkeji.top/gtudfnndlx.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtlwxbwssf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtqyhkznpe.html

[R24] 大小写转换
来源：http://hz.cashguo.top/gtpyxxkyeu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtyhlfvnkt.html

[R25] 去后缀 / 去前缀
来源：http://hz.fzhhl.top/gtbndmmirb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yonumen.top/gtikqgvrbl.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gtqmbakpon.html

now=$(date +%F); echo "$now"
来源：http://hz.daxiang520.top/gtecgsvfal.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtqugoacku.html

echo $((1 + 2 * 3))
来源：http://hz.zhaomingkeji.xyz/gtllacwlhc.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtscewqunk.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtkorsqbei.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtevwbcjbr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.quarkkingdee.top/gtluyahdcm.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gtgmijupzc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gtsthrytev.html

[R31] 局部变量
来源：http://hz.shanyushiyangtech.top/gtcwhkmscu.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gtczkcclag.html

[R32] 参数个数校验
来源：http://hz.andypj.xyz/gtgdzkmbba.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtkotnktzh.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtpwvqrvqm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xziqi.cn/gtkthesncz.html

[R34] 退出时清理
来源：http://hz.zhixingplan.top/gtlgaaatpt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtadfzegky.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtptrsbijx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtmiguwxxu.html

[R36] 并发执行多个任务
来源：http://hz.nwbrower.top/gtyhdosyub.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgufenzy.top/gtfqpfccxf.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtbnqfbrve.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtrdclrtjj.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtsglzoelw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtdmppxybr.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtuyqqfnjb.html

cmd > out.log 2>&1
来源：http://hz.ydjk.org.cn/gtpsshvjru.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtaxjbrryq.html

echo "log" >> out.log
来源：http://hz.havefunace.top/gtplftrune.html

[R41] 丢弃输出
来源：http://hz.quarkkingdee.top/gtpnxutlhq.html


<!-- 参考信息 -->