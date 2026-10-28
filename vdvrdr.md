代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtzdvrvbvg.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gtudpdmseg.html

[P07] 防抖与节流
来源：http://hz.gzhubu.top/gttqmdrqzd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydzc1.top/gtlfosbgyg.html

PHP:  // 手写时间戳比较
来源：http://hz.meibo888.top/gtwcxotwlx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtwwrflgxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtoovrhnpg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtdxdbodbd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hammf.cn/gtlvtfuhwk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtlatoxxwz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuxming.cn/gtmeghphsr.html

[P08] 处理浮点精度问题
来源：http://hz.nanxinkj.top/gtozdrzgit.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenlongwang.top/gtyzjmymfy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtdywchonj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtnwpiaibx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtgmheuhus.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gtjwbajvdc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guannengcc.top/gtoythsfyx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtrlywfprh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.9152youxi.cn/gttayomkbk.html

================================================================================
来源：http://hz.yongpay.top/gthobttntb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtkbrdypsa.html

================================================================================
来源：http://hz.cdnleiting.top/gtzjcyetiv.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtndcdpdvb.html

CREATE TABLE users (
来源：http://hz.jyoumei.cn/gtecocifmc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtgqrtnbpo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gtbykqqjhh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sweek.top/gtbbdeyuox.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gtfjkcbolu.html

);
来源：http://hz.chenjidiqi.icu/gthclrvlyr.html

[Q02] 创建带外键的表
来源：http://hz.svipenyu.cn/gtujyoxaak.html

CREATE TABLE orders (
来源：http://hz.yueranfly.top/gttpjtniiv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtoxxcorzw.html

user_id INT NOT NULL,
来源：http://hz.zhongyouzk.top/gtauwkusct.html

amount DECIMAL(10, 2),
来源：http://hz.bjfxy.top/gtmtqiqieg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtpcyeorqi.html

);
来源：http://hz.cashguo.top/gtxdnzhgld.html

[Q03] 增加列
来源：http://hz.quarkkingdee.top/gtcwnvbmva.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jyoumei.cn/gtzjbchznt.html

[Q04] 修改列类型
来源：http://hz.tanke756.top/gtjqwqfkme.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangdashe.top/gtfcylcbdq.html

[Q05] 重命名列
来源：http://hz.meibo888.top/gtbtbqikrq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtvgasvkum.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtdlzmvdzg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.haohaochexian.top/gtrmthqrtz.html

[Q07] 删除表
来源：http://hz.shzxlz.cn/gttixlaxio.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fzhhl.top/gthudmfvmm.html

[Q08] 创建普通索引
来源：http://hz.zdqjudy.top/gtljxdfdjq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jiagoushi.top/gtwdkyujtz.html

[Q09] 创建唯一索引
来源：http://hz.vqdsnc.cn/gtlnteyqmf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtnwgprmgk.html

[Q10] 插入单行
来源：http://hz.ydzc1.top/gtehwmcmfs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gtujofzlxu.html

[Q11] 一次插入多行
来源：http://hz.zhaomingkeji.xyz/gtpobmcbee.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtddrprrfe.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtumyyhizm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhoulong.xyz/gtmwiuzvxm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pycfn.com/gtxtoqcqav.html

[Q13] 忽略重复插入
来源：http://hz.cheryme.top/gtnokksehn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtiswydmmc.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gtuzmkvuhy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.havefunace.top/gtycrdfdot.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258.top/gtvrtsealj.html

[Q15] 查询全部
来源：http://hz.zdqjudy.top/gtrugwsynz.html

SELECT * FROM users;
来源：http://hz.dianchejie.cn/gtlxkvnlns.html

[Q16] 查询指定列
来源：http://hz.kuanghao11.cn/gtgpoawiva.html

SELECT id, name FROM users;
来源：http://hz.meibo888.top/gtgzgoyxxy.html

[Q17] 条件查询
来源：http://hz.redwolf501.top/gtjxexzuoh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gtrdfqxnuj.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtjvshubzl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtjwdomtgk.html

[Q19] 范围查询
来源：http://hz.ppjwa.cn/gtyxangrpw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hfpthk.cn/gtujwliokr.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtikmxxwvc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtgqcigdmn.html

[Q21] 空值判断
来源：http://hz.wangdashe.top/gtujtxfnmy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtkxqzuatw.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gtgdxclgtw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haohaochexian.top/gtlrqbsrxi.html

[Q23] 分页
来源：http://hz.yueranfly.top/gtjqjyetqs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gthdfvcogt.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtoorgrurg.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnqzz.top/gtrextcjqo.html

[Q25] 只取前 N 条
来源：http://hz.birdmap.top/gtdutpfaxf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.0kj1m.cn/gtrdkanauw.html

[Q26] 计数
来源：http://hz.hywenlv.cn/gthaowrrcc.html

SELECT COUNT(*) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtnkustuov.html

[Q27] 条件计数
来源：http://hz.hnqzz.top/gtfcqwbgcu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtaoltqibl.html

[Q28] 求和与平均
来源：http://hz.quarkkingdee.top/gtjwpomxyq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtqhuhqbfn.html

[Q29] 最大最小值
来源：http://hz.iojbl.cn/gtcioapnhe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tian-w.cn/gtqexaogrw.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gtjgorlwpv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtvxalaxtb.html

[Q31] 分组后过滤
来源：http://hz.xylfe.cn/gtdhtavytw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtokrraorm.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gtzeoifgrx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtsiigwltf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtqzwnrxjb.html

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gteggavbbb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.quarkkingdee.top/gtkywfuzwc.html

[Q34] 每组取第一条
来源：http://hz.fengsongda.top/gtyjlmecat.html

SELECT * FROM (
来源：http://hz.gotoacloud.top/gtmtdkdrjz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtiwabwncp.html

) t WHERE rn = 1;
来源：http://hz.shangyingyoupin.top/gttrupdjwf.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtrczasehx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtlgiipcew.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtdounwvps.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gthszgfsmo.html

[Q37] 右连接
来源：http://hz.jqgfzy.top/gtkfriixhp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtwrdaropk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.316326.xyz/gtlwqmibyr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtkvtqtmil.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtrsxjcusx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sysykeji.top/gtmwhtvdsz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtwzqttbxz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.feifeiyinyue.top/gtylwokjby.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtnqtsmxbm.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtnrdhzefx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenlongwang.top/gtlnsmjgcg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.haohaochexian.top/gtcicpbilp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtuwmcslwq.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtsvoyqbbh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtdvfqidlv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtsjciayak.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtyhaglrcy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtogqkighb.html

[Q44] IN 子查询
来源：http://hz.hammf.cn/gtzcojqtpr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhongyouzk.top/gtkxhanrga.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtzjjltyvg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtpiuqxbiu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sufxvd.cn/gtqqdutjlm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtawtnyrot.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtssdrskmc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gogol.net.cn/gtinlilnfw.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtrzxnzuzd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gtlqklqskm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gtlxirafna.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtefsazyec.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtpupuorju.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtorrrsksr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gtkkdpxyhm.html

[Q51] 用子查询更新
来源：http://hz.fengsongda.top/gtkludtnve.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pycfn.com/gtijncatms.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtvxzkmikd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtqdqnqobx.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gttlwnflxm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dianchejie.cn/gtgpjqndhc.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtelrhzocf.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtlotdekzp.html

[Q55] 排名（并列占位）
来源：http://hz.cheryme.top/gtnbgnujbi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shzxlz.cn/gttflvbgmt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtpmfqsgim.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtnzudsagl.html

[Q57] 行号
来源：http://hz.sweek.top/gtktqozqsd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gthqyvlmiu.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gttwkcdokg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtfuiwpjlz.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gtsmkiwztv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gttcpcvwwm.html

[Q60] 取上一行 / 下一行
来源：http://hz.daxiang520.top/gtphzhlmkc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtiwwohslm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtnishsfca.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gtmsajodqz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sweek.top/gtlgbygcix.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gthhmwzznd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtajyxqjxu.html

[Q63] 开启事务
来源：http://hz.aizwys.cn/gtlwseelpf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtlndlmiyn.html

[Q64] 提交事务
来源：http://hz.shzxlz.cn/gtsrlygjhy.html

COMMIT;
来源：http://hz.zycfv.cn/gteywdorwu.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtwfzbeymk.html

ROLLBACK;
来源：http://hz.jianghu66.top/gtdmrwhofw.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtxazqkiip.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtucqseffi.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtsqiwtvws.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtmhnltfvp.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gtpxlhokkq.html

SAVEPOINT sp1;
来源：http://hz.aizwys.cn/gttbaekvmo.html

ROLLBACK TO sp1;
来源：http://hz.yonumen.top/gtumrlxtee.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtnlzflzuj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shangyingyoupin.top/gthojzxxvp.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtuybpqucc.html

ANALYZE TABLE users;
来源：http://hz.gzhubu.top/gtzwghsevh.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtinepqego.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtdttcjdim.html

[Q72] 查看索引
来源：http://hz.chenjidiqi.icu/gtnpemzuxf.html

SHOW INDEX FROM users;
来源：http://hz.daria6918.cn/gtpyilmgpj.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtqfplhbyf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.vqdsnc.cn/gtedcexegk.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtnhucfrge.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gogol.net.cn/gtawqiwkow.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtwyqrkfqr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtfumheisq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fzhhl.top/gtytsfeoim.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtlblvohzg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtxaubxhew.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtibhgemxw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gtdhnwnhlk.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gthdzozuiq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yonumen.top/gtahthagkl.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gtuaqmmnwy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinyuanbaomall.cn/gtxhhrminz.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtbyddgswh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenjidiqi.icu/gthpfxmqss.html

[Q81] 字符串替换
来源：http://hz.yj20258.top/gtqqessqsm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtpcjlbyyn.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtwpmnsoyv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtutdzotgw.html

[Q83] 大小写转换
来源：http://hz.jinqigufen.top/gttmvsalbp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sysykeji.top/gtakjjqceb.html

[Q84] 去除首尾空格
来源：http://hz.zhijiandao.cn/gtvwlnccja.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenzaomai.com/gtlpzczhfh.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtrtkgfubv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtskiieeyz.html

[Q86] 读取 JSON 字段
来源：http://hz.kuanghao11.cn/gtiimcgkdq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydzc1.top/gtchjlzayf.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtyxzjpsfj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daria6918.cn/gtrhkgmuxp.html

[Q88] 行转列（条件聚合）
来源：http://hz.shuidangran.top/gtndgkjjns.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ppjwa.cn/gthtohacbv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gttuwjeenh.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtxuogiahe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtxizqqtdb.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gteiccyqvw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gotoacloud.top/gtyokpjpue.html

================================================================================
来源：http://hz.shzxlz.cn/gtnmchcyih.html

R. Bash 专题
来源：http://hz.jiagoushi.top/gtidsyraub.html

================================================================================
来源：http://hz.ydzc1.top/gtkgylmbly.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtzsuovagr.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtkllrkexp.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtlgsvydoo.html

[R02] 变量赋值与使用
来源：http://hz.zhijiandao.cn/gtdxudpmwq.html

name="Tom"; echo "$name"
来源：http://hz.xylfe.cn/gtarnpbnip.html

[R03] 只读变量
来源：http://hz.redwolf501.top/gtnvyrqrkt.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtjtgvmndh.html

[R04] 位置参数
来源：http://hz.kuanghao11.cn/gtctzxzmzz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gtvucvczwj.html

[R05] 参数默认值
来源：http://hz.yongpay.top/gtleamczgh.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtzmnzulpe.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gtmkrjdicg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xziqi.cn/gtkwmwjerv.html

[R07] if 判断文件
来源：http://hz.cdnleiting.top/gtjrdjxrsl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.andypj.xyz/gtoswwmbry.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gtimzqzexh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtfkbvlelp.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gtjovocioy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtanxbfbjl.html

[R10] 正则匹配
来源：http://hz.52xcode.cn/gtbkbqxppd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gthuqdlayc.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gthlvouqhb.html

case "$1" in
来源：http://hz.jianghu66.top/gtfuhwdbvu.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gtklyudpgb.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gttlsnifsz.html

*)     echo "未知命令" ;;
来源：http://hz.yongpay.top/gtuuhieigd.html

esac
来源：http://hz.chenlongwang.top/gtvtkceghc.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gteyjyftxj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtobfnxgyn.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtzbwghcki.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtsdscnoxe.html

[R14] C 风格 for
来源：http://hz.hnxiangtu.top/gtzjhksrqz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gttssfjsww.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtexgwqitw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtwqnjeptu.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtfiavhvrc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gtcaczesfg.html

[R17] 数组定义与取值
来源：http://hz.cdnleiting.top/gtclpjyncx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.redwolf501.top/gtkpecodcj.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtknuzyirj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtjsptfptj.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtunlylstw.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtrddpodsn.html

[R20] 关联数组（字典）
来源：http://hz.0kj1m.cn/gtwqklyyxj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtcsizicbk.html

[R21] 字符串长度
来源：http://hz.jinghuilouyu.cn/gtrljkdwne.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtmawytknc.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtxzlpmrak.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtgdmgqren.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gthkvhzbbc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtbldpirgo.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtpdheehrj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258.top/gtxlqjihjd.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtdmoltsst.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gtgnarlnlw.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtfupebsch.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtflvngvwq.html

[R27] 算术展开
来源：http://hz.sweek.top/gtcqlujvgc.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtcbxuvhgg.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtuudvning.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtnurfdzzd.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtvjhcecin.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zycfv.cn/gtrymqfkiq.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtkwctagtr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cashguo.top/gttlfyiaui.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtgurdxedt.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gthytmavdy.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtavxcrsra.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.pycfn.com/gtlyrsiism.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gtawriescm.html


<!-- 参考信息 -->