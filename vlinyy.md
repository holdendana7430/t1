代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtzeltqjju.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuanzx.com/gtzrxbatnt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtfsokffhc.html

Ruby: a == b
来源：http://hz.yuanzhike.top/gtgwdeuakb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258.top/gtbvesgtzr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuetiantiany.cn/gtotfusidp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gtqohlwipg.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gtwchdlvgp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aizwys.cn/gtumhoukgm.html

TS:   if (x == null) {}
来源：http://hz.aibaodan.cn/gtdkompvmv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtipnwzhli.html

Go:   if x == nil {}
来源：http://hz.zycfv.cn/gtdzaucdgl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtpqwnppkn.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtvdfodchb.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gtcrjhdvzz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gtsojoiqzj.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtpnblhecg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtertgeqki.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gttndhgqji.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.feifeiyinyue.top/gtdjfjrdrc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cdnleiting.top/gtakxxcbsq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.smart0.xyz/gtyiqsxunp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenzaomai.com/gtcewfoqrl.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtvkrwoxlp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.snrcjt.cn/gttdxlzcrb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gotoacloud.top/gtvjsjccuq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.0kj1m.cn/gtjutszfhb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.quarkkingdee.top/gtvkfhrabw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtvlknjahz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xinyue.icu/gtqmkdpljs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtcyxrcccs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtyuqmknpv.html

================================================================================
来源：http://hz.hfpthk.cn/gttvqpajal.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jianghu66.top/gtqralabxz.html

================================================================================
来源：http://hz.yuanzhike.top/gtosibttmu.html

[Q01] 创建表
来源：http://hz.ydjk.org.cn/gtzdyjmmwr.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtykntbjjw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gtkmvcuqrh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtkrdvnttz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sysykeji.top/gtgawwkbzf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gteshrvgft.html

);
来源：http://hz.yueranfly.top/gtmxjipasa.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtngzxeubn.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtbngaimyl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtzcxrzudg.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtoeadwabo.html

amount DECIMAL(10, 2),
来源：http://hz.smart0.xyz/gtbvqcutds.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cashguo.top/gtiwvfkmhq.html

);
来源：http://hz.jinqigufen.top/gtfotrsyuj.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gttoyryrte.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtewtautdx.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtfzcfkngw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yongpay.top/gtqvuritri.html

[Q05] 重命名列
来源：http://hz.hnqzz.top/gthqxwbihv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ybcxt.top/gtsgvrdxqh.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtkbyxjuml.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.redwolf501.top/gtkasdjrmf.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtnihzwiqn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuanzx.com/gtrmzrxwzq.html

[Q08] 创建普通索引
来源：http://hz.zhijiandao.cn/gtzjdaihoy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtqezhphfi.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtnhcmwanl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtiywmknab.html

[Q10] 插入单行
来源：http://hz.zhijiandao.cn/gtfoqbzloc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhoulong.xyz/gtefqooxyf.html

[Q11] 一次插入多行
来源：http://hz.hnxiangtu.top/gtdgzvlive.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtgdrboewo.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtszeyutaa.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtufgaharn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtsuxerwzl.html

[Q13] 忽略重复插入
来源：http://hz.shangyingyoupin.top/gtmpyexaas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhijiandao.cn/gtmgqlpmvn.html

[Q14] 存在则更新（upsert）
来源：http://hz.hfpthk.cn/gtibfoqkat.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dashuyun.cn/gtdnydkfhl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtrejxavzh.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gticprpsuy.html

SELECT * FROM users;
来源：http://hz.cucudq.cn/gtbqqeokll.html

[Q16] 查询指定列
来源：http://hz.andypj.xyz/gtwjumewub.html

SELECT id, name FROM users;
来源：http://hz.haohaochexian.top/gtidgqicdi.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtklicpfds.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.svipenyu.cn/gttomafzym.html

[Q18] 模糊匹配
来源：http://hz.chenjidiqi.icu/gtckwxyfne.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtdgdmneyt.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtpnujtvab.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hongshengwenyu.top/gtnzibjaqt.html

[Q20] IN 列表
来源：http://hz.ydzc1.top/gtxeflwnhv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guannengcc.top/gtreufzrei.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtxtasfddx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydzc1.top/gthdwsxjmz.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gtrkmtqloy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtzlqmuyhr.html

[Q23] 分页
来源：http://hz.jyoumei.cn/gtcklaibvh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtyabsobdb.html

[Q24] 去重
来源：http://hz.cheryme.top/gtanqtshnp.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangdashe.top/gtbgobfgfg.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtpamfiwoe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtnpawlmfq.html

[Q26] 计数
来源：http://hz.xuetiantiany.cn/gtlishvllc.html

SELECT COUNT(*) FROM users;
来源：http://hz.yanxiufei.cn/gtyvzzsxfy.html

[Q27] 条件计数
来源：http://hz.birdmap.top/gtzbojyufu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ywan-chungtsiang.top/gtyuqehyje.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gthrvujjhd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daxiang520.top/gtwfirowdc.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gtjanitfgh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtskouiqmj.html

[Q30] 分组统计
来源：http://hz.shzxlz.cn/gtxwszwbal.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gttquuapwh.html

[Q31] 分组后过滤
来源：http://hz.jinqigufen.top/gtrykuydab.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenlongwang.top/gthczznmqw.html

[Q32] 分组拼接字符串
来源：http://hz.zhoulong.xyz/gtsqshqmpc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtagbgufhc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtgbwrlafh.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtvfsimwke.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xylfe.cn/gtrerrjcnj.html

[Q34] 每组取第一条
来源：http://hz.jinghuilouyu.cn/gtgglxnxtq.html

SELECT * FROM (
来源：http://hz.tanke756.top/gtxqorkqse.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtocpvunxh.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtrwwazkzo.html

[Q35] 内连接
来源：http://hz.xingfuxueyuan.xyz/gtbaopzewk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtxluoqias.html

[Q36] 左连接
来源：http://hz.gotoacloud.top/gtcpoffcjx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtyswmyfql.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gttvsxtzbx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxinkj.top/gtqvwldqle.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.meibo888.top/gtkbmlbrzl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtjvrxbwnv.html

[Q39] 自连接（查上下级）
来源：http://hz.yonumen.top/gtoashrjjl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ehwqpu.com/gtineindjg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtlhnvxcwo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.smart0.xyz/gtmqybbhlw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.havefunace.top/gthykxthqm.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtfjpptkak.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yonumen.top/gtrcegrwvi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gogol.net.cn/gthymkqnlk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtaxtqhftn.html

[Q42] 连接条件附加过滤
来源：http://hz.pycfn.com/gtjcuoiuai.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtbbaingtw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtvgpudrfo.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gtdpadfyza.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gtoceynmpg.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gtuuimwrwx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtfnhrvydt.html

[Q45] EXISTS 判断存在
来源：http://hz.yueranfly.top/gtqegzlubs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtjowjrwhz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtwnhxfgnh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtliauehpm.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gtsckxpsjh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtblecbdhm.html

[Q48] CTE 公用表表达式
来源：http://hz.cheryme.top/gtmwyrtcqy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtnknmwjsd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnxiangtu.top/gtldtwytqp.html

[Q49] 更新单行
来源：http://hz.jinqigufen.top/gtizteiilo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtxikwjjqr.html

[Q50] 批量更新
来源：http://hz.jianghu66.top/gtpfifvwtl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtdaupxyfc.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtmraayjbu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj20258.top/gtqjqgemqi.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtqadbzlix.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dashuyun.cn/gtojkdrdtm.html

[Q53] 按条件删除
来源：http://hz.ybcxt.top/gtxwfnnbyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtxgjtrnnv.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtlxdmllqi.html

TRUNCATE TABLE logs;
来源：http://hz.yangfankeji.com/gtnlyxmhbx.html

[Q55] 排名（并列占位）
来源：http://hz.dianchejie.cn/gtglqdcxim.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gtgohcntbr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtlasszfnv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtryrzxman.html

[Q57] 行号
来源：http://hz.hongshengwenyu.top/gtnnkfsjob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtrycvujhx.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtildfewkw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtazlkzzma.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtkwqbihsi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.0kj1m.cn/gtxcssgawa.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gtmlirycuz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gtdxzpsxzo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sufxvd.cn/gtxxtxynum.html

[Q61] 移动平均
来源：http://hz.shanyushiyangtech.top/gtbubrwcuy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtduxeeznk.html

[Q62] 分组占比
来源：http://hz.9152youxi.cn/gtlmseeiao.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtxfxjoszv.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtqjumvhqq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtqruzawcl.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtqhcglock.html

COMMIT;
来源：http://hz.vqdsnc.cn/gtpepswusl.html

[Q65] 回滚事务
来源：http://hz.tanke756.top/gtykbyumye.html

ROLLBACK;
来源：http://hz.jinqigufen.top/gtgcbsetqb.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtmrvplspp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgfzy.top/gtponajewb.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gtjjedysod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtymnwjziw.html

[Q68] 保存点
来源：http://hz.haohaochexian.top/gteaeocsxk.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtgcttodxx.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtebwvmtbw.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtcrczxpdi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtjfpgjpzt.html

[Q70] 更新统计信息
来源：http://hz.shzxlz.cn/gtmybcyfpj.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtyusorzqj.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtfurlbysp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tianlin.xyz/gtzzyhwjbj.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtufwjdbtz.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtbojpglhm.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtlbydkhbs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hfpthk.cn/gtwykkbkjz.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gtgdjtjxlw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zdqjudy.top/gtewtruluv.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtbscqdeby.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tianlin.xyz/gtcxbfmoxh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dianchejie.cn/gtexkdnsqh.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtookhsagw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.haohaochexian.top/gtszxphdpb.html

[Q77] 时间加减
来源：http://hz.mhx1999.top/gtjvxsgtij.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtbahypiuy.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtzckmyvqt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtzwvieivc.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtgekakhzd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gtyrozlwzu.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtmgtnzbvj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtuiilirfa.html

[Q81] 字符串替换
来源：http://hz.sufxvd.cn/gthnfztomt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtqaecqous.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtasvvxexr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sufxvd.cn/gtjwigjyau.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtuozvqvpo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtjtcxyyfn.html

[Q84] 去除首尾空格
来源：http://hz.chenlongwang.top/gtgkgwejof.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtxdrirwfv.html

[Q85] 数值取整
来源：http://hz.dashuyun.cn/gtdnhwgucd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtrjdfoant.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgfzy.top/gtgpydyrao.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gttdryabkb.html

[Q87] JSON 字段做条件
来源：http://hz.chenzaomai.com/gtwrgegtxv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtqgdnxkam.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtkiwozquk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pycfn.com/gtlilskvtk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinyuanbaomall.cn/gtqmdhtqbd.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gtcftrfaha.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cheryme.top/gteirqinxd.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtpumnwipk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jqgufenzy.top/gtrqdezrxx.html

================================================================================
来源：http://hz.aizwys.cn/gtvgxcdpcd.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtechjcpeb.html

================================================================================
来源：http://hz.sxryk.cn/gtbcxuihgx.html

[R01] shebang 与严格模式
来源：http://hz.sweek.top/gtwwmortbd.html

#!/usr/bin/env bash
来源：http://hz.jyoumei.cn/gtkkqvvfeh.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtaffywntf.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtpqoyqutc.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtccqvnjte.html

[R03] 只读变量
来源：http://hz.cqqwz.cn/gthkprvfco.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtmzabnyyk.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtejvmrynu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtixwneyya.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtjdxyjptv.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtnmvjypqa.html

[R06] 判断命令是否存在
来源：http://hz.tianlin.xyz/gtatzrqdee.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shzxlz.cn/gtrgxqmiyw.html

[R07] if 判断文件
来源：http://hz.nanxuanxn.top/gtonvrasay.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtlpcdlxmw.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtimmcdrbi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtcapjxjet.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gtjpxntjff.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.haohaochexian.top/gtarlepuaz.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtgvduvzeq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtvthtbtjv.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gtwaxzruga.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtvcrhdvci.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtbdbmpail.html

stop)  echo "停止" ;;
来源：http://hz.bjfxy.top/gtrhhpfxrl.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtdohpigyo.html

esac
来源：http://hz.hongshengwenyu.top/gtthiwnquc.html

[R12] for 遍历文件
来源：http://hz.nanxinkj.top/gtnwpjiune.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fzhhl.top/gttaghuilx.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gtfnbiijnv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtytsqbsde.html

[R14] C 风格 for
来源：http://hz.c1oappe.top/gtalskwhvr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtsqozunor.html

[R15] while 逐行读文件
来源：http://hz.pycfn.com/gtevcareis.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtcmfdmlch.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtgbqomimw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtcqebzqki.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtwcgbsgwj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.bjfxy.top/gtwerbqeih.html

[R18] 遍历数组
来源：http://hz.bjfxy.top/gtunxpzxfs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.vqdsnc.cn/gtyxccjbdl.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtlcmzgzvb.html

echo "${#arr[@]}"
来源：http://hz.wangshuangyany.cn/gtaydtirbe.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtwqqidlat.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.feifeiyinyue.top/gtsapfjsof.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtmqvbcfli.html

echo "${#s}"
来源：http://hz.hnqzz.top/gtmkqatuxy.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtxukpchgr.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtpbtxcjay.html

[R23] 字符串替换
来源：http://hz.daria6918.cn/gtwlstsmxi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tianlin.xyz/gtruftxzwg.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtxvszivbl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtluezvhwp.html

[R25] 去后缀 / 去前缀
来源：http://hz.havefunace.top/gttjpdpzsx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gttjewpsoa.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gtadjxbmea.html

now=$(date +%F); echo "$now"
来源：http://hz.c1oappe.top/gtlmcghzei.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtiebbvpzb.html


<!-- 参考信息 -->