代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tian-w.cn/gtmysqnehr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gttpcnmrgm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtydfkrjvp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtrgadlrbr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtvanymbwu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.meibo888.top/gttqwqvbar.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtwxmsalog.html

[P04] 求长度
来源：http://hz.xylfe.cn/gtiqbhcojy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yueranfly.top/gtgnrgnfcn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtfdqjgptg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtvlvmooem.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jiagoushi.top/gtipafsbyw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shuidangran.top/gtnlitchht.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gtkqjrihoo.html

Ruby: x.length;  x.size
来源：http://hz.yonumen.top/gtetgcbdsj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gtumucbktf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jiagoushi.top/gtsemmmisr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zycfv.cn/gtglsaovbf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gteozadjwy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhijiandao.cn/gthgxgjuwi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtguvmmslm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daria6918.cn/gtysgkzzik.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yongpay.top/gtroiogbiz.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtezfigkyw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.quarkkingdee.top/gtcgcpkgqk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gaohongyu789.top/gtfigoojdz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.0kj1m.cn/gtsedjdxvf.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtileoqdto.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yongpay.top/gteqylshjt.html

TS:   if (x == null) {}
来源：http://hz.jiagoushi.top/gtvypcglpq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtqachrqrl.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtwnrusbep.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtovtjdfjl.html

C#:   if (x is null) {}
来源：http://hz.jinqigufen.top/gtldkwvkrr.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gttviejszj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtrskaxccc.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtrqksysql.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtpwrjsnrh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtmgxrqewe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtvvuzitzt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gthcamhqhx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtjojiyvim.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtbpbfkekv.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtevxgztzd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shzxlz.cn/gtnkybcjvt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yuanzhike.top/gtwgotbmbp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pengpengdd.cyou/gtmykvpuvn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.52xcode.cn/gtwsmvqtcm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtpslyteuz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtyqvosips.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtaeskjmgn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yangfankeji.com/gtdxxcncvx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfrtzgyxu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigfzy.top/gtamgvxvub.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbtuhwtwu.html

[Q01] 创建表
来源：http://hz.meibo888.top/gtnqgcxztx.html

CREATE TABLE users (
来源：http://hz.hnxiangtu.top/gtmdealgrh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtmvfpjpmf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.birdmap.top/gtsdqablbs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yueranfly.top/gtpnfcipxb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.mhx1999.top/gtvnywoisx.html

);
来源：http://hz.jinghuilouyu.cn/gtktdfiywz.html

[Q02] 创建带外键的表
来源：http://hz.jinqigufen.top/gtduaofnxt.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtksxrzzxr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtocwwnfxj.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtoclsephh.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtaqobfoqx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.0kj1m.cn/gtblalqzzt.html

);
来源：http://hz.xingfuxueyuan.xyz/gtqazmfzds.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtoapsudrg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tian-w.cn/gtpmkpzeds.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtinxbttda.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.9152youxi.cn/gtdokpbafn.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gthzyscryl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtgqqqrncp.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gtidqhnjkz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gtzagsvzrz.html

[Q07] 删除表
来源：http://hz.hfpthk.cn/gtyljntusf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtliowxgbv.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtokmenhyw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.havefunace.top/gtjwwicwou.html

[Q09] 创建唯一索引
来源：http://hz.yj20258888.top/gtqbpdhpfj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zycfv.cn/gtcikrbreg.html

[Q10] 插入单行
来源：http://hz.ivvv.top/gtuwcevcdn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gthpwwbvng.html

[Q11] 一次插入多行
来源：http://hz.ybcxt.top/gtmfjcsrkn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xinyue.icu/gtfpjedsnd.html

[Q12] 插入后取自增 ID
来源：http://hz.dianchejie.cn/gtcihjoiyh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gtpxynzyym.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ivvv.top/gtqpvtlthl.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtcmsijaop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtswpnwzze.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtdhkcparo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ywan-chungtsiang.top/gtdbnnxqkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.havefunace.top/gtduuehswi.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtyrxqzwhh.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtwcsyekmc.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gtlcbkuazt.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtmuorohql.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtoihroarv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yvedp.cn/gtsnjgclos.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtbdkvcwor.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cdnleiting.top/gtktyaiemw.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtucuaprai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtmszqvzlm.html

[Q20] IN 列表
来源：http://hz.svipenyu.cn/gtjfbxhzxq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtpegfsjnk.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gtcdmwitks.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fengsongda.top/gtvzayheea.html

[Q22] 排序
来源：http://hz.sysykeji.top/gtdaxtaeoc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gtbklctfqo.html

[Q23] 分页
来源：http://hz.wangdashe.top/gtuzkhercn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258888.top/gtrtqzukad.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtqvmbubhe.html

SELECT DISTINCT city FROM users;
来源：http://hz.xylfe.cn/gtycjqdqkn.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtpaloenhx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtixmfkydy.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gtzysubwxw.html

SELECT COUNT(*) FROM users;
来源：http://hz.shangyingyoupin.top/gtigdqpmqr.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gtjnotjivm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gtlznposln.html

[Q28] 求和与平均
来源：http://hz.iojbl.cn/gtzgcafglk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtfjtnyaec.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtoognotfg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.kuanghao11.cn/gtcyaupmtp.html

[Q30] 分组统计
来源：http://hz.xinyue.icu/gtmsykofou.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtzyazpdel.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtizdtiglh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.fengsongda.top/gtsomajswg.html

[Q32] 分组拼接字符串
来源：http://hz.xziqi.cn/gtrgtibiwg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtotpyprsy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gttzugaoqx.html

[Q33] 多列分组
来源：http://hz.chenjidiqi.icu/gtbjwxquje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dashuyun.cn/gtjjdaearo.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gtejjgqwyd.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtniuapudz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtvprmnusl.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtwawhiaer.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtzimpecod.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtlwqoesqv.html

[Q36] 左连接
来源：http://hz.jqgfzy.top/gtnnlkpcnf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtofrejjfr.html

[Q37] 右连接
来源：http://hz.jyoumei.cn/gtyrceodvm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtlezrlakd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtdaqobxrh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtztbbspyn.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gtymrgkvrh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pycfn.com/gtluuutguo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nwbrower.top/gtnufsztsc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtprlgffrc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinyuanbaomall.cn/gtmzknbuak.html

[Q41] 多表连接
来源：http://hz.316326.xyz/gtbdmhrhkb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydzc1.top/gtwebxodrr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtncwivqpe.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tanke756.top/gtqyhorhsd.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gttzbgsqpw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ppjwa.cn/gtvsgutpgj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.quarkkingdee.top/gtblbaludd.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtjobmhjod.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gttbefstvn.html

[Q44] IN 子查询
来源：http://hz.0kj1m.cn/gtnfajqzeq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnqzz.top/gttjbfkdrz.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtqcokguye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtsabxxjrw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gthxkgncir.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtrvzdlipl.html

[Q47] 与平均值比较
来源：http://hz.cdnleiting.top/gtshfylzfr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtdeliarkw.html

[Q48] CTE 公用表表达式
来源：http://hz.shzxlz.cn/gtfpdarjdq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuanzx.com/gtufnjvjim.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtbvfdotzv.html

[Q49] 更新单行
来源：http://hz.sysykeji.top/gtcknyxuzv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhengqikj.top/gtkdhdjuue.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtnsbnxvoj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gtttnpjcfv.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtrkmklkct.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sweek.top/gtdoclsiob.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gtxmbehdnm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtbegknxgh.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtefejabro.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pengpengdd.cyou/gttvknfblv.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtprkirmlp.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gtwoprkxac.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtubvzjhbw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtqdxmezai.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtzoutvwpt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangtech.top/gthzqsdtlm.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtwoptksfj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtpgoxsxfo.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtkxjgayjv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gtwwasvwzh.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtxqzjwezm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtkzuvixhi.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtzokjlqnx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yonumen.top/gtscqyvitx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.snrcjt.cn/gtczqoyjzy.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gtluxrroca.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtointipqf.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gtfsivamlx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtoomqifym.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gtbofmheib.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yangfankeji.com/gttelfbxjr.html

[Q64] 提交事务
来源：http://hz.jqgufenzy.top/gtmdcyujks.html

COMMIT;
来源：http://hz.daxiang520.top/gtxqevkjto.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtnbsekgrx.html

ROLLBACK;
来源：http://hz.zhongyouzk.top/gtnjptyenr.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gtrtyxgjem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shzxlz.cn/gtkiqugcea.html

[Q67] 设置隔离级别
来源：http://hz.daxiang520.top/gtixwcdiue.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtgyxyltbm.html

[Q68] 保存点
来源：http://hz.yj202588.top/gthrdmoobd.html

SAVEPOINT sp1;
来源：http://hz.316326.xyz/gtulaovlll.html

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtfurhmagk.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtsnyipivn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.bjfxy.top/gtbtrixsvf.html

[Q70] 更新统计信息
来源：http://hz.zhijiandao.cn/gtnqmaoqsn.html

ANALYZE TABLE users;
来源：http://hz.fzhhl.top/gtzpajohja.html

[Q71] 查看建表语句
来源：http://hz.nanxinkj.top/gttvpgytfu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhengqikj.top/gtfgpduzik.html

[Q72] 查看索引
来源：http://hz.aizwys.cn/gtgqdkayna.html

SHOW INDEX FROM users;
来源：http://hz.zycfv.cn/gtzjsgqtox.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gtyqcxfkwy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtmsjnszje.html

[Q74] 强制使用索引
来源：http://hz.yonumen.top/gtmdbpclpf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtavioftdt.html

[Q75] 日期格式化
来源：http://hz.9152youxi.cn/gtqcydcpai.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtjoofqbwq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtjkttzciu.html

[Q76] 按天统计
来源：http://hz.xinyue.icu/gtsjaavwkx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtxilwhcpt.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtimwheuws.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yongpay.top/gtblckjmdd.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtvxjnjwvf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtmjntydlt.html

[Q79] 字符串拼接
来源：http://hz.birdmap.top/gtpjazlfyj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhongyouzk.top/gtefsrmcmw.html

[Q80] 字符串截取
来源：http://hz.gzhubu.top/gtnucxtzpd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtwqdmutxf.html

[Q81] 字符串替换
来源：http://hz.cqqwz.cn/gthlanswnw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtgjozxahg.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtphjlupdu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cashguo.top/gtykjzuzwn.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtbyjnxkut.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daria6918.cn/gtaiymfjiz.html

[Q84] 去除首尾空格
来源：http://hz.gaohongyu789.top/gtjnexugzl.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtzdykopdy.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gtklcfrvbo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daria6918.cn/gtnesvizvo.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtktkpeard.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtacdvyrlv.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtsavcghny.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtmbpwoyns.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtzbhweqil.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xinyue.icu/gtjrcunkep.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtnadbedwp.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtffnzulcs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtthlxhpsm.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gteqldhnqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtaeehrbmi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtuzkrojtp.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtrkdqcdkd.html

================================================================================
来源：http://hz.9152youxi.cn/gtweelzrjm.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtonozjdek.html

#!/usr/bin/env bash
来源：http://hz.aizwys.cn/gtrtofrcox.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtzccyphrb.html

[R02] 变量赋值与使用
来源：http://hz.zhijiandao.cn/gtmvgmuuzt.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtvvgmdhmd.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtupplmvnp.html

readonly PI=3.14
来源：http://hz.xuanzx.com/gteojkkohd.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtttfarcfn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.9152youxi.cn/gtumtwtkhy.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtaftdyzai.html

name="${1:-default}"
来源：http://hz.sweek.top/gtyzslvbhr.html

[R06] 判断命令是否存在
来源：http://hz.jqgufenzy.top/gtihcyacrc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtelxfjmvd.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtjujbhlzr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nwbrower.top/gtfnhzcclv.html

[R08] 数值比较
来源：http://hz.jyoumei.cn/gtjqhyepam.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.havefunace.top/gtkudmwofq.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtnwzrodif.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenzaomai.com/gtiingfmwx.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gtesrihtbu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtbzocecee.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtyvnoobxp.html

case "$1" in
来源：http://hz.daxiang520.top/gtpdbufyzm.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtcbqaypox.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtdevzumuu.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gthpcezknn.html

esac
来源：http://hz.smart0.xyz/gtjgfyszch.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtyuztkkbu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxinkj.top/gttepdwoct.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gttjipsyrs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtkoyzqebx.html

[R14] C 风格 for
来源：http://hz.wangdashe.top/gtuowmlduw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtvlpkanka.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gtutrupywc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtftzrvhko.html

[R16] until 等待条件
来源：http://hz.cheryme.top/gtdppsslfh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtmmbiuaee.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtupfrxqkj.html


<!-- 参考信息 -->