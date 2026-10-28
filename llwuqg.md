代发 wailian999

================================================================================
来源：http://hz.nwbrower.top/gteqfkoajx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuxming.cn/gtqjnwqura.html

================================================================================
来源：http://hz.yvedp.cn/gtxluzkywa.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtyjcdwuqc.html

CREATE TABLE users (
来源：http://hz.zhaomingkeji.xyz/gtwovscxxy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtfcwcnvew.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtfpyirrgi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtzmakdlbu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gtxbtazjlg.html

);
来源：http://hz.pycfn.com/gttjgqqqih.html

[Q02] 创建带外键的表
来源：http://hz.wangdashe.top/gthvcocmkq.html

CREATE TABLE orders (
来源：http://hz.pengpengdd.cyou/gtxpeancxb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtwgzjrpgb.html

user_id INT NOT NULL,
来源：http://hz.hammf.cn/gtwqihzlfm.html

amount DECIMAL(10, 2),
来源：http://hz.hongshengwenyu.top/gtasfadssy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtmkynojmz.html

);
来源：http://hz.aibaodan.cn/gtycruqxtd.html

[Q03] 增加列
来源：http://hz.zhijiandao.cn/gtfyhtcbqi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtorjnoqnb.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gtwxrsqidb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gtpejoditr.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtassuzeer.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtjuuhbimz.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtwwuyimkm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gtmtfeafaa.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtsfciheng.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtreyphptl.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtpmizqher.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aizwys.cn/gtwtpobjws.html

[Q09] 创建唯一索引
来源：http://hz.cheryme.top/gtgaeyltyx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtppmxrlnj.html

[Q10] 插入单行
来源：http://hz.zycfv.cn/gtrlbdkzkf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cdnleiting.top/gtksrmhtdk.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gtgizxtrmt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuanzhike.top/gtcwlntdhj.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtlwtuhzog.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.svipenyu.cn/gtatlvglib.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtkxmqssby.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtizvcaair.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtgorrpogj.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuetiantiany.cn/gtrzlqmbkg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtvxbgpwea.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtexxxzvep.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtxklylnhw.html

SELECT * FROM users;
来源：http://hz.cucudq.cn/gtfpxopfyc.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtkabkfgtn.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtgoocxbpb.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtfkiwbdhg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuanzx.com/gtnejgvpto.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtgexoraop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtcnedqfom.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gtcqxnzghu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gtowiwkztz.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtahjvvxgb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sweek.top/gtjgswphqz.html

[Q21] 空值判断
来源：http://hz.mhx1999.top/gthqrlmile.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guowangkeji.top/gtfdfvwbtm.html

[Q22] 排序
来源：http://hz.jlsjyb.cn/gttyjmjocs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxinkj.top/gtmllgprhr.html

[Q23] 分页
来源：http://hz.meibo888.top/gtciqkdcte.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cqqwz.cn/gtrgqwplgd.html

[Q24] 去重
来源：http://hz.zhongyouzk.top/gtfpcnvxnr.html

SELECT DISTINCT city FROM users;
来源：http://hz.smart0.xyz/gtoiinqvte.html

[Q25] 只取前 N 条
来源：http://hz.tian-w.cn/gtjujidezz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gtevlwtllh.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtrqrzjllv.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtqyokfkem.html

[Q27] 条件计数
来源：http://hz.yvedp.cn/gtlhuwixcc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangtech.top/gtvjujjwui.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtlxqiyepb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtzsvgcsfy.html

[Q29] 最大最小值
来源：http://hz.jianghu66.top/gtxmxnrnug.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtnddophnx.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gtptcdtkov.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtccbilgjn.html

[Q31] 分组后过滤
来源：http://hz.hysaishi.cn/gtquubjtmd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtoptifjnq.html

[Q32] 分组拼接字符串
来源：http://hz.cqqwz.cn/gtssolctwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtmcxbwmhb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtrrxrpugv.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtosctukod.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gtsellvkmo.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtzxkualhm.html

SELECT * FROM (
来源：http://hz.ybcxt.top/gtyhhirotv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtbcxydffg.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtgtztwwdj.html

[Q35] 内连接
来源：http://hz.xinyue.icu/gtolhvayof.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtnnaxsxrv.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtypraoeaw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gthdauwypf.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtwdjxfxob.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yueranfly.top/gtcjyeltyc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxuanxn.top/gtasdeikyv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yanxiufei.cn/gtttujkvuv.html

[Q39] 自连接（查上下级）
来源：http://hz.zdqjudy.top/gtkevhoftv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guannengcc.top/gtwprxqgyk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gtorotzmwz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sufxvd.cn/gtychpomwe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtpmgffxun.html

[Q41] 多表连接
来源：http://hz.9152youxi.cn/gtcmcbkhyy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jlsjyb.cn/gtdktsgnzt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuanzx.com/gtgktmukbo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fzhhl.top/gtulymcavy.html

[Q42] 连接条件附加过滤
来源：http://hz.tianlin.xyz/gtbjnmxymc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtchigdxch.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pengpengdd.cyou/gtbvbkkhgd.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gtjbklibgi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gogol.net.cn/gttgxiidvd.html

[Q44] IN 子查询
来源：http://hz.daxiang520.top/gtjfrwqtyg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtcabubulp.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gthywurjid.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtdxoupszv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigfzy.top/gthicojinw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtqrmotpfq.html

[Q47] 与平均值比较
来源：http://hz.cqqwz.cn/gtvjpwwdwh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigufen.top/gtbycvjxxe.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gtetemljet.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtfawgguxb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtenvasymj.html

[Q49] 更新单行
来源：http://hz.jinqigfzy.top/gtgucejhda.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtknrnlrld.html

[Q50] 批量更新
来源：http://hz.dashuyun.cn/gtebncojtl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtagrjszft.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtaatolnwd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtsknnzixp.html

[Q52] 删除指定行
来源：http://hz.nwbrower.top/gtxncaqips.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xziqi.cn/gtzghgawmv.html

[Q53] 按条件删除
来源：http://hz.meibo888.top/gtfqbbzrsi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtyatrfdcs.html

[Q54] 清空表
来源：http://hz.jqgufenzy.top/gtwtjzmris.html

TRUNCATE TABLE logs;
来源：http://hz.dianchejie.cn/gtewmtddkp.html

[Q55] 排名（并列占位）
来源：http://hz.snrcjt.cn/gtxibebvps.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtrxijxmdg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gtmaxyulpv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtjiqmemmr.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtneubfzfk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtdlpwnoow.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gthdaojzyl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtseyjcxxx.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtqwyarczz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.vqdsnc.cn/gtdtgnxled.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gthfsvdbmh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.0kj1m.cn/gtfwdrtjsb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtswhdjpdp.html

[Q61] 移动平均
来源：http://hz.chenjidiqi.icu/gtsvhyodlx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.quarkkingdee.top/gtulykbywo.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtgmlwzzkv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtuqioupte.html

[Q63] 开启事务
来源：http://hz.dianchejie.cn/gtltgchbzu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtmdjlhtey.html

[Q64] 提交事务
来源：http://hz.aizwys.cn/gtpygnkyks.html

COMMIT;
来源：http://hz.jiagoushi.top/gtwfefgfyc.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtfvdfgatk.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtxhcuitkt.html

[Q66] 行锁查询
来源：http://hz.snrcjt.cn/gtkmhoyynf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.smart0.xyz/gtrvoqdhjy.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gteuynpuvj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gturziidyc.html

[Q68] 保存点
来源：http://hz.dianchejie.cn/gtlttwvwai.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gtyclbujpu.html

ROLLBACK TO sp1;
来源：http://hz.mhx1999.top/gtxpdkheel.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtdrebstbb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtnicmsgse.html

[Q70] 更新统计信息
来源：http://hz.xingfuxueyuan.xyz/gtkcifuctd.html

ANALYZE TABLE users;
来源：http://hz.ppjwa.cn/gtrtnhrxat.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtasqchzmd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtigevzyxn.html

[Q72] 查看索引
来源：http://hz.gzhubu.top/gtrrmmuhlg.html

SHOW INDEX FROM users;
来源：http://hz.svipenyu.cn/gtpeipbhsj.html

[Q73] 查看表状态
来源：http://hz.guannengcc.top/gteekyksdf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daria6918.cn/gtxkgcyfyg.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtmgcykper.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtkbvlpnav.html

[Q75] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtbunekdor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtojbqkpgs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtlesozkbg.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtntuetghm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuanzhike.top/gthnrhtfbf.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtcgqjtesc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhijiandao.cn/gttbwtzsyq.html

[Q78] 当前时间
来源：http://hz.xingfuxueyuan.xyz/gtrsudxiyv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ybcxt.top/gtsdpyxkxv.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gtotmzpeeq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtblsxvmji.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtljstpvnt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.9152youxi.cn/gtqwmtfzhe.html

[Q81] 字符串替换
来源：http://hz.snrcjt.cn/gtjsietkpc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gtfjgaltag.html

[Q82] 字符长度与字节长度
来源：http://hz.cashguo.top/gtsbxbvgba.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtigyvvabk.html

[Q83] 大小写转换
来源：http://hz.chenjidiqi.icu/gtcknkwqav.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtnutmqizf.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtmxviardt.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtawxrqhle.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtrakvsngx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gthohcxwlw.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtcaylgbam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtevnnkdiw.html

[Q87] JSON 字段做条件
来源：http://hz.ppjwa.cn/gtbosztmqe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgfzy.top/gtdpcvrrll.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtnqazlkwo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gthqcfltpo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guannengcc.top/gtpcdvasrl.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtjeffaqmw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtjrtscihr.html

[Q90] 生成序号列
来源：http://hz.yongpay.top/gtaxoxwbmh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtwbcqkjhl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmhqkfhpk.html

R. Bash 专题
来源：http://hz.ivvv.top/gtycjmtfoa.html

================================================================================
来源：http://hz.ydzc1.top/gtaaxjybjs.html

[R01] shebang 与严格模式
来源：http://hz.havefunace.top/gtkejcfkol.html

#!/usr/bin/env bash
来源：http://hz.mhx1999.top/gtvfwtraik.html

set -euo pipefail
来源：http://hz.xziqi.cn/gtbczveykh.html

[R02] 变量赋值与使用
来源：http://hz.ehwqpu.com/gtuezxfpmx.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtqfiursly.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtwemywkpe.html

readonly PI=3.14
来源：http://hz.pycfn.com/gtgaedpbtq.html

[R04] 位置参数
来源：http://hz.yj202588.top/gtlpadkppg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gogol.net.cn/gtwsyftpve.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtedskkjwe.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtlttpucfq.html

[R06] 判断命令是否存在
来源：http://hz.ivvv.top/gtkyslysow.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtvstgjxhm.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtmtyzpoul.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnqzz.top/gtmsrsgtip.html

[R08] 数值比较
来源：http://hz.wangdashe.top/gtwhzbfoiz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.9152youxi.cn/gtekirohyh.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtizhkifhj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yongpay.top/gtozsfwual.html

[R10] 正则匹配
来源：http://hz.xylfe.cn/gtdwddyccx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnxiangtu.top/gtxxucobij.html

[R11] case 多分支
来源：http://hz.fzhhl.top/gtlwagwuwy.html

case "$1" in
来源：http://hz.ppjwa.cn/gthyipvcfs.html

start) echo "启动" ;;
来源：http://hz.gogol.net.cn/gtkjabdrzl.html

stop)  echo "停止" ;;
来源：http://hz.wangdashe.top/gtjxfxyirg.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtuptswlby.html

esac
来源：http://hz.zhixingplan.top/gtevrnyrjj.html

[R12] for 遍历文件
来源：http://hz.ppjwa.cn/gtptirmxow.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gaohongyu789.top/gtfzsnqsdx.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtpcbhiqpt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gtxgrpfvik.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtcgqfpquz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtxrriepub.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gttqmjzwnf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gtyctkrypx.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtomwjitbb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gtgkzpjhex.html

[R17] 数组定义与取值
来源：http://hz.feifeiyinyue.top/gtiiczrtnm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258.top/gtbcealdbb.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtkczjhafp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtkazgduim.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtbeyfagjt.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gtdkawcuyv.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gteguytqmq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtitpwmmjl.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtzxiugbgi.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtsphclvam.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtiefyhqcb.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtzkfhciet.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtftwqwpcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ehwqpu.com/gtvtdvztri.html

[R24] 大小写转换
来源：http://hz.yanxiufei.cn/gtujuentsv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangdashe.top/gtnzwwfbml.html

[R25] 去后缀 / 去前缀
来源：http://hz.shuidangran.top/gtelagfjph.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtxwrcxxau.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gtjhienyxm.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtvflyuuyk.html

[R27] 算术展开
来源：http://hz.sweek.top/gtnvsvjitm.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtzcvoplwk.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtpkmaqvzp.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuanzx.com/gtpkmxsqch.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtrmgphlho.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gtmgdhsyyj.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtrqwblbky.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yvedp.cn/gtazhrfsmt.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtrngebboz.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxinkj.top/gtgjrfcwus.html

[R32] 参数个数校验
来源：http://hz.jinghuilouyu.cn/gtwynnyamz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.pycfn.com/gtwkuvijgo.html

[R33] 捕获错误并提示行号
来源：http://hz.chenjidiqi.icu/gtfhwxfnwl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtwrqmineb.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gtjixwgivn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtlrjdyqxy.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtaegbxkap.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtoshrkmab.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtppoatrvm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtohebhkat.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gttznwjbew.html

files=$(ls -1)
来源：http://hz.yuanzhike.top/gtdmwnrphv.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtznbkecip.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtoyejgcwu.html

[R39] 重定向标准输出与错误
来源：http://hz.gzhubu.top/gtzyfdccyv.html

cmd > out.log 2>&1
来源：http://hz.tianlin.xyz/gtmlbzkmiv.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gtiotpuzzc.html

echo "log" >> out.log
来源：http://hz.cdnleiting.top/gtqtgpdbvn.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtaaenimqc.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangtech.top/gtkxgegoee.html

[R42] 输入重定向
来源：http://hz.yonumen.top/gtrnmwdiig.html

wc -l < a.txt
来源：http://hz.zhixingplan.top/gtodfbipmp.html

[R43] 按名字查找文件
来源：http://hz.0kj1m.cn/gtnqktxkcv.html


<!-- 参考信息 -->