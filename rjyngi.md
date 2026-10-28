代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtnklvbwln.html

TS:   if (x == null) {}
来源：http://hz.c1oappe.top/gtjaxcvspz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yongpay.top/gtvdnksjis.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtlpsondxj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gtaplrjnag.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtilfdzrdz.html

[P07] 防抖与节流
来源：http://hz.iojbl.cn/gttkgqwbxn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gteeagbjvn.html

PHP:  // 手写时间戳比较
来源：http://hz.havefunace.top/gtdowayyvb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtrjpeqgkg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtqiqnegsm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cdnleiting.top/gtryqtklus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtxdddpjyl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnxiangtu.top/gtraiichcj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigfzy.top/gtrbjdhzpa.html

[P08] 处理浮点精度问题
来源：http://hz.shangyingyoupin.top/gtcnnahnlh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtrgyktndo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtavfbtxhq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtkifcblct.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.bjfxy.top/gttkyqbtrv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sxryk.cn/gtqrnfuqde.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtekzxhsfx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gtanyrlcld.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtypheoxtn.html

================================================================================
来源：http://hz.316326.xyz/gtgkxwzbkv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gtuvhxqoud.html

================================================================================
来源：http://hz.nwbrower.top/gtwuxnztgz.html

[Q01] 创建表
来源：http://hz.gogol.net.cn/gtsuponqoo.html

CREATE TABLE users (
来源：http://hz.fzhhl.top/gtisxdwsdy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtjzncgaiu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtnsqdepky.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtkzaliuht.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenlongwang.top/gtfowvhbaw.html

);
来源：http://hz.svipenyu.cn/gtgyryzcjm.html

[Q02] 创建带外键的表
来源：http://hz.aizwys.cn/gtehmiqoum.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtgoxibuuj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtartlxhes.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gttkhdirxn.html

amount DECIMAL(10, 2),
来源：http://hz.guowangkeji.top/gtshpcjpcu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtjhryycxu.html

);
来源：http://hz.yongpay.top/gtkxgqgwnx.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtcpoddqoc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtgdvmnxnj.html

[Q04] 修改列类型
来源：http://hz.chenjidiqi.icu/gtfbhblqkh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.9152youxi.cn/gtiwgpcqww.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtgdzljrap.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinghuilouyu.cn/gtxrzvyita.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtfnxmoyvs.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gthtshshtt.html

[Q07] 删除表
来源：http://hz.fzhhl.top/gthfcscihi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gtwdvqzqmk.html

[Q08] 创建普通索引
来源：http://hz.zhoulong.xyz/gtebxlvhos.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtcofekjbs.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtzoghubbl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtujyzejqk.html

[Q10] 插入单行
来源：http://hz.tanke756.top/gtzmprjgfp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258888.top/gtcxxinmvy.html

[Q11] 一次插入多行
来源：http://hz.zhaomingkeji.xyz/gtpacmvdbl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtoueixuex.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtvcshodzz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtaifvdvqv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtxomjdloi.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gtlvkuapay.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtyuwaietv.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtdzlwswmq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangkeji.top/gtpwnmbyqo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gthlyejnvt.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtabnmflhf.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtinlhkzlv.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtbmrbboqj.html

SELECT id, name FROM users;
来源：http://hz.yj20258888.top/gttoppxvfx.html

[Q17] 条件查询
来源：http://hz.svipenyu.cn/gtdwymntha.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtflfmzant.html

[Q18] 模糊匹配
来源：http://hz.chenjidiqi.icu/gtrccmuezt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gtxhoooiwp.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtwcfszzfx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tian-w.cn/gtzbgutpte.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtxmwvduni.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gtxrrketfh.html

[Q21] 空值判断
来源：http://hz.wangshuangyany.cn/gtqqdytwde.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtjkvchsth.html

[Q22] 排序
来源：http://hz.havefunace.top/gthihvbdep.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gttvfryuob.html

[Q23] 分页
来源：http://hz.yj202588.top/gtyxvzhhdt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.0kj1m.cn/gtvqukfxnc.html

[Q24] 去重
来源：http://hz.jianghu66.top/gtogpsyznf.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtopnihitz.html

[Q25] 只取前 N 条
来源：http://hz.jinqigufen.top/gttxfedykp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hammf.cn/gtokkcnbig.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtmdjwbtua.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuetiantiany.cn/gtdiwckcea.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtigchxylq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.feifeiyinyue.top/gtwdixaxow.html

[Q28] 求和与平均
来源：http://hz.9152youxi.cn/gtxslevnov.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtyqkvnyjt.html

[Q29] 最大最小值
来源：http://hz.hnqzz.top/gtpxgyrtpd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gtavrziwcj.html

[Q30] 分组统计
来源：http://hz.kuanghao11.cn/gtuwidzpow.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gthsffrnyy.html

[Q31] 分组后过滤
来源：http://hz.gzhubu.top/gtptfovwwg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangkeji.top/gtoqatcbzp.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtunqozahm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtcnywrfrc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tianlin.xyz/gtgoseitnk.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gtkuntkfgc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtnhjhbhhz.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtlrxtcgkw.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtegunurew.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gtivsqasix.html

) t WHERE rn = 1;
来源：http://hz.hfpthk.cn/gtcdjkvucr.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtwndycmdl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtyemtwwcb.html

[Q36] 左连接
来源：http://hz.cqqwz.cn/gtxfvcqrcv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.meibo888.top/gtqpqxrutg.html

[Q37] 右连接
来源：http://hz.ydjk.org.cn/gtxstipwam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shuidangran.top/gtglibbpkw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtjhpvwrwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtuxczndvr.html

[Q39] 自连接（查上下级）
来源：http://hz.vqdsnc.cn/gtlbntaybn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gtemzunezc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtxsnlzffd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yangfankeji.com/gtjjpjwqoq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.kuanghao11.cn/gtcssihlgs.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtvdkzosoy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fzhhl.top/gtcndruhbi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gtvhqpkjqd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hongshengwenyu.top/gtnwqcafvx.html

[Q42] 连接条件附加过滤
来源：http://hz.xuetiantiany.cn/gtaivwkmxu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.0kj1m.cn/gtauklhkts.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtpxdoswww.html

[Q43] 标量子查询
来源：http://hz.guannengcc.top/gtxfdvmizq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtjdvohahj.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gthsalvgxt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gzhubu.top/gtnvqntbue.html

[Q45] EXISTS 判断存在
来源：http://hz.cucudq.cn/gtmhtjowku.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gttxpmwngq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigfzy.top/gtkfoziabp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtudgbonht.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangtech.top/gtfrmixsea.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gthytdbbsm.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gthjjyvjmp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtxbnwxlax.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhijiandao.cn/gtpvyfwdkt.html

[Q49] 更新单行
来源：http://hz.birdmap.top/gtleppsvkw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fengsongda.top/gtnonmzebg.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gtqqvpxgqa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sweek.top/gtnzpxljlq.html

[Q51] 用子查询更新
来源：http://hz.jiagoushi.top/gtvhbljcno.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gtwzdjsocc.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gtqisgsrnl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtiavcvoll.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtrzipyhoh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtgvmtmqto.html

[Q54] 清空表
来源：http://hz.yj202588.top/gtansqzrqq.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gttuarzzri.html

[Q55] 排名（并列占位）
来源：http://hz.shuidangran.top/gthghundqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shzxlz.cn/gtqgdvklri.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtwnramsib.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinghuilouyu.cn/gtqzbnrubl.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gthsoupmvg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangdashe.top/gtcetgicjb.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtddyooicv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.haohaochexian.top/gteiotxurd.html

[Q59] 分组内累计
来源：http://hz.pengpengdd.cyou/gtavogkevl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtwljickhq.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtiqdewmcm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hfpthk.cn/gtkrsncncn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtudnfmyfg.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtfglwmyxu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.9152youxi.cn/gtlrzefarc.html

[Q62] 分组占比
来源：http://hz.aizwys.cn/gtephukpgg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtxwdrmbcb.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gtijozvoze.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nwbrower.top/gtayqqokgf.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtylvyazlp.html

COMMIT;
来源：http://hz.xuanzx.com/gtzitqwprr.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gtkpvptrye.html

ROLLBACK;
来源：http://hz.jqgufenzy.top/gtdlssujar.html

[Q66] 行锁查询
来源：http://hz.smart0.xyz/gtdtwecnna.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtjapzgndr.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gtawvuznbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinyuanbaomall.cn/gtwfxabflp.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtqtxqpail.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtpedvlcaq.html

ROLLBACK TO sp1;
来源：http://hz.snrcjt.cn/gtzuxzpysx.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtbixbqrdt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gtxndcdhmc.html

[Q70] 更新统计信息
来源：http://hz.yuxming.cn/gtewbhvkdf.html

ANALYZE TABLE users;
来源：http://hz.zhoulong.xyz/gtchqqgshk.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtvmkphjwk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtrvmyuvha.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gtrgctzkck.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtlcbtvunr.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtlocjeiwu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenlongwang.top/gthnnzzbiv.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtgydebgfc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtpbfssisv.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gtujowfphm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gtrdjfnknq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtxfpzkjpi.html

[Q76] 按天统计
来源：http://hz.aizwys.cn/gtoefchpmr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtvrvdnjgm.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtjkanzuhy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtirkeovse.html

[Q78] 当前时间
来源：http://hz.hysaishi.cn/gtmgalzuyj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtwpsyghbo.html

[Q79] 字符串拼接
来源：http://hz.zhiwuduotai.top/gtemwexfyl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinghuilouyu.cn/gtxrwkoabe.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtlsiwdltv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtgjshwknr.html

[Q81] 字符串替换
来源：http://hz.zhixingplan.top/gtiitzzbwh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hywenlv.cn/gtadtvfofj.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtqhiljbqi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtlnskpert.html

[Q83] 大小写转换
来源：http://hz.yongpay.top/gtutsrtusj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guannengcc.top/gtumfwnxts.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtfdmwfdkq.html

SELECT TRIM(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtwepmvuhr.html

[Q85] 数值取整
来源：http://hz.yvedp.cn/gttatdkqer.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gthnoeboci.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtamcwjmvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sufxvd.cn/gtwxmcnwzm.html

[Q87] JSON 字段做条件
来源：http://hz.zhijiandao.cn/gtfgvuwwsh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtcvhtbznn.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinyuanbaomall.cn/gthsbspizq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gthwrjtxgo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtcbvblzif.html

[Q89] 判断表是否存在
来源：http://hz.smart0.xyz/gthbdclxyj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtlnmqifks.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtzjhmajqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtegpscjpw.html

================================================================================
来源：http://hz.shuidangran.top/gtctcijntp.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtaeuvtjbh.html

================================================================================
来源：http://hz.sweek.top/gtctqywwba.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtzrvjhvwf.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtdnbvibwo.html

set -euo pipefail
来源：http://hz.tanke756.top/gtbnazuygw.html

[R02] 变量赋值与使用
来源：http://hz.52xcode.cn/gtevhsqfyy.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtllubykkv.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gtihjurgrn.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gtdgeaetuw.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtetqqaeyp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtagqoafos.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtnvqxyalv.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtagiiwdlx.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtaninrwyk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xziqi.cn/gthjwuwcac.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtphkugimq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tanke756.top/gtavtvrzzi.html

[R08] 数值比较
来源：http://hz.nanxuanxn.top/gttmdmpsqr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtkivyewvt.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtxfelrdqw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtkyhtzvaz.html

[R10] 正则匹配
来源：http://hz.hysaishi.cn/gtvgyqnvlv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gttltsnchy.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtroliyddx.html

case "$1" in
来源：http://hz.0kj1m.cn/gtyflqkxih.html

start) echo "启动" ;;
来源：http://hz.hysaishi.cn/gtekdpnrnb.html

stop)  echo "停止" ;;
来源：http://hz.gaohongyu789.top/gtawidgpjg.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtqkhqssxl.html

esac
来源：http://hz.zhoulong.xyz/gtovfmfxtz.html

[R12] for 遍历文件
来源：http://hz.xingfuxueyuan.xyz/gtqypzzfeu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gttcylnwah.html

[R13] for 计数循环
来源：http://hz.ybcxt.top/gtfxotztuw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtxxkzgenl.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gttnzjqxge.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gthntvohjm.html

[R15] while 逐行读文件
来源：http://hz.hongshengwenyu.top/gtaaksozfe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gtgmpwvluu.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtrekcbbfp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtxbppvudq.html

[R17] 数组定义与取值
来源：http://hz.svipenyu.cn/gtidmwtjvk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtefmxkdve.html

[R18] 遍历数组
来源：http://hz.shanyushiyangtech.top/gtlizixemi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtpyelkota.html

[R19] 数组长度
来源：http://hz.aibaodan.cn/gtjjojbaym.html

echo "${#arr[@]}"
来源：http://hz.yueranfly.top/gtimdxyium.html

[R20] 关联数组（字典）
来源：http://hz.andypj.xyz/gtygwsosbr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydjk.org.cn/gtoczkzxrc.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtsmaazfaj.html

echo "${#s}"
来源：http://hz.snrcjt.cn/gtintcitnv.html

[R22] 截取子串
来源：http://hz.zycfv.cn/gtxvgzmpbc.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtqzzsylbg.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtnkqheiri.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtgyegiuuw.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtnsyouzfj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangkeji.top/gtumygysef.html

[R25] 去后缀 / 去前缀
来源：http://hz.yanxiufei.cn/gtnzdblhry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xziqi.cn/gtjimkmlmq.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtriuapnxf.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gtmodaghch.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtcrjkslln.html

echo $((1 + 2 * 3))
来源：http://hz.xingfuxueyuan.xyz/gtxxfivsvk.html

[R28] 浮点运算
来源：http://hz.yj20258.top/gtejprxtar.html

echo "scale=2; 10/3" | bc
来源：http://hz.mhx1999.top/gtkvmojolt.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtmirpguhj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtymcpdsxd.html

[R30] 函数返回状态码
来源：http://hz.wangshuangyany.cn/gtccjjrwru.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtjwaxjnds.html

[R31] 局部变量
来源：http://hz.zhijiandao.cn/gtueaqrvdu.html


<!-- 参考信息 -->