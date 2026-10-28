代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtcqcquvww.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gthldjsjza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtgzzldqsz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtzlmvvmwf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtrreihdyo.html

Go:   len(arr);  len(m)
来源：http://hz.zhaomingkeji.xyz/gtecblhimy.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gthzbhjxnt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgufenzy.top/gtbayaoncg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ehwqpu.com/gtkskbkhpp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gteibyairu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shuidangran.top/gtwxmryigy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.smart0.xyz/gtfpsnupmx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtiodtepin.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.52xcode.cn/gtprmwdwfd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cheryme.top/gtfevesiuc.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gtcdghpssw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gtsrmastpn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtglksufef.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhijiandao.cn/gtavcjelms.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtjwzltqck.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xingfuxueyuan.xyz/gtvogpkfmh.html

TS:   if (x == null) {}
来源：http://hz.xuetiantiany.cn/gtukykgybf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtbryavwob.html

Go:   if x == nil {}
来源：http://hz.cdnleiting.top/gtfjkgviox.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtzpweusep.html

C#:   if (x is null) {}
来源：http://hz.daxiang520.top/gtuuyvviml.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtciwmlsgs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cqqwz.cn/gtcbptwtce.html

PHP:  // 手写时间戳比较
来源：http://hz.ppjwa.cn/gthyualcze.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtyeuvgabr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtceopqbwg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtxkajfvco.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jianghu66.top/gtgniccxqd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydjk.org.cn/gtardrdmgh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydjk.org.cn/gtyrslawds.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtjbdsftrz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtmntmfnuf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sufxvd.cn/gtkjrjkreu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtaurgxdyt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtkmyemdry.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtkncjxfru.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daxiang520.top/gtxaelsvon.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtwvvbryrc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtatantxan.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkkrbrldw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtwtqqlaro.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmjezxjgv.html

[Q01] 创建表
来源：http://hz.sufxvd.cn/gtlnkogwmt.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtcyfgbiep.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtvaumqjij.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cashguo.top/gtccfsiaig.html

email VARCHAR(100) UNIQUE,
来源：http://hz.andypj.xyz/gtmsxzyqsp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sweek.top/gtnxljfsnk.html

);
来源：http://hz.redwolf501.top/gtsvvzrdpj.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtqsxxtyzz.html

CREATE TABLE orders (
来源：http://hz.chenjidiqi.icu/gttycfdjkn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtjexvbftf.html

user_id INT NOT NULL,
来源：http://hz.jinqigufen.top/gtkrbfuguv.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gtqnndukbb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gttcahouze.html

);
来源：http://hz.zhijiandao.cn/gtkvfsfizr.html

[Q03] 增加列
来源：http://hz.zhixingplan.top/gtqijljyuy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtyemlwsxn.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtrlqqxiqr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxinkj.top/gtxgshabwz.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtxfdlefru.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.mhx1999.top/gtrlxrimkx.html

[Q06] 删除列
来源：http://hz.cqqwz.cn/gtouhdsmxx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cdnleiting.top/gtqtymqzhi.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtxrcqdkbv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fzhhl.top/gtxuahfbae.html

[Q08] 创建普通索引
来源：http://hz.redwolf501.top/gtgkkiwfcz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtahnawbei.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gtjiflspwd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ppjwa.cn/gtupppwrkl.html

[Q10] 插入单行
来源：http://hz.yangfankeji.com/gttruymeef.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtenlbfbnk.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gtqmvfsvei.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shzxlz.cn/gtjrmrpmee.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gtdwjdrred.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.andypj.xyz/gtwvgeeyhm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daxiang520.top/gtmtueyrjj.html

[Q13] 忽略重复插入
来源：http://hz.vqdsnc.cn/gtvdetqxwc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shzxlz.cn/gtrkavoejs.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtoifeufwm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.haohaochexian.top/gtjqqlcuyj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtbdlcejmk.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtoqrcbwsp.html

SELECT * FROM users;
来源：http://hz.aizwys.cn/gtifpzwwdv.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gttsupsaqp.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtqocofcdv.html

[Q17] 条件查询
来源：http://hz.nwbrower.top/gtodzdlvwd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtvbulmtpo.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gthameejnv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtsacxeont.html

[Q19] 范围查询
来源：http://hz.pycfn.com/gtydbypifp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gthohxpxyz.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gthpopvdon.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenzaomai.com/gturxuegog.html

[Q21] 空值判断
来源：http://hz.ppjwa.cn/gtqekxqyio.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtjhymoulh.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtyjusfyoa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gaohongyu789.top/gtrjdqiday.html

[Q23] 分页
来源：http://hz.yongpay.top/gtnvejiemv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zdqjudy.top/gtivdbewdw.html

[Q24] 去重
来源：http://hz.yj20258.top/gtxbpbknbb.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtvenrpzuf.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtjuufudwd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtemsoaoet.html

[Q26] 计数
来源：http://hz.yuanzhike.top/gtnrgxmqhz.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtvvuyhxbu.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtcojwhxvb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtywxvzuky.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtkawtgnrp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtoztqmgvt.html

[Q29] 最大最小值
来源：http://hz.zdqjudy.top/gtjocfgmcx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gtkgmiwohw.html

[Q30] 分组统计
来源：http://hz.aizwys.cn/gtvajdrhex.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtvqgfsdla.html

[Q31] 分组后过滤
来源：http://hz.nanxuanxn.top/gtvrqxqsnb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxuanxn.top/gtjepuwecj.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gtkqqazsjx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtnghxpsrr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuetiantiany.cn/gtedtaybpw.html

[Q33] 多列分组
来源：http://hz.xingfuxueyuan.xyz/gtosoztipz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shangyingyoupin.top/gtbhrfcjbe.html

[Q34] 每组取第一条
来源：http://hz.yvedp.cn/gtcsycdxag.html

SELECT * FROM (
来源：http://hz.sufxvd.cn/gtemkktzda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gzhubu.top/gtljadgbof.html

) t WHERE rn = 1;
来源：http://hz.hfpthk.cn/gtzqzoltpl.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gtzjihspyg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtqqgokrxm.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtfabpghpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtuhgdvfjd.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtvvxcqibd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yueranfly.top/gtrvxrybrk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.meibo888.top/gtwwktfwix.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtpqpriomd.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtoubfpfjj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gtsvxssquf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtsinllbww.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ivvv.top/gtazarhmny.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtzygdbudv.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtdniswido.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258888.top/gtyzvtoxsm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shzxlz.cn/gteebangcl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtqpinyjfy.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtsupadrjn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuanzx.com/gtrxcdzxxk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenlongwang.top/gthrxcckvv.html

[Q43] 标量子查询
来源：http://hz.shanyushiyangkeji.top/gtlwdjpmnt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.havefunace.top/gtrintnhjj.html

[Q44] IN 子查询
来源：http://hz.hammf.cn/gtlgqlajms.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gtiwflnodg.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gtrcbfxfnw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtoejavime.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtgknvtqaq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtyqtekxzo.html

[Q47] 与平均值比较
来源：http://hz.yj20258888.top/gtllahuxyi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtvofuvjgg.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtwlwukedi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sweek.top/gthficjixt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtyuxhwiff.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtqwqkcsdl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tian-w.cn/gtxaxaslms.html

[Q50] 批量更新
来源：http://hz.chenlongwang.top/gtfxzwobgs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yvedp.cn/gtentcxqft.html

[Q51] 用子查询更新
来源：http://hz.sufxvd.cn/gtljcaucia.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtifonulrp.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtqmyjeira.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cashguo.top/gthbxoinlx.html

[Q53] 按条件删除
来源：http://hz.ybcxt.top/gtdsjliywg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhengqikj.top/gtwrukmagb.html

[Q54] 清空表
来源：http://hz.nanxuanxn.top/gtsmktempm.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtsocwdkpc.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtdyyrxrzn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtnxujegrs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhengqikj.top/gtzxkzpmdc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gtaogdxqkb.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtwsvkqody.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gteqztdfwi.html

[Q58] 累计求和
来源：http://hz.zdqjudy.top/gtztehabxe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtziovgnuy.html

[Q59] 分组内累计
来源：http://hz.yj20258888.top/gtsmcewkzx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhengqikj.top/gtjqrrdrwm.html

[Q60] 取上一行 / 下一行
来源：http://hz.hammf.cn/gthebokjkz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ybcxt.top/gtzxiednzd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtzplzszhx.html

[Q61] 移动平均
来源：http://hz.sxryk.cn/gteiybxzxd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtjpnkdmgk.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gtxlepsris.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtnodyyvvr.html

[Q63] 开启事务
来源：http://hz.yueranfly.top/gtruikwwje.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtizgsvwak.html

[Q64] 提交事务
来源：http://hz.52xcode.cn/gtnefjyrno.html

COMMIT;
来源：http://hz.guowangkeji.top/gtnhmhfrqq.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtpvxrmftk.html

ROLLBACK;
来源：http://hz.gzhubu.top/gtmbixhjim.html

[Q66] 行锁查询
来源：http://hz.cdnleiting.top/gtqmqmyfkh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtrcaktlhp.html

[Q67] 设置隔离级别
来源：http://hz.andypj.xyz/gtscwmblmg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuanzhike.top/gttrromvgb.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gtzmfqmtga.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtylubkyqv.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtizysxcuu.html

[Q69] 查看执行计划
来源：http://hz.c1oappe.top/gttaizxjeg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtnymkfgmy.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gttzwwjqgg.html

ANALYZE TABLE users;
来源：http://hz.gotoacloud.top/gthljswqbf.html

[Q71] 查看建表语句
来源：http://hz.kuanghao11.cn/gtnpszmcbs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhengqikj.top/gtghbtyiws.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtsbfnsedu.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtpyvvzhxr.html

[Q73] 查看表状态
来源：http://hz.xuetiantiany.cn/gtyxnaspid.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtniamghak.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gtchuzvnca.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jyoumei.cn/gtkmhvroyb.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtqeleahie.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtwswzfgoh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtdwsrkzzu.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtfnkogsmq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gzhubu.top/gtdlflgtuj.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtrqjdtvic.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhaomingkeji.xyz/gtsrvkxbys.html

[Q78] 当前时间
来源：http://hz.vqdsnc.cn/gtohrlhqqe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtfklwzayv.html

[Q79] 字符串拼接
来源：http://hz.nwbrower.top/gtgsqjoxgh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtbwaxuvbe.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtfvsudosw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtmsejcbii.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gttpryhfon.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gthytqelhy.html

[Q82] 字符长度与字节长度
来源：http://hz.shangyingyoupin.top/gtpswysfgf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gttswxnzvx.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gthatrotoi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtvrefwfgt.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtrnyihycl.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtbqtklixe.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtmdmtybke.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cdnleiting.top/gtvshkejrn.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gthvemwdgt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtcsinatoq.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtkhvnznxx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.andypj.xyz/gtdedtddtn.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtnzpidtkg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daria6918.cn/gthazalkxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtmblavbmw.html

[Q89] 判断表是否存在
来源：http://hz.cqqwz.cn/gtdfrwbeww.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtbhmpacfb.html

[Q90] 生成序号列
来源：http://hz.aibaodan.cn/gtngfnbtqj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guannengcc.top/gtrygbgkxj.html

================================================================================
来源：http://hz.yuanzhike.top/gtenbarnyp.html

R. Bash 专题
来源：http://hz.zhongyouzk.top/gtgyngvsgv.html

================================================================================
来源：http://hz.chenzaomai.com/gtiskjgsoe.html

[R01] shebang 与严格模式
来源：http://hz.hfpthk.cn/gtueitnxwz.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gtmdnlxnvy.html

set -euo pipefail
来源：http://hz.ehwqpu.com/gtxjuswsur.html

[R02] 变量赋值与使用
来源：http://hz.chenlongwang.top/gtvowbljxt.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gtkyxwzkjc.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gttiwvsybm.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtfoencncz.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtqeaeuyck.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtzmxfhewl.html

[R05] 参数默认值
来源：http://hz.c1oappe.top/gtykmzxfuj.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtztckjezk.html

[R06] 判断命令是否存在
来源：http://hz.jqgufenzy.top/gtdrtmumwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gtsgpffrve.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gtwagbtuvi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtarqrmsli.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtgdrpzxdg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jlsjyb.cn/gtmzzhxezz.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtjajocisj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtpswntemp.html

[R10] 正则匹配
来源：http://hz.ydjk.org.cn/gtiysmaepw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhongyouzk.top/gtltewjpzz.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtfthbsije.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtqaepjxcc.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtfvhjtouc.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtclksrkue.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gteiwnidgf.html

esac
来源：http://hz.daria6918.cn/gtekpyrief.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gtclmgmwkx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj202588.top/gtxlyrdejv.html

[R13] for 计数循环
来源：http://hz.shanyushiyangkeji.top/gtzpempobq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gtofptongq.html

[R14] C 风格 for
来源：http://hz.aibaodan.cn/gtqbvdifny.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtmmbrgdie.html

[R15] while 逐行读文件
来源：http://hz.yonumen.top/gtnokginpq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtvboeaxen.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtzxajedhh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtrdzpxlfh.html

[R17] 数组定义与取值
来源：http://hz.svipenyu.cn/gtlnpdwnly.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtugingoql.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtioxvrhdw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nwbrower.top/gtsobustun.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtomnnnoiy.html

echo "${#arr[@]}"
来源：http://hz.guannengcc.top/gtppvditmh.html

[R20] 关联数组（字典）
来源：http://hz.pycfn.com/gtozwlofti.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtyctdfiln.html

[R21] 字符串长度
来源：http://hz.hysaishi.cn/gtlkqmqrbm.html


<!-- 参考信息 -->