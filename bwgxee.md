代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtxckzyafj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangkeji.top/gtvpszjlpr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtdlobigzn.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtoatnqpqd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sufxvd.cn/gtqbjlsfvs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtiwlevbax.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtldngbeyr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtlzrzroyw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shuidangran.top/gtgkludjpw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtxrawiedi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtumejwvsu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aibaodan.cn/gtrqhvnorg.html

================================================================================
来源：http://hz.fengsongda.top/gtbtjdcnhk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gthtzrlasq.html

================================================================================
来源：http://hz.yvedp.cn/gtftvmgocc.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtzanygpqp.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtcwiyjlfs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtsnydailo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.9152youxi.cn/gtiyedonjz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtwtdvhymt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.smart0.xyz/gtwmzslwio.html

);
来源：http://hz.sweek.top/gtbesptflq.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtnlsbgzmu.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtwtzzjaed.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtiymprtwz.html

user_id INT NOT NULL,
来源：http://hz.zhengqikj.top/gtsxehfizp.html

amount DECIMAL(10, 2),
来源：http://hz.ehwqpu.com/gtbbzuhyry.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yongpay.top/gtnfjqgrxm.html

);
来源：http://hz.iojbl.cn/gtptkookmu.html

[Q03] 增加列
来源：http://hz.smart0.xyz/gttpjbhixt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtlwbyognx.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtskrzagbu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuetiantiany.cn/gtaidkijoj.html

[Q05] 重命名列
来源：http://hz.wangdashe.top/gtusaohrmw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtljxjcgha.html

[Q06] 删除列
来源：http://hz.sweek.top/gtkzokjcdj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhijiandao.cn/gtllaqvutv.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtwfxoeled.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hongshengwenyu.top/gtlmihufpb.html

[Q08] 创建普通索引
来源：http://hz.mhx1999.top/gtpzvfdfxs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtabtgumuk.html

[Q09] 创建唯一索引
来源：http://hz.birdmap.top/gtfmzayrgp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gtxammplvo.html

[Q10] 插入单行
来源：http://hz.jinghuilouyu.cn/gtlajgvjcp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daxiang520.top/gtxynfxvoz.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtcphbtunc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gthhsbrgds.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtipnhgnam.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgfzy.top/gtfxmwfpxq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.316326.xyz/gteqdxzopn.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gtswxpknjs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.bjfxy.top/gteccboots.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gtpohrzoro.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtcpvbnwdt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtjyriaenz.html

[Q15] 查询全部
来源：http://hz.hnxiangtu.top/gtisreiksn.html

SELECT * FROM users;
来源：http://hz.hammf.cn/gtvvkgloyj.html

[Q16] 查询指定列
来源：http://hz.daria6918.cn/gtizqzgcoj.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtaaygaebj.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtsifyhblx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtvhtvzbsw.html

[Q18] 模糊匹配
来源：http://hz.fengsongda.top/gtqeiacdik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtzybaqikk.html

[Q19] 范围查询
来源：http://hz.mhx1999.top/gtdlfwxzrb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xinyue.icu/gtokglcjtz.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtkpthcwvj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtjifzdxkn.html

[Q21] 空值判断
来源：http://hz.smart0.xyz/gtfxnsspfl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtxsfbpfke.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtzbqsgpvj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhijiandao.cn/gttthynptx.html

[Q23] 分页
来源：http://hz.mhx1999.top/gtigavledf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtfjewyawq.html

[Q24] 去重
来源：http://hz.snrcjt.cn/gthgctvtjm.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhaomingkeji.xyz/gtmiscgufz.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtdpdyivlg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtyovbwaar.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtkakktoui.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtmnzinaih.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gthmsfirmi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.quarkkingdee.top/gteqrzdibo.html

[Q28] 求和与平均
来源：http://hz.yueranfly.top/gtxhrdqaqh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gthzzwvpgr.html

[Q29] 最大最小值
来源：http://hz.hnqzz.top/gtpamdcscp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtvjjvaqox.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtkpnpursc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtympnznku.html

[Q31] 分组后过滤
来源：http://hz.cdnleiting.top/gtdthiswxq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gtzhiredxd.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtzwyexsug.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtdbfrhhmu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtynbkntnj.html

[Q33] 多列分组
来源：http://hz.zhijiandao.cn/gtlsqcqgsm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtcgkmsqec.html

[Q34] 每组取第一条
来源：http://hz.zhoulong.xyz/gtcpbwtobs.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtztzwvvgs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hysaishi.cn/gtqyiledwt.html

) t WHERE rn = 1;
来源：http://hz.xingfuxueyuan.xyz/gtkuxviwrr.html

[Q35] 内连接
来源：http://hz.zycfv.cn/gtorpmmnrt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtjcsuznaj.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtaxejhzmt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtbyjucisy.html

[Q37] 右连接
来源：http://hz.c1oappe.top/gttonmhrgi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtjpbhidkd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtguqohuey.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtdvtbmhit.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gteuktwjzj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gotoacloud.top/gtofxsbqfr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtnjypsndr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gzhubu.top/gtkajhitlm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtucfhyycl.html

[Q41] 多表连接
来源：http://hz.vqdsnc.cn/gtdmmgumuh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtyywntbyt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtouvqwpje.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gtktqylvxm.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtfdutozkf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhixingplan.top/gtytemvcze.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtbaftlbql.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtuahjjkep.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydzc1.top/gthpfzfmjw.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gtevegolpt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtsngljvgm.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtjkqmckjq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtebzqlqoo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cqqwz.cn/gtahqdzsrf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtpwanphca.html

[Q47] 与平均值比较
来源：http://hz.cdnleiting.top/gtiwkehsoz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangshuangyany.cn/gtnftjthzj.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtlwuzwpir.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhaomingkeji.xyz/gtuecopbww.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtbrahkwme.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtzvliescy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtfgeiuspz.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtpdbfzibh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtbhvpewzj.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtzimovhmq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhaomingkeji.xyz/gtbvjbinil.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtpksckixo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtblrlggzf.html

[Q53] 按条件删除
来源：http://hz.cqqwz.cn/gtffxkbjzn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shuidangran.top/gtfqrvrupq.html

[Q54] 清空表
来源：http://hz.sweek.top/gtvhnohlsg.html

TRUNCATE TABLE logs;
来源：http://hz.zycfv.cn/gtgyjokofp.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtmijevmna.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gtwdzogkmw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj202588.top/gtnkgifluh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinyuanbaomall.cn/gttkexlajw.html

[Q57] 行号
来源：http://hz.meibo888.top/gtgnpoudem.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sxryk.cn/gtlctyssqq.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtnfftqlhc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangshuangyany.cn/gtwwpyagad.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtvsihcqdk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtavlspfio.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhengqikj.top/gtephaurvb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtifplafaa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fengsongda.top/gtdeqgvjyq.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtlhzqbptz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258888.top/gtlhxmnhdp.html

[Q62] 分组占比
来源：http://hz.jinqigufen.top/gtqitqdjmp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtxdwbbsgh.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtflwjruxs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sweek.top/gtyrjiievh.html

[Q64] 提交事务
来源：http://hz.wangdashe.top/gtjhjuvnzd.html

COMMIT;
来源：http://hz.sufxvd.cn/gtmocarwtv.html

[Q65] 回滚事务
来源：http://hz.jiagoushi.top/gtlwxcvkzc.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtzwwjhabe.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtbfvrmxkm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenlongwang.top/gtkjrshiio.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gtaztfpefn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gttqznotfu.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtnlvzyzez.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtpbzxxhwq.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtudcwaywh.html

[Q69] 查看执行计划
来源：http://hz.fzhhl.top/gtkrjbjajs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sweek.top/gtmgkqqtvb.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtushthpbw.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gteaesspbs.html

[Q71] 查看建表语句
来源：http://hz.redwolf501.top/gttunkkenk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258.top/gtshumyurv.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtytrifeph.html

SHOW INDEX FROM users;
来源：http://hz.jinqigufen.top/gtrjowhkci.html

[Q73] 查看表状态
来源：http://hz.jianghu66.top/gtpzkmzsej.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gtdzzkyukj.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtntrgqwfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gthqozevjr.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtltdadiji.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gtrszmydsj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xingfuxueyuan.xyz/gttycqdcqe.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtwpkdbhsa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zdqjudy.top/gtqvsgdemq.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtttudcmmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtambpkzed.html

[Q78] 当前时间
来源：http://hz.hongshengwenyu.top/gtpuorspxe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtyzcmefzc.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gttchzwlyj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtdbqnjgwp.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtjduagroe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtvtcquukk.html

[Q81] 字符串替换
来源：http://hz.sweek.top/gtcljplscp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtqbdeskja.html

[Q82] 字符长度与字节长度
来源：http://hz.sxryk.cn/gtfqmuivnp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtijjulpjj.html

[Q83] 大小写转换
来源：http://hz.0kj1m.cn/gtyxckvsyk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangdashe.top/gtmzjssmsy.html

[Q84] 去除首尾空格
来源：http://hz.vqdsnc.cn/gtppvfwaik.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtnekongdh.html

[Q85] 数值取整
来源：http://hz.shanyushiyangkeji.top/gtqawyocvz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtddxijjmz.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtbbgkwljj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtkvykidpv.html

[Q87] JSON 字段做条件
来源：http://hz.hnqzz.top/gtgudmztuc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtrkdpitge.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtzpxanxzn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtezdpoltm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gtakavcqvd.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gthokzxjhy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gtxeogdtpu.html

[Q90] 生成序号列
来源：http://hz.ydzc1.top/gtgeafykmk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtwzqaenib.html

================================================================================
来源：http://hz.gotoacloud.top/gthzeuznvh.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtvakxizcl.html

================================================================================
来源：http://hz.ehwqpu.com/gttxzvxqta.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtbbnhruxu.html

#!/usr/bin/env bash
来源：http://hz.quarkkingdee.top/gtjdnrncoh.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtjecntora.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gtaxzdlzvd.html

name="Tom"; echo "$name"
来源：http://hz.jyoumei.cn/gtsgzjklwe.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtailnsisf.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtugksmgls.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtlcojbbap.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtxzgfkkuw.html

[R05] 参数默认值
来源：http://hz.ydjk.org.cn/gteqvuylcc.html

name="${1:-default}"
来源：http://hz.hongshengwenyu.top/gtjiucqwfb.html

[R06] 判断命令是否存在
来源：http://hz.guowangkeji.top/gtyhgziprp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jlsjyb.cn/gtntnrrrwb.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtronnhcio.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtmkyfolvp.html

[R08] 数值比较
来源：http://hz.zhijiandao.cn/gtjqbxsqdl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtdiqwjffn.html

[R09] 字符串比较
来源：http://hz.svipenyu.cn/gtbfnrhxyo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtvqjxzgvp.html

[R10] 正则匹配
来源：http://hz.xylfe.cn/gtvwutxwst.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pycfn.com/gtkeczituv.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtxeyylyip.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtsobajoil.html

start) echo "启动" ;;
来源：http://hz.iojbl.cn/gtsraxihyb.html

stop)  echo "停止" ;;
来源：http://hz.shangyingyoupin.top/gtfdyxjpmu.html

*)     echo "未知命令" ;;
来源：http://hz.xinyue.icu/gtbcrgazlu.html

esac
来源：http://hz.yongpay.top/gtuuvyufle.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtioejmvhh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtgqdswzzy.html

[R13] for 计数循环
来源：http://hz.zhongyouzk.top/gtgjygxpcm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dashuyun.cn/gtglaldpee.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtgdixbebq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.birdmap.top/gtfifkalxw.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtcnvkgxsh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtfkcnsmmm.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gttprdkhwo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtpwmzfgnl.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtwkthafel.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dashuyun.cn/gtypkvvkrd.html

[R18] 遍历数组
来源：http://hz.0kj1m.cn/gtyytebyac.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtbhcltndm.html

[R19] 数组长度
来源：http://hz.meibo888.top/gtdrucpzum.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtecwldshn.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtvjxccosh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhengqikj.top/gtfyonimys.html

[R21] 字符串长度
来源：http://hz.vqdsnc.cn/gtwcgnwrxk.html

echo "${#s}"
来源：http://hz.c1oappe.top/gtfcgajrfj.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtxxzoohip.html

echo "${s:0:5}"
来源：http://hz.sysykeji.top/gthqbnrqvj.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtxlnetefi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtychjicce.html

[R24] 大小写转换
来源：http://hz.jinqigfzy.top/gtsodmvihr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtkfhkhqvb.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtyqenzcvt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtnbzbonzx.html

[R26] 命令替换
来源：http://hz.ehwqpu.com/gtwrlmiusu.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtoqjahrxb.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtdaohcpcv.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtbdskwkkj.html

[R28] 浮点运算
来源：http://hz.shzxlz.cn/gttzyvgxwn.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhoulong.xyz/gtbaehnkwh.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtqkpfritc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtohqprtxa.html

[R30] 函数返回状态码
来源：http://hz.jqgfzy.top/gtnulpkfar.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtwuodzrwc.html

[R31] 局部变量
来源：http://hz.vqdsnc.cn/gtymsixaxu.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gtksfpyybn.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtfqjmdvlq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gtpxohplys.html

[R33] 捕获错误并提示行号
来源：http://hz.316326.xyz/gtvwqxhrjv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtcrpmhyis.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtzhumjake.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtgqttavdj.html

[R35] 后台执行并等待
来源：http://hz.zhiwuduotai.top/gtelzhexzz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtxhqcyjaz.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtpxpjpglu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cqqwz.cn/gtmsgaauyc.html

[R37] 把输出赋给变量
来源：http://hz.guowangkeji.top/gtdohtdjjc.html


<!-- 参考信息 -->