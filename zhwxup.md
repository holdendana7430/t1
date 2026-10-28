代发 wailian999

[P01] 生成 UUID
来源：http://hz.fzhhl.top/gtavdmrewb.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gtaktjpftm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtxcbacunw.html

JS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtipxcdlcs.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtdrfqestf.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtjmvhgbfs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhongyouzk.top/gthakycdbb.html

Ruby: SecureRandom.uuid
来源：http://hz.guannengcc.top/gtykwlhbia.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtsdlstkwg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinyuanbaomall.cn/gtxtaubfis.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtbgowwavj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gteqebjufs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jianghu66.top/gtvzstosqn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtdcetsuzw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gogol.net.cn/gtprkoclpj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gttaxxdzct.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtrgierpnr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ehwqpu.com/gttsjvmddu.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtaigqrodw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sysykeji.top/gtuzxmstsz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gttiogwkbp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtvsdgldzk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtxqwuvpsy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenjidiqi.icu/gtixhxhhgi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangtech.top/gthizyzcti.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gtgrwhcgjo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtcwimouji.html

[P04] 求长度
来源：http://hz.ppjwa.cn/gtmwlanpoq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gtvcymccps.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtnhozjnso.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtybhpnwrm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.iojbl.cn/gtydlaexqa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jlsjyb.cn/gtrxxtwpbk.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtkbpvjwqy.html

Ruby: x.length;  x.size
来源：http://hz.yj202588.top/gtzzjghcct.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtlxbvzysy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuanzx.com/gtuydisfxp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.0kj1m.cn/gthqygppjt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtwfwvozbo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtafbdejzn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtbnnuetgd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gthanagbef.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtwgwfhzih.html

Ruby: a == b
来源：http://hz.pycfn.com/gtggjsvfvx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gthfkixizq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtqjtsazzy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuetiantiany.cn/gteslcjtup.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtmnxhatft.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenlongwang.top/gtylibolkw.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtmfsusvkq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtkzjnupch.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtbwzgxmrc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gtcylnclzc.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtxnzjygqw.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtomyojadv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtsscqrwye.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgufenzy.top/gtodfekyoq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gteruxkduh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtqwsgcaec.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxuanxn.top/gtuvrimkyq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gtqfvpudkm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xziqi.cn/gtdkkidnnz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guannengcc.top/gtyhebkzlk.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gtflxynpxh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangshuangyany.cn/gtsdstouye.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtsmkntgrx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.smart0.xyz/gtudhnhrey.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ppjwa.cn/gtzuwviakv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtxcboipew.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhongyouzk.top/gtkvwmfziz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gzhubu.top/gtychskkxh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtzpseapva.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtieyvkiwg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gtlpdrpgms.html

================================================================================
来源：http://hz.ybcxt.top/gtjbnkkshj.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtttlscrry.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtqffzazho.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gttmwovcwf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ydzc1.top/gtfqmcuqsj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtglyhvgbm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.haohaochexian.top/gtblejbayp.html

);
来源：http://hz.dianchejie.cn/gtowbtomqi.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtkfpxbifn.html

CREATE TABLE orders (
来源：http://hz.yanxiufei.cn/gtaoeiyzfl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtjmlvhqdu.html

user_id INT NOT NULL,
来源：http://hz.kuanghao11.cn/gtwggorqph.html

amount DECIMAL(10, 2),
来源：http://hz.xuetiantiany.cn/gtnwzpbcvz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aizwys.cn/gttqlsmjfz.html

);
来源：http://hz.iojbl.cn/gtljohvjjo.html

[Q03] 增加列
来源：http://hz.jiagoushi.top/gtfgwxiuqp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gtrzjhpxff.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gttamgskyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daxiang520.top/gtjapwxreo.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gtlbcdorpt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.redwolf501.top/gtntxhztpu.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtxkwpyarc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xinyue.icu/gtgeyxridw.html

[Q07] 删除表
来源：http://hz.xziqi.cn/gtmtfwelqj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtbowyulqy.html

[Q08] 创建普通索引
来源：http://hz.9152youxi.cn/gtjemkhqow.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gtqbosslgn.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gtqhphjnnj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtvwsncsyo.html

[Q10] 插入单行
来源：http://hz.chenzaomai.com/gtmhgondrx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtaqctxwbr.html

[Q11] 一次插入多行
来源：http://hz.birdmap.top/gtcbwmxkhi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtxpjayuoo.html

[Q12] 插入后取自增 ID
来源：http://hz.cashguo.top/gtnylywojr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jyoumei.cn/gtsuxzguad.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gttomonkmj.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gtrwmwolts.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aibaodan.cn/gtdkynotgz.html

[Q14] 存在则更新（upsert）
来源：http://hz.redwolf501.top/gtjojfljct.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gthnzccjrj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuxming.cn/gtecflrvln.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gtyllguahl.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtvjgrwggj.html

[Q16] 查询指定列
来源：http://hz.havefunace.top/gtloxvhcpe.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtrjekutkj.html

[Q17] 条件查询
来源：http://hz.gotoacloud.top/gtynpgrplr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gtaswzelfp.html

[Q18] 模糊匹配
来源：http://hz.hongshengwenyu.top/gtlyhqvgwo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtdcvwwqsz.html

[Q19] 范围查询
来源：http://hz.jlsjyb.cn/gtbbviafdk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtkvaqspqh.html

[Q20] IN 列表
来源：http://hz.smart0.xyz/gtwgpdaveb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dianchejie.cn/gtehxrtobl.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtblccuxyj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guannengcc.top/gtckzebwys.html

[Q22] 排序
来源：http://hz.zhijiandao.cn/gtqjfzavdc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenzaomai.com/gtwmztitqv.html

[Q23] 分页
来源：http://hz.nanxinkj.top/gtnueqcqkn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxinkj.top/gtfwlvzzei.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtctnczorb.html

SELECT DISTINCT city FROM users;
来源：http://hz.cqqwz.cn/gtinvfkbgz.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtincanshc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fengsongda.top/gtcbyysokp.html

[Q26] 计数
来源：http://hz.nanxinkj.top/gtidnasaai.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtancdbdpq.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtixcyowgr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxinkj.top/gtsjoewcba.html

[Q28] 求和与平均
来源：http://hz.sufxvd.cn/gtkvnvkqwf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gttpnnxqyd.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gtenxzomgn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bjfxy.top/gtzlvyayti.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtfvozcwtx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtuisohzsi.html

[Q31] 分组后过滤
来源：http://hz.tian-w.cn/gtcqlvfabh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xylfe.cn/gtwxttmrgi.html

[Q32] 分组拼接字符串
来源：http://hz.yangfankeji.com/gtogjazurs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtgypibkfe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shangyingyoupin.top/gtprjcqxof.html

[Q33] 多列分组
来源：http://hz.zhaomingkeji.xyz/gtonaldbdo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtpbqynxpm.html

[Q34] 每组取第一条
来源：http://hz.fengsongda.top/gttxorjodu.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtphogidvw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yongpay.top/gtamfbdmro.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtuzhbixom.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtwhfhzvjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtlheomaxq.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gttdqwztge.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtnbcopvwk.html

[Q37] 右连接
来源：http://hz.andypj.xyz/gtetcayysb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cucudq.cn/gtjxvkpgce.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhoulong.xyz/gtfvdfwash.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtkzxlgjvq.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtchnysicc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtrvregmji.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yueranfly.top/gtmwhbziiz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtoudtpbdp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.kuanghao11.cn/gtrhmlndqa.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gticyhntvc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.9152youxi.cn/gtajddaosi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigfzy.top/gteajrzqco.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gtilmslvlz.html

[Q42] 连接条件附加过滤
来源：http://hz.ywan-chungtsiang.top/gthvauedbj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxuanxn.top/gthztlvads.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gtikqnmpet.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtzxsrbdsd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xylfe.cn/gtmturowke.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtmisympci.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhongyouzk.top/gtoruvfkzt.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gtmfoclhfk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtjmgaytaw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtpefnmsrh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtimtypzra.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gthmlignnx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gtafatpclh.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtlhxlqlqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtdzxpeqjh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gttehhigse.html

[Q49] 更新单行
来源：http://hz.cdnleiting.top/gtzhkkttay.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtkzuqnhui.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtauszifql.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zdqjudy.top/gtkgtblqre.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtjvvbtozt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.birdmap.top/gtosyhryvs.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtwuthkzwb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hysaishi.cn/gtajnugcmb.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtwdxieexe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zdqjudy.top/gtpofeuelr.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtothdohfn.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gthauagznj.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtcizomzou.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtisnligip.html

[Q56] 密集排名（并列不占位）
来源：http://hz.iojbl.cn/gtvtgyimwx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dianchejie.cn/gtyeykoxkh.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gtynlvoaec.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtwgyrbrcs.html

[Q58] 累计求和
来源：http://hz.yongpay.top/gtfadwjazl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fengsongda.top/gtdogrsdnc.html

[Q59] 分组内累计
来源：http://hz.tian-w.cn/gtiflcbmuf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtmktjtxve.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtvkubiywr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.andypj.xyz/gtnsbsmjxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gtriejwqsw.html

[Q61] 移动平均
来源：http://hz.xziqi.cn/gttwivrepi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtmybdchrt.html

[Q62] 分组占比
来源：http://hz.hongshengwenyu.top/gtadzbtdew.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtjvrkcvbz.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtruudogyd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shuidangran.top/gtjqpwlnqu.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtvzbxxkte.html

COMMIT;
来源：http://hz.yuanzhike.top/gtozcsfbiu.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtyxrqdeke.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtrnahhzjq.html

[Q66] 行锁查询
来源：http://hz.9152youxi.cn/gtuciydaow.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtuchbkytt.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtdfmohzuz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.fengsongda.top/gthnuahntl.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtklbgdzhq.html

SAVEPOINT sp1;
来源：http://hz.xuanzx.com/gtoqbajieh.html

ROLLBACK TO sp1;
来源：http://hz.zhengqikj.top/gtsyabuhql.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gtqlbonpmm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtbgevpgza.html

[Q70] 更新统计信息
来源：http://hz.yj202588.top/gtrnurjzlj.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gtgyjsswgv.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtvpbtxpwh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtrgmieskg.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gttzbfahul.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtcecimsoq.html

[Q73] 查看表状态
来源：http://hz.vqdsnc.cn/gtaiyjuhhp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtedkyrbtt.html

[Q74] 强制使用索引
来源：http://hz.andypj.xyz/gtcubytdqf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gtrjtvfisg.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gtaflhqptw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ivvv.top/gtiyeppaen.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtlxoojzez.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtjseqqoxg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtvdqymxwm.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtnvkipexo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aibaodan.cn/gtlnmevyxj.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtlcfoxbir.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtlxbtzyuc.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtvsziqibe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gtxuaqguja.html

[Q80] 字符串截取
来源：http://hz.52xcode.cn/gtqsballjd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtnmvaeqbl.html

[Q81] 字符串替换
来源：http://hz.cdnleiting.top/gtrvorbzoz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuanzx.com/gtivnrnymv.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtwuzfhalh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.meibo888.top/gtmpvzlyqs.html

[Q83] 大小写转换
来源：http://hz.yuxming.cn/gtdfyqqxvn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtzraolpfp.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtwsmujdzq.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuanzx.com/gtzbpqpkha.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtxdiighbr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhengqikj.top/gtvzlpivoo.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gthuxckvmx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtjetetkuu.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtzdbkrnxr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtyzivwbau.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtnbwxvcsy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtjccfjokq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhengqikj.top/gtfymmuvjk.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtihdrxfhi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dashuyun.cn/gtxhdoyzym.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtgiuuyauu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xinyue.icu/gtwrzybyhr.html

================================================================================
来源：http://hz.xinyue.icu/gtqtebvioc.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtrqgbmxis.html

================================================================================
来源：http://hz.jinqigfzy.top/gthabekwco.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gtqnhajjzw.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtfucnezrh.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtpxbpenlz.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gtsouthdsq.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtcpugjnoj.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtaohmsdjz.html

readonly PI=3.14
来源：http://hz.fzhhl.top/gttbaxqpie.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtdwxejqdb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtjsdcvnkj.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtnynvsshk.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtwufsdjmj.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtmrfwipys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtkqcgvpuv.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtwhfcaztn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hammf.cn/gttmmljcxh.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtxljwmeri.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.svipenyu.cn/gtbbrwfgnl.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtdqzwuqgs.html


<!-- 参考信息 -->