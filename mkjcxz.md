代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtpjqhkjqu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtwggzjsmc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtvugcpyef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtqpvazksc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hywenlv.cn/gtjsxwirji.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gthiziufsd.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtisrwmmjp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gthbhqhpgs.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gttnhsbrbh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtiyzcepcf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gotoacloud.top/gtzqvwjqyd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gaohongyu789.top/gtmdrwwyyo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigfzy.top/gtimnuuhqk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtlxwhhhmc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtzijqegbt.html

Ruby: a == b
来源：http://hz.52xcode.cn/gtvvvxsizl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gtfzrbdtdz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj202588.top/gtgmfhswfl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yangfankeji.com/gtzzaxruru.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gttqoxlrsa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtfizjyzna.html

TS:   if (x == null) {}
来源：http://hz.ehwqpu.com/gtzvcybado.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtebwjxcdw.html

Go:   if x == nil {}
来源：http://hz.wangshuangyany.cn/gtdkdmxmnl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ivvv.top/gtjviheqhi.html

C#:   if (x is null) {}
来源：http://hz.kuanghao11.cn/gtcrwqfnmr.html

[P07] 防抖与节流
来源：http://hz.hammf.cn/gtgwigijup.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hysaishi.cn/gtbhsmwzrh.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtfdkbncuo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtyvpoujrc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtxmehoxvx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtamuavtot.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yonumen.top/gtwsjgvxbg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtmojnrqyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtrfnfbpwp.html

[P08] 处理浮点精度问题
来源：http://hz.cashguo.top/gtferspfau.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtjsheguzw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangkeji.top/gttworjhpn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gthftmuyxs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangdashe.top/gtrqzvzehg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gaohongyu789.top/gtcsgdncdb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxuanxn.top/gtxuuctyxc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sysykeji.top/gteaghzlee.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aibaodan.cn/gtzvdrdcsk.html

================================================================================
来源：http://hz.jqgfzy.top/gtbacxiuwu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gtxgpfuxgt.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmkpelyvd.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gthlbcdaxf.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtbfsuyymz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtieagroob.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tianlin.xyz/gtjlvmzlsb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtniqwelxl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtbocdfseh.html

);
来源：http://hz.bjfxy.top/gtexbxcuvg.html

[Q02] 创建带外键的表
来源：http://hz.wangdashe.top/gtklswkuov.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gttrqgerbc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gthtorxdjh.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtcnnjbgjw.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtizmtzipv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtxmuemlov.html

);
来源：http://hz.feifeiyinyue.top/gtompyskgw.html

[Q03] 增加列
来源：http://hz.nanxuanxn.top/gtnodwkeos.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tian-w.cn/gturkctjpe.html

[Q04] 修改列类型
来源：http://hz.c1oappe.top/gtzbzdxogy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnxiangtu.top/gtlczluduu.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtlhuuwksk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtjfiggvld.html

[Q06] 删除列
来源：http://hz.tian-w.cn/gtmwswzrjx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtozrlkpuy.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtpoqiueyx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtcaenprmo.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtamrgwbgi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangdashe.top/gtbamctico.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtggxvjvas.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtvpbrpwuq.html

[Q10] 插入单行
来源：http://hz.316326.xyz/gtlmmmlmmq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258888.top/gtstfzjgtr.html

[Q11] 一次插入多行
来源：http://hz.cucudq.cn/gtzmppsxlz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtfhexcadb.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtdqjjgkth.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.0kj1m.cn/gtjuicvsta.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtlznpbyva.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gttaxmijrh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.redwolf501.top/gtzryyrduq.html

[Q14] 存在则更新（upsert）
来源：http://hz.mhx1999.top/gtkrgmyfcx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yonumen.top/gtpzunyocs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xylfe.cn/gtbmrpgylx.html

[Q15] 查询全部
来源：http://hz.quarkkingdee.top/gtzdbyjacx.html

SELECT * FROM users;
来源：http://hz.jinqigfzy.top/gtuocetuhi.html

[Q16] 查询指定列
来源：http://hz.svipenyu.cn/gtuirezryr.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtpdglutup.html

[Q17] 条件查询
来源：http://hz.gotoacloud.top/gtpspnuiiz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gttnfebcdp.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtmktjdmez.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtuyhnheqv.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gtojtujqzr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangshuangyany.cn/gtpkvgjamw.html

[Q20] IN 列表
来源：http://hz.andypj.xyz/gtxjmvcayg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtstusgesq.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtyctspbwu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sysykeji.top/gtkwzgidew.html

[Q22] 排序
来源：http://hz.jqgufenzy.top/gtlormnfea.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pengpengdd.cyou/gthonxpsss.html

[Q23] 分页
来源：http://hz.yangfankeji.com/gtrvzlmedo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtedhxcvrv.html

[Q24] 去重
来源：http://hz.shuidangran.top/gtrxrbisql.html

SELECT DISTINCT city FROM users;
来源：http://hz.316326.xyz/gtmjdjalha.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtkqgdebvf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yueranfly.top/gtjynzinrr.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtbygyftse.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxinkj.top/gthbflqhhg.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtszwukvtq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtxuimimje.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gthpbtlime.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gtokbmqvpi.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtgnsbzpal.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sysykeji.top/gtmeuvwduc.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtisoaxqkh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtvjddaqiz.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtcftwboon.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtfxbhewtb.html

[Q32] 分组拼接字符串
来源：http://hz.xylfe.cn/gtmqrlzxma.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtwsnnwwfs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jyoumei.cn/gtkwtqbclx.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtpfaucvcp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sxryk.cn/gtdkafixkf.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtoeyuteoy.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtnxdmntdm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gtvdltcdel.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtgiilmjeu.html

[Q35] 内连接
来源：http://hz.sxryk.cn/gtdcsupcir.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtvnqkwenb.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gtgsuwfyfk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtcrqmqnzl.html

[Q37] 右连接
来源：http://hz.gzhubu.top/gtjlbmotun.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tanke756.top/gtmbomwvik.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtyrlbjmle.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtmxjsiapw.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258888.top/gtnnygxsso.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cqqwz.cn/gtpyxhorsu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtulmaiwam.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtrcbyrcqo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtvzprgbxj.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtdymjspfo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangtech.top/gtomeglrvr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtzszrwhnh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sysykeji.top/gtpljtezqo.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtepknixhf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtjriunxtj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuanzx.com/gtfvcfatji.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gthckmrdlz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gtuneckfny.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtdquqzstm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnqzz.top/gtswzurgfc.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtzwmgdiah.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtmxlibqef.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtglhsfxtz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtqforfnup.html

[Q47] 与平均值比较
来源：http://hz.ppjwa.cn/gtjowomkhk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xinyue.icu/gtosheyukv.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtcbfzrmpk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtawjrudcs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtcpgachlw.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtuqemfsgb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtkaisdxld.html

[Q50] 批量更新
来源：http://hz.daxiang520.top/gttdmqzbyt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtjumsuxbz.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtuhqjzgki.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shuidangran.top/gtvkrolmjo.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gtdwwnenhl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tanke756.top/gtyeyblggn.html

[Q53] 按条件删除
来源：http://hz.sufxvd.cn/gtjessqimy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtqeokxwht.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtoadgickz.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtcfhptcgr.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtzdelporu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtzsyqsjqa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gthcdhyjtc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtvpytnbnq.html

[Q57] 行号
来源：http://hz.cheryme.top/gtktoryntl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtcxswarnj.html

[Q58] 累计求和
来源：http://hz.zhengqikj.top/gtzwovxbwj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gttsslmjqi.html

[Q59] 分组内累计
来源：http://hz.nanxinkj.top/gtrkhehiri.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenzaomai.com/gtjkdtstcr.html

[Q60] 取上一行 / 下一行
来源：http://hz.sxryk.cn/gtwukvwrir.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtvgiljvkl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aibaodan.cn/gtcztszgcj.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtyvimbcma.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gtnmxacwol.html

[Q62] 分组占比
来源：http://hz.dianchejie.cn/gtxfjwplwo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtpomqdubq.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gtlqvcfnrl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtumlysmny.html

[Q64] 提交事务
来源：http://hz.yueranfly.top/gtmyoztzke.html

COMMIT;
来源：http://hz.hongshengwenyu.top/gtkucfzblp.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtuaqgfrvh.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtptsjnvft.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gtljurxrdo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jianghu66.top/gtjgxkzrok.html

[Q67] 设置隔离级别
来源：http://hz.tanke756.top/gttxtcmtaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.fzhhl.top/gthueyqplm.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gthaclhcph.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtqpygtbga.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtecrtexab.html

[Q69] 查看执行计划
来源：http://hz.xuanzx.com/gteszolxwu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtcocbsull.html

[Q70] 更新统计信息
来源：http://hz.cashguo.top/gtitwtzydc.html

ANALYZE TABLE users;
来源：http://hz.yueranfly.top/gtypawkndn.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gtqbjosqle.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydzc1.top/gtlyhwsrej.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtbgjfzgev.html

SHOW INDEX FROM users;
来源：http://hz.sysykeji.top/gtgcjhyhol.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gtioukrivp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xingfuxueyuan.xyz/gtpmbqyaqg.html

[Q74] 强制使用索引
来源：http://hz.ppjwa.cn/gtcekqyoya.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ppjwa.cn/gtfkqtxhwx.html

[Q75] 日期格式化
来源：http://hz.snrcjt.cn/gtqdsuniuz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtpsjyzalt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.snrcjt.cn/gtcqtvhgzx.html

[Q76] 按天统计
来源：http://hz.hfpthk.cn/gtrbyedzxt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.bjfxy.top/gtiesrbbuu.html

[Q77] 时间加减
来源：http://hz.fengsongda.top/gtonwwkkfi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gttscrbaaa.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gtcgzxfqld.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gtpnvzncxv.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtifmttxtf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtyehcghxx.html

[Q80] 字符串截取
来源：http://hz.daria6918.cn/gtqgjpkfhq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtolkhlphk.html

[Q81] 字符串替换
来源：http://hz.sufxvd.cn/gtzcygvalv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sysykeji.top/gtrokgekck.html

[Q82] 字符长度与字节长度
来源：http://hz.meibo888.top/gtqulbyrbw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gtqahsnjsv.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtiordcxdd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtigaxjssb.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtkrsitupw.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenlongwang.top/gtnmuzygch.html

[Q85] 数值取整
来源：http://hz.jinghuilouyu.cn/gtvndybded.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtjvwjornd.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtqymsvnag.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtmibztzui.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtqowcusnl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigufen.top/gtpuvujdbl.html

[Q88] 行转列（条件聚合）
来源：http://hz.xylfe.cn/gtqykaimbh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhixingplan.top/gtxmrawzoh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hysaishi.cn/gtrrleknuf.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gthjyvmauk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtnusjdtkm.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtovqdgfiv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gthsoaeevk.html

================================================================================
来源：http://hz.jiagoushi.top/gtxkpxpzai.html

R. Bash 专题
来源：http://hz.dianchejie.cn/gtitvwptcr.html

================================================================================
来源：http://hz.xuanzx.com/gteyvunmhc.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtxmixaeot.html

#!/usr/bin/env bash
来源：http://hz.ydzc1.top/gtrzxyshve.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtyxtxbqyr.html

[R02] 变量赋值与使用
来源：http://hz.cqqwz.cn/gtuefchtlj.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtowupfzgu.html

[R03] 只读变量
来源：http://hz.wangshuangyany.cn/gthwibzwxp.html

readonly PI=3.14
来源：http://hz.cashguo.top/gtmyheosml.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtbzsuehax.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dashuyun.cn/gtbcbmjzgg.html

[R05] 参数默认值
来源：http://hz.meibo888.top/gtzcsirppj.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtwxklofky.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtzqwclvbn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gzhubu.top/gtmyhynfax.html

[R07] if 判断文件
来源：http://hz.dashuyun.cn/gtzlrfewht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtxfuoxbck.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gteamkgdmm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gtkuekuyho.html

[R09] 字符串比较
来源：http://hz.shanyushiyangtech.top/gtroebsdyj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtiuxxdcfo.html

[R10] 正则匹配
来源：http://hz.jiagoushi.top/gttkoauuwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.0kj1m.cn/gtgkrwnysv.html

[R11] case 多分支
来源：http://hz.sweek.top/gtdfxqbrox.html

case "$1" in
来源：http://hz.xziqi.cn/gtdoggskyw.html

start) echo "启动" ;;
来源：http://hz.xuetiantiany.cn/gtydffkzjg.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtdgngopwp.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtixtukime.html

esac
来源：http://hz.snrcjt.cn/gtyttmttpd.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtuquykmdt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gtitwznjtt.html

[R13] for 计数循环
来源：http://hz.yvedp.cn/gtvsvezbjm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtwhqeriut.html

[R14] C 风格 for
来源：http://hz.zdqjudy.top/gtjbcljbdd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgfzy.top/gtsbgegkyo.html

[R15] while 逐行读文件
来源：http://hz.chenjidiqi.icu/gtvltxpmdz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtccsulydm.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtzbpauasy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtacjfkyba.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtlcgtwknt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtijgkjjmq.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtkrkuypyh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtfpjrtuwe.html

[R19] 数组长度
来源：http://hz.svipenyu.cn/gtyjlanilc.html

echo "${#arr[@]}"
来源：http://hz.xingfuxueyuan.xyz/gtltscwetf.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtszdotbui.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtvlsnxjsy.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gttadbognm.html


<!-- 参考信息 -->