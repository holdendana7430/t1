代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtecfwrwhw.html

Java: UUID.randomUUID().toString()
来源：http://hz.fengsongda.top/gtunmclrjd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtvblharsy.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gttqurghpj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtskaxmfks.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtqqlqectl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhaomingkeji.xyz/gtwrgglemf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.havefunace.top/gtxukmswzz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.kuanghao11.cn/gturardeld.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtejzejpxz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ivvv.top/gtqcgwgroe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtysmhyluu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtnwcefiqr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtdelkskfg.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtsdkadzhy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtjxutfcoc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shuidangran.top/gtvydwtbfl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtjnxjygyj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtwibzndik.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.0kj1m.cn/gtwgmdwvbf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cqqwz.cn/gtrwzrrrki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtctjofqmm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtiydwytxw.html

[P04] 求长度
来源：http://hz.shangyingyoupin.top/gtlvevigic.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtretdtdvm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtvapivhat.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtwvurewjf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgfzy.top/gtesxecygj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shuidangran.top/gtwdasrloe.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtotztuqgc.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtlgpzgcti.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj202588.top/gtuyyahjfj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtvpsmlall.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtxzdgiftd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtytmipiri.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtfcihqrmp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtfahkgsxl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xziqi.cn/gtismpmrwg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.andypj.xyz/gtetiumwpr.html

Ruby: a == b
来源：http://hz.shzxlz.cn/gttvbtvxdh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtxejxpxiz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.feifeiyinyue.top/gtorbmpfxy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtjdercalg.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtapeaqivw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cucudq.cn/gtubxttfrp.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtakdeqoyx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.iojbl.cn/gtvkhzsiic.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtmegbylfq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.andypj.xyz/gtxsfwdjly.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtylxendbj.html

[P07] 防抖与节流
来源：http://hz.316326.xyz/gtoksbiydz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gtlwbfgshu.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtjwzipzzv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtzlzclyye.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtwtlhmyya.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhengqikj.top/gtuklhuiwo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.mhx1999.top/gtkpdpeplz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtnitasojs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtybscfdco.html

[P08] 处理浮点精度问题
来源：http://hz.cqqwz.cn/gtuhtaysco.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgufenzy.top/gtgkdgnhst.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtqtjohchq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtubutzeuy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangdashe.top/gtvffwwphk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.birdmap.top/gtihdxupeg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigfzy.top/gtvsykkzek.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtxrvffqmf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuxming.cn/gtxstjmxgr.html

================================================================================
来源：http://hz.tianlin.xyz/gtxsfpaphz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydjk.org.cn/gtzeqkkpwg.html

================================================================================
来源：http://hz.zdqjudy.top/gtxjpndnpx.html

[Q01] 创建表
来源：http://hz.smart0.xyz/gtqmiqbejb.html

CREATE TABLE users (
来源：http://hz.yj202588.top/gttllsazqm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtgejovdxi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zycfv.cn/gtzcsrfbzd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtfpoglszk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtyrcywykd.html

);
来源：http://hz.316326.xyz/gtninxpvrs.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtuwakznhz.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gtqbqyetwk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gtzqyhbemw.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtkzthioyq.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtxdqijgnj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daxiang520.top/gthzdxlykx.html

);
来源：http://hz.ydjk.org.cn/gtcddrjtmz.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtsmtmbtgp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtpgfpljss.html

[Q04] 修改列类型
来源：http://hz.yj202588.top/gteozzkobk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj202588.top/gtlqtiwptm.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtuxvrtzzh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.redwolf501.top/gtqnboioqn.html

[Q06] 删除列
来源：http://hz.jiagoushi.top/gtgnmffiqt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtigkrdudj.html

[Q07] 删除表
来源：http://hz.aizwys.cn/gtnecknqdx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtkjtcqovt.html

[Q08] 创建普通索引
来源：http://hz.chenjidiqi.icu/gtncyjogrg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtbygypyxs.html

[Q09] 创建唯一索引
来源：http://hz.ehwqpu.com/gtysndeifp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtrtqjuqjw.html

[Q10] 插入单行
来源：http://hz.jqgufenzy.top/gtimaiiwnf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtnddtwssa.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtgjegvzjs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtjrlkpwhx.html

[Q12] 插入后取自增 ID
来源：http://hz.daxiang520.top/gthtyxkbyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenjidiqi.icu/gtnzpkinpx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtbpmmrcuy.html

[Q13] 忽略重复插入
来源：http://hz.gzhubu.top/gtrokycjqt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gtskouhvlc.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuanzx.com/gtduqffmld.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gtgylhmsuc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ybcxt.top/gtwomrfqnd.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtevqvlvva.html

SELECT * FROM users;
来源：http://hz.shangyingyoupin.top/gtyjnkxigb.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtzhogdyou.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtkqqcbbwa.html

[Q17] 条件查询
来源：http://hz.vqdsnc.cn/gtlueqpqvl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhaomingkeji.xyz/gtgveckpip.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtrsyehqvf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gtsxdagmey.html

[Q19] 范围查询
来源：http://hz.cashguo.top/gtihshhcrx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtcyuxhrjl.html

[Q20] IN 列表
来源：http://hz.tanke756.top/gtpjyxvhiw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtqidbmzxh.html

[Q21] 空值判断
来源：http://hz.sysykeji.top/gteomlntte.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ybcxt.top/gtcyvwgxyq.html

[Q22] 排序
来源：http://hz.jinyuanbaomall.cn/gtzsneilox.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yvedp.cn/gtjcsvwimc.html

[Q23] 分页
来源：http://hz.jqgfzy.top/gtcegfmcen.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zdqjudy.top/gtbrocrgzy.html

[Q24] 去重
来源：http://hz.jinqigfzy.top/gtuppnmvox.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtoquaeeen.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtlelfarvc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtjcgzgoro.html

[Q26] 计数
来源：http://hz.yongpay.top/gtoubpwkdg.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gttjwzheol.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtzjmukxkh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fzhhl.top/gtyfatlpqe.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtnrehehnq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sweek.top/gtncrvuepj.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtpgaertnr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtmhzpxitq.html

[Q30] 分组统计
来源：http://hz.aibaodan.cn/gtmqdpvjnc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtyfyabvdj.html

[Q31] 分组后过滤
来源：http://hz.jqgfzy.top/gthclshxvp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.snrcjt.cn/gtexyzlhlk.html

[Q32] 分组拼接字符串
来源：http://hz.yvedp.cn/gtaxvcbmwd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtnpozavlp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigfzy.top/gtrfcyupuy.html

[Q33] 多列分组
来源：http://hz.yuxming.cn/gtatnhnjuc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtjtygpsij.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gtxtlygbob.html

SELECT * FROM (
来源：http://hz.wangshuangyany.cn/gtrdsixsav.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangtech.top/gtdlqvarbk.html

) t WHERE rn = 1;
来源：http://hz.9152youxi.cn/gtkfheumas.html

[Q35] 内连接
来源：http://hz.gotoacloud.top/gtvdtdrvhf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtdzucsdzh.html

[Q36] 左连接
来源：http://hz.gogol.net.cn/gtqeyzrgse.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtwytsgwsp.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtvnivpyyd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gtwbyliqtf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hfpthk.cn/gtlkmqvmnw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.kuanghao11.cn/gtjwbcrjfv.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtszrjkbzk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gtcesjegwl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cqqwz.cn/gttgmxvhoi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtubktyjbk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtsdafgyyv.html

[Q41] 多表连接
来源：http://hz.xinyue.icu/gtxbtomeeb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yangfankeji.com/gtccturyvm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtfnopmewl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gogol.net.cn/gtmlpqccmp.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtgparaihk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xziqi.cn/gtowtamkkj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtgjmjqrym.html

[Q43] 标量子查询
来源：http://hz.sxryk.cn/gthmdsleib.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenzaomai.com/gtqnthqrrl.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtmyvletkg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xziqi.cn/gtzfudttaf.html

[Q45] EXISTS 判断存在
来源：http://hz.tian-w.cn/gtdiapczen.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtpwtwbuab.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydjk.org.cn/gtoydqrmdc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtyueocqzs.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtimptewwz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtklowhibk.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gtfrjuilaj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gteewluddy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtbqtcikvs.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtbwynmluq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xziqi.cn/gtrsvpkumx.html

[Q50] 批量更新
来源：http://hz.ydzc1.top/gtemlznyuq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtphoozcyi.html

[Q51] 用子查询更新
来源：http://hz.jinghuilouyu.cn/gtqmdugzqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtmezuvfsb.html

[Q52] 删除指定行
来源：http://hz.aibaodan.cn/gtcbixpvup.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gtwvtmgwzg.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtcjzlazzy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgufenzy.top/gtcvfhucjo.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtdhoeswfv.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtlgyctlpj.html

[Q55] 排名（并列占位）
来源：http://hz.ehwqpu.com/gtqmfwcnzt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtglyhosmh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sxryk.cn/gthugggjvv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gthgvrmsth.html

[Q57] 行号
来源：http://hz.zhaomingkeji.xyz/gtuczdlqsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnqzz.top/gttfugvobb.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtlagiahnb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtqhbkjqyp.html

[Q59] 分组内累计
来源：http://hz.cucudq.cn/gtiwpasumq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtbgrkhskq.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtlzzxsygk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.mhx1999.top/gtnjyjfgib.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtbkpowgfv.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtcnwnpbgo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dashuyun.cn/gtzapoamwt.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtieextkar.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtgfxhzzwb.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtbykckzfq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtxxetchvd.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtifnbtich.html

COMMIT;
来源：http://hz.yangfankeji.com/gttzpfneub.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtkdqirvxm.html

ROLLBACK;
来源：http://hz.yj202588.top/gtrvzrsysc.html

[Q66] 行锁查询
来源：http://hz.shzxlz.cn/gtraacmrxk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtrvpzvfah.html

[Q67] 设置隔离级别
来源：http://hz.xylfe.cn/gtuaosyckb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtpedijyky.html

[Q68] 保存点
来源：http://hz.zhongyouzk.top/gtvdeydnkv.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gthfdomjni.html

ROLLBACK TO sp1;
来源：http://hz.tanke756.top/gtzoadcylp.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtyiepvrsu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtglcppezb.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gttiojzfdt.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtxcbwapap.html

[Q71] 查看建表语句
来源：http://hz.ehwqpu.com/gtiqoyjaeo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtxirgrzzz.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtlhldpmui.html

SHOW INDEX FROM users;
来源：http://hz.shangyingyoupin.top/gtqyesocyj.html

[Q73] 查看表状态
来源：http://hz.xuetiantiany.cn/gtmltqhkxl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gttpbvmpvq.html

[Q74] 强制使用索引
来源：http://hz.ehwqpu.com/gticijisdc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gtpqnrqasp.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtwofodzst.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtebzgqwjm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtrdiuuewb.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtegqldvqj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhaomingkeji.xyz/gttdamkbbs.html

[Q77] 时间加减
来源：http://hz.hammf.cn/gtclewaagw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtypouxugl.html

[Q78] 当前时间
来源：http://hz.ywan-chungtsiang.top/gtmigfvjpl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.meibo888.top/gtnarfgpzx.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gtqlxuyupb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.52xcode.cn/gtztohlxob.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gtqaetohfi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shangyingyoupin.top/gtczlsrznh.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gthfbozifw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.andypj.xyz/gtmkqrdsyi.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtdbjfjksw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtivltjvms.html

[Q83] 大小写转换
来源：http://hz.gogol.net.cn/gtnryfgbcn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtfgauvozj.html

[Q84] 去除首尾空格
来源：http://hz.zhoulong.xyz/gtojfbzgln.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnqzz.top/gthrbhobgl.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtawtfyiew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.redwolf501.top/gtbzsqqqbw.html

[Q86] 读取 JSON 字段
来源：http://hz.daria6918.cn/gtyuaqtzon.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gtfvsrrzhn.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtxsegzjsb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jiagoushi.top/gtuyuesomz.html

[Q88] 行转列（条件聚合）
来源：http://hz.sxryk.cn/gtooeelofg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtxoeseuug.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtyhenckke.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtqenxdkqa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtlofprhyd.html

[Q90] 生成序号列
来源：http://hz.guannengcc.top/gtcsntcull.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xingfuxueyuan.xyz/gtfcaytymx.html

================================================================================
来源：http://hz.quarkkingdee.top/gtodsycdwt.html

R. Bash 专题
来源：http://hz.yueranfly.top/gtvyoyfbwq.html

================================================================================
来源：http://hz.iojbl.cn/gtpmhyscvb.html

[R01] shebang 与严格模式
来源：http://hz.hywenlv.cn/gtpseyzrta.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtqowgunwm.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtwukkmvsv.html

[R02] 变量赋值与使用
来源：http://hz.yj20258.top/gttlrelvic.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtejvbinxe.html

[R03] 只读变量
来源：http://hz.cashguo.top/gtqatuzroz.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gtivvecfcy.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtsacmkimk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtzubkeyba.html

[R05] 参数默认值
来源：http://hz.sxryk.cn/gtenmolkjm.html

name="${1:-default}"
来源：http://hz.havefunace.top/gtqalfysyi.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtrawlyndj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hywenlv.cn/gtfsgspahk.html

[R07] if 判断文件
来源：http://hz.svipenyu.cn/gtpboppwkf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtfafguapp.html

[R08] 数值比较
来源：http://hz.jinqigufen.top/gtemdbpngy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.c1oappe.top/gtpherrkwy.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gtsjhbntet.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtcknwyhut.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtvnizpgln.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtqkkhzeff.html

[R11] case 多分支
来源：http://hz.cucudq.cn/gtkzesdicv.html


<!-- 参考信息 -->