代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.hnqzz.top/gtwezwodzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jlsjyb.cn/gtodcawfkf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtewhfnsbu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtooabiwnm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxuanxn.top/gthsgyjzqb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhoulong.xyz/gtmnbffnhx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtvuolskof.html

Ruby: a == b
来源：http://hz.9152youxi.cn/gtffbxkxtb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtohfywndf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.mhx1999.top/gtbvcemojh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gtenmvzogl.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gthjcyibdy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yonumen.top/gtqtvlyxyf.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtjmojtqcu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258888.top/gtgckgiuyx.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtnucaifmy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgufenzy.top/gtrinhoagf.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtdleyqwea.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtjevaukww.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fzhhl.top/gtpmkkxkpt.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtmoligjfm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtjklaoenh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gthnjevqza.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gtxpvtvzzs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ybcxt.top/gtbbdpcxuc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtjgnegndl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtkfmchegx.html

[P08] 处理浮点精度问题
来源：http://hz.hnqzz.top/gtmckibgfr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gteiamxyhs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.feifeiyinyue.top/gtoiqzckbz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtlmiwrqyt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj202588.top/gtfzcvhgkd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.9152youxi.cn/gtjtqduaut.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtcbnncrbm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtucmwchqh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydzc1.top/gtuovebgys.html

================================================================================
来源：http://hz.shuidangran.top/gtpfhhlldh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxuanxn.top/gttueapllh.html

================================================================================
来源：http://hz.gotoacloud.top/gtkkwqhcrd.html

[Q01] 创建表
来源：http://hz.gogol.net.cn/gtqkntiazq.html

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtreshhzew.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtdzdbbqsj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtcwyickhx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.bjfxy.top/gtthbpdyhw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gtcvkojjay.html

);
来源：http://hz.chenjidiqi.icu/gtbagorjvx.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtepydfwai.html

CREATE TABLE orders (
来源：http://hz.52xcode.cn/gtjvufuugs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtpwoinqaa.html

user_id INT NOT NULL,
来源：http://hz.fzhhl.top/gtqzfwqnwf.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtfudidtsb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtqcixjcho.html

);
来源：http://hz.yj20258.top/gtdpafpqgv.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtglrsjzvd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinyuanbaomall.cn/gtepufvlfz.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtpbaeynpg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gtglticyrx.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtqbxyusvg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shzxlz.cn/gteracbqoq.html

[Q06] 删除列
来源：http://hz.hongshengwenyu.top/gttloehnzd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shuidangran.top/gtxveooevm.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtewoccebx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gttgnkpixg.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gthuanmgcc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj20258888.top/gtwqvcmpph.html

[Q09] 创建唯一索引
来源：http://hz.yuxming.cn/gtfzlarcbr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fengsongda.top/gtrtdwjuwk.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtdiupbxow.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtzqgjutyn.html

[Q11] 一次插入多行
来源：http://hz.xylfe.cn/gtrrxyzblq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gteijpzdvj.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtuuduurhb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtcibabcld.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtzskxwjzz.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtmxdiwgvu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtqrxsxtsj.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtukdykvcd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtasnqypgz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gtusauwery.html

[Q15] 查询全部
来源：http://hz.c1oappe.top/gtpozrwxvy.html

SELECT * FROM users;
来源：http://hz.shzxlz.cn/gtghnykdmh.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtfvuqqglr.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtmgyylzvk.html

[Q17] 条件查询
来源：http://hz.xuanzx.com/gtlxrmuvkp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigfzy.top/gtwhcshbky.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangkeji.top/gtjbdmrtuu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yvedp.cn/gttqhmqlzx.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtohsrohay.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gtftkcddhy.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtxbxrjznb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtmadfzvkr.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gtwygxtdkj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gthpakffey.html

[Q22] 排序
来源：http://hz.jlsjyb.cn/gtpsrzridu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.feifeiyinyue.top/gtqepfcgkz.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtelywobmj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtyvpgxjmr.html

[Q24] 去重
来源：http://hz.ivvv.top/gtexniovhq.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtbkskvunf.html

[Q25] 只取前 N 条
来源：http://hz.vqdsnc.cn/gtxywzfdhb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zycfv.cn/gtneowxmae.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtavwpejzs.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtptozpcun.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gteqyozmfm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtlqiqgapv.html

[Q28] 求和与平均
来源：http://hz.jqgufenzy.top/gtvewvskvm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.quarkkingdee.top/gtwndplfet.html

[Q29] 最大最小值
来源：http://hz.ehwqpu.com/gtywkejnwi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuetiantiany.cn/gtjtfcbupp.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtnpzieirs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtvybfttxz.html

[Q31] 分组后过滤
来源：http://hz.chenzaomai.com/gthgpstjpy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtmxfyxvzp.html

[Q32] 分组拼接字符串
来源：http://hz.bjfxy.top/gtwkrrjghc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gttcwtvbff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtmvlyvslx.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gtufgbxsof.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtpytunzbz.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gthgwccqqi.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtxbxsdwma.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtpezsxyev.html

) t WHERE rn = 1;
来源：http://hz.bjfxy.top/gtqaqizdlv.html

[Q35] 内连接
来源：http://hz.xuetiantiany.cn/gtafripzdg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtiybjeojz.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtnluvtfzt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtwxihbpnw.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gtnxxywqbe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gzhubu.top/gtzirvqkza.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gzhubu.top/gtqhtolqfu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtwmcaowfr.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangkeji.top/gtqmfzrqjc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtigqebewj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.mhx1999.top/gtqmegkxjt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gtdazcqxfc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtfclvjmhz.html

[Q41] 多表连接
来源：http://hz.ydzc1.top/gtsfwoqfsx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yangfankeji.com/gtudlsxbyb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtlcuyueqg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtchppyjuf.html

[Q42] 连接条件附加过滤
来源：http://hz.zhiwuduotai.top/gtlhnoigob.html

SELECT u.name, o.amount FROM users u
来源：http://hz.birdmap.top/gtcoqbzfbm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxinkj.top/gtdoayihvt.html

[Q43] 标量子查询
来源：http://hz.nanxuanxn.top/gttsvpzjkp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cucudq.cn/gtsygndupn.html

[Q44] IN 子查询
来源：http://hz.jlsjyb.cn/gtlpkkdoxn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.mhx1999.top/gttrzjtacc.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtnwgapuhh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtkeanrwpu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtwlduxacd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtmxpzpxhd.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtfqjwvebo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtaqccbeak.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtohumnsos.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gttyuupdnu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gogol.net.cn/gtvxjbktcx.html

[Q49] 更新单行
来源：http://hz.yj20258888.top/gtgtfqajjn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtwpxzzpyt.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtotrdkxcd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangshuangyany.cn/gtbsneqzjl.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtrnckzipf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtdjeenzpa.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtydqyrsua.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ivvv.top/gtivfdcqbv.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtjbuednlw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.bjfxy.top/gtcewclhxk.html

[Q54] 清空表
来源：http://hz.gaohongyu789.top/gtdgiowufo.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtrsqqegvz.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtpvkjgnlt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258888.top/gtpcksauoc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtpfnsltmj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.smart0.xyz/gtagnrwpft.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gtmixqhwnj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtvpgxtvyp.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtysceiipa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtargfwniv.html

[Q59] 分组内累计
来源：http://hz.hfpthk.cn/gtobbhxswo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtokbehitk.html

[Q60] 取上一行 / 下一行
来源：http://hz.tianlin.xyz/gtpdxsunvh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtwqfhkbuf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtoamxflgj.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtmfmkurxj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtviitdzzm.html

[Q62] 分组占比
来源：http://hz.0kj1m.cn/gtjjabslwz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gttokfaayb.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gteeacbyoz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtxtojovsi.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtsebepegr.html

COMMIT;
来源：http://hz.zhixingplan.top/gttlpbikdh.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtelbasbkm.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtpbqeffvu.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtftadljwl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.316326.xyz/gtgvhqnlvh.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gthyqjbmxv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtplxhzymm.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtjrmtbcai.html

SAVEPOINT sp1;
来源：http://hz.cqqwz.cn/gtiuzqgyiy.html

ROLLBACK TO sp1;
来源：http://hz.cdnleiting.top/gtzwusejmu.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtxxnujdmr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daxiang520.top/gtmrqgdfre.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtfmnvczzh.html

ANALYZE TABLE users;
来源：http://hz.316326.xyz/gtmjmyitgj.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gtrzoewhuo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtplrxpwxs.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtwdndbotg.html

SHOW INDEX FROM users;
来源：http://hz.0kj1m.cn/gtzjvuwnvu.html

[Q73] 查看表状态
来源：http://hz.zhengqikj.top/gtzmldresi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtmlnfgtla.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gthnuzrpxi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daxiang520.top/gtuijhdiwh.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtzydjoieu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zycfv.cn/gttylfqwyz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtmwyiriyr.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtamnlfowd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yanxiufei.cn/gtoujowrcn.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtizbbxuug.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.0kj1m.cn/gteoomzcfz.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtyhyopeow.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ehwqpu.com/gtlzjavlzf.html

[Q79] 字符串拼接
来源：http://hz.chenlongwang.top/gtrvmkqegd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhoulong.xyz/gtuxysfcar.html

[Q80] 字符串截取
来源：http://hz.daria6918.cn/gthjkbeuyn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtwngyqxfz.html

[Q81] 字符串替换
来源：http://hz.wangshuangyany.cn/gtyvkyyxil.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gtiisqrtdp.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgfzy.top/gtrrzercue.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yueranfly.top/gtbbeyaucr.html

[Q83] 大小写转换
来源：http://hz.jlsjyb.cn/gtevrgcnac.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydjk.org.cn/gtyqwekibs.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtllijpdro.html

SELECT TRIM(name) FROM users;
来源：http://hz.c1oappe.top/gtubrjthzb.html

[Q85] 数值取整
来源：http://hz.jqgufenzy.top/gtovvzigje.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtmoetchgr.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtanswdsem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtldbicmwz.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtwuvuhgoo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtwjajcfok.html

[Q88] 行转列（条件聚合）
来源：http://hz.kuanghao11.cn/gtnhlkhfin.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydjk.org.cn/gtugbvkgoh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydjk.org.cn/gtzwnjwjaj.html

[Q89] 判断表是否存在
来源：http://hz.cqqwz.cn/gtzqhynfmt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dianchejie.cn/gtqsqohihy.html

[Q90] 生成序号列
来源：http://hz.hnqzz.top/gtbwhbfwfy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gteyohozfk.html

================================================================================
来源：http://hz.guowangkeji.top/gtschezfrp.html

R. Bash 专题
来源：http://hz.gaohongyu789.top/gtkmlevgur.html

================================================================================
来源：http://hz.tian-w.cn/gtpwegstua.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtabrdermh.html

#!/usr/bin/env bash
来源：http://hz.jinyuanbaomall.cn/gtbjncfnyf.html

set -euo pipefail
来源：http://hz.shanyushiyangkeji.top/gtykglsevg.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtwsgsjpri.html

name="Tom"; echo "$name"
来源：http://hz.zhongyouzk.top/gtmhchpmaj.html

[R03] 只读变量
来源：http://hz.daxiang520.top/gtxbooubuk.html

readonly PI=3.14
来源：http://hz.nwbrower.top/gtadaqcbpm.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtdtkbumjj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gtkxyuczvt.html

[R05] 参数默认值
来源：http://hz.yj20258.top/gtfsqlwetq.html

name="${1:-default}"
来源：http://hz.jyoumei.cn/gttectthon.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtwlcrbkkm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cucudq.cn/gtwniuwira.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtuozbbdqh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtzmkjkbfe.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gtfpktdatl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtudglhcvn.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gttgedzyrx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fzhhl.top/gttljsnvvv.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtwtzpygmq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigfzy.top/gtjtbssfwh.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtrbynnmhq.html

case "$1" in
来源：http://hz.smart0.xyz/gtpjbxgrbj.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtprcjxagu.html

stop)  echo "停止" ;;
来源：http://hz.birdmap.top/gtrxmevjla.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gthnusmjon.html

esac
来源：http://hz.tian-w.cn/gtftmbekrc.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gttmpxsdaa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tianlin.xyz/gtvizwdmdx.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtqktlhera.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hfpthk.cn/gthszcjqyl.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtvhwcwvld.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtwtdptifg.html

[R15] while 逐行读文件
来源：http://hz.yj20258888.top/gtomdhgely.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.bjfxy.top/gthpnzotbk.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtmgqhkjew.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gtxjtltibk.html

[R17] 数组定义与取值
来源：http://hz.cashguo.top/gtpdfrlxsq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtzqfntzni.html

[R18] 遍历数组
来源：http://hz.xziqi.cn/gtjuallbvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtgftwaghq.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtjzvekauq.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtutccygfz.html

[R20] 关联数组（字典）
来源：http://hz.cashguo.top/gtgmyyipvt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtxxrcyyti.html

[R21] 字符串长度
来源：http://hz.yuxming.cn/gtllkaftro.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtxavleegg.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gttrsiirtz.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gtnswhayeu.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtolrvqnid.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gticjrptkq.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtwegwmfjc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yuanzhike.top/gtiuayxcnt.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtapqttzyh.html


<!-- 参考信息 -->