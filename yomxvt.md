代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtopozpfen.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtwhbzzczi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtmpqcmupt.html

[P04] 求长度
来源：http://hz.mhx1999.top/gtnodipycg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pengpengdd.cyou/gtvitujspc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtxxexowra.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gthtjegltc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtspgoktua.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gttgfqojyk.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtxhzxoiad.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gtxxsvlppg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtcpubmszi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sxryk.cn/gtfotuqksv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fzhhl.top/gtesesqiyu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgufenzy.top/gtfkobtikh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fzhhl.top/gtpqydoake.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigufen.top/gttfsltqns.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cdnleiting.top/gtuyduasgs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj202588.top/gtfwytzbeh.html

Ruby: a == b
来源：http://hz.chenlongwang.top/gtworitysn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtnumyfiwc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtxpimipmy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtqteafemq.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtodnhjxpo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gtnldxtzlk.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gtunupaqxo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258888.top/gtdbnsrrtb.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gttwerefpi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtqjmqgtip.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gtuifuosaa.html

[P07] 防抖与节流
来源：http://hz.cashguo.top/gtsmpswqsr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtfpesgctb.html

PHP:  // 手写时间戳比较
来源：http://hz.yvedp.cn/gtklnrmeub.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtpfriyrzg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtwpaotqoo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtjjmfkamp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhongyouzk.top/gtjczypsug.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtfgxascis.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtexvbgpdk.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtuuqvqsdo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shangyingyoupin.top/gtvshmqrhb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.vqdsnc.cn/gtjhhjywfm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtitzdeylv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tian-w.cn/gtcwiqoula.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenlongwang.top/gtuhfldrec.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtkeimosxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.iojbl.cn/gtiysvqycp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gthdincdkp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtlavuxzjp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ywan-chungtsiang.top/gttuyhkstw.html

================================================================================
来源：http://hz.dashuyun.cn/gtzyydivmz.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtfdvmproy.html

CREATE TABLE users (
来源：http://hz.pengpengdd.cyou/gtuacnmngo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtozorjmhz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gthjwrrhdi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gtcyiimqxx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtwugajyle.html

);
来源：http://hz.zycfv.cn/gtfhfbdxsp.html

[Q02] 创建带外键的表
来源：http://hz.9152youxi.cn/gtejwxpric.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtpnahizsc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtdvlvtzvf.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gtqrwdmykf.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtdbmlfrxr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydzc1.top/gtzcicbgjc.html

);
来源：http://hz.jyoumei.cn/gtzwiepoqf.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtdfubkfoy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tian-w.cn/gtsiewoiks.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtpknnhzoc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hammf.cn/gtvujseenu.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtgmdvqmkh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtuairfpth.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtezoryfmc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daxiang520.top/gtycjhmrfx.html

[Q07] 删除表
来源：http://hz.smart0.xyz/gtceeiksjd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtpfhtvufp.html

[Q08] 创建普通索引
来源：http://hz.jinghuilouyu.cn/gtwgzydqhd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gtbghzblci.html

[Q09] 创建唯一索引
来源：http://hz.yuanzhike.top/gtlvajboac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cheryme.top/gtqpmcldjc.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtgwqelxlx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtyozaypdw.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtijpgcive.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtvenfwiuv.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtlaoqmkhe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtuwbcvxns.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtjgxuuwpa.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtwifjdtmw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guowangkeji.top/gtkwnsgdrz.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gtsxlbwazw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtujauvban.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtfgjfxamz.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtjnbeznak.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtfanijsds.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtxcyvhxab.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gthrxmyrfd.html

[Q17] 条件查询
来源：http://hz.yuxming.cn/gtujcdykhc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtrhuhfbwm.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtgojmqcvs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtxzqngraw.html

[Q19] 范围查询
来源：http://hz.yueranfly.top/gtnvnlnnvz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hammf.cn/gthupfvlla.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtbdwimlxj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtxzxtxhgc.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtvpezszti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtkajleaeo.html

[Q22] 排序
来源：http://hz.fengsongda.top/gtvmuazvgz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtxnrgkfrj.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtqlyqpyve.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtgzqyaccj.html

[Q24] 去重
来源：http://hz.quarkkingdee.top/gtbqiaoasz.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtpqbqialc.html

[Q25] 只取前 N 条
来源：http://hz.chenzaomai.com/gtgusgtjvy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sweek.top/gtaziwnmow.html

[Q26] 计数
来源：http://hz.sysykeji.top/gtbvvmkmpb.html

SELECT COUNT(*) FROM users;
来源：http://hz.fzhhl.top/gtuhvzsnhx.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtpaudvkfc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenjidiqi.icu/gterahfwoh.html

[Q28] 求和与平均
来源：http://hz.yueranfly.top/gtgzsnrchb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhongyouzk.top/gtxvssrcfi.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtrofsjwnm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtkoigrron.html

[Q30] 分组统计
来源：http://hz.yuxming.cn/gtyfbkrryx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtbkkagwlc.html

[Q31] 分组后过滤
来源：http://hz.zycfv.cn/gtdprnybdw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtsomtqnyc.html

[Q32] 分组拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtekaynpld.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtjdfxxgfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sweek.top/gtepbrjenm.html

[Q33] 多列分组
来源：http://hz.yonumen.top/gtyyycgfag.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gtnrtghpdp.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gtomqgwmuq.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gtxhqdbsrx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigufen.top/gtgqcuoeka.html

) t WHERE rn = 1;
来源：http://hz.jlsjyb.cn/gtrrxtjlgm.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtjblvquwp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtyklinpdv.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtbowizzwn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtuojldkur.html

[Q37] 右连接
来源：http://hz.52xcode.cn/gtacibpizm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtkugmecvr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cucudq.cn/gtolfnwpbn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ppjwa.cn/gtydkajiaa.html

[Q39] 自连接（查上下级）
来源：http://hz.xylfe.cn/gtaswkacgz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenzaomai.com/gtrufmierf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jyoumei.cn/gtdztmtifr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aizwys.cn/gtcuqposvl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daria6918.cn/gtihtqospe.html

[Q41] 多表连接
来源：http://hz.xuetiantiany.cn/gtfjfgncjx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtwakgmnxy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhengqikj.top/gtmcyfetwd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtnwsrfctx.html

[Q42] 连接条件附加过滤
来源：http://hz.chenzaomai.com/gtaiwezlao.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gtbbwflhvl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtgbujrvol.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gttgxnnmyt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gaohongyu789.top/gtjrxtpxqs.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtcomngstp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.andypj.xyz/gtssfjvcki.html

[Q45] EXISTS 判断存在
来源：http://hz.cqqwz.cn/gtnahjqgde.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtigsqvaic.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yongpay.top/gtfcknhzfr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtmxzmjqkm.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtazsuecrg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtxktsotyk.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtmzvtjoym.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtpngljyko.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtdwdiopuq.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gtcqaxudyh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.mhx1999.top/gteztzkivf.html

[Q50] 批量更新
来源：http://hz.gogol.net.cn/gtrxpxtxbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gthakwzbrn.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtxxybdurs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gtabpajqzm.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtavduvevy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtgxpbxojb.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtfnpnylxq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinyuanbaomall.cn/gtnqflzuow.html

[Q54] 清空表
来源：http://hz.aizwys.cn/gtfjawsuqr.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gtwlmdemeq.html

[Q55] 排名（并列占位）
来源：http://hz.hammf.cn/gtlpkgrkzy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cqqwz.cn/gtvpeihriq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sufxvd.cn/gtzpcpgiwo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtpmbwlhlh.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtrrjantsm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.bjfxy.top/gtfnueblkx.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gteppozdmv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhixingplan.top/gtrcnwnejl.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtfbdazbui.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangdashe.top/gtwdwflbmb.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258888.top/gtcxqxnzsd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtrsehisvo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhiwuduotai.top/gtakseiljo.html

[Q61] 移动平均
来源：http://hz.jianghu66.top/gtizqmmxpt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtfonkumqz.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtdpfwqbno.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtdsalxjeu.html

[Q63] 开启事务
来源：http://hz.zhengqikj.top/gtdpmdiorf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj202588.top/gtrguxmbtu.html

[Q64] 提交事务
来源：http://hz.hnxiangtu.top/gtsjewehpb.html

COMMIT;
来源：http://hz.jinghuilouyu.cn/gtnrsgbwir.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gttkwfwoad.html

ROLLBACK;
来源：http://hz.yj202588.top/gttgcvymcf.html

[Q66] 行锁查询
来源：http://hz.yvedp.cn/gtnssptkqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daxiang520.top/gtwjgbmxfo.html

[Q67] 设置隔离级别
来源：http://hz.nanxuanxn.top/gtmdmgvmsk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gtogtfkqbi.html

[Q68] 保存点
来源：http://hz.yongpay.top/gtyjygkuby.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtzxvdekgj.html

ROLLBACK TO sp1;
来源：http://hz.gotoacloud.top/gtumqnkzcv.html

[Q69] 查看执行计划
来源：http://hz.fzhhl.top/gtyqhppaur.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtsoyxcbwk.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtuebrgwlt.html

ANALYZE TABLE users;
来源：http://hz.svipenyu.cn/gtnvrtxdno.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtyamrkyif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuetiantiany.cn/gtozcgkarp.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gtlvstosnd.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtmzknpzys.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtxkyenerk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xylfe.cn/gtwmnteqif.html

[Q74] 强制使用索引
来源：http://hz.jinghuilouyu.cn/gtkzggqwmd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtxuysktjx.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gttvipalxx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yangfankeji.com/gtxsflaxhn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgufenzy.top/gtmllcunel.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtijgkijfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hywenlv.cn/gtoffvsdyg.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtrtopnbfo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtcktzimmr.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtddtbbjzj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtydwzsmvn.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtsgwmbsfi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gtwydebvzl.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gttmhkrhpf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtizopdikq.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gthtieuvqz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zdqjudy.top/gtkipiyuun.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtoqwgfuor.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtukkjhcgn.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtqhtrmkql.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangdashe.top/gtvbrmjoiy.html

[Q84] 去除首尾空格
来源：http://hz.hammf.cn/gtzxjhwlms.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtdcvrfwcv.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtyyurhjeq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtgvkixinx.html

[Q86] 读取 JSON 字段
来源：http://hz.hongshengwenyu.top/gteaoersrz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtzwvtgrrp.html

[Q87] JSON 字段做条件
来源：http://hz.wangshuangyany.cn/gttrcwftpi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtjtjfhnoy.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtjmoxfnxv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtugnaaxja.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtuqxyhnjp.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gthckdalql.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.9152youxi.cn/gtgesefysm.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtrwuscfos.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtztiodsxa.html

================================================================================
来源：http://hz.jyoumei.cn/gtwxvrobgh.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtovfypmxd.html

================================================================================
来源：http://hz.gotoacloud.top/gtouvrmpla.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtioeifjrj.html

#!/usr/bin/env bash
来源：http://hz.kuanghao11.cn/gtxkcqxflo.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtretsmjbt.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gtdgrjfvxq.html

name="Tom"; echo "$name"
来源：http://hz.c1oappe.top/gtlrbmqakr.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtvkeoyosm.html

readonly PI=3.14
来源：http://hz.jiagoushi.top/gtkgvrhpvj.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtfvsqloyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtocqusmms.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gteshzrygn.html

name="${1:-default}"
来源：http://hz.dianchejie.cn/gtrctaxrzk.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gticoyewhn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydjk.org.cn/gtwdjzxjxw.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtjgxtqkro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ivvv.top/gtleezhldb.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtxlyxkfgu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.9152youxi.cn/gtzhmtflzx.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtvfvasbkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtdqufoyzs.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtdvkdmqlw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ppjwa.cn/gtztettrdl.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtwlswekdy.html

case "$1" in
来源：http://hz.wangdashe.top/gticfqkgwr.html

start) echo "启动" ;;
来源：http://hz.cdnleiting.top/gthfkomujo.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtwjdexqrx.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gtaonmawev.html

esac
来源：http://hz.dianchejie.cn/gtbiqwansz.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtftphzevk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gtjcvpixkb.html

[R13] for 计数循环
来源：http://hz.9152youxi.cn/gtrgmsibun.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtnstfmbqn.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtaxybhlkr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtksonqcpj.html

[R15] while 逐行读文件
来源：http://hz.daria6918.cn/gtyafrjipg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hongshengwenyu.top/gtddydaefw.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtasipkuxt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gtesjhyirt.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtfhgsqncc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuanzhike.top/gttjedbucc.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtbwimclmw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtddeeagls.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtkthaohke.html


<!-- 参考信息 -->