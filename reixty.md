代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ybcxt.top/gtsghyyrkr.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtsmqdpvzn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gtkcpdhkae.html

Go:   if x == nil {}
来源：http://hz.daxiang520.top/gtagjtmxrn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtphjqkfgy.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtwiaxolar.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtijuqqbxy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtmnenrlum.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gtpcxduyhm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtubakomlw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtcbcfnwul.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.birdmap.top/gtvussjmvb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gtmipszlfa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxuanxn.top/gtntkmwfgi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhiwuduotai.top/gtmcrwozwk.html

[P08] 处理浮点精度问题
来源：http://hz.xylfe.cn/gtmmamylqh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.iojbl.cn/gtrmutitip.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtcyyhivhh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.birdmap.top/gtcyksgryw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.havefunace.top/gtkywnkpze.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhiwuduotai.top/gtzmkcftjj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nwbrower.top/gtkardwovf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhijiandao.cn/gtprilnuoa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtilqztdov.html

================================================================================
来源：http://hz.zycfv.cn/gtbnojnpuf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhijiandao.cn/gtbwuioemb.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtdhagmsah.html

[Q01] 创建表
来源：http://hz.cdnleiting.top/gtdmydajhe.html

CREATE TABLE users (
来源：http://hz.quarkkingdee.top/gtnanhcamz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtauvbrhla.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guowangkeji.top/gtidvlclid.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtgkhqxbth.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.316326.xyz/gtcfreycqw.html

);
来源：http://hz.vqdsnc.cn/gttjonnbrx.html

[Q02] 创建带外键的表
来源：http://hz.52xcode.cn/gtokjhgghd.html

CREATE TABLE orders (
来源：http://hz.smart0.xyz/gtahmtxoky.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtcwscxxku.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtoflmphhm.html

amount DECIMAL(10, 2),
来源：http://hz.andypj.xyz/gtzprdybte.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuanzx.com/gtupredeht.html

);
来源：http://hz.shzxlz.cn/gtkgolhtpi.html

[Q03] 增加列
来源：http://hz.ywan-chungtsiang.top/gtgkomwybp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.0kj1m.cn/gtctxaotwu.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtxqritjqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sxryk.cn/gtoxllcwlt.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtikzxbnwe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtnndhyuee.html

[Q06] 删除列
来源：http://hz.gotoacloud.top/gtvaszhuji.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gtluaajttn.html

[Q07] 删除表
来源：http://hz.chenjidiqi.icu/gtmjofiewn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtqifhzxjy.html

[Q08] 创建普通索引
来源：http://hz.jinqigfzy.top/gtjwiymhkw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtxxrrgjrz.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtzlmhhcrq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jiagoushi.top/gtzinzlluu.html

[Q10] 插入单行
来源：http://hz.sysykeji.top/gtnsydxqph.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtatbsqqiw.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtlhmjbyhr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtmmaukoqh.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gteunaqntc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.svipenyu.cn/gtuphjhzij.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtqpaokweh.html

[Q13] 忽略重复插入
来源：http://hz.pengpengdd.cyou/gtsenlysfx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtrhzozhpk.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtobngjgfj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hysaishi.cn/gtxgnolqiu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.52xcode.cn/gtalxqobaa.html

[Q15] 查询全部
来源：http://hz.dashuyun.cn/gtmrthjdqx.html

SELECT * FROM users;
来源：http://hz.vqdsnc.cn/gtytljfyqi.html

[Q16] 查询指定列
来源：http://hz.yj202588.top/gtbhlkiimp.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtadziinji.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtaxjeosft.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.havefunace.top/gtsjtldzqb.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtfxsppour.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnxiangtu.top/gtymkagsky.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gtwryqshyk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gogol.net.cn/gtuvlicliq.html

[Q20] IN 列表
来源：http://hz.yj202588.top/gtfzgjvuca.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cqqwz.cn/gtuywbgrli.html

[Q21] 空值判断
来源：http://hz.gogol.net.cn/gtaclnqbno.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtscmvxbmn.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtopofjagi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtekarrubv.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtnzwhntmy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtcwkofjqt.html

[Q24] 去重
来源：http://hz.fengsongda.top/gteumekkkd.html

SELECT DISTINCT city FROM users;
来源：http://hz.tanke756.top/gtnwtuwzbg.html

[Q25] 只取前 N 条
来源：http://hz.tanke756.top/gtboflkikv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cucudq.cn/gtdqwdtkiq.html

[Q26] 计数
来源：http://hz.yanxiufei.cn/gtxishbjwm.html

SELECT COUNT(*) FROM users;
来源：http://hz.yangfankeji.com/gthjcabgqm.html

[Q27] 条件计数
来源：http://hz.316326.xyz/gtwetlenjx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtvpfozsyh.html

[Q28] 求和与平均
来源：http://hz.ywan-chungtsiang.top/gtpryudvwh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.kuanghao11.cn/gtkdmqlpen.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtyitlaoet.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gtgrbsnnky.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtyxjspllr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtbzsyqqhz.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gtggesuqzx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nwbrower.top/gtwmzkrfwi.html

[Q32] 分组拼接字符串
来源：http://hz.havefunace.top/gtrvjonhjw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtaibwbbdf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ehwqpu.com/gthecgjtoy.html

[Q33] 多列分组
来源：http://hz.redwolf501.top/gtklspubfm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtydvgubya.html

[Q34] 每组取第一条
来源：http://hz.cheryme.top/gtrranpcrm.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtqdssrjvk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtbxqdoojj.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtkbtjsttu.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gtxgwgvitu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtwirdsyfd.html

[Q36] 左连接
来源：http://hz.cucudq.cn/gtbtvisywb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtsoyngllm.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtkhiokrgp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shzxlz.cn/gtycldhyhn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gthiwbubzi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtjmkkneas.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigufen.top/gtievvayor.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yangfankeji.com/gtwwrlrsfh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtaurlldaf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jyoumei.cn/gtsoeargku.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gttpcgciqg.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtayjtihkq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jiagoushi.top/gtcbfjqcks.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shzxlz.cn/gtdwummmtn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gthmtokrwf.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtjffaldti.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenjidiqi.icu/gtjwrjooix.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ybcxt.top/gtbmvccnab.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtmamsqzmz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.iojbl.cn/gtragxvuxe.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gtemoychri.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.haohaochexian.top/gtsehdzhow.html

[Q45] EXISTS 判断存在
来源：http://hz.sxryk.cn/gtudwggqeo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtatisfgka.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gtgoykyqlu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtyldhfzkf.html

[Q47] 与平均值比较
来源：http://hz.shangyingyoupin.top/gtjfbiwsgb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.svipenyu.cn/gtpwutiftg.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxinkj.top/gtxxljcljx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtoomzflke.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gticxqozlx.html

[Q49] 更新单行
来源：http://hz.xingfuxueyuan.xyz/gtisjqsati.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xinyue.icu/gthvwvfhwc.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtpumpknen.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtqmyyyied.html

[Q51] 用子查询更新
来源：http://hz.ybcxt.top/gtotbhuzio.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gotoacloud.top/gteonsgsrv.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtsfoblhen.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtxmtyxjbn.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtigbjmsfv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtgbmmyrlg.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtgygudgmk.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtcjpobzkx.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtagcswlmm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenzaomai.com/gtugjxohvz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtwlsnwwab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhongyouzk.top/gtjgfnpsvy.html

[Q57] 行号
来源：http://hz.hnqzz.top/gtyctwmptv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtyzqysqhd.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gtdognzsut.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtffpyfpoy.html

[Q59] 分组内累计
来源：http://hz.cqqwz.cn/gtmoccjhvd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtvvrybqbs.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtikfdkzoi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtheweopkc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxuanxn.top/gtcvuikmiq.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtidjgaido.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnxiangtu.top/gtywtlgerw.html

[Q62] 分组占比
来源：http://hz.zhiwuduotai.top/gtcgajmemb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtxozflqoe.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gtwlgfulxf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtxbhhhobb.html

[Q64] 提交事务
来源：http://hz.xinyue.icu/gtqaaxiaex.html

COMMIT;
来源：http://hz.ydjk.org.cn/gthxlxlbbt.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtkjzuqteq.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtkcpazitj.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gttuxhwpyn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtjsqzvxow.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangtech.top/gtktsbzphn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtqojdrjav.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtnkiwpkry.html

SAVEPOINT sp1;
来源：http://hz.jinghuilouyu.cn/gtvonqnfdj.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtnvvdkwbr.html

[Q69] 查看执行计划
来源：http://hz.yuxming.cn/gtsshwsdrc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gtzetuytff.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtuarcvsse.html

ANALYZE TABLE users;
来源：http://hz.ehwqpu.com/gtqhdbddsj.html

[Q71] 查看建表语句
来源：http://hz.jinqigfzy.top/gtdflvhbhc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.birdmap.top/gtzibwmnxh.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtqckteqyh.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtaylxrkvd.html

[Q73] 查看表状态
来源：http://hz.nanxinkj.top/gtksllizvf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gtjhiwvtqk.html

[Q74] 强制使用索引
来源：http://hz.guannengcc.top/gtrhpscjdq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtzuedeciy.html

[Q75] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtftbsszjw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtnapqzczw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtwpzjlxic.html

[Q76] 按天统计
来源：http://hz.sxryk.cn/gtezhiysty.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenlongwang.top/gtakkyxeun.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtwunpqbbu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtrrjbqphs.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gtvbkkvnyk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtfzkqhlhy.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtdgvyrsxn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtkhevfmav.html

[Q80] 字符串截取
来源：http://hz.zhengqikj.top/gtnxzjjraa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.9152youxi.cn/gtkgemvaix.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gthuwjxugx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhaomingkeji.xyz/gtdkesxcae.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtogjhvyny.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtqffbvfrb.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtalgsaueq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.quarkkingdee.top/gthvwbswtw.html

[Q84] 去除首尾空格
来源：http://hz.yj20258.top/gttpdpnrxh.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gtbscqgczu.html

[Q85] 数值取整
来源：http://hz.yonumen.top/gtylivxmfc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gzhubu.top/gtfvzodulz.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtisezgxhv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.mhx1999.top/gtxklwwkyc.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtvygaukqy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtbycezzmq.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtmcfdafru.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ywan-chungtsiang.top/gtmfbkkpyj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gtkkfepxgs.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtaktohyex.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtroigqvga.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtecsdpmzq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtpgzgubyf.html

================================================================================
来源：http://hz.hfpthk.cn/gtbmjhjxzi.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtfbxzmujb.html

================================================================================
来源：http://hz.tianlin.xyz/gtwjqgnrgz.html

[R01] shebang 与严格模式
来源：http://hz.zdqjudy.top/gtubuofpbq.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtdbyjnuhl.html

set -euo pipefail
来源：http://hz.jinqigufen.top/gthjkuwuqw.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gtiwaafykp.html

name="Tom"; echo "$name"
来源：http://hz.guannengcc.top/gtfvahyzpd.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtbraxjchw.html

readonly PI=3.14
来源：http://hz.316326.xyz/gtwadpqapq.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gtnfywwuvt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hongshengwenyu.top/gtlkjzzbri.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtttitnzle.html

name="${1:-default}"
来源：http://hz.52xcode.cn/gtgzoczpfc.html

[R06] 判断命令是否存在
来源：http://hz.chenlongwang.top/gtprvogemy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtvqtddbyd.html

[R07] if 判断文件
来源：http://hz.daxiang520.top/gtavunpnfm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtirplpqwy.html

[R08] 数值比较
来源：http://hz.yangfankeji.com/gtmyxevzoj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtkhpyudft.html

[R09] 字符串比较
来源：http://hz.yvedp.cn/gtzwqzdpxh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtnngtzaug.html

[R10] 正则匹配
来源：http://hz.havefunace.top/gtzkxbarcu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aibaodan.cn/gtojgefwbc.html

[R11] case 多分支
来源：http://hz.ydzc1.top/gtfaslsgxh.html

case "$1" in
来源：http://hz.dianchejie.cn/gttyxqjaky.html

start) echo "启动" ;;
来源：http://hz.zhiwuduotai.top/gtccmnggwz.html

stop)  echo "停止" ;;
来源：http://hz.xuetiantiany.cn/gteyuifhgm.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtjebbxjuh.html

esac
来源：http://hz.cheryme.top/gtlbvqexhr.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtjwvfdfig.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtlxjpxxlj.html

[R13] for 计数循环
来源：http://hz.9152youxi.cn/gtaruknvqp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtvbtmjzao.html

[R14] C 风格 for
来源：http://hz.cqqwz.cn/gtewgndecs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtmhbnfamd.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtdbzimcom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ppjwa.cn/gtynbnmuef.html

[R16] until 等待条件
来源：http://hz.cqqwz.cn/gtplxpzuzg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hywenlv.cn/gtritbdnpv.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtwxeuhojo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtfvshisfw.html

[R18] 遍历数组
来源：http://hz.yuxming.cn/gtwdzytent.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gtcywefwlt.html

[R19] 数组长度
来源：http://hz.fengsongda.top/gtrjelbzmr.html

echo "${#arr[@]}"
来源：http://hz.wangdashe.top/gtvpeujmal.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtsndudqmv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtiuhmehlx.html

[R21] 字符串长度
来源：http://hz.svipenyu.cn/gtpkspjhhf.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtqldvdrla.html

[R22] 截取子串
来源：http://hz.gotoacloud.top/gtherzyrzu.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtubhnfvci.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtcyrxghvs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydzc1.top/gtpauzctdf.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtnitspfdi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtafpnxffq.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtympywnkb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtgwqlkhvb.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtmzkfbfro.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gtxbjcfvtz.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtqmavqrmk.html

echo $((1 + 2 * 3))
来源：http://hz.yuxming.cn/gtjoyfyfan.html

[R28] 浮点运算
来源：http://hz.gaohongyu789.top/gteztkiifu.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtdsrhzkep.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtfkkflisy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ivvv.top/gteshskpwe.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtoiwcgnun.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtbtbqdxub.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtziuuvzpc.html


<!-- 参考信息 -->