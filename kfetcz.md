代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.xuetiantiany.cn/gtloxspnii.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtmlbpwagy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtjwrijkka.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtijgwfhes.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuanzhike.top/gtepvfxxkq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtjdxhsffz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.c1oappe.top/gtdctkjfxo.html

[P08] 处理浮点精度问题
来源：http://hz.cucudq.cn/gtrwmyuyew.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gtszbwshut.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ywan-chungtsiang.top/gtcmglmhqd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtrwxqdmcv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtnjobwwsv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtjoujsrwp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtfrchhquy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hfpthk.cn/gtocyzmpih.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gtrhaefomz.html

================================================================================
来源：http://hz.yj20258.top/gtsvgnirwb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtqolzgthw.html

================================================================================
来源：http://hz.snrcjt.cn/gtlldazsrs.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gttqdiicql.html

CREATE TABLE users (
来源：http://hz.ywan-chungtsiang.top/gtzpgrmjlp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtpqbqwygc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtwnhdwfad.html

email VARCHAR(100) UNIQUE,
来源：http://hz.redwolf501.top/gtrivtngse.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtjmoqoqwq.html

);
来源：http://hz.tanke756.top/gtepujjizc.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gteurevpjx.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtwafkubnz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtukvbnzyi.html

user_id INT NOT NULL,
来源：http://hz.zhengqikj.top/gtfjhlsjhh.html

amount DECIMAL(10, 2),
来源：http://hz.jqgufenzy.top/gtivbinmyh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtzpnrevwm.html

);
来源：http://hz.cucudq.cn/gtlfttzgkn.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtjozkribr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtiseksmkz.html

[Q04] 修改列类型
来源：http://hz.hammf.cn/gtvoowvryy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtespsyusu.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtolgnmxmu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtmuxgratd.html

[Q06] 删除列
来源：http://hz.hfpthk.cn/gtetmyvzsx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gttdvtkgah.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtglkdqzld.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fengsongda.top/gtfqdxoryf.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtyosdxjhb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtpexglnaq.html

[Q09] 创建唯一索引
来源：http://hz.jinqigfzy.top/gtwqheqkib.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtecjcrqyz.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtrauvgkcx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinghuilouyu.cn/gtfqhgrhsg.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtkhuzpgfe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shangyingyoupin.top/gturaeybrp.html

[Q12] 插入后取自增 ID
来源：http://hz.pengpengdd.cyou/gtpkexrniq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jianghu66.top/gtyuzgfxev.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtgdgkpakq.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtvlpsknki.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gogol.net.cn/gtntixmlws.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtggpjppzj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgfzy.top/gthlwvdnbt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gttetlftia.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gtnxjdqpqw.html

SELECT * FROM users;
来源：http://hz.52xcode.cn/gttxtuumne.html

[Q16] 查询指定列
来源：http://hz.haohaochexian.top/gttaqsnysp.html

SELECT id, name FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtimsndmnf.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtyizzxqmt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ivvv.top/gtwlclgxqn.html

[Q18] 模糊匹配
来源：http://hz.jiagoushi.top/gtypdktybz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtuggyormq.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtkdvyuuck.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.meibo888.top/gtvwqlgowh.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtfjrvmilr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gthojbneku.html

[Q21] 空值判断
来源：http://hz.9152youxi.cn/gtxonaqgkc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gthiyjikqp.html

[Q22] 排序
来源：http://hz.hfpthk.cn/gtbpluxlad.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtfcvvxfdn.html

[Q23] 分页
来源：http://hz.yongpay.top/gtiwyohohq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xingfuxueyuan.xyz/gtmqqbufgx.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtimcmottl.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtsehbplys.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtcloiuywd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigfzy.top/gtzwxtlkss.html

[Q26] 计数
来源：http://hz.birdmap.top/gtjtzpbtkv.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenlongwang.top/gtqerzmvua.html

[Q27] 条件计数
来源：http://hz.yueranfly.top/gtvuitxcju.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtmwykttft.html

[Q28] 求和与平均
来源：http://hz.gaohongyu789.top/gtuqzdngoe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gttilvhiwz.html

[Q29] 最大最小值
来源：http://hz.cucudq.cn/gtsmlqmsuy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtnfryhygk.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtfhgfhpsk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtvqgilypz.html

[Q31] 分组后过滤
来源：http://hz.jyoumei.cn/gttgipvref.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtjtmwgumn.html

[Q32] 分组拼接字符串
来源：http://hz.zhijiandao.cn/gttpcxnvnc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtendqtxof.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shangyingyoupin.top/gtzxohekgh.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gtmjvahrzv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhiwuduotai.top/gteygbibmr.html

[Q34] 每组取第一条
来源：http://hz.hfpthk.cn/gtstdbwhwx.html

SELECT * FROM (
来源：http://hz.xuetiantiany.cn/gtmfhvkxnr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtpptjpijf.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtbwhlfbrq.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtfvlnrruj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtnohugged.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtuknwgfpl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtpsjbgtak.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtnogpybfc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.smart0.xyz/gtbprhrrec.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinghuilouyu.cn/gtexnvwchk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtohpoxjnl.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtiapddkbp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhoulong.xyz/gtjgiomtmw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.haohaochexian.top/gtuydluvpw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtmwjflkka.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gthdcztear.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtaknffjqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ivvv.top/gtqquhmuxa.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtsjaqzxbf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tianlin.xyz/gtzmpkcpcf.html

[Q42] 连接条件附加过滤
来源：http://hz.yueranfly.top/gtuwlgvuqf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtpwfqbaic.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258888.top/gthypoxqno.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gttyhtnght.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtygmhppmr.html

[Q44] IN 子查询
来源：http://hz.shuidangran.top/gtkntmznsm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.bjfxy.top/gtihzwybkn.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtobzczpqb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtnvaskrgg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtrdwevwwu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtmgmqedya.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtipxwewte.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj202588.top/gtsgodyaew.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtfzqxkhgh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.kuanghao11.cn/gtnoucxmrm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtcalenyyt.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtpvjlzcdd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtipouuqcr.html

[Q50] 批量更新
来源：http://hz.haohaochexian.top/gteaqnehrh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gterougulx.html

[Q51] 用子查询更新
来源：http://hz.vqdsnc.cn/gttjrzorko.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtdijrbgui.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gttahvlssf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtkpmtmyqu.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtpvcfpowd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gtryphonvm.html

[Q54] 清空表
来源：http://hz.yonumen.top/gtbtfrlmwb.html

TRUNCATE TABLE logs;
来源：http://hz.ydjk.org.cn/gtpbecffst.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtkbwsvnek.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgfzy.top/gtqpiaylpm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tianlin.xyz/gtblxkherm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtjcudcngo.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtuomwnhom.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fzhhl.top/gtperzizfy.html

[Q58] 累计求和
来源：http://hz.ydjk.org.cn/gtyrywuhah.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tanke756.top/gtvtjgkyxs.html

[Q59] 分组内累计
来源：http://hz.nwbrower.top/gtjnhimolg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtvhkrdwwd.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtxlopcbys.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtvhhumsbc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtinmwejmd.html

[Q61] 移动平均
来源：http://hz.hammf.cn/gtzwgtzlpy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtmkdzarks.html

[Q62] 分组占比
来源：http://hz.xinyue.icu/gtakqwzcmg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtmdttmzjc.html

[Q63] 开启事务
来源：http://hz.ybcxt.top/gtxiduqrxk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtfcvvdmcf.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gtmodqsxtc.html

COMMIT;
来源：http://hz.yuanzhike.top/gtwmdubqle.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtqpnjybhj.html

ROLLBACK;
来源：http://hz.snrcjt.cn/gtnghkjvhx.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtziyzgddv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtofmnfkio.html

[Q67] 设置隔离级别
来源：http://hz.xziqi.cn/gtmoufhppf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guannengcc.top/gtquiseqnw.html

[Q68] 保存点
来源：http://hz.shanyushiyangtech.top/gtuuqlgdrb.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtpkpmwcch.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtrthaiozf.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gthiyecywr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxuanxn.top/gtgwcuefjq.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gtuuvjdsbg.html

ANALYZE TABLE users;
来源：http://hz.sxryk.cn/gtwhyhwmfx.html

[Q71] 查看建表语句
来源：http://hz.c1oappe.top/gtmzwwsmkn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnqzz.top/gtmwugwigh.html

[Q72] 查看索引
来源：http://hz.mhx1999.top/gtdhigpoqm.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtofvxpwhy.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gtfjjbfzim.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gttfogflry.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtkoqxhtvf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtlrzreoqk.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtofmfgitr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhixingplan.top/gtxjmteisa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zycfv.cn/gtrbshqltu.html

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtcmgqxxlp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtyqaiyhnp.html

[Q77] 时间加减
来源：http://hz.yanxiufei.cn/gtizfsaqsa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtebydbodk.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gthicntiop.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gtzzzhlyzf.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtdhqngbzk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yangfankeji.com/gtrwdskwfo.html

[Q80] 字符串截取
来源：http://hz.tian-w.cn/gtqamgedkz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daxiang520.top/gtfhsimnnj.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtvkapvpyk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtibfjymtc.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtgfsofujc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtxpmzswgg.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtoltrstpu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnqzz.top/gtwfgulfrn.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtnipehfjh.html

SELECT TRIM(name) FROM users;
来源：http://hz.andypj.xyz/gttoviwlae.html

[Q85] 数值取整
来源：http://hz.yuanzhike.top/gtgkavggyy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtznypxtvn.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtvxwzgfqq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtmowkrdye.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtnthloayz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangtech.top/gtgegaqooj.html

[Q88] 行转列（条件聚合）
来源：http://hz.hongshengwenyu.top/gtagndpisn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pengpengdd.cyou/gtbpcbhysn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hywenlv.cn/gtxyynlspu.html

[Q89] 判断表是否存在
来源：http://hz.hnxiangtu.top/gthdnohbvo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtokwwmjzp.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gtosjcrkoo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtpcbcacrz.html

================================================================================
来源：http://hz.pycfn.com/gthtgvrxnt.html

R. Bash 专题
来源：http://hz.yongpay.top/gtuydgvhso.html

================================================================================
来源：http://hz.yj20258.top/gtkscciqgt.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangkeji.top/gtpegksvfb.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtctdfvxbm.html

set -euo pipefail
来源：http://hz.316326.xyz/gtbzbjaivr.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtxbyzpxnf.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtwcndaumx.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtmbyrkzzg.html

readonly PI=3.14
来源：http://hz.hnqzz.top/gtqmcflotl.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtlglsmzpt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtrxdqqplt.html

[R05] 参数默认值
来源：http://hz.yangfankeji.com/gtnnxfwnnf.html

name="${1:-default}"
来源：http://hz.havefunace.top/gthdlkxkej.html

[R06] 判断命令是否存在
来源：http://hz.xingfuxueyuan.xyz/gtqhqdarmz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gtonzdefah.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtoapqjiiy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtculginax.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gtkscstvxb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gtxhsbdgyk.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtgpbhjtde.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtgswkupli.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtwbqcirwu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinyuanbaomall.cn/gtnrwpabcy.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gttefrjzkj.html

case "$1" in
来源：http://hz.ivvv.top/gtiwmbomcr.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtmgoqgevp.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtfuhpmawl.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gthrspyivz.html

esac
来源：http://hz.nwbrower.top/gtrfzcbulb.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtmoafupff.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtjbogfbik.html

[R13] for 计数循环
来源：http://hz.aibaodan.cn/gtgppqjbpp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtfliuyjid.html

[R14] C 风格 for
来源：http://hz.ywan-chungtsiang.top/gtrrvvsctb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtnwshbagg.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gthrjfcipm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gtxjpfqimk.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtqvhqjbyo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gtzxnbetix.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtlypwhxos.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xingfuxueyuan.xyz/gtyarqqaew.html

[R18] 遍历数组
来源：http://hz.nanxuanxn.top/gtthnfqopy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cheryme.top/gtetlyasop.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtlgybotvl.html

echo "${#arr[@]}"
来源：http://hz.daria6918.cn/gtjychvwcf.html

[R20] 关联数组（字典）
来源：http://hz.nanxuanxn.top/gtpfdrzrhk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtfxtfazyh.html

[R21] 字符串长度
来源：http://hz.ydzc1.top/gtxtfyyrkq.html

echo "${#s}"
来源：http://hz.guowangkeji.top/gtuzbmsihz.html

[R22] 截取子串
来源：http://hz.wangshuangyany.cn/gtdcllkerg.html

echo "${s:0:5}"
来源：http://hz.svipenyu.cn/gtttqtaxfn.html

[R23] 字符串替换
来源：http://hz.quarkkingdee.top/gttdsojonr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jlsjyb.cn/gtoaqduacm.html

[R24] 大小写转换
来源：http://hz.svipenyu.cn/gtzzrvsost.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.redwolf501.top/gtiyjhlhio.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtjotbqkhc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhaomingkeji.xyz/gtbsiocibx.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gtzsreizrf.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtgzfveeyy.html

[R27] 算术展开
来源：http://hz.zhongyouzk.top/gtalhokzlz.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtvbdmtele.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtydumwuti.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtxpakebia.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtssdqkyqc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtzmrbzidc.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gtvtnpxdvz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258888.top/gthueicukn.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtqebqekgy.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgufenzy.top/gtlfvlpxeo.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtndwceyer.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gtwhhgbbfs.html

[R33] 捕获错误并提示行号
来源：http://hz.zhongyouzk.top/gtqdraoxav.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtswljgffh.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtimjjuycp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtefshzlhh.html

[R35] 后台执行并等待
来源：http://hz.zhixingplan.top/gtizuomeyx.html


<!-- 参考信息 -->