代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtyztrydqe.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtzkuxqgfu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtgqizpjnl.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtmlpwxepx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sufxvd.cn/gtvaqkamog.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pycfn.com/gtaevjvmre.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtiefpzcfe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtqlvzlrih.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtzzdsccnk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtonntdrxk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuanzhike.top/gtfwbzosph.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yanxiufei.cn/gtzpxctyrp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtrgtthdew.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daxiang520.top/gtytepobwb.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtqfsqswpe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.mhx1999.top/gtdhckvyub.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.snrcjt.cn/gtxsvdubcj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtpxdhupps.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtiuutmpuw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hfpthk.cn/gtiaxrsegr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtxquylwdp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tanke756.top/gtgpcslttd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gttyesrnee.html

[P04] 求长度
来源：http://hz.fzhhl.top/gtpheimfun.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtypmspiyl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtpsgshyho.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtjfvgepqh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtqbvfqbka.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gtrzgsekcq.html

Go:   len(arr);  len(m)
来源：http://hz.yuxming.cn/gttqksombb.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtgluztqnh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtoocsafae.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuanzhike.top/gtrwpkiyin.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtyowtgdzc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.smart0.xyz/gtkxxdoyvk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtleqgtbss.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtcwtewics.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtppenwitz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtmhnistvr.html

Ruby: a == b
来源：http://hz.xuetiantiany.cn/gtpkbkighl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.quarkkingdee.top/gtvpphjlmp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.316326.xyz/gtwoiaqexb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yangfankeji.com/gttsekgevo.html

PHP:  if (empty($x)) {}
来源：http://hz.0kj1m.cn/gtfbovabhc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gtfwmrffbn.html

TS:   if (x == null) {}
来源：http://hz.feifeiyinyue.top/gtzaqhyvpy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtdpequobu.html

Go:   if x == nil {}
来源：http://hz.9152youxi.cn/gtpqljywzv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtlaublevh.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtmsbtpkkk.html

[P07] 防抖与节流
来源：http://hz.xinyue.icu/gtzvlofhbw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.meibo888.top/gtycfuljrn.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtwnkbqwxj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtcxjxoeqc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtkhwcsifr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtshnpcaqq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtfjnoprmy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cheryme.top/gtaxudzuhe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtswunvpnw.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtomydfodx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ywan-chungtsiang.top/gtgnnmsxlm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cucudq.cn/gtupyzkdyg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jyoumei.cn/gtpmabgcut.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.snrcjt.cn/gtcmdlvypk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinghuilouyu.cn/gtenkinwkx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.feifeiyinyue.top/gtckxleuat.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xylfe.cn/gtddohttkp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtnnpqakun.html

================================================================================
来源：http://hz.jqgufenzy.top/gtctezavrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gtbofzsbnh.html

================================================================================
来源：http://hz.xylfe.cn/gthwfbctwa.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtidjtlelx.html

CREATE TABLE users (
来源：http://hz.jqgfzy.top/gtqqhnmvrj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gttfniafet.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258888.top/gtwrwvuxkn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gtylwpykbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtgiipeukt.html

);
来源：http://hz.gogol.net.cn/gtaelyifge.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtsrzynfri.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtdksirwjh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtlnsoizgp.html

user_id INT NOT NULL,
来源：http://hz.tanke756.top/gtjoinutmj.html

amount DECIMAL(10, 2),
来源：http://hz.shangyingyoupin.top/gtteqldysj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtkqtdpmcf.html

);
来源：http://hz.jinyuanbaomall.cn/gtppwuhyuk.html

[Q03] 增加列
来源：http://hz.hysaishi.cn/gtrzusrmmu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tanke756.top/gturelqffc.html

[Q04] 修改列类型
来源：http://hz.nanxuanxn.top/gtkhdtvsna.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgufenzy.top/gtmrmwsyxb.html

[Q05] 重命名列
来源：http://hz.nanxuanxn.top/gtrezmgwxc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtyxgvhgjb.html

[Q06] 删除列
来源：http://hz.chenzaomai.com/gtxiluhkmu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtdjefjppc.html

[Q07] 删除表
来源：http://hz.yuanzhike.top/gtxfxkpkoj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zycfv.cn/gtohyenpjb.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtzcdoszjr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtqikpabfy.html

[Q09] 创建唯一索引
来源：http://hz.havefunace.top/gtnxfufvux.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gthrxmaqgj.html

[Q10] 插入单行
来源：http://hz.iojbl.cn/gtmovxvmvc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtptqwviih.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gtjunurbkn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aibaodan.cn/gtiyrklmhc.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtwpguvyvi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gthcuremxp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtylufolwf.html

[Q13] 忽略重复插入
来源：http://hz.hongshengwenyu.top/gtarsvevub.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gtgnajhnco.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258888.top/gtfopwebiy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jyoumei.cn/gthajexvra.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gttudgeesu.html

[Q15] 查询全部
来源：http://hz.nanxinkj.top/gtxerajhod.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtzpbkyhva.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gtnqpbvldk.html

SELECT id, name FROM users;
来源：http://hz.yangfankeji.com/gtbbwslnep.html

[Q17] 条件查询
来源：http://hz.hysaishi.cn/gtqzzcwjwy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinghuilouyu.cn/gtjkvkyxtj.html

[Q18] 模糊匹配
来源：http://hz.sweek.top/gtwqvpozgf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.quarkkingdee.top/gtfyhljpkh.html

[Q19] 范围查询
来源：http://hz.hywenlv.cn/gtmkywaepz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.iojbl.cn/gtcqwodplu.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gtojnoesys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtlnzddkiu.html

[Q21] 空值判断
来源：http://hz.fengsongda.top/gtqrmxrycr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydjk.org.cn/gtgbscppkl.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtvzkjwuno.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yonumen.top/gthtvznjrh.html

[Q23] 分页
来源：http://hz.cdnleiting.top/gthktgdztf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydjk.org.cn/gtjakabfjk.html

[Q24] 去重
来源：http://hz.meibo888.top/gtthwtfvup.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gtspdenofp.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtdtkaewvx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtkescylbj.html

[Q26] 计数
来源：http://hz.cucudq.cn/gtfanefaqw.html

SELECT COUNT(*) FROM users;
来源：http://hz.jiagoushi.top/gtgmpbncvv.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtiermxcgv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gotoacloud.top/gtluldqxsz.html

[Q28] 求和与平均
来源：http://hz.shuidangran.top/gtdzvmgwtc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aibaodan.cn/gttvhwmesy.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtzjvnielf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jiagoushi.top/gtrcomkuqb.html

[Q30] 分组统计
来源：http://hz.ppjwa.cn/gttpgxkjfz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtpwwtscru.html

[Q31] 分组后过滤
来源：http://hz.daria6918.cn/gtcwyswmon.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtvzumldbk.html

[Q32] 分组拼接字符串
来源：http://hz.birdmap.top/gticffqgao.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtlxstmnfu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtkbvwonnq.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtwyjhlyud.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtzzzumftq.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtxbayskiz.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gtyksoneev.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cdnleiting.top/gtlfochhaa.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gterngzvje.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtanzobwlz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtetrsxmdt.html

[Q36] 左连接
来源：http://hz.tanke756.top/gtdvehfwxz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtgfpjlrxo.html

[Q37] 右连接
来源：http://hz.gogol.net.cn/gtwcjwmoha.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gttmyrewkp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gtixruuzdx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gtbzlqpjfa.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtgaulqihp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtongaadbs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cqqwz.cn/gttqczqtsn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.svipenyu.cn/gtauysrtbf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtcjqylmmz.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gttijdzxjx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigufen.top/gtehzsvmpl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtgbtqneni.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtigjazbdo.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtdjusjmcp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgfzy.top/gthxzcjxlq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cucudq.cn/gtsjqmthjh.html

[Q43] 标量子查询
来源：http://hz.cqqwz.cn/gtuydcxqtb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtdgvljlva.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtgfyumzkw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.0kj1m.cn/gtdueoiuor.html

[Q45] EXISTS 判断存在
来源：http://hz.shzxlz.cn/gtoufvyiew.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtuffayfan.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxinkj.top/gtiqqvegkv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtaahxoxeg.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtfuxjzjca.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gzhubu.top/gtdaxfzmih.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtswrcsoom.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtfsstwyty.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtmiyfdfmg.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtqltfiwrp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yueranfly.top/gtwzwmtqxf.html

[Q50] 批量更新
来源：http://hz.quarkkingdee.top/gtwuedavxt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtfxrwfdns.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangkeji.top/gtbqptqajb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.c1oappe.top/gtbhtpgldx.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtuoyipmel.html

DELETE FROM users WHERE id = 10;
来源：http://hz.bjfxy.top/gtqbyjzfcc.html

[Q53] 按条件删除
来源：http://hz.guowangkeji.top/gtwyhgfqvd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtvekclqya.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtfguevslf.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtacthdqdc.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtiecbjakm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtyilfrvau.html

[Q56] 密集排名（并列不占位）
来源：http://hz.andypj.xyz/gtnnhevbkc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fzhhl.top/gtshatfqct.html

[Q57] 行号
来源：http://hz.jianghu66.top/gtezjhsanz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.9152youxi.cn/gtxatdoeoj.html

[Q58] 累计求和
来源：http://hz.gzhubu.top/gtifqguxjr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gogol.net.cn/gtfqncernz.html

[Q59] 分组内累计
来源：http://hz.tanke756.top/gtnduoicst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gtpxlhdluu.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gtfoygbxml.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtfmibknbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhongyouzk.top/gtvcnuhksn.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gtvnyftcbf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinghuilouyu.cn/gticffziub.html

[Q62] 分组占比
来源：http://hz.jinghuilouyu.cn/gtghkbdldl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtffvxdkij.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gtrzknsnos.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtgngigyhh.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtayluacdx.html

COMMIT;
来源：http://hz.fzhhl.top/gtqftwrbvm.html

[Q65] 回滚事务
来源：http://hz.0kj1m.cn/gtpehbqsbk.html

ROLLBACK;
来源：http://hz.chenlongwang.top/gtzthibthz.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtsrkexqob.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sxryk.cn/gtabhdkqvf.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtllatbzuw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nwbrower.top/gtknwzhdbo.html

[Q68] 保存点
来源：http://hz.xuanzx.com/gtwtkryafs.html

SAVEPOINT sp1;
来源：http://hz.52xcode.cn/gtnaasqdue.html

ROLLBACK TO sp1;
来源：http://hz.c1oappe.top/gtaztqjfov.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gteqadlnjs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gtuoqdzysc.html

[Q70] 更新统计信息
来源：http://hz.aizwys.cn/gtlxzihxim.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gteqkvltnf.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtseoavviz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shuidangran.top/gtbqswhnyj.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gteudlacwu.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtxmrjawmc.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtsexbmgec.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jlsjyb.cn/gtdlbbqnlx.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangkeji.top/gtpqvgwxik.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtguihdnrs.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtngrzbonb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtkripcefi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shangyingyoupin.top/gtezgsedqh.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtkrdhuzzh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gtweonhmhe.html

[Q77] 时间加减
来源：http://hz.fzhhl.top/gtmmheuzrj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtzwalnzio.html

[Q78] 当前时间
来源：http://hz.jinqigfzy.top/gtyypxwxuh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtqbkfyqog.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtjpsvnrjo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtwzispxhn.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtsrpxoxbw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtdedmglkn.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtpdpcapvz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.redwolf501.top/gttzeqosqu.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtdawzfmgt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtghotjdtn.html

[Q83] 大小写转换
来源：http://hz.guowangkeji.top/gttmaogxft.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gtdopwswuq.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtlwyfjalu.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnxiangtu.top/gtwdpmwuxz.html

[Q85] 数值取整
来源：http://hz.mhx1999.top/gtxmqnsyzp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtosrergqs.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtdopcsznq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sysykeji.top/gtlgcxhiqm.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtqlqmbrtv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhengqikj.top/gttoruzkam.html

[Q88] 行转列（条件聚合）
来源：http://hz.gzhubu.top/gtigyhzqvh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daria6918.cn/gthooctvph.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinghuilouyu.cn/gtdjexwedp.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtplwmrlho.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yueranfly.top/gtdhxosrww.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtdpmwzpvm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtghkrzyws.html

================================================================================
来源：http://hz.fengsongda.top/gtzrtybxmb.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtgnznehqm.html

================================================================================
来源：http://hz.iojbl.cn/gtkkxgpkmd.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtbspqgxcl.html

#!/usr/bin/env bash
来源：http://hz.chenzaomai.com/gtxkaoocyt.html

set -euo pipefail
来源：http://hz.shangyingyoupin.top/gtszrmvtbe.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtkejxmzxx.html

name="Tom"; echo "$name"
来源：http://hz.zhixingplan.top/gtordtxixl.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtazfhpawh.html

readonly PI=3.14
来源：http://hz.cdnleiting.top/gtndxoqbsu.html

[R04] 位置参数
来源：http://hz.meibo888.top/gtbcnnxazd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtmepswbwd.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtsbiwlejw.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gtoerlzwya.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtnjnbcmgr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.andypj.xyz/gtcelthdgf.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gtovnkweyj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.52xcode.cn/gtnwxwztvi.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gtpvoppocs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenlongwang.top/gtoxliytep.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gthpbttioh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtdwsmhimn.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtruvwatdz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhiwuduotai.top/gtwtfmybrj.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtxiqkbqvt.html


<!-- 参考信息 -->