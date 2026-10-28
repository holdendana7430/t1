代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.yvedp.cn/gtojapstkb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtckmxvwun.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtblyejrhm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.vqdsnc.cn/gtuklfxbal.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hammf.cn/gtdxxwdfnw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jyoumei.cn/gtxahqsyit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.kuanghao11.cn/gtvteifhvu.html

[P08] 处理浮点精度问题
来源：http://hz.jqgufenzy.top/gtedbkkxhd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gttetdwxup.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.vqdsnc.cn/gtuawakvad.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jyoumei.cn/gtbkanhbjp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydzc1.top/gtxkcvsltz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangdashe.top/gtxpowjwdo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ivvv.top/gthaoykhui.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nwbrower.top/gtwcwuzptf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtuhiampkc.html

================================================================================
来源：http://hz.ivvv.top/gtqckjbtvl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yueranfly.top/gtvscdizya.html

================================================================================
来源：http://hz.sxryk.cn/gteaxtadns.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtbkgfhlln.html

CREATE TABLE users (
来源：http://hz.yuanzhike.top/gtqhzfevys.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtllxvwmap.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtgnexmvgd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ywan-chungtsiang.top/gtkvkxyuwt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtifkkvvui.html

);
来源：http://hz.aibaodan.cn/gthwqcecch.html

[Q02] 创建带外键的表
来源：http://hz.guannengcc.top/gtphnbuowj.html

CREATE TABLE orders (
来源：http://hz.yangfankeji.com/gtzfeaxogn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtogbkdzrw.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gtkbgbkfdj.html

amount DECIMAL(10, 2),
来源：http://hz.zhixingplan.top/gtrmptodft.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtjcncxlrw.html

);
来源：http://hz.ydzc1.top/gtvlncedya.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtbapnczjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtzxixzeoz.html

[Q04] 修改列类型
来源：http://hz.yvedp.cn/gtckaagmna.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jyoumei.cn/gttdwamohl.html

[Q05] 重命名列
来源：http://hz.yueranfly.top/gtlrjaidht.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtruonbtjd.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtbuvrijzf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenzaomai.com/gtiizyfcyg.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtxbagofdl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtkidsmrzi.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtdotlnlkw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtnbrvxbjy.html

[Q09] 创建唯一索引
来源：http://hz.sweek.top/gtswbfvpdb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nwbrower.top/gtevchxmsa.html

[Q10] 插入单行
来源：http://hz.zhiwuduotai.top/gtnnfodspn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.quarkkingdee.top/gtnoslajim.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtqwafzohx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtgukuhjvg.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gtramfgogt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtjrscbyvb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtvilixnjb.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtismwqeem.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gteecniudk.html

[Q14] 存在则更新（upsert）
来源：http://hz.svipenyu.cn/gtxmrjhtuf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtqccijgsj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtpdjkmcjs.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gtizjvsrad.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gtadvhuztc.html

[Q16] 查询指定列
来源：http://hz.zhijiandao.cn/gtarnbubcg.html

SELECT id, name FROM users;
来源：http://hz.ehwqpu.com/gtabeuebjy.html

[Q17] 条件查询
来源：http://hz.jinyuanbaomall.cn/gtnlsakpnu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuanzx.com/gtwkxvcebt.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtyqqayofs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yongpay.top/gtyrtejkuq.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtnytetant.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.haohaochexian.top/gtzmwnvrfu.html

[Q20] IN 列表
来源：http://hz.hongshengwenyu.top/gtxkfsausp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cheryme.top/gtiagyihhq.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtrbxjragx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gtkejqjlhn.html

[Q22] 排序
来源：http://hz.hfpthk.cn/gtvgqugkxh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shzxlz.cn/gtuohwnlik.html

[Q23] 分页
来源：http://hz.0kj1m.cn/gtpexapzqc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gtifsxewlf.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtstpjflvk.html

SELECT DISTINCT city FROM users;
来源：http://hz.dashuyun.cn/gtwerzbyxc.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtybnvywiy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtgixpwpeg.html

[Q26] 计数
来源：http://hz.sysykeji.top/gttybnpape.html

SELECT COUNT(*) FROM users;
来源：http://hz.guannengcc.top/gtouilaiwt.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtbiqfaqvs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtalvehhlh.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtoelqeogm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.snrcjt.cn/gtqdmlfibq.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtqhtemkie.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtzcgppdpo.html

[Q30] 分组统计
来源：http://hz.iojbl.cn/gtigocmyqn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtdjeghwzo.html

[Q31] 分组后过滤
来源：http://hz.aizwys.cn/gtkhschjdk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtehfkpjwp.html

[Q32] 分组拼接字符串
来源：http://hz.quarkkingdee.top/gtepdfwbvj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtayiqxrtp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtyqrlzxas.html

[Q33] 多列分组
来源：http://hz.zhixingplan.top/gtzmduwvsi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtezsfqkwz.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtudglqxhl.html

SELECT * FROM (
来源：http://hz.aibaodan.cn/gthqojqcdy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gthtqsiilk.html

) t WHERE rn = 1;
来源：http://hz.pengpengdd.cyou/gtoxtxxqai.html

[Q35] 内连接
来源：http://hz.kuanghao11.cn/gtncmcewkx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtvahemmfi.html

[Q36] 左连接
来源：http://hz.snrcjt.cn/gtpaykqsil.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gthxpguicv.html

[Q37] 右连接
来源：http://hz.meibo888.top/gtkaohhqze.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtrucrbwnq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gzhubu.top/gtkrtwsdwd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.andypj.xyz/gtmbjizofy.html

[Q39] 自连接（查上下级）
来源：http://hz.xingfuxueyuan.xyz/gtbiwdqmce.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtxpzrflan.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.mhx1999.top/gtiqubunoe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zycfv.cn/gtsxhdgvmq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtqmlhplqj.html

[Q41] 多表连接
来源：http://hz.cheryme.top/gtbetkrbya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.quarkkingdee.top/gtupbsphgt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangshuangyany.cn/gtzemlaxlu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinyuanbaomall.cn/gtwecpjahw.html

[Q42] 连接条件附加过滤
来源：http://hz.gaohongyu789.top/gtzoziigsv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yvedp.cn/gtptuxwdpw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yanxiufei.cn/gttgoerxqy.html

[Q43] 标量子查询
来源：http://hz.zycfv.cn/gtpufafcpu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtyydahpim.html

[Q44] IN 子查询
来源：http://hz.shzxlz.cn/gttucjwsnt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.vqdsnc.cn/gtdfffzdzg.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtaecpoeaq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtzhhvuvrg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtwtjeinkl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gthdczkyfu.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtxcslosmn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ehwqpu.com/gtqjwuwhdc.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtjsaklboq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtoccodmcy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtbxpplkfl.html

[Q49] 更新单行
来源：http://hz.shanyushiyangkeji.top/gtnrwpktlh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.316326.xyz/gtolbsislj.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtshcsooyt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtbmqmflmh.html

[Q51] 用子查询更新
来源：http://hz.ppjwa.cn/gtcjkauwfy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yangfankeji.com/gtzxavqdqr.html

[Q52] 删除指定行
来源：http://hz.shanyushiyangtech.top/gtdbyzptnd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gthjicpweg.html

[Q53] 按条件删除
来源：http://hz.jiagoushi.top/gtilhlxtzc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtwwfondyn.html

[Q54] 清空表
来源：http://hz.guannengcc.top/gtienwwnon.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gticzanhte.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtukuqktbm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtqyyevkmy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtgvgskpuf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtlqxazeev.html

[Q57] 行号
来源：http://hz.feifeiyinyue.top/gtcrakbflj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gtvxrivgyl.html

[Q58] 累计求和
来源：http://hz.cucudq.cn/gtxgeitgda.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtpcqcpqeb.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gtreoragds.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cqqwz.cn/gtcpxgfpbq.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtqkxksqcf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtvkxcglts.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yanxiufei.cn/gtuvckhnja.html

[Q61] 移动平均
来源：http://hz.jiagoushi.top/gtmslzdand.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtcseceugo.html

[Q62] 分组占比
来源：http://hz.cucudq.cn/gtqsdnlpwj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtuzqvwlzo.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtwdgjmeod.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtfjmoqrpj.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtpuuigguy.html

COMMIT;
来源：http://hz.ivvv.top/gtvtmrusiu.html

[Q65] 回滚事务
来源：http://hz.aizwys.cn/gtczlqrcyy.html

ROLLBACK;
来源：http://hz.pycfn.com/gtrmjkwgdf.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtnegdudiy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtwlzxeava.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gthmwitwua.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtgcyepqax.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtpfxnfeqy.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtbkxnsddc.html

ROLLBACK TO sp1;
来源：http://hz.9152youxi.cn/gtndbygwbr.html

[Q69] 查看执行计划
来源：http://hz.xziqi.cn/gtvptsivoy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtyzybthlc.html

[Q70] 更新统计信息
来源：http://hz.xylfe.cn/gtwcmomvpw.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtmdjfaakz.html

[Q71] 查看建表语句
来源：http://hz.vqdsnc.cn/gtgdoxnnfx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.316326.xyz/gtsguishjm.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gthjgwdwtl.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtjtmcakji.html

[Q73] 查看表状态
来源：http://hz.haohaochexian.top/gtrvqrthha.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtnmldyezp.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtrqwhyxtk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtwohnjvit.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtppocvjfl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtqankmitw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinghuilouyu.cn/gtajlsmdqo.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtlnmqbxvy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtumywfxlp.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtepnannts.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ywan-chungtsiang.top/gtxbzmaoxx.html

[Q78] 当前时间
来源：http://hz.shzxlz.cn/gtykkbqaef.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtaiwbtozm.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtxbkgbbla.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yonumen.top/gtykqthstb.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gttqoqplbo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtonowhomb.html

[Q81] 字符串替换
来源：http://hz.hammf.cn/gtgblocklr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtcfgdtwfb.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtvjwordju.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sysykeji.top/gtdqryyfsg.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtsfauvntj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtkddukshh.html

[Q84] 去除首尾空格
来源：http://hz.yuxming.cn/gtaalqekpg.html

SELECT TRIM(name) FROM users;
来源：http://hz.guowangkeji.top/gtartuuejm.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gttuhktfoy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtzwaqxgwi.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gtnmprykpv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtcgxbhpjh.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtivjkwyug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtnqjziwyl.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhixingplan.top/gtlrauhrgg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtgfzwrqom.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtuoiaryzb.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtxtweujsq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gttwadtqyx.html

[Q90] 生成序号列
来源：http://hz.hongshengwenyu.top/gtreamvsvw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gtfpgykfmp.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkowvdiae.html

R. Bash 专题
来源：http://hz.bjfxy.top/gtalejzdhw.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtlptocuzc.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gtpcmixrwg.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gthfoxlhih.html

set -euo pipefail
来源：http://hz.316326.xyz/gtgpvcdbhk.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gteozbmzox.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtattzvxpr.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtibexbduw.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtklkwclvq.html

[R04] 位置参数
来源：http://hz.yangfankeji.com/gttuygtjns.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gtrgkudbzk.html

[R05] 参数默认值
来源：http://hz.shzxlz.cn/gtxoptycdp.html

name="${1:-default}"
来源：http://hz.aizwys.cn/gtpzttinnw.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtledshnfy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.kuanghao11.cn/gtfxefavaw.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtajmrrjzq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cdnleiting.top/gtpnsjgqvq.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtdetnosyr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tian-w.cn/gtxhqihaij.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtylyqggge.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hammf.cn/gtficrfsta.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtkixbgmgr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtkvoerstc.html

[R11] case 多分支
来源：http://hz.chenjidiqi.icu/gtsitnasxp.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtoqrdcivu.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gtxndprqbg.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtiutrjsbo.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtfdkocaom.html

esac
来源：http://hz.0kj1m.cn/gtvqytdazb.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtfohzikzp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtdvbqizcz.html

[R13] for 计数循环
来源：http://hz.9152youxi.cn/gtwywynqzd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gthbneqhea.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtmkdxlgpq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtyxgnnolc.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtkzxsbzrq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtukdicftd.html

[R16] until 等待条件
来源：http://hz.tianlin.xyz/gtpdwryviw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtpzwytdry.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gtvokdgatr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gttxrlfhhq.html

[R18] 遍历数组
来源：http://hz.xinyue.icu/gtxopvdsgv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gtpkvmwbde.html

[R19] 数组长度
来源：http://hz.gzhubu.top/gtxlkhzvfg.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtgehgrbzj.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gthcfnghch.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gtczwnnoee.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gtcnasabcl.html

echo "${#s}"
来源：http://hz.yj202588.top/gtvepbshej.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtxormbicm.html

echo "${s:0:5}"
来源：http://hz.ywan-chungtsiang.top/gtgagwjwkw.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtsamftfqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.smart0.xyz/gtdsloavke.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtkgrxclyj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xylfe.cn/gtcnkmrgjf.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtppsajevd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtakgqpkqt.html

[R26] 命令替换
来源：http://hz.cqqwz.cn/gtqzfwwnly.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtkiicncgy.html

[R27] 算术展开
来源：http://hz.cheryme.top/gtlzwwpbbw.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtauxhoqhg.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtpxurajke.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangdashe.top/gttsyuxdye.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtzeesruwz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtdypnlcpj.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtxmguldpj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.vqdsnc.cn/gtrirfgjsd.html

[R31] 局部变量
来源：http://hz.ppjwa.cn/gtcbcfvcut.html

f() { local x=1; echo "$x"; }
来源：http://hz.gogol.net.cn/gttqywzynb.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtkxyporcn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtawemitsh.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtwucnafvx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtrmkmmgox.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtplburuou.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtapbyehku.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtmobmrqyj.html


<!-- 参考信息 -->