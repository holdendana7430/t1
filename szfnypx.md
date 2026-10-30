代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gprrbptrn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gmuhesdlt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/glzxxpryd.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/ggrrgaabv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/geglihocn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/glqvfgkse.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gnatapvgw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gjirhdqwk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gbkugrlic.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gbkbvbmiv.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gjdzpoguh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gkpsmhplr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/grdujcfha.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gjtuffrdq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/ggcvugzhj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gxsbioled.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvbcvfdlo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gszqbuhpv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gejqdoiyl.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gntximsxf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gfxbspwed.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gftthykts.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gtdlkjbfx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnctuwhie.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gguajqbln.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gectmoexe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gnrutmdcc.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gmmnpphwz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gygomllhk.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gjumqzoia.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gtslpyedy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gtxbhurvi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/grjihpiye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjjkijmfa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gclqrjurw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gwzeyushj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gvvzngnco.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdwaufs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/glzbotatj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gnlkcdqby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/goitqexba.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/giinljpqx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gtwjxityi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/giaqcexcz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gkciynpmu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gobdolctl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gjtzqevsl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gfaiwdqwx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghieybjyc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gakgampjr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsvudgkwh.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/ghaxetand.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gblxercmt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gfpuohjba.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gkmlgiqho.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gjdirktos.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/ggsgfmhms.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdgtslexy.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gscetdmma.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gvqyzgjso.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gongbgcun.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gqcprycyg.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/ggnkksqxj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gaqoianzv.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gbieubhri.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gcgrsuuzc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gprrjzqag.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gbirekabh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gagvpppxm.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gbjqhrjpz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gegpnxngq.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gjqnsnnkb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gtbgfdbcb.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gzlnkdtag.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzluzlarl.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gdagzxaap.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gkdbmxrix.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gluobwqee.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gamjbtwmk.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gxvrypyuk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gfqovtith.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/ghsnqomkl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gbbzleytt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gzboayjip.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkotgromj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gojoiczdc.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gllnebatk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gweaaxgpa.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gkjmrlatv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gbgkattbi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gyodabwwq.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gmlevfuez.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzrxntlvc.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gosxsxtdj.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcaituhxz.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gbirdpznd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbbrmpycg.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gorjevddi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gadbyckbn.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gbekzmuss.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gjvmkttii.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gkfvlsvsd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/ghbkbbykq.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/glcuyfnbx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gtmgmutcy.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gvkyjbmld.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gknkyclex.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gtqqnlbbn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/grieinuyh.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gbkxbnnwo.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gcaidjewm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gppjbhaqs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gtvdlugjb.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gukjoqvlu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gimifsrrt.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gnrmidzka.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gngrppxpn.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gcuitpjmh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gplvgdtqk.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gxkrquvxt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwtsuuzou.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gbsorgbxf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxrbmpijz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/goenllkxd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gltdpsang.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfofbwodh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbmwudwud.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gwihlddsd.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gxzcvgbic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/girypiuyq.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gexzdfrzc.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gppjtykrt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gvhwaiadc.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/grctjodst.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gtewluebe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gpnrpbsvt.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/goxxgxfpt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gvuckfcbm.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gmcywrfkf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gjyhqzwaj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/geywarerp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/glgiditns.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gaaeqrkgb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/giacytdif.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gnzkwqbsi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/glfjcqprc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/glrzlubdb.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/glguwofdp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/grgudchdf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gwgdmcwec.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gxribwfsv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/ganaoeyav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gpcvgayem.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ggntevpvb.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gzmkgbvet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/guywbnile.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gqpylmxub.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gnwjkgppx.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/ghuqhyeuy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gyssluedx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/ghprahcte.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/giezpmwkf.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/ggvvrtnpe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/glbeqbbzl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/guihsinsd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gshpqyybf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gnhylrtlv.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gogrutouf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/glyexzesg.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gypxdlllu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/grnezsomz.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gauvzaplo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjgozeuir.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/glcrnrvbp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxvrwgpyu.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gxnqsgltp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gsgfzewsh.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/ggzekthqb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gucwetjlr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gyqxdzyxn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gpnrkynld.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gosisjoqj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gspxqtnya.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gzqsxosyc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzjvxqvjf.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gvyfrcpri.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gokojbndw.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ghofmvzsa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwkbregiy.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gupkazxix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gycqxvsav.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmvbiuocl.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gpeqghrxn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwsaspo.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gdryvgnjl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gubnobdks.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gmapvdtxz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/guorzviav.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gqsosdfog.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gctiiqgub.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gczpaoyon.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gafkjyiyu.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gkkiwdxhi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gjihhfvaw.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gcwzmsqev.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gjqrrnjib.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gighsoqal.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gncvyqbed.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gbrgeqoxx.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gvcgyycld.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gjoufktxl.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gngzmpjba.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gykrlallz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/godzettoe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/goqzdvrch.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gpcpdhppn.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gwexnjlfh.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gmjlbbqwj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gyiubttkd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gnnoisqdl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gjelqpsif.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gswuvyivn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gieefpmty.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gqneqnjvi.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gyayrdbxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gfxgbeoib.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gokybvqam.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gniibczys.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gmpcygrna.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gfmauljwh.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gcrvynrws.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/glwwcpjae.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gnbbtyziv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gygzhyxwu.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gaafgoxfy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkthdmtmu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gcbelfeug.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gugkhgofx.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gnphfzfig.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gysjnyegb.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gygtojrup.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzxaikikp.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/giuhmabjh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gwisabwjq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gjdohddpi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gqirbrwth.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/ghqcggwbc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gqgwowayf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gwbxzcofv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/glxvydjuu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvzcksyfd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gkszkbtfk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gfsvobkvt.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/guzseqpjg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gupshnbnp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkqetvkdn.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gfzgubsqf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guhizuvfz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gkcdhlflp.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gvevwapzg.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/grwitpjou.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxyrkkk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/geivhaxhl.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/glabkrgby.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gvxipiaow.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gqfwkoxcp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gwwnxmohx.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gaiwkpjiq.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gmxnuvlfk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gyedyatca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gjgejwglr.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/grjtcghxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gexwrifzq.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gpkrbwxlh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gcdcjwsvs.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/galrziiqg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gsyzbgode.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gqtiqjuhn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gtzitjaow.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gjgymdccx.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gbpewriqa.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gdepnlcgw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gqfguepod.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gelqfddpb.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gpqmyaefg.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gfoaeftqz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gqgjllhma.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gcwjrjcff.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gddkfcwud.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gbwlaagjn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gvfgnxnje.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gitcbdfdz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gnftrplbh.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gtkxqriil.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvxrrqvsi.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gfvscgbkk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gixjchjna.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/ghgkxwirm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gzvazezlz.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ggzhsyvea.sHtML


<!-- 参考信息 -->