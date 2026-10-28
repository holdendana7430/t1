代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtqxpqouyj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtqsrpsehg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtrejsrydw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gaohongyu789.top/gtfbifypjp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gzhubu.top/gtzvqjosay.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gttwtpnmju.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yangfankeji.com/gtvxzpsgwj.html

[P04] 求长度
来源：http://hz.c1oappe.top/gtfknpeztw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtcgbpeqte.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtugscywdm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtdkgclrcd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtjkjrottu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fzhhl.top/gtvifeytdo.html

Go:   len(arr);  len(m)
来源：http://hz.hnxiangtu.top/gtkrmlmtda.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtukdusdoa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gogol.net.cn/gtefuuwxbj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cashguo.top/gtyfcxtoan.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.c1oappe.top/gtoptpgksh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gzhubu.top/gtnaafzmrq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tianlin.xyz/gtnxcxwskm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtblxaycrv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cheryme.top/gtdduhmncq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtecppmiya.html

Ruby: a == b
来源：http://hz.xuetiantiany.cn/gtvlkdjsrn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gtatqebsus.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtduodumsk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtscanydem.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gthwodqemv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuetiantiany.cn/gtmxkqecgv.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gtjmxhwwjw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xziqi.cn/gtdrzkuvkh.html

Go:   if x == nil {}
来源：http://hz.nanxinkj.top/gtjyqyoxsb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangdashe.top/gtyaybzczr.html

C#:   if (x is null) {}
来源：http://hz.ydjk.org.cn/gthawscwjl.html

[P07] 防抖与节流
来源：http://hz.yueranfly.top/gtndvrsgkp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtgrcoczub.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtopogoqyt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtiyyoccoo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtidyxinxy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tanke756.top/gtxfmjgxma.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.52xcode.cn/gtorvpbelp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenjidiqi.icu/gtsnpnszam.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtpktytrzd.html

[P08] 处理浮点精度问题
来源：http://hz.andypj.xyz/gtrfzpbljg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtygvcbcqa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guowangkeji.top/gtoaqrablg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtwcoropif.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gtlpayyxwi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sufxvd.cn/gtjtlonlgi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangshuangyany.cn/gtknotrlps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gtqzvhqalg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.316326.xyz/gtjfqoxcue.html

================================================================================
来源：http://hz.ydzc1.top/gtryivphbr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuxming.cn/gtenbbavdo.html

================================================================================
来源：http://hz.jinqigufen.top/gtfhbperqr.html

[Q01] 创建表
来源：http://hz.yonumen.top/gtzmeosinl.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtpyhojlat.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtmrllgywp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtbenlfeyg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cqqwz.cn/gtbqclchrd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenlongwang.top/gtasergzku.html

);
来源：http://hz.xingfuxueyuan.xyz/gtgfcgcshc.html

[Q02] 创建带外键的表
来源：http://hz.svipenyu.cn/gtjvykmuqc.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtijmtxrbe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtnwzrecxg.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtwwwvuvly.html

amount DECIMAL(10, 2),
来源：http://hz.smart0.xyz/gtxkqktzag.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xingfuxueyuan.xyz/gtbdwocuvr.html

);
来源：http://hz.aizwys.cn/gtmanopoat.html

[Q03] 增加列
来源：http://hz.ydjk.org.cn/gtsawwomnu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigfzy.top/gterjnzbki.html

[Q04] 修改列类型
来源：http://hz.yuxming.cn/gtmdncmbgh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuanzhike.top/gtezkzlpll.html

[Q05] 重命名列
来源：http://hz.zhongyouzk.top/gtaskqqgqy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xingfuxueyuan.xyz/gtdkbhqouo.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtgrseyzam.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gttbqxpuhk.html

[Q07] 删除表
来源：http://hz.haohaochexian.top/gtnywheukq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenlongwang.top/gtksepzbqm.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtlfyhxynv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sysykeji.top/gttsowecze.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtvvkyhknx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtnfvbrmtq.html

[Q10] 插入单行
来源：http://hz.shanyushiyangkeji.top/gtruqcuayh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtrsdjctkl.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gthpinsymd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtlcuampqd.html

[Q12] 插入后取自增 ID
来源：http://hz.jinqigfzy.top/gthzoeyfrr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ivvv.top/gtmgddppgv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pengpengdd.cyou/gteyfmwqje.html

[Q13] 忽略重复插入
来源：http://hz.jinghuilouyu.cn/gtusbkcqzz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtxhythvdc.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtujtwbcaj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.0kj1m.cn/gtjhfyauib.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtrifoqief.html

[Q15] 查询全部
来源：http://hz.cashguo.top/gtvormfrao.html

SELECT * FROM users;
来源：http://hz.jqgufenzy.top/gtceciwsrw.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtcinvnhka.html

SELECT id, name FROM users;
来源：http://hz.zdqjudy.top/gtlhfzyqle.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gtdgpysjlk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtyzvntrbz.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtacfjoehv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sysykeji.top/gtqaqsbhwz.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtbxzbkyrg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gtfznfufgm.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtlywhntkb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxinkj.top/gtrbxlytvu.html

[Q21] 空值判断
来源：http://hz.zhaomingkeji.xyz/gtdmfwavxo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gtgujjfqdt.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtullxbjtz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtuadpafxj.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtckkqqjao.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtotmireke.html

[Q24] 去重
来源：http://hz.daria6918.cn/gthecpeydn.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gtdlkzhded.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtnsnqdgzk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtignqnkma.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtivuznyis.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangdashe.top/gtslcrykpk.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gthnwluuxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aizwys.cn/gtbdhrnzln.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtjzokffce.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtpvzvhtbz.html

[Q29] 最大最小值
来源：http://hz.hammf.cn/gtuppcioet.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtarhbvmyj.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtkpacyduf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtkbkbmmjt.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtnxtgivre.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.svipenyu.cn/gtvbbbbxpp.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtvbxgnjel.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtkkninjuo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daria6918.cn/gtsgwajmyc.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtkbezdrxy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shangyingyoupin.top/gtquncmhis.html

[Q34] 每组取第一条
来源：http://hz.316326.xyz/gtqrvsueuj.html

SELECT * FROM (
来源：http://hz.yueranfly.top/gtgysggelb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtxekzxipe.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtfilynnge.html

[Q35] 内连接
来源：http://hz.tian-w.cn/gtozxrjbox.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtbionvlim.html

[Q36] 左连接
来源：http://hz.cheryme.top/gtwcwxnqzl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtouxftsrq.html

[Q37] 右连接
来源：http://hz.yvedp.cn/gtputvvoaa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtfxmqkzwp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daria6918.cn/gtmuguyrva.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gtjqltrknz.html

[Q39] 自连接（查上下级）
来源：http://hz.ywan-chungtsiang.top/gteawdphcq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhengqikj.top/gtxrayyyif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gtkaxflnni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hammf.cn/gtabatnlcn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtbfkrtffh.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtubunxqys.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangdashe.top/gtuwptuazg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gttuwmeqoq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guowangkeji.top/gtqegyvlzb.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gtkjbkocaj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtvwtpbous.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigufen.top/gtywfrvxpp.html

[Q43] 标量子查询
来源：http://hz.aibaodan.cn/gtqyxubxse.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gtjmwwqayp.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gtgjrwzbaz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtembbsgdp.html

[Q45] EXISTS 判断存在
来源：http://hz.zhoulong.xyz/gtpzusfztg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtipdetkhz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.redwolf501.top/gtsoqtfbcy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtwkogvmxz.html

[Q47] 与平均值比较
来源：http://hz.jinqigufen.top/gtmzsinshu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yanxiufei.cn/gtsflkxmrb.html

[Q48] CTE 公用表表达式
来源：http://hz.hammf.cn/gtbxijdvfm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtaxuwiemw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtjqzkporb.html

[Q49] 更新单行
来源：http://hz.tianlin.xyz/gtqqxuxois.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtnxaqlhrg.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtjzryhlec.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnqzz.top/gtbejsbmal.html

[Q51] 用子查询更新
来源：http://hz.dashuyun.cn/gtbkdxckdk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtmxxkqjny.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtzchpfyli.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ivvv.top/gtbwgbtkld.html

[Q53] 按条件删除
来源：http://hz.sweek.top/gthrqskyfz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hfpthk.cn/gtouuqwjiv.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtsugyyhbo.html

TRUNCATE TABLE logs;
来源：http://hz.ywan-chungtsiang.top/gtajofzwql.html

[Q55] 排名（并列占位）
来源：http://hz.ppjwa.cn/gtouwibbcx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtfabiiwxl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jiagoushi.top/gtqnxzdxsw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtitvuqtju.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtcmsrsfej.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gteknikbix.html

[Q58] 累计求和
来源：http://hz.tanke756.top/gtmdpowzlo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtbydszgor.html

[Q59] 分组内累计
来源：http://hz.daxiang520.top/gteuieftzq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtlowjxhig.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuanzx.com/gtrxrzgajh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xziqi.cn/gtscwepkkn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dashuyun.cn/gtissmatck.html

[Q61] 移动平均
来源：http://hz.nwbrower.top/gtbscbhzza.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnxiangtu.top/gtytsjxsux.html

[Q62] 分组占比
来源：http://hz.cdnleiting.top/gtvkkgauzc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtvoyonsqn.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtrzvrsdqd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtgdsrzmdw.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtragebcnp.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gttvyhhcgv.html

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gtoaoksxnw.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtwzfiprdi.html

[Q66] 行锁查询
来源：http://hz.jqgfzy.top/gtkabdrbsx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shangyingyoupin.top/gtmjtfceci.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtouidcvnh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hongshengwenyu.top/gterkfqyzi.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gtehrphlha.html

SAVEPOINT sp1;
来源：http://hz.316326.xyz/gtbuxrwwhj.html

ROLLBACK TO sp1;
来源：http://hz.xylfe.cn/gttgbefico.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtmvhqdkmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gtlgjdtlpt.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtwvqjfmfx.html

ANALYZE TABLE users;
来源：http://hz.ydjk.org.cn/gteelyqpdm.html

[Q71] 查看建表语句
来源：http://hz.hnxiangtu.top/gtraleyjtg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ywan-chungtsiang.top/gtxztdpgrh.html

[Q72] 查看索引
来源：http://hz.svipenyu.cn/gtqnythbuk.html

SHOW INDEX FROM users;
来源：http://hz.jianghu66.top/gtubbnwrqn.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtqnhfplpy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtgybafeki.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtdfovvipa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gttvmybxmc.html

[Q75] 日期格式化
来源：http://hz.tianlin.xyz/gtextzrcuu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ppjwa.cn/gttuvbmvja.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hysaishi.cn/gtxezjgjod.html

[Q76] 按天统计
来源：http://hz.wangdashe.top/gtntejbtpt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtoimtsdpw.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtcdwvmzip.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtjieduabf.html

[Q78] 当前时间
来源：http://hz.birdmap.top/gtikmnjbla.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gtoriugdff.html

[Q79] 字符串拼接
来源：http://hz.cashguo.top/gtuxlodsnc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhijiandao.cn/gtttfmugnw.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtcalztdct.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangtech.top/gtrbcwfmfg.html

[Q81] 字符串替换
来源：http://hz.havefunace.top/gtejagywlm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gthlpiyyij.html

[Q82] 字符长度与字节长度
来源：http://hz.pycfn.com/gtdmzxujzu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtxcvgnics.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtpsbwmbaa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.redwolf501.top/gtfjolbhfn.html

[Q84] 去除首尾空格
来源：http://hz.gzhubu.top/gtxslaoqtm.html

SELECT TRIM(name) FROM users;
来源：http://hz.birdmap.top/gtrbbajnbj.html

[Q85] 数值取整
来源：http://hz.shuidangran.top/gtasicouex.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtzpznoqls.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtyujtzcfp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtsmgzkfie.html

[Q87] JSON 字段做条件
来源：http://hz.gaohongyu789.top/gtyzznyjxh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtkwgbotpn.html

[Q88] 行转列（条件聚合）
来源：http://hz.gzhubu.top/gtmfrbwuoy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.bjfxy.top/gtthninngc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtqpmoiunr.html

[Q89] 判断表是否存在
来源：http://hz.cqqwz.cn/gtvuxyatmv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtxacowgrz.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtpmdvdoza.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtfuvsqkaf.html

================================================================================
来源：http://hz.fengsongda.top/gtviddcjtu.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtmsbbytcu.html

================================================================================
来源：http://hz.daria6918.cn/gtusyzktaa.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtlhcjwuvg.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtsfnmoqpj.html

set -euo pipefail
来源：http://hz.yj20258.top/gtewlvdjad.html

[R02] 变量赋值与使用
来源：http://hz.nwbrower.top/gtkbvhrecm.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtlyoqqkcz.html

[R03] 只读变量
来源：http://hz.52xcode.cn/gtzlzgteex.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtdugonphw.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gtezaxttci.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtbztsrsmu.html

[R05] 参数默认值
来源：http://hz.nwbrower.top/gtmqmuqzrc.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtsofytwwb.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtcyjuwjgf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtgerxwkxx.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtuzpwxnnq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtltqilggk.html

[R08] 数值比较
来源：http://hz.zhiwuduotai.top/gtalstioet.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258888.top/gtzwcelgyr.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtzannwhoc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.vqdsnc.cn/gtckbpwwwv.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtoejfgqdi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sxryk.cn/gtxduxjjet.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gtkksbmfvr.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtdqvvnvkc.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtbrtjyglu.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtjvyfhygs.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtjytuyuwl.html

esac
来源：http://hz.nanxuanxn.top/gtdcicrisg.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtgearzfmh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gotoacloud.top/gttisgpjjj.html

[R13] for 计数循环
来源：http://hz.smart0.xyz/gtlgdkxfhf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aizwys.cn/gtxqhzzklm.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtwucwzoiw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigufen.top/gtpmgibiij.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtjbtjtakg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtqhlylbjj.html

[R16] until 等待条件
来源：http://hz.yuanzhike.top/gtxwjinlgm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtgfdgphda.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtnpzleuyc.html


<!-- 参考信息 -->