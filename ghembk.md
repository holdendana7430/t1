代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.c1oappe.top/gtwkkrrmbr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtvjtansao.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pengpengdd.cyou/gtvbalkmgo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cqqwz.cn/gtqoyqtszj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhiwuduotai.top/gtmuycuywr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cheryme.top/gteixkorzv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gttocxvwmg.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtokeepsdw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtrjrbbyfx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gterhbpnhd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtpvwaetee.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtojvtgxpr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ehwqpu.com/gtnffqeyaf.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gttyjprade.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtwjamycis.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangdashe.top/gtizwcrzgy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj202588.top/gtjetokjvq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hammf.cn/gtirmmtgjb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guowangkeji.top/gtaeazngyf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shangyingyoupin.top/gtgatwtpek.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtstrobojr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.mhx1999.top/gtillholop.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtwhugzcsc.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtpzwurxwe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtdpwrspzn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigufen.top/gtdsakbyjz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.feifeiyinyue.top/gtskmuxzus.html

PHP:  if (empty($x)) {}
来源：http://hz.zhaomingkeji.xyz/gtxhhjafvz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinghuilouyu.cn/gtslqgxpnq.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtraixxexd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtbtmhvmgq.html

Go:   if x == nil {}
来源：http://hz.yangfankeji.com/gtyfeaoeiv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gttlgmsqyf.html

C#:   if (x is null) {}
来源：http://hz.zhoulong.xyz/gtzdhzsgaj.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtkxykvxte.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhengqikj.top/gtcqbjpcjo.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtqhnubosh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gttbfhunhe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtdnrugvni.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cheryme.top/gtwrutkfen.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtaiemxkrd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gtkzmdzecz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxuanxn.top/gtrzcdwzxs.html

[P08] 处理浮点精度问题
来源：http://hz.xingfuxueyuan.xyz/gtjvinouql.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gtqhaakbmw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtodozmusw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtuqcsuifl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gtclbyaywi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.birdmap.top/gtkwtrzpjr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydjk.org.cn/gtambqlvbz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ywan-chungtsiang.top/gtkbovgifd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtawyblwxx.html

================================================================================
来源：http://hz.yanxiufei.cn/gtreuwetxc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xziqi.cn/gtbdiodoyf.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcrxvenbz.html

[Q01] 创建表
来源：http://hz.nwbrower.top/gtuimauvwu.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gtopxhqlnb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtpnwuzxmp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangshuangyany.cn/gtjcnnbnnd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gtahfxlsfi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cdnleiting.top/gtzogvygho.html

);
来源：http://hz.hfpthk.cn/gtdfzpkgut.html

[Q02] 创建带外键的表
来源：http://hz.tanke756.top/gtcxjwbuba.html

CREATE TABLE orders (
来源：http://hz.yj20258888.top/gtjokpkiqd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtnecausae.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtpmcualyk.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtbagtzune.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtexthlamw.html

);
来源：http://hz.jianghu66.top/gtrdohmeoz.html

[Q03] 增加列
来源：http://hz.cqqwz.cn/gthobwkbrv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtrhtonceq.html

[Q04] 修改列类型
来源：http://hz.svipenyu.cn/gtpvjwuhum.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hywenlv.cn/gtmyubxcsd.html

[Q05] 重命名列
来源：http://hz.havefunace.top/gtluffdtww.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nwbrower.top/gtzxghsnde.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gtcgjgpcrc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtcqpksxpx.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtrgjfgxar.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtslpkprpg.html

[Q08] 创建普通索引
来源：http://hz.iojbl.cn/gtldelkhnz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtnzjsavfi.html

[Q09] 创建唯一索引
来源：http://hz.quarkkingdee.top/gtvjhkguhm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yonumen.top/gtkmfxtkfo.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtgdsweben.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxuanxn.top/gtkekhqbvb.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gthusisbae.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtqwbqeest.html

[Q12] 插入后取自增 ID
来源：http://hz.xziqi.cn/gtvlrxplyx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtnomoodst.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gtcrtcwxxt.html

[Q13] 忽略重复插入
来源：http://hz.quarkkingdee.top/gtoxliyloj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gtjqptamny.html

[Q14] 存在则更新（upsert）
来源：http://hz.guowangkeji.top/gtsrvoaujs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.aizwys.cn/gtzimskwnx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gteeowimtw.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtiytvophg.html

SELECT * FROM users;
来源：http://hz.guannengcc.top/gtasgwnaei.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gthvfxahoz.html

SELECT id, name FROM users;
来源：http://hz.ywan-chungtsiang.top/gtnjxtbexy.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtarnuclld.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtmtxqwltl.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtcuscdspj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtreupoaoi.html

[Q19] 范围查询
来源：http://hz.9152youxi.cn/gtzqcuppdz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gtibxphnmf.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gteaunagxw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258888.top/gtqemtaibz.html

[Q21] 空值判断
来源：http://hz.52xcode.cn/gtgxcenifz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenjidiqi.icu/gtihlkfahv.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtzchdbmbl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtpfqkqztl.html

[Q23] 分页
来源：http://hz.tian-w.cn/gtnavrraxq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.feifeiyinyue.top/gtfajayxbf.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtivaqttlr.html

SELECT DISTINCT city FROM users;
来源：http://hz.mhx1999.top/gtrutyxmah.html

[Q25] 只取前 N 条
来源：http://hz.guannengcc.top/gtxxgbiqop.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtgbqoihem.html

[Q26] 计数
来源：http://hz.haohaochexian.top/gtnmayshmd.html

SELECT COUNT(*) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtmzyxzzpw.html

[Q27] 条件计数
来源：http://hz.yonumen.top/gttrwbwqzq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yongpay.top/gtqyxocrpk.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gtvdkannhb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxinkj.top/gtevcshtuy.html

[Q29] 最大最小值
来源：http://hz.haohaochexian.top/gtmgjsbjrj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtrtrbngvk.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gtzzgfxfjo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtklpxzecv.html

[Q31] 分组后过滤
来源：http://hz.zhixingplan.top/gtmnozboqp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gtagwbwpwz.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtqofkytkf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtmambyehv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtqyfqqzgp.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gtaabvbsgn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtvoohawez.html

[Q34] 每组取第一条
来源：http://hz.jiagoushi.top/gtspxxccwv.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtmosdhoui.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtnmcrhlze.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtjxvmtmsi.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtlxhivrdq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtrlnswwjx.html

[Q36] 左连接
来源：http://hz.pycfn.com/gtzxpwlaxw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtvcurkdtt.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gtzzvpbkdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gthauwgpou.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtaqrfcgfg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtcbijneva.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtmzbwtqgz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtcaaslhmp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhongyouzk.top/gtacqhbndg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtuzwwpqqp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtgbgsodkq.html

[Q41] 多表连接
来源：http://hz.yvedp.cn/gtwudtnxzt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtunldeqko.html

JOIN users u ON u.id = o.user_id
来源：http://hz.snrcjt.cn/gtbhmykouv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gtuwgsssnq.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258888.top/gtzlmrjgcb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj202588.top/gtintitidx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sxryk.cn/gtrianquyn.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtkjtrtyrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gtnzpmacfp.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangtech.top/gtbcejzwei.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gteyajilck.html

[Q45] EXISTS 判断存在
来源：http://hz.chenjidiqi.icu/gtbgcuxhjk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gtcqatohwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gtlqnhzdpl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtmcivkpqp.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gtvvbjaqrj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtwnmxcdlo.html

[Q48] CTE 公用表表达式
来源：http://hz.gotoacloud.top/gtipchnubc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.feifeiyinyue.top/gtrwarzswv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuanzx.com/gtchaxaqok.html

[Q49] 更新单行
来源：http://hz.chenzaomai.com/gtvbptsszf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtjryxpblk.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtfylhpdbw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hammf.cn/gtofvtyjwu.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtzcvmlplf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtvmtcwyxs.html

[Q52] 删除指定行
来源：http://hz.yonumen.top/gterawhqbc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtjalrcvub.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtvmtasfms.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shuidangran.top/gtropuivhj.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtgnrytyql.html

TRUNCATE TABLE logs;
来源：http://hz.havefunace.top/gtfkmdfufc.html

[Q55] 排名（并列占位）
来源：http://hz.316326.xyz/gtbzcxyemw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cqqwz.cn/gttglntagp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ivvv.top/gtoblmqnye.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydzc1.top/gtpcywpfnq.html

[Q57] 行号
来源：http://hz.hammf.cn/gtumpswfui.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gtjgbhygem.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtfisyzofn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhengqikj.top/gtvfyjnegx.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtrtfyfiuq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.meibo888.top/gtwailsutj.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtzjmiaqhh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtcgizbvaw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtgwbtivin.html

[Q61] 移动平均
来源：http://hz.316326.xyz/gtoqvsfhfq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yangfankeji.com/gtmnkswdqz.html

[Q62] 分组占比
来源：http://hz.tian-w.cn/gtajwqyuvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtgltxvflm.html

[Q63] 开启事务
来源：http://hz.xuetiantiany.cn/gtdgjolcni.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtojeohnaa.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtuxelhhie.html

COMMIT;
来源：http://hz.pengpengdd.cyou/gthnhdceph.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtkwhniajz.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtghmfoqaz.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gtblqirqtl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangtech.top/gtffrtzpjh.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtgroggbbm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cashguo.top/gtisxensvi.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtmwdfrgho.html

SAVEPOINT sp1;
来源：http://hz.shzxlz.cn/gtlysdcdid.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtunonxfbp.html

[Q69] 查看执行计划
来源：http://hz.ivvv.top/gtemojwytd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtmixkdroc.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gthrobnjgj.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtneftvlhx.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtxxaiaqmk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenlongwang.top/gtpqpuivlw.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtdlcbklzd.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtbpoovxca.html

[Q73] 查看表状态
来源：http://hz.guowangkeji.top/gtngahyqju.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtjnpinfhf.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gtbxlqwvea.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.9152youxi.cn/gtvhqzlxif.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtxcwpctoe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.c1oappe.top/gtxzaaqkmp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtrfxpypth.html

[Q76] 按天统计
来源：http://hz.cashguo.top/gtdbyottad.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.haohaochexian.top/gtrgqoujsc.html

[Q77] 时间加减
来源：http://hz.cdnleiting.top/gtxsauclja.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.haohaochexian.top/gtqjxrkrux.html

[Q78] 当前时间
来源：http://hz.andypj.xyz/gtoqyizcqx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guannengcc.top/gtwlszezlb.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtuvxwldvz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtccfjbphm.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtbdtbomlc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtmvvbnvsf.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtraetnqfv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtgxwplulq.html

[Q82] 字符长度与字节长度
来源：http://hz.ybcxt.top/gtkfersshp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gtqmsyqqfr.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gttxphimpd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gtruyljnwh.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gtvyrdefuk.html

SELECT TRIM(name) FROM users;
来源：http://hz.quarkkingdee.top/gteulxprsn.html

[Q85] 数值取整
来源：http://hz.pengpengdd.cyou/gtqkrpiqtw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtrlyckagc.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gthwqtazzx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tianlin.xyz/gthjwanxui.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigfzy.top/gtkbrciond.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtdrsqgibd.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydzc1.top/gtkjfloqbu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtiuevxktx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pycfn.com/gtfriyauzj.html

[Q89] 判断表是否存在
来源：http://hz.zhoulong.xyz/gtjcbcffdv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.c1oappe.top/gtxaizqjnd.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gtfpxbigoq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gtlnijhmdu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtyxentuuy.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtbvkyjgad.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrjcbelxh.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtnpokyjmr.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtpouvbdfm.html

set -euo pipefail
来源：http://hz.wangshuangyany.cn/gtyxssuoia.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gttkeymsai.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtjyoxgjtb.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtfpwefrgz.html

readonly PI=3.14
来源：http://hz.tian-w.cn/gtqigdoyzl.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtmouudbhu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtxfnyhrrq.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtzewxuhdy.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gteuglwpkp.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtkltvwhal.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhixingplan.top/gtmfllxpfq.html

[R07] if 判断文件
来源：http://hz.dianchejie.cn/gttlzmenox.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtdbxzvguq.html

[R08] 数值比较
来源：http://hz.dianchejie.cn/gtxfmrvaex.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtnnelcufd.html

[R09] 字符串比较
来源：http://hz.zhengqikj.top/gtpvdqxstn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtnqocjzlh.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gthhwdvopn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtcgcnctfs.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtcuiijrcm.html

case "$1" in
来源：http://hz.xinyue.icu/gtdwwmxtid.html

start) echo "启动" ;;
来源：http://hz.shangyingyoupin.top/gtaqelrffb.html

stop)  echo "停止" ;;
来源：http://hz.sysykeji.top/gtlrpkmkom.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtvmomkzdu.html

esac
来源：http://hz.pycfn.com/gtnsqwqgrw.html

[R12] for 遍历文件
来源：http://hz.zhiwuduotai.top/gtcmbrgydm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gtnfmzevtd.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtitgensoz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuxming.cn/gtywretdsq.html

[R14] C 风格 for
来源：http://hz.guowangkeji.top/gtpemzxzlk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258.top/gteqitjcpu.html

[R15] while 逐行读文件
来源：http://hz.zhongyouzk.top/gtmjippczb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtxxqszdcn.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtskexgrom.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fengsongda.top/gtfxmgcexv.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gtewowqqwd.html


<!-- 参考信息 -->