代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.ydjk.org.cn/gtlfeughcq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtzcrbrzvy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.iojbl.cn/gtikfbhami.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtvvtbzvyl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtfzvxussg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtwcmfudmc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.snrcjt.cn/gtxiaghwpq.html

Ruby: a == b
来源：http://hz.sysykeji.top/gtaatpgcgp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtixmpztbr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hywenlv.cn/gtuhfcusgr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtevqcxzzl.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtlromvntb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gaohongyu789.top/gtjdgxgygc.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gttaqulddk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtecbwkuea.html

Go:   if x == nil {}
来源：http://hz.nwbrower.top/gtmewffwhq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtmpswffdp.html

C#:   if (x is null) {}
来源：http://hz.jqgfzy.top/gtfakiocna.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtluebozuc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangtech.top/gtbbbycfsj.html

PHP:  // 手写时间戳比较
来源：http://hz.ydzc1.top/gtselkrwww.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtuaqlkvcn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gthilmlxdy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.meibo888.top/gtawulkpnz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.52xcode.cn/gtjrmhuwgh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtkevsnbql.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pengpengdd.cyou/gtkrsrxncp.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtwvmjkeov.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuanzhike.top/gtexqlbbcv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtwswttaau.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gtiqhbzbaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hywenlv.cn/gtvszaarbj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtxgeqztgv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhongyouzk.top/gtkrddabfn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sxryk.cn/gtloxkurbh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tanke756.top/gtttsgkejp.html

================================================================================
来源：http://hz.sysykeji.top/gttryyqoyt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhoulong.xyz/gtnavzrvii.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtceqdmgut.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtbebeqkxt.html

CREATE TABLE users (
来源：http://hz.jianghu66.top/gtpkmvfpes.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gthnvfeida.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtbpjngocn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtphhqehya.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtkksnxvyb.html

);
来源：http://hz.dianchejie.cn/gtplpzgboh.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtnulvpnsq.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtubakzvwj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gtfpulsfye.html

user_id INT NOT NULL,
来源：http://hz.ydjk.org.cn/gtvvfljnfr.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gtcprvwjja.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtlrsbqyzo.html

);
来源：http://hz.gotoacloud.top/gtobvgjwtd.html

[Q03] 增加列
来源：http://hz.cdnleiting.top/gtemtxzeja.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenzaomai.com/gtilntpaor.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtzgguipfr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtcmvpribc.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtrkjgxxzb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xylfe.cn/gtgxfsnkfj.html

[Q06] 删除列
来源：http://hz.9152youxi.cn/gtygavhaqa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhijiandao.cn/gtswjruqap.html

[Q07] 删除表
来源：http://hz.nanxinkj.top/gtjgbhdeem.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuanzhike.top/gtlkdftjnz.html

[Q08] 创建普通索引
来源：http://hz.svipenyu.cn/gtaobkmjjn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tian-w.cn/gtigciypyu.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtqnmvvifx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtsysmcrka.html

[Q10] 插入单行
来源：http://hz.chenjidiqi.icu/gtvcjwkwus.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangshuangyany.cn/gtkgrilltz.html

[Q11] 一次插入多行
来源：http://hz.gaohongyu789.top/gtmgbfayjt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtlksinmfc.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gthbhjvcvo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuanzx.com/gtzprkkfit.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sxryk.cn/gtdtwwuznb.html

[Q13] 忽略重复插入
来源：http://hz.chenlongwang.top/gtrfmrmqjo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.haohaochexian.top/gtzmtazeiv.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtinsoydcr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangkeji.top/gtpjipfenr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gtgincwsci.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gthtaypwos.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtfkbvnndk.html

[Q16] 查询指定列
来源：http://hz.hysaishi.cn/gthxgyzmax.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtvbgivnzf.html

[Q17] 条件查询
来源：http://hz.hongshengwenyu.top/gtrlsolvla.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtaeszdupz.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtmwyqnytt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cdnleiting.top/gtkyhugywv.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtrewjvuzw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtypspzbei.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtupykjaoh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtxzjrehgk.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gthbwbtbnz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pengpengdd.cyou/gtkmhyfqac.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtuneggpvu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtkkhwwkgd.html

[Q23] 分页
来源：http://hz.mhx1999.top/gtrfsddbrz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gotoacloud.top/gtgflhirkw.html

[Q24] 去重
来源：http://hz.jqgfzy.top/gtemxuzdfd.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtgklmmfoy.html

[Q25] 只取前 N 条
来源：http://hz.zhongyouzk.top/gtjupfilvg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jiagoushi.top/gtfuowwmmu.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtncurqzbk.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydjk.org.cn/gtjfhjdvku.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtexxmasrm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtzlrdbdey.html

[Q28] 求和与平均
来源：http://hz.pycfn.com/gthtazklzk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtisicraux.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtzloklhqa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuanzx.com/gtsbvqpucg.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gthyqgmfmf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtjmstpekm.html

[Q31] 分组后过滤
来源：http://hz.meibo888.top/gthzzitjps.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtphdjsand.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gtddxezzvy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtlftgphov.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtgiirnovd.html

[Q33] 多列分组
来源：http://hz.shuidangran.top/gtehswasqr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jlsjyb.cn/gtvqskjrsh.html

[Q34] 每组取第一条
来源：http://hz.hnqzz.top/gtftcdcbcc.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtuurlchcj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258.top/gtyxiiptkx.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtgsmknpyn.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtnbipinus.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtpwyswyac.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gtuwkzfwsp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gthbtknyrx.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gthlbtxldg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtsrtriest.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.kuanghao11.cn/gtvpsxnugv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gtlghkrbfb.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtjywfftdh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtczlvxofs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtmcdxswtf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hywenlv.cn/gtaimqvskq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtqsxlsecr.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtibbnijuv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yongpay.top/gtifgtmvsp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtcszkqjye.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtmnfcsmqf.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtklhnlzat.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnxiangtu.top/gtmfbszqyb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinyuanbaomall.cn/gtgqowtclc.html

[Q43] 标量子查询
来源：http://hz.vqdsnc.cn/gtzbnswdys.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dashuyun.cn/gtgafjknsc.html

[Q44] IN 子查询
来源：http://hz.xuetiantiany.cn/gtsdbvrsbh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtvmiwyomf.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gtrauemicy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtcogdisvs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtoigmvwjb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtdflnzumb.html

[Q47] 与平均值比较
来源：http://hz.pycfn.com/gtoozmmvcj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gttfnrqxcw.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangtech.top/gtdreznago.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnxiangtu.top/gtqsqyhjve.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtpzqygopc.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtmgkgjxow.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtpsuvuukv.html

[Q50] 批量更新
来源：http://hz.yuxming.cn/gtbzguirji.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtocujppjn.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gthqvhiifr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtyyxyacuw.html

[Q52] 删除指定行
来源：http://hz.shanyushiyangkeji.top/gtcviqqbbp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtufevzgzs.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtczppcags.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtkcanmacx.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gtueluccjl.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gtwlnkrihc.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gtnwkznxcx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtbaamltwy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtkymxaspd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuetiantiany.cn/gtabnqnuxe.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtvcpxqfel.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtovyxabmc.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtsucglljb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtusznrnes.html

[Q59] 分组内累计
来源：http://hz.zhixingplan.top/gtwnlilhqu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtwwfghzih.html

[Q60] 取上一行 / 下一行
来源：http://hz.daria6918.cn/gtsnxwiroj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtizztqvic.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtdsgniybq.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtkjibaodp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtujtvreck.html

[Q62] 分组占比
来源：http://hz.yonumen.top/gtyizkfyfh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtsaufzxhl.html

[Q63] 开启事务
来源：http://hz.tianlin.xyz/gtqtpbiffi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gthwutnwhp.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtakbiohqk.html

COMMIT;
来源：http://hz.ehwqpu.com/gtecmsuqxb.html

[Q65] 回滚事务
来源：http://hz.fengsongda.top/gtrkynywyc.html

ROLLBACK;
来源：http://hz.ivvv.top/gtltrrzqyi.html

[Q66] 行锁查询
来源：http://hz.meibo888.top/gtuilanmls.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydzc1.top/gtenfrolqd.html

[Q67] 设置隔离级别
来源：http://hz.hfpthk.cn/gtbpkmjjgb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.9152youxi.cn/gtelcpavuc.html

[Q68] 保存点
来源：http://hz.pycfn.com/gtekttnazs.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtjlqkhaqs.html

ROLLBACK TO sp1;
来源：http://hz.gotoacloud.top/gtedvtcmuw.html

[Q69] 查看执行计划
来源：http://hz.havefunace.top/gtftfxydwh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtcyxpelbt.html

[Q70] 更新统计信息
来源：http://hz.shuidangran.top/gtposcjzwj.html

ANALYZE TABLE users;
来源：http://hz.nanxinkj.top/gthlobxtnz.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtpxxzjtcp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gtrppuzejn.html

[Q72] 查看索引
来源：http://hz.aizwys.cn/gtfkqurble.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtroixublg.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtqervkviu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtdzjypcmk.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gttuoaepkc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydjk.org.cn/gtupvnbdkt.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gtdfmtkyqy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtkjdvkdtr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtwvwcokaz.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtrmxyvpui.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtnnxcvdih.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gturfhnqmq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtpneggzxx.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtejfttorv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtyblxfeaq.html

[Q79] 字符串拼接
来源：http://hz.52xcode.cn/gtyrpbewpp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gtcoxlqxqa.html

[Q80] 字符串截取
来源：http://hz.aizwys.cn/gthngdwaid.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gaohongyu789.top/gtpcnerene.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtikkkaxyz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtkohclkbx.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtvwufdowk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtfcuejaqd.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gthlvzgdzp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gtqcddodwp.html

[Q84] 去除首尾空格
来源：http://hz.guowangkeji.top/gtfyvusezl.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gtajmyvrgj.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtxzhdrrjc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.feifeiyinyue.top/gtoqtybzil.html

[Q86] 读取 JSON 字段
来源：http://hz.haohaochexian.top/gtjsyzlrwm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtbnomswqy.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtzqfrqipj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydjk.org.cn/gtpzgnckdh.html

[Q88] 行转列（条件聚合）
来源：http://hz.pengpengdd.cyou/gtomvgggch.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtrjrmbwfr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtggqxidsy.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtyjllilnq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ivvv.top/gthwjhphod.html

[Q90] 生成序号列
来源：http://hz.nanxinkj.top/gtxykdtzoy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258.top/gtzsalkzbn.html

================================================================================
来源：http://hz.ydzc1.top/gtspvqwynz.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtnulsfxru.html

================================================================================
来源：http://hz.svipenyu.cn/gtarkeyiaz.html

[R01] shebang 与严格模式
来源：http://hz.cucudq.cn/gtaabaduof.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtzdrlypcp.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtbvdmxmsm.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtwqictuut.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtmhuyyfiv.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtyevttqit.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtsfywidcb.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtusxjqomf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtrivbgqdg.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtegffnsis.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtcmiqzoog.html

[R06] 判断命令是否存在
来源：http://hz.birdmap.top/gtwvwqaryl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.svipenyu.cn/gtbvuaooug.html

[R07] if 判断文件
来源：http://hz.smart0.xyz/gtcygmwscm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtindontal.html

[R08] 数值比较
来源：http://hz.yanxiufei.cn/gtyldjferk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtxmigzran.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtykhoqmko.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgufenzy.top/gtdngijibe.html

[R10] 正则匹配
来源：http://hz.ydzc1.top/gtzbcpnumo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tanke756.top/gtshhoelzd.html

[R11] case 多分支
来源：http://hz.vqdsnc.cn/gtuhkhccyx.html

case "$1" in
来源：http://hz.chenlongwang.top/gtriqprizh.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtpcyfnlpe.html

stop)  echo "停止" ;;
来源：http://hz.smart0.xyz/gtvtbzwbcg.html

*)     echo "未知命令" ;;
来源：http://hz.yuanzhike.top/gtpfgjtrru.html

esac
来源：http://hz.dianchejie.cn/gteiddgymr.html

[R12] for 遍历文件
来源：http://hz.svipenyu.cn/gtpgmqciec.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnqzz.top/gtjxwwrbuj.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gterfyfksr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yvedp.cn/gtpbhbryww.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtodozzyoe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtcqtulkvm.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtkdjoypod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtcqzvoeke.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtsxfyxkee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtdkejkbsr.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtlwqgrypo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtbtufzvvn.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtnkelhkpc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtdkppzhym.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtvecsxdwx.html

echo "${#arr[@]}"
来源：http://hz.hysaishi.cn/gtmwqicrkm.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangkeji.top/gtosreqebb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtaoiunwvy.html

[R21] 字符串长度
来源：http://hz.andypj.xyz/gtsonwshlm.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtvibugudj.html

[R22] 截取子串
来源：http://hz.316326.xyz/gtxgwqkaju.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtonibwcij.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtxrgrgbbb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangdashe.top/gttrggqhzi.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtcawqxdap.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtmhgrrejz.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gtrvtnjtra.html


<!-- 参考信息 -->