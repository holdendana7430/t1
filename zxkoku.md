代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.xylfe.cn/gtsadlqfvi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtluowufux.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtdquykdpp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtuxdfirgu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ehwqpu.com/gtkszublsy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigfzy.top/gtpkgyrnbj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.mhx1999.top/gtafpptirw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gogol.net.cn/gtdmauxxbr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtvbdjmdrg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tanke756.top/gtbznequxi.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtejllxeee.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtnaecvggl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtxhjxitoh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gteeqwsuge.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtdptjlrgv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.bjfxy.top/gtdtbnpadg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtfcumoxlj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gtnyfluhrn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtyydwbfkw.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtakabfnwr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtcyovbynk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtrwpiydki.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtiaufmwyn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtubonthsc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtpfpruwsu.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gttzmosjgb.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtodzilkrh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtlunqelyu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtokiyefcg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ivvv.top/gtfgwsomxc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtgdzgoyys.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtaqsbphun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtnklbgurr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtvvzonwlc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.andypj.xyz/gtupqeupxv.html

Ruby: a == b
来源：http://hz.gotoacloud.top/gtlskcysxh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tanke756.top/gtexcxvdtk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gtdsrybcch.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.quarkkingdee.top/gtasmpupss.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtqjrexvpy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fzhhl.top/gtxlczpidm.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtijkbnauj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xinyue.icu/gtqumkuksn.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtqgkjandn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.316326.xyz/gtyfjmspdx.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtajxzxhdj.html

[P07] 防抖与节流
来源：http://hz.jqgufenzy.top/gtfylnngxw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.0kj1m.cn/gtlhwzidgi.html

PHP:  // 手写时间戳比较
来源：http://hz.xinyue.icu/gtpanclrgr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtlkkibytf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtijmvtyff.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zycfv.cn/gtofpdojtr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.svipenyu.cn/gtxxlaqefd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gtagvaiuvs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.svipenyu.cn/gtwekkeias.html

[P08] 处理浮点精度问题
来源：http://hz.andypj.xyz/gtjcmptekn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtqbwhmcdw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtyilbtmoj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gogol.net.cn/gtejxgpqnw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtgbdtntjg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtwpidtqlg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cdnleiting.top/gtzxzctgmi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxuanxn.top/gtemitokeo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gthlwpsmix.html

================================================================================
来源：http://hz.zhongyouzk.top/gtphwamidr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtzbteebtm.html

================================================================================
来源：http://hz.xziqi.cn/gtkdleqvqy.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtezoatoaz.html

CREATE TABLE users (
来源：http://hz.yvedp.cn/gtwaqwagsh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtoiqxazlq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sxryk.cn/gtruxtwkig.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ivvv.top/gtnfyphmqd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.quarkkingdee.top/gttmawjsip.html

);
来源：http://hz.gzhubu.top/gtbbuzmots.html

[Q02] 创建带外键的表
来源：http://hz.hnxiangtu.top/gtmlbzlzya.html

CREATE TABLE orders (
来源：http://hz.xuanzx.com/gtoulbzewx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtmxieyhxu.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gtkodstopc.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtusvaaeeo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gtymylspdk.html

);
来源：http://hz.nwbrower.top/gtukptjcfr.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtvcimqsnm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtpafeoaym.html

[Q04] 修改列类型
来源：http://hz.meibo888.top/gtjuduvdjy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jianghu66.top/gtzgvgdanb.html

[Q05] 重命名列
来源：http://hz.jiagoushi.top/gtcevrzbjf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtxiffkbez.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtvypikohq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pycfn.com/gttnxmbsaa.html

[Q07] 删除表
来源：http://hz.hongshengwenyu.top/gtnborisza.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daxiang520.top/gtafdlvtoi.html

[Q08] 创建普通索引
来源：http://hz.jqgfzy.top/gtlpynjxsq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtcculfehs.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtygowbnag.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jianghu66.top/gtlukbehgc.html

[Q10] 插入单行
来源：http://hz.snrcjt.cn/gtzetfkxze.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenjidiqi.icu/gtailddjpf.html

[Q11] 一次插入多行
来源：http://hz.hongshengwenyu.top/gttflfgznu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgfzy.top/gtywzkvsiq.html

[Q12] 插入后取自增 ID
来源：http://hz.yueranfly.top/gtltbagkxs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtnvpzldjt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtndpxkmnx.html

[Q13] 忽略重复插入
来源：http://hz.ydjk.org.cn/gtgefzrhgu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guannengcc.top/gtxehswamn.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtrvugqlib.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydzc1.top/gtbrvfkrvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtdxbobqrs.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtmohjstes.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtwybklkjp.html

[Q16] 查询指定列
来源：http://hz.ehwqpu.com/gtsotrckki.html

SELECT id, name FROM users;
来源：http://hz.chenjidiqi.icu/gtjljnthqx.html

[Q17] 条件查询
来源：http://hz.tian-w.cn/gtmjhizovm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtkjhwqotx.html

[Q18] 模糊匹配
来源：http://hz.redwolf501.top/gtevncytmr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gtzuhdcfqb.html

[Q19] 范围查询
来源：http://hz.yuxming.cn/gtctrxlbts.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtssuerqdm.html

[Q20] IN 列表
来源：http://hz.hammf.cn/gtxnokeaso.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtaievtfji.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtpyzlxria.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hongshengwenyu.top/gtuvhdjnhm.html

[Q22] 排序
来源：http://hz.zhengqikj.top/gtfoahzrpl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtqpilhyoj.html

[Q23] 分页
来源：http://hz.yj20258.top/gtcrxhplxh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtyfqgmddd.html

[Q24] 去重
来源：http://hz.chenjidiqi.icu/gtbnfjfssy.html

SELECT DISTINCT city FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtyspvwapi.html

[Q25] 只取前 N 条
来源：http://hz.cdnleiting.top/gtetqeyytr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gtmnlcpzzz.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtmvqaiiro.html

SELECT COUNT(*) FROM users;
来源：http://hz.gaohongyu789.top/gtvlxzxlrh.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtnqwqobrq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinghuilouyu.cn/gthchwgqyv.html

[Q28] 求和与平均
来源：http://hz.quarkkingdee.top/gthazdorht.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtfssxikrg.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtutedmpdb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yvedp.cn/gtxluztqwg.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtzycizyhi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtvwaaciou.html

[Q31] 分组后过滤
来源：http://hz.jyoumei.cn/gtyszfqgee.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtsiqluxnw.html

[Q32] 分组拼接字符串
来源：http://hz.hysaishi.cn/gtzqtmjuca.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtjrmpadrr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxuanxn.top/gtxhxcwskz.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtjbujfwne.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtzgtxwiqt.html

[Q34] 每组取第一条
来源：http://hz.xziqi.cn/gtclwavgnj.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtdijvtnql.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daria6918.cn/gtgljkkdfm.html

) t WHERE rn = 1;
来源：http://hz.c1oappe.top/gtwynqviup.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtvionuvll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtufkcipis.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtzezvhpzl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtkvezyeiy.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gtalxsbxld.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sysykeji.top/gtkbjuvxei.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtfcufdqad.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtgratmtjg.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtevaulskc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtfqyjjjxn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtbtnhqkto.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtdlxtkumd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gogol.net.cn/gthuvmimbp.html

[Q41] 多表连接
来源：http://hz.quarkkingdee.top/gtotwqgdrw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nwbrower.top/gtgihjeuhn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yonumen.top/gtsajqmwcn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtxscgdris.html

[Q42] 连接条件附加过滤
来源：http://hz.svipenyu.cn/gtqmmsbuvr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtprftvaje.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gttyphpnpc.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gtupxbakvx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shzxlz.cn/gttqrzcumt.html

[Q44] IN 子查询
来源：http://hz.cqqwz.cn/gtqsovmiqp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zycfv.cn/gtngwhoqzu.html

[Q45] EXISTS 判断存在
来源：http://hz.fzhhl.top/gtlkmnidad.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtleoapxaz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gthwxwimha.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtfiukqpka.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtkrrppbpl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtsnczuksd.html

[Q48] CTE 公用表表达式
来源：http://hz.hnxiangtu.top/gtoxvrfazp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ybcxt.top/gtocqhgfzq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gotoacloud.top/gtjgyuefnp.html

[Q49] 更新单行
来源：http://hz.0kj1m.cn/gtbkaezpwj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtpvnagkdo.html

[Q50] 批量更新
来源：http://hz.mhx1999.top/gtceoqzubx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtmzbchlvb.html

[Q51] 用子查询更新
来源：http://hz.yj20258888.top/gtoowvyyln.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtpujcmeix.html

[Q52] 删除指定行
来源：http://hz.c1oappe.top/gtbcmsmlek.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xinyue.icu/gtrtkalzde.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtqkjfewnl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ybcxt.top/gtbwwdwlgx.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtqefxrpvz.html

TRUNCATE TABLE logs;
来源：http://hz.redwolf501.top/gthnubvpmz.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258888.top/gtggowbeoz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhijiandao.cn/gtijfbbdzj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dianchejie.cn/gtzbkzrxki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtgzjuuwcc.html

[Q57] 行号
来源：http://hz.redwolf501.top/gtoazufziu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yanxiufei.cn/gtdflqrubx.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtsoslayrd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtwxrhidym.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtufvcpgdw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtfkqvdspl.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gtkqgirrct.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtgyegkpaw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dashuyun.cn/gtzbfwsapt.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gtykehdiyg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ehwqpu.com/gtuqnxcsrz.html

[Q62] 分组占比
来源：http://hz.jianghu66.top/gtxaqfhytp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtccsihpuz.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gtabjfayyb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtmdpqyocs.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gththlqhml.html

COMMIT;
来源：http://hz.zhaomingkeji.xyz/gtditbqrnb.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtnvnixxdi.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtyqhcwjyd.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtnhhzbyjd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtfagcuisy.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtotpxtmvp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tianlin.xyz/gtaefqlqyh.html

[Q68] 保存点
来源：http://hz.yj20258888.top/gtgbcwjtiw.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gtldmkmeho.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtothnvnau.html

[Q69] 查看执行计划
来源：http://hz.zhiwuduotai.top/gtbphszznl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtishzpzni.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtioovijaa.html

ANALYZE TABLE users;
来源：http://hz.jinqigufen.top/gtienxjblx.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gtrbwvqbvc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtucgdxzjb.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtuqqkrejf.html

SHOW INDEX FROM users;
来源：http://hz.cucudq.cn/gtakziwija.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtewyqonmq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtgrouluea.html

[Q74] 强制使用索引
来源：http://hz.aibaodan.cn/gtxdxwwtza.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nwbrower.top/gtbbdcgeqo.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtlcwxbqxh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gtvkkwzszx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtbtlougux.html

[Q76] 按天统计
来源：http://hz.nanxuanxn.top/gtyrdreufl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtztpsxvrp.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtajpshube.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guowangkeji.top/gtnrsloojd.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gtzgrylqng.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hammf.cn/gtlpfbeeoq.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtfqbqwzlo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtilnuphms.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtfjqadrig.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gthdzlfbzu.html

[Q81] 字符串替换
来源：http://hz.xuanzx.com/gtdpinflkc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtmfollrqt.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtavlmbpqx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gttrrpxxbi.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtuqomlsst.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tianlin.xyz/gtrnsbwrse.html

[Q84] 去除首尾空格
来源：http://hz.jianghu66.top/gtmshykvuz.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtmtrbkjmp.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtihmantcx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtfljkmcox.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtwkbujzvu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gthwtvpsdg.html

[Q87] JSON 字段做条件
来源：http://hz.cucudq.cn/gtmniexpth.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtuptivcpe.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gthsaeeinp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhixingplan.top/gtsgngzlcj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cdnleiting.top/gteeepwgwl.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtwletxrdk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.316326.xyz/gtksnxprpo.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtdepdxpmj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtltcfhnvj.html

================================================================================
来源：http://hz.hnqzz.top/gtgjfijkwx.html

R. Bash 专题
来源：http://hz.yj20258.top/gtxqhgkijh.html

================================================================================
来源：http://hz.nanxinkj.top/gtqhvfljqq.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtrotomson.html

#!/usr/bin/env bash
来源：http://hz.hfpthk.cn/gtltcawajv.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtpboufybd.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtrfbjvecb.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtkythrunw.html

[R03] 只读变量
来源：http://hz.sufxvd.cn/gtfjpsbyra.html

readonly PI=3.14
来源：http://hz.wangdashe.top/gtusrufiea.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtpoyzcubz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hywenlv.cn/gttddzdmcy.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtaozokcme.html

name="${1:-default}"
来源：http://hz.nanxinkj.top/gtkwjisgbi.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtxaskomfu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gtjirewvgg.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtoplmyrqc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtvjqfipua.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gtdeyafsdm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtwwkvpcpc.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtaytyrqnz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtfogrpqzf.html

[R10] 正则匹配
来源：http://hz.yvedp.cn/gtesqhcmsn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtiepymylu.html

[R11] case 多分支
来源：http://hz.bjfxy.top/gtvaycrtxu.html

case "$1" in
来源：http://hz.daxiang520.top/gtbfeifalt.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtgcwwlccn.html

stop)  echo "停止" ;;
来源：http://hz.jinghuilouyu.cn/gtblksadiw.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangtech.top/gtmllbymxy.html


<!-- 参考信息 -->