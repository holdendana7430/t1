代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtxxgweakk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gtcufdhvek.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cdnleiting.top/gtthdskxkm.html

Ruby: a == b
来源：http://hz.tianlin.xyz/gttdbfzmsw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.mhx1999.top/gttqsekcjg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ywan-chungtsiang.top/gthdzrtvix.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtmplusdad.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtoepmnqjk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtrcnberog.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtwnelubad.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtmnosqsyf.html

Go:   if x == nil {}
来源：http://hz.dashuyun.cn/gtazurhmqs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtscufhkeh.html

C#:   if (x is null) {}
来源：http://hz.hysaishi.cn/gtgtelhwct.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtcaxibpzg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenzaomai.com/gtrlptyckn.html

PHP:  // 手写时间戳比较
来源：http://hz.gaohongyu789.top/gtsocrsjdn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtswiaimhe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtytuxitaq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigufen.top/gtvtqgqoyd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtkvfanwed.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gtlgxlurjj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtggtibatf.html

[P08] 处理浮点精度问题
来源：http://hz.xingfuxueyuan.xyz/gtjjsduobi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtaindymdx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cdnleiting.top/gtvlfaqcgr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xingfuxueyuan.xyz/gttrmhbhmg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ehwqpu.com/gtvfvjmjid.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtfvpwyout.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xinyue.icu/gtjivbyqeo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinghuilouyu.cn/gtjyqrrsfv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gtptsudtqw.html

================================================================================
来源：http://hz.jianghu66.top/gthofiggtz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtqvnpqbgg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgateybai.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtlgzmnyyz.html

CREATE TABLE users (
来源：http://hz.shanyushiyangtech.top/gtkaxitlvb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gtadfilmya.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtgjvxskwd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtxgslpodo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtjyenrtmt.html

);
来源：http://hz.svipenyu.cn/gtalhdrowa.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gtjffutowa.html

CREATE TABLE orders (
来源：http://hz.yuxming.cn/gtdzoiewht.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtdxngtszz.html

user_id INT NOT NULL,
来源：http://hz.jinqigufen.top/gtfmofdamj.html

amount DECIMAL(10, 2),
来源：http://hz.zhijiandao.cn/gtugcmvybt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tian-w.cn/gtkdbcyrvh.html

);
来源：http://hz.guannengcc.top/gtzszvykfk.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtzbfpsfbm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gturjqdevb.html

[Q04] 修改列类型
来源：http://hz.zhijiandao.cn/gtmjtdnqew.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sxryk.cn/gtxfvdlhlj.html

[Q05] 重命名列
来源：http://hz.nanxuanxn.top/gtejbwqmpg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtciwexerd.html

[Q06] 删除列
来源：http://hz.xingfuxueyuan.xyz/gtcjlytnfm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hywenlv.cn/gtntwuhhgb.html

[Q07] 删除表
来源：http://hz.fengsongda.top/gtvbxccalt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gticwtbyfe.html

[Q08] 创建普通索引
来源：http://hz.xylfe.cn/gtxtlkijwe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtcbkximwf.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtsabbrnbp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtceybvgxh.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gtmioikrdi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gtzwstmboz.html

[Q11] 一次插入多行
来源：http://hz.gogol.net.cn/gtecaocjnm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtvvxjiayc.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtuzsslidi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dianchejie.cn/gtrikneqro.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.9152youxi.cn/gtwildsujx.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtikqgmsfb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtdshebzkg.html

[Q14] 存在则更新（upsert）
来源：http://hz.gzhubu.top/gtqzcgodzw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.andypj.xyz/gtqvbheasr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtssjweyjb.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtrszmxkxz.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtzekhteld.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtskehrsta.html

SELECT id, name FROM users;
来源：http://hz.kuanghao11.cn/gthlqoxqet.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtykiuylah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtbmpoifqe.html

[Q18] 模糊匹配
来源：http://hz.yuxming.cn/gtdsdesfda.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.andypj.xyz/gtlldmmllu.html

[Q19] 范围查询
来源：http://hz.bjfxy.top/gtrxwodkca.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhaomingkeji.xyz/gtluyezovw.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtnrouwaii.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.kuanghao11.cn/gtqkjdzyij.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gttvgrmcod.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gteowejnzs.html

[Q22] 排序
来源：http://hz.zhongyouzk.top/gtidomzycz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtzlxgovuo.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtgmazuzmb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gtiikvoupj.html

[Q24] 去重
来源：http://hz.meibo888.top/gtuosjqlxv.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtxdzkbifj.html

[Q25] 只取前 N 条
来源：http://hz.dianchejie.cn/gtumizsiuc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sweek.top/gtakjsjtwp.html

[Q26] 计数
来源：http://hz.52xcode.cn/gtznrvwcga.html

SELECT COUNT(*) FROM users;
来源：http://hz.yueranfly.top/gtgbmaxxmn.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtiiotfozc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gttiygkned.html

[Q28] 求和与平均
来源：http://hz.yangfankeji.com/gtoicyjelk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gtndqpamfy.html

[Q29] 最大最小值
来源：http://hz.shuidangran.top/gthdctbspi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gtipwoheom.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtqamgazjo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtudgpclct.html

[Q31] 分组后过滤
来源：http://hz.smart0.xyz/gtjkmpaodr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aibaodan.cn/gtfvvwbzxt.html

[Q32] 分组拼接字符串
来源：http://hz.jinghuilouyu.cn/gtpshhvshb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gthmkdeziw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.birdmap.top/gtiufbffrt.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtekklstgd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtfjoflxml.html

[Q34] 每组取第一条
来源：http://hz.52xcode.cn/gtwonmonyb.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtdcukxcig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtlkuhedzb.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtysgxwkll.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtekaiaakc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtsxxnmtyd.html

[Q36] 左连接
来源：http://hz.zhongyouzk.top/gtnlnihdga.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtdfdkkwog.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtzsrjparp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtnahuhlev.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenjidiqi.icu/gtagquxlgu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtjdcfduzs.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258888.top/gttnauldwo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtrpmnasgf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gtsqrsqsxb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtgvsxqbyb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daria6918.cn/gtcdghxvrn.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtrbpxhwev.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gttjlzeant.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sweek.top/gtqqnvsecz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.mhx1999.top/gtokmliphx.html

[Q42] 连接条件附加过滤
来源：http://hz.zycfv.cn/gtuhvjjciv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shangyingyoupin.top/gtuztyrzsq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fzhhl.top/gtbxgtabeh.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtzmpxvnzn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gttmtztyue.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtqatemzzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hywenlv.cn/gttffhcmzw.html

[Q45] EXISTS 判断存在
来源：http://hz.aizwys.cn/gtoueejmwi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenjidiqi.icu/gtiqebrrls.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenjidiqi.icu/gtmvzjqeyk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtptaicjxj.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtovmmvjvg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtaqhmxynz.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtdgvqabrw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gtfqjjpdaj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtunzoltcd.html

[Q49] 更新单行
来源：http://hz.jiagoushi.top/gtsysmainm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gtjovxrrcw.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gtmlkycrew.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtpenolahg.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtmnuzvbbl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgfzy.top/gtdkfnrlku.html

[Q52] 删除指定行
来源：http://hz.shuidangran.top/gtjrvfscuk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtutltuwad.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtapanivff.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gtepketxcg.html

[Q54] 清空表
来源：http://hz.yvedp.cn/gtetkvjfvx.html

TRUNCATE TABLE logs;
来源：http://hz.yangfankeji.com/gtkezrlgtr.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gtwgdtroiz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hongshengwenyu.top/gtgrrrzotx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtruhkagtw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenjidiqi.icu/gtjfqnbpvp.html

[Q57] 行号
来源：http://hz.shuidangran.top/gtbmimnzba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sxryk.cn/gtexdqbnou.html

[Q58] 累计求和
来源：http://hz.jianghu66.top/gtgwemquia.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gtjyffnfjz.html

[Q59] 分组内累计
来源：http://hz.xinyue.icu/gtlywlvkns.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydjk.org.cn/gtctianwbr.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtqdjxsyuo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtsddapvbr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtzzxvebor.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gtqtrgqqnv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhoulong.xyz/gteypacgif.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gtrbuuhzhx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtiqrhmuzh.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gthfwpjswy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shuidangran.top/gtticxdpkl.html

[Q64] 提交事务
来源：http://hz.meibo888.top/gtiypbdmih.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtpprrmyoo.html

[Q65] 回滚事务
来源：http://hz.52xcode.cn/gtktocnhij.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtsbuwtixg.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtggtrtolb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daxiang520.top/gtchxgrqqe.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtxnokekqq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shzxlz.cn/gtjytskffp.html

[Q68] 保存点
来源：http://hz.hammf.cn/gtuppgwzmw.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtocvcafam.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gthkolyspg.html

[Q69] 查看执行计划
来源：http://hz.cucudq.cn/gtfbwewgob.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnxiangtu.top/gthovsbtfw.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gtzwiiezsx.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtfopkkxdk.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtbnmaorgv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtzzndooyf.html

[Q72] 查看索引
来源：http://hz.daxiang520.top/gtwhibcwtw.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtpaizyfxp.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtyrjhxhvo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuxming.cn/gtamwbltey.html

[Q74] 强制使用索引
来源：http://hz.wangdashe.top/gtfxfcheyb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sxryk.cn/gtqbuavbpz.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtiaejaepd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gthhqgtvns.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtrpurajyo.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtyrmswygi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgufenzy.top/gtrzxkuppi.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtannrfkhw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtrqjzzyim.html

[Q78] 当前时间
来源：http://hz.aibaodan.cn/gtlzahcjmz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtasmgwlyb.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gttcvsqpqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtdyndrkxe.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtqrduaqcq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xziqi.cn/gtsqmwdjsp.html

[Q81] 字符串替换
来源：http://hz.xinyue.icu/gtxbzipekg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtdhbcaiwy.html

[Q82] 字符长度与字节长度
来源：http://hz.xuetiantiany.cn/gtmpitiqar.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.svipenyu.cn/gtpxqmdahw.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtuqyjsasb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhengqikj.top/gtvyctbaqd.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtadqxlljq.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gtzcfvtjrh.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtlbnmuyxb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtkjhsekuv.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtrimmwjmi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtsfnvrkdb.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtlvdnuwhy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxuanxn.top/gtsjblbrmj.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangtech.top/gtvcnyovyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gtksopbixm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtoeczkstn.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtcmxkpjol.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gtcwupqspy.html

[Q90] 生成序号列
来源：http://hz.pycfn.com/gtetagdjrm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuanzx.com/gtodxjdygx.html

================================================================================
来源：http://hz.yj20258888.top/gtqyooowzg.html

R. Bash 专题
来源：http://hz.iojbl.cn/gttwhyihfb.html

================================================================================
来源：http://hz.guowangkeji.top/gtixnyhfmk.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtpfzlouox.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gttgksfclx.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtgjaionwl.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gttiikimqo.html

name="Tom"; echo "$name"
来源：http://hz.fzhhl.top/gtxwflfxtw.html

[R03] 只读变量
来源：http://hz.quarkkingdee.top/gtoxctkvgu.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtwakqlxja.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtazdcgurc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtrtaldire.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtrabhcypi.html

name="${1:-default}"
来源：http://hz.nwbrower.top/gtzqlsspxk.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtmgebvbxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtxyaxjwbi.html

[R07] if 判断文件
来源：http://hz.kuanghao11.cn/gtjxkgpian.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuanzx.com/gtinychftk.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtlyccopjs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gteztfizaq.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtskrgtbzs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhongyouzk.top/gtmmzslqrt.html

[R10] 正则匹配
来源：http://hz.quarkkingdee.top/gtqyozcevm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtvqxngmxn.html

[R11] case 多分支
来源：http://hz.vqdsnc.cn/gtjhwqndtz.html

case "$1" in
来源：http://hz.sxryk.cn/gthxyfzaph.html

start) echo "启动" ;;
来源：http://hz.zhengqikj.top/gtamndpant.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtqagjoqoo.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtirhjmqys.html

esac
来源：http://hz.tian-w.cn/gteeqclwih.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtfvsbueyx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhijiandao.cn/gtkqiiqikl.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtdmkvwqsh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtctpuavon.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtlcfqqmvj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtxybxegcf.html

[R15] while 逐行读文件
来源：http://hz.xinyue.icu/gtgjynmjdw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtoljqnhfp.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtpzvdlooe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnqzz.top/gtncoqasre.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gtyehxbvrb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.0kj1m.cn/gtlrgzfsfh.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtrzygjhnj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinghuilouyu.cn/gtrmybmqnj.html

[R19] 数组长度
来源：http://hz.pengpengdd.cyou/gtmyazqveh.html

echo "${#arr[@]}"
来源：http://hz.ehwqpu.com/gtrrmthgpu.html

[R20] 关联数组（字典）
来源：http://hz.ivvv.top/gtujhfqlvy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.52xcode.cn/gtowlbxmxy.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gteebqjodu.html

echo "${#s}"
来源：http://hz.zhixingplan.top/gtzrmhmdmc.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtsqatwtll.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtqdgooezi.html

[R23] 字符串替换
来源：http://hz.jlsjyb.cn/gtxetffsjf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtsduomjeb.html

[R24] 大小写转换
来源：http://hz.yuanzhike.top/gtkwootmtp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hysaishi.cn/gtrrxeprlg.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtreqztqyf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydjk.org.cn/gtihxgrilu.html

[R26] 命令替换
来源：http://hz.yueranfly.top/gtpcjarwss.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gtciiaxwju.html

[R27] 算术展开
来源：http://hz.xuanzx.com/gtjbzjgkkh.html


<!-- 参考信息 -->