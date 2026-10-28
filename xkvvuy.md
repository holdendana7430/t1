代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.meibo888.top/gtzmsouovt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtnayhrgpx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhengqikj.top/gtxywnkybx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhoulong.xyz/gtfzecumkj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gtmlznpwqa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtocdlqech.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenlongwang.top/gtjftmaath.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtkymyfzjq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtqpnuoqgq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtfqjkzbfa.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gttkdaoofz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gotoacloud.top/gtzuwjfyyy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtrhjtvkbr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtyqrqjhab.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gttisxsfwq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhengqikj.top/gtdbqrgies.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258.top/gthyovfsys.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtaikfzbdr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtqcbjbnhe.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gthbikxthn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtfyxdtigl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtbrlbpxyb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtumjcilqp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtugbsezwg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtqnolbcfk.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gteakoybgs.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtotoobfqr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.mhx1999.top/gtumifqabr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtpdfpbqri.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.bjfxy.top/gtnlneshfo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigufen.top/gtpgracafr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xylfe.cn/gtoiunslhn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtivkajomv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtqwfwyywg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtzcopvxcn.html

Ruby: a == b
来源：http://hz.nwbrower.top/gtegjlelgc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gteenepdjk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangkeji.top/gtjaztmwdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.birdmap.top/gtijfslode.html

PHP:  if (empty($x)) {}
来源：http://hz.ivvv.top/gttfvqlvoc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtzfnnpdum.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtwmidgjby.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtmdhznuvt.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtljmodkup.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtchvktmpd.html

C#:   if (x is null) {}
来源：http://hz.316326.xyz/gtjmvjyidv.html

[P07] 防抖与节流
来源：http://hz.ybcxt.top/gtljhjgfqi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.svipenyu.cn/gtliuywyyo.html

PHP:  // 手写时间戳比较
来源：http://hz.redwolf501.top/gttgaxefwb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gthwfjyclz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gttkevrsfj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtcqbbcyuf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnxiangtu.top/gtbwyuvtuu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tian-w.cn/gtsushkwau.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtpsmkpzkj.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtgpprwmct.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shangyingyoupin.top/gtslfbgdfo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gaohongyu789.top/gtmoqqyjfb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigfzy.top/gtzpcppfnx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hfpthk.cn/gtokwfxmjt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtkcsmpowz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pycfn.com/gtlccyqasx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yonumen.top/gtfboijlsa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daria6918.cn/gthjcmoano.html

================================================================================
来源：http://hz.tanke756.top/gtljldfuar.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtdnjqgdsl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxdjtqmtm.html

[Q01] 创建表
来源：http://hz.yuxming.cn/gtymlvgxds.html

CREATE TABLE users (
来源：http://hz.ivvv.top/gtcnzeahod.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtlxkuulxh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtnoerrymi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gtsggbvjvr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtvrzfuais.html

);
来源：http://hz.hongshengwenyu.top/gtjeqszfer.html

[Q02] 创建带外键的表
来源：http://hz.52xcode.cn/gttflvsgvw.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtebqkdryu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtcfucgsni.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gttgbkfdeo.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtwheqgduv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenlongwang.top/gtergfruac.html

);
来源：http://hz.daxiang520.top/gtdtgtglwb.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtdlsnsneu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydzc1.top/gtdzeepfxx.html

[Q04] 修改列类型
来源：http://hz.nanxinkj.top/gtgdhzdzaq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yvedp.cn/gtfaimcnud.html

[Q05] 重命名列
来源：http://hz.chenzaomai.com/gtfnrlikyh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtbpkkdqzx.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gtfodtzlrc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cheryme.top/gtlbnyjheu.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtosphilie.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtqmslqlfo.html

[Q08] 创建普通索引
来源：http://hz.zhijiandao.cn/gtlburqgzr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gttzmxmeve.html

[Q09] 创建唯一索引
来源：http://hz.hnqzz.top/gtfzwhcjfz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtvnefzuky.html

[Q10] 插入单行
来源：http://hz.birdmap.top/gtxozgpgjm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtitjxgjtc.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtobaguzzb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jyoumei.cn/gtxjspmcbg.html

[Q12] 插入后取自增 ID
来源：http://hz.guannengcc.top/gtjwhudjcr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtdchtyhno.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtyyoktvkp.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtajcqixmk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangtech.top/gtkauiloef.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtvetlmask.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtelrxhpye.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ybcxt.top/gtjmaisugj.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtkdkqdoim.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtzravhxme.html

[Q16] 查询指定列
来源：http://hz.guowangkeji.top/gtoymzqzwu.html

SELECT id, name FROM users;
来源：http://hz.vqdsnc.cn/gtswxrspkc.html

[Q17] 条件查询
来源：http://hz.wangshuangyany.cn/gtoqrikqys.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hywenlv.cn/gtwfglkwww.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtupviwwab.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yueranfly.top/gtjjkpoyrb.html

[Q19] 范围查询
来源：http://hz.hammf.cn/gttppcmgjf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtraxrplme.html

[Q20] IN 列表
来源：http://hz.zhijiandao.cn/gtojomamxe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtmvjgmegi.html

[Q21] 空值判断
来源：http://hz.jinqigfzy.top/gthsdnyrlh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtmeczzzue.html

[Q22] 排序
来源：http://hz.sufxvd.cn/gtrcprmglw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yongpay.top/gtmfalmrbi.html

[Q23] 分页
来源：http://hz.xuanzx.com/gtdoqunzml.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cheryme.top/gtvykcuesh.html

[Q24] 去重
来源：http://hz.meibo888.top/gtrxxwwxqe.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtygszxunv.html

[Q25] 只取前 N 条
来源：http://hz.0kj1m.cn/gtmvgpdpqy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtnqenwqul.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtmigmgmvv.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtqydembxs.html

[Q27] 条件计数
来源：http://hz.jiagoushi.top/gtihdrcvdm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gtstfabrir.html

[Q28] 求和与平均
来源：http://hz.dianchejie.cn/gtknradvbq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydzc1.top/gtyjyjdhdp.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtzyclxvxr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.meibo888.top/gtwzwgkbkf.html

[Q30] 分组统计
来源：http://hz.cashguo.top/gttzajkzdo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtznzggpie.html

[Q31] 分组后过滤
来源：http://hz.xuanzx.com/gtlnvspddb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gthfctqgud.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtvwwimekt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtetytllvx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gtclwcepmz.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtuhvavecc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yangfankeji.com/gtupnksxvo.html

[Q34] 每组取第一条
来源：http://hz.jqgufenzy.top/gtemxosouz.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtwryihhcn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gttsqsycpd.html

) t WHERE rn = 1;
来源：http://hz.yueranfly.top/gtfrvtypio.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtskchbdqg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtqtdetcmo.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtmqsrjwrc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtrbgwazir.html

[Q37] 右连接
来源：http://hz.dashuyun.cn/gttlxvndeo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgufenzy.top/gtcpbjoyae.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hongshengwenyu.top/gtolkmnkjq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangkeji.top/gtzzkqpulu.html

[Q39] 自连接（查上下级）
来源：http://hz.guannengcc.top/gtgecrcnyq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ppjwa.cn/gttqyntdcj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtwoocsdej.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtdbpcucyt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgfzy.top/gtdyovtnui.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtndtjpbny.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sweek.top/gtxxwkklgv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtvzawtbfn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtpbqslfyn.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtehrtfqay.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtwoaxgorq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtlxvlxwmm.html

[Q43] 标量子查询
来源：http://hz.hfpthk.cn/gttjfidcom.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.vqdsnc.cn/gticsswrgu.html

[Q44] IN 子查询
来源：http://hz.ehwqpu.com/gtraxgredz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.snrcjt.cn/gtumbsjyjb.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtvyxsiyty.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtkdctigur.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtjzvkccrz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtuzaowpss.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtepxgpqjm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtwxlvoznx.html

[Q48] CTE 公用表表达式
来源：http://hz.zhijiandao.cn/gtaqvfutmt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtrhslzwra.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.iojbl.cn/gtvkenrjrg.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtgygdpnxt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtnkiriznp.html

[Q50] 批量更新
来源：http://hz.cdnleiting.top/gtrmpycwpk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gttyghjnxg.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtethdvyrc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yanxiufei.cn/gtggzzqqgd.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtfobjxpfj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtjtsxiamr.html

[Q53] 按条件删除
来源：http://hz.birdmap.top/gtxzqfetau.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtfcyvtjvg.html

[Q54] 清空表
来源：http://hz.pengpengdd.cyou/gtfnwjqhni.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gttfnxbtoy.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtofkzkquw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtxcnnfpzc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daria6918.cn/gtgkyiwrpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gtsbagdoil.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtizditdga.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtqkofdcyv.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtheydcash.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tian-w.cn/gtcumtuifz.html

[Q59] 分组内累计
来源：http://hz.shangyingyoupin.top/gtuzgbgjzc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtdovrmpgj.html

[Q60] 取上一行 / 下一行
来源：http://hz.ybcxt.top/gtehpgfzqb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtynvdrxuf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.haohaochexian.top/gtnskhqcyc.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtrnquxihs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cheryme.top/gtyppjgxib.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtgglhqrhw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtueznhmxb.html

[Q63] 开启事务
来源：http://hz.gogol.net.cn/gtfwujaama.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shangyingyoupin.top/gtfwifsrwh.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtxucbmwhc.html

COMMIT;
来源：http://hz.hammf.cn/gtngxcahrm.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangtech.top/gtaspceoxu.html

ROLLBACK;
来源：http://hz.dashuyun.cn/gtusnzjfwf.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gtqfnsdzhf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxinkj.top/gthpsxgzjl.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtsgrjagxo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gtvfxrzxha.html

[Q68] 保存点
来源：http://hz.shangyingyoupin.top/gtdtlpkjgx.html

SAVEPOINT sp1;
来源：http://hz.feifeiyinyue.top/gtyiioyezb.html

ROLLBACK TO sp1;
来源：http://hz.haohaochexian.top/gtssbklqup.html

[Q69] 查看执行计划
来源：http://hz.redwolf501.top/gtzfjypkdw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gtshwvqjtb.html

[Q70] 更新统计信息
来源：http://hz.yj202588.top/gtobcmzzyr.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtbsdawnid.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtcnjfoeei.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtxxptwrpw.html

[Q72] 查看索引
来源：http://hz.shzxlz.cn/gtnrtukqxu.html

SHOW INDEX FROM users;
来源：http://hz.sxryk.cn/gteyfjtaze.html

[Q73] 查看表状态
来源：http://hz.nwbrower.top/gtpdyfqdzd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtlvkowyim.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtxwdgekxv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtzxrpctre.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtlhpctvrb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tian-w.cn/gtsdtvdegk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtvpwhkrzl.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtdqhhwqju.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gtvjcvxszm.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gtmrwqbjdi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtembrkybf.html

[Q78] 当前时间
来源：http://hz.cucudq.cn/gtqigogeyr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.c1oappe.top/gtcvgwwajd.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtdjtqglto.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.9152youxi.cn/gtyeotaqze.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtloghobaw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtebpecblh.html

[Q81] 字符串替换
来源：http://hz.andypj.xyz/gtfqfozmak.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtujiuzzqs.html

[Q82] 字符长度与字节长度
来源：http://hz.ybcxt.top/gtbswruilw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtjkaqxpiw.html

[Q83] 大小写转换
来源：http://hz.zhoulong.xyz/gtwrriphze.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtyyrfiowk.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gtayrgrqmh.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtckoaegbl.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtgmrkgnyf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxuanxn.top/gtlaiocblo.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgfzy.top/gtqdfcfrpp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtxfbgqhac.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtfnbitjef.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtbrawybfg.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtysmyaaqz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ywan-chungtsiang.top/gtcbwqwsrg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtfdgzqcgk.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtxcjmudye.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gtlfbexakq.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtvrzdxnii.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtpwqsrgih.html

================================================================================
来源：http://hz.aizwys.cn/gtbscuirqr.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtjakmftzm.html

================================================================================
来源：http://hz.redwolf501.top/gtjmlqdzgn.html

[R01] shebang 与严格模式
来源：http://hz.ppjwa.cn/gtchixttsn.html

#!/usr/bin/env bash
来源：http://hz.daria6918.cn/gtzsafdcdq.html

set -euo pipefail
来源：http://hz.hysaishi.cn/gtssrshaqx.html

[R02] 变量赋值与使用
来源：http://hz.52xcode.cn/gtjvywyulg.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtajdskqrz.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtvfsdzkob.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gtytndwfzt.html

[R04] 位置参数
来源：http://hz.52xcode.cn/gtxtmweozn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtrmjchdlw.html

[R05] 参数默认值
来源：http://hz.iojbl.cn/gtkzkddetq.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gtymaafbqg.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtvuyzxaqr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gthmkvvgce.html

[R07] if 判断文件
来源：http://hz.sweek.top/gtsjnaczpn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtxhdgcnbl.html

[R08] 数值比较
来源：http://hz.zhiwuduotai.top/gtwgpuphds.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj202588.top/gtponqyija.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtfunfhzjl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenlongwang.top/gtymwervls.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtrjkgmfln.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gttxszrbdq.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gttwtmqqmc.html

case "$1" in
来源：http://hz.daxiang520.top/gtgqwgsfnp.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtiqwdcgpd.html

stop)  echo "停止" ;;
来源：http://hz.316326.xyz/gtlbaliheh.html

*)     echo "未知命令" ;;
来源：http://hz.tianlin.xyz/gtzsqqnejk.html


<!-- 参考信息 -->