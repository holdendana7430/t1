代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.316326.xyz/gtpyhqwcld.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigfzy.top/gtevvkkofx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.svipenyu.cn/gtssqncquc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtixlcphgy.html

================================================================================
来源：http://hz.haohaochexian.top/gtnsmnzieu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtqhbcmzku.html

================================================================================
来源：http://hz.zhongyouzk.top/gtscglwyhv.html

[Q01] 创建表
来源：http://hz.daxiang520.top/gtdfrdbgso.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gthspcagpr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtsdhntbsr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhengqikj.top/gtvrlgfmzv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guowangkeji.top/gtrmliipkh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuetiantiany.cn/gtjrsopger.html

);
来源：http://hz.zdqjudy.top/gtcjfyxvwo.html

[Q02] 创建带外键的表
来源：http://hz.sxryk.cn/gtcutluqos.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtoecvtzyk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtmidcjhou.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtwbxnyqmi.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtlwvvamxm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.birdmap.top/gtzvivhadb.html

);
来源：http://hz.feifeiyinyue.top/gtljgdripo.html

[Q03] 增加列
来源：http://hz.feifeiyinyue.top/gtiddgrgdj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtaaeubchv.html

[Q04] 修改列类型
来源：http://hz.dashuyun.cn/gtpjctdcoz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sufxvd.cn/gtvlfufjob.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtmpccewxf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtwpmbewnw.html

[Q06] 删除列
来源：http://hz.jqgfzy.top/gtyogwjmyo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtokyalwps.html

[Q07] 删除表
来源：http://hz.0kj1m.cn/gtgxdwsjki.html

DROP TABLE IF EXISTS orders;
来源：http://hz.havefunace.top/gtfhztfeou.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtmdcwntty.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nwbrower.top/gtrikxtuav.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtyosdlgrk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuanzx.com/gtqwwwuwkl.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtdubidxak.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgfzy.top/gtreugatcc.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gtsoicprsr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gttpxvprmr.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtwfxxmjzp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtdwurttav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtxljxmgyd.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtekuqhcby.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gtiyhdpqpl.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtqbqxlnki.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hongshengwenyu.top/gtcaoekmii.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258.top/gttesklnsx.html

[Q15] 查询全部
来源：http://hz.ydzc1.top/gtyygauuvm.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtpisluzxv.html

[Q16] 查询指定列
来源：http://hz.feifeiyinyue.top/gtisbiheoc.html

SELECT id, name FROM users;
来源：http://hz.jqgufenzy.top/gthegzplzw.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gtaipvoybn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtbcenviaw.html

[Q18] 模糊匹配
来源：http://hz.jlsjyb.cn/gtgzgufmzj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtqssithfz.html

[Q19] 范围查询
来源：http://hz.52xcode.cn/gtlsthqgvs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtzkgfrcon.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtgzoebyeo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtrpmcaciw.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtwfaxotzs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jiagoushi.top/gtokbugahh.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtqnekllhr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtonrmkito.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtryitqpng.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.bjfxy.top/gtiycerehc.html

[Q24] 去重
来源：http://hz.yonumen.top/gtlkaiffhv.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gtsgizscbb.html

[Q25] 只取前 N 条
来源：http://hz.cashguo.top/gtgorwiava.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxinkj.top/gtopgoskxr.html

[Q26] 计数
来源：http://hz.9152youxi.cn/gtyzehhies.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtnimedrzh.html

[Q27] 条件计数
来源：http://hz.sweek.top/gtfqopmcrw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtascxqnun.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtwifforah.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtbbzwmsna.html

[Q29] 最大最小值
来源：http://hz.yuanzhike.top/gtnkpxiozi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtvqqzxemy.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtlhkqanbe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtzmgjsrgr.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtgsryvwad.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtefojcezv.html

[Q32] 分组拼接字符串
来源：http://hz.0kj1m.cn/gtduxfbkdu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtrpnewpfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sufxvd.cn/gtpzhbrvyh.html

[Q33] 多列分组
来源：http://hz.hnqzz.top/gtufgkmknr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtbwibttzt.html

[Q34] 每组取第一条
来源：http://hz.daria6918.cn/gtgirfsrxk.html

SELECT * FROM (
来源：http://hz.gaohongyu789.top/gthwtrfyai.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gtedbpkagr.html

) t WHERE rn = 1;
来源：http://hz.jqgfzy.top/gtzrkzuuut.html

[Q35] 内连接
来源：http://hz.zhongyouzk.top/gthutgrrlu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtnfywtxaz.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gtooqeodyu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtjbkpjswx.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtdfjdcwcz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtozpivtyb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgufenzy.top/gtzrwomwce.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtoxfziynx.html

[Q39] 自连接（查上下级）
来源：http://hz.guannengcc.top/gtcmavzlxn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.vqdsnc.cn/gtlnbxvexd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gttgcqrqen.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtpdlgnbcp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtqelejncc.html

[Q41] 多表连接
来源：http://hz.ybcxt.top/gttzmalqna.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtaagpvxsj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jianghu66.top/gtrpalvusv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.haohaochexian.top/gtitgmleum.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtzssbilhy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtogkhjagb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuxming.cn/gttdkbmwdb.html

[Q43] 标量子查询
来源：http://hz.zhaomingkeji.xyz/gthwkekyuj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtpltnncyn.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtnkxwntuh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtcqqqldkg.html

[Q45] EXISTS 判断存在
来源：http://hz.0kj1m.cn/gtdwmuqgni.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtujwnjjky.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gtrpbpwyrv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtldzjldty.html

[Q47] 与平均值比较
来源：http://hz.jiagoushi.top/gtqgoghvoo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nwbrower.top/gtwbqoeeqd.html

[Q48] CTE 公用表表达式
来源：http://hz.ehwqpu.com/gttgkfweek.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pengpengdd.cyou/gtsmiwbvlu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gteyzoviel.html

[Q49] 更新单行
来源：http://hz.zycfv.cn/gtaysvcwuh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtxmhtxaby.html

[Q50] 批量更新
来源：http://hz.cheryme.top/gtolqwwjnh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtiwztweua.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtmrfslfbf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtkdlajkgi.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtwusgopzf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtxfghdzhl.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtbznsfngr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gogol.net.cn/gtenuhhusk.html

[Q54] 清空表
来源：http://hz.guannengcc.top/gtntqjpksa.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gtkwjyzlbx.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtyfsszeto.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtpgqbsehj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtwzlywimf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258.top/gtujbufylc.html

[Q57] 行号
来源：http://hz.kuanghao11.cn/gtudcnfyum.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtzcywhame.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gtzlipuznb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtsikckdsw.html

[Q59] 分组内累计
来源：http://hz.zhixingplan.top/gtrqahxrtq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ivvv.top/gttzivxqpd.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenjidiqi.icu/gtqwgzydoz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gtscmulies.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtrwjjyyhk.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtsosjpevq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sxryk.cn/gtqsqtltxb.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtvnbocwnt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtjafwurwh.html

[Q63] 开启事务
来源：http://hz.ppjwa.cn/gttadwbibp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtpqmxnlpu.html

[Q64] 提交事务
来源：http://hz.0kj1m.cn/gtbotfhwkz.html

COMMIT;
来源：http://hz.ppjwa.cn/gttypynwqv.html

[Q65] 回滚事务
来源：http://hz.gaohongyu789.top/gtgpkoejhp.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtbqbewdtg.html

[Q66] 行锁查询
来源：http://hz.sufxvd.cn/gtbphqsfke.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtslcnqmar.html

[Q67] 设置隔离级别
来源：http://hz.cucudq.cn/gtfvhtwgkb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gtihppwbxk.html

[Q68] 保存点
来源：http://hz.jianghu66.top/gtesnemepd.html

SAVEPOINT sp1;
来源：http://hz.sysykeji.top/gtvhwirwgw.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gteiiymcon.html

[Q69] 查看执行计划
来源：http://hz.sufxvd.cn/gtpsysqngt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.9152youxi.cn/gtaxmdztqs.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gtnminwono.html

ANALYZE TABLE users;
来源：http://hz.ybcxt.top/gtswstaydn.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gtmseajfrv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenlongwang.top/gtqccsafmw.html

[Q72] 查看索引
来源：http://hz.shangyingyoupin.top/gtxefhmsde.html

SHOW INDEX FROM users;
来源：http://hz.bjfxy.top/gtswtucmow.html

[Q73] 查看表状态
来源：http://hz.nanxinkj.top/gteisapfgr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtwzckyymi.html

[Q74] 强制使用索引
来源：http://hz.xuetiantiany.cn/gthegkoafl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yongpay.top/gtbkwhwwjy.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtmthdqavt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.redwolf501.top/gtbfdondrt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.0kj1m.cn/gtrnecbnot.html

[Q76] 按天统计
来源：http://hz.andypj.xyz/gtxqekijni.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gtelttzedx.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtecckxmty.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtvlcpohbo.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gttyenhoiw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtxnewdtif.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtgplwubox.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtvpkraqbn.html

[Q80] 字符串截取
来源：http://hz.ydzc1.top/gtyavfhgev.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtmeavwsql.html

[Q81] 字符串替换
来源：http://hz.jyoumei.cn/gtlmobluxi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xziqi.cn/gtwdkbthav.html

[Q82] 字符长度与字节长度
来源：http://hz.jinyuanbaomall.cn/gtxuxhrauk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.mhx1999.top/gtgduxbplb.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtbvsgbtvy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dashuyun.cn/gtevagdjus.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtvjobsnzw.html

SELECT TRIM(name) FROM users;
来源：http://hz.aibaodan.cn/gtzlmxtkqm.html

[Q85] 数值取整
来源：http://hz.nanxuanxn.top/gtppialzvo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtfifawgjp.html

[Q86] 读取 JSON 字段
来源：http://hz.pengpengdd.cyou/gtqflijahb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtgrzwydbe.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtajqlnghz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtftqldtae.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gtklmjjrnb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtltynhrsm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtgjcjfdxk.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gtrmcxonhi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtowvfxdhs.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtokemofre.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.dashuyun.cn/gtfhynbrpt.html

================================================================================
来源：http://hz.316326.xyz/gthlebkxms.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gtaktdohrd.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjlidopvv.html

[R01] shebang 与严格模式
来源：http://hz.ydjk.org.cn/gtpknooewz.html

#!/usr/bin/env bash
来源：http://hz.ivvv.top/gtwumykxtg.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gtgtsolawc.html

[R02] 变量赋值与使用
来源：http://hz.yvedp.cn/gtxbpiqekp.html

name="Tom"; echo "$name"
来源：http://hz.fengsongda.top/gtjwgxzrsv.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtllvufdvx.html

readonly PI=3.14
来源：http://hz.0kj1m.cn/gtdwaimksu.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtncmetkih.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtplswcudu.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtpnaawrtw.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gttnducaua.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtiwdmfrfp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtsybfmyov.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtaqilvqww.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yueranfly.top/gtdgdjfaku.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtvbfhvbcr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtfgmtyodo.html

[R09] 字符串比较
来源：http://hz.daria6918.cn/gtalaxzpci.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gtnjixquee.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtolxnvemt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtvfnmrted.html

[R11] case 多分支
来源：http://hz.yanxiufei.cn/gtzqhfltxt.html

case "$1" in
来源：http://hz.daria6918.cn/gtnrgeesjz.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gteilazpem.html

stop)  echo "停止" ;;
来源：http://hz.9152youxi.cn/gtnaetizjl.html

*)     echo "未知命令" ;;
来源：http://hz.jqgufenzy.top/gtdzlmydtu.html

esac
来源：http://hz.316326.xyz/gtbtaecqcz.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtmfuyahsk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hysaishi.cn/gtxkldblpk.html

[R13] for 计数循环
来源：http://hz.hysaishi.cn/gtobowtwnw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtdjotqtaq.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gttqckfioc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jyoumei.cn/gtjrtejbqg.html

[R15] while 逐行读文件
来源：http://hz.redwolf501.top/gtrfsdbogp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtddgyesft.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtiblxhemx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtknofiqqn.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtjjrkgczv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtbypafubf.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtijkawpgp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gthigsiqtl.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtnzxzzffv.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtpjcstxtt.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtcixmjbez.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtmomasuhu.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gtuuyxiyho.html

echo "${#s}"
来源：http://hz.yongpay.top/gttrmpubmv.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtfhtunrvh.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtuauogtyn.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtdaljxgps.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtwcdcpaov.html

[R24] 大小写转换
来源：http://hz.hysaishi.cn/gtlltnlrrq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ppjwa.cn/gtgpkrexiv.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtosyzrmze.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yonumen.top/gtjynokzdm.html

[R26] 命令替换
来源：http://hz.daxiang520.top/gtaufavcix.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtntxzfmcd.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtjalqfpcr.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtumivuvsg.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtogxsudlk.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtbpxpcdsr.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtuxtgpfjk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gtafwzbthg.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtarktgcvr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gtzkdofcys.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gtxmeomqld.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtpukxjgan.html

[R32] 参数个数校验
来源：http://hz.tian-w.cn/gtubkxukwq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gtrqxekdkh.html

[R33] 捕获错误并提示行号
来源：http://hz.cheryme.top/gtklopymie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtvypgmbre.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtuarqjrtc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtkslltzfm.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtraifgrlf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gaohongyu789.top/gtjakxpwwi.html

[R36] 并发执行多个任务
来源：http://hz.quarkkingdee.top/gtnbuuoogx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gtnfhmiugt.html

[R37] 把输出赋给变量
来源：http://hz.yanxiufei.cn/gtdiutlzlr.html

files=$(ls -1)
来源：http://hz.iojbl.cn/gtwdclmrvs.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtfjlboqry.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinyuanbaomall.cn/gtlfhotrru.html

[R39] 重定向标准输出与错误
来源：http://hz.fzhhl.top/gtuxlsojzv.html

cmd > out.log 2>&1
来源：http://hz.smart0.xyz/gtptquobfn.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gtmibysdgy.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtovbwbrzb.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtlqpyerhg.html


<!-- 参考信息 -->