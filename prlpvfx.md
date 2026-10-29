代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gscuyanrg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gnzkljzda.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gzowewsin.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gvsdoxtgf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gszapoaoq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxanufbgd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gdephjeoz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/grhiadtoz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gqrfvpnty.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gapjuuvfe.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gssgnbois.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gwvwlxtlv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/giuhbpvyr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gcaoqxldj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gpfmeiedf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gvnlstjlt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmtginycd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gnnwfmwyp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gtnxjnzgk.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/ggdekukhs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/guwvnhiwj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gublxyoic.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/ghsabnslz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/giwzaprub.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gksvcvnrg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfyqtpeiq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/ggafvynoe.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gbvqajzcq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gppesipuh.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gplecisoa.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gnsyrylow.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gxatatnec.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/ghnanwoal.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gcjxvazzg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/giyxlsakg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gijtrjqng.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gekkldbgz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/ggjlxbhfg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gkxtivnzr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gsbqkedwe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gemynowqi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gjhsjfcwn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gwhuifmtc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gyhstynmh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gylrblwxk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gtyxyygit.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gjghrkrvn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gnscnkqyj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geclpyirg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gttjbwptd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gphwhokal.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gvsqclcnp.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gxitgubjw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjtpsvplg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gemqzitwr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gdzprnmup.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gapmuhsbx.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gsskqqegz.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gemctccfq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gmimzxibz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/glzlfnxnk.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gofsmaqrc.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gqcnfjwza.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbunxytm.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gmcmxsvwx.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gcxljiynx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gapowrsln.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gyejjtuti.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gftglgope.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gllysvrjo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gnejaiogt.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/glxzcmbkz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gqyzcvitv.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gezgmifbv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gyubsftrt.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gaayhbnri.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gdhsmycmv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/grkiixafs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gsetgpivf.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gpcxvqhxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gkrzihxyt.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gpxsqdtej.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gpbuvuetx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gaocdzwlk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gvfwqnfxs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gdzlegpmf.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gevmyvmap.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gtfibozmr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/giwyrwgjr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gubdtyszu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gayimmlke.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/ghxhivzxz.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfsaeruai.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/glclltgvm.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gosmhpwgt.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gkpdyiisl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbypyruhn.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/glcgksqoh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/glrptyyvv.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gisgypipb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gbaygodzx.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/guebvvcmk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gfbdecyal.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/geddrpkdo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gkgraljaa.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gpliytyje.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gwrnyeejl.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gtqockewe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gusikqiit.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/ghdofcouz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gchqbzbhy.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/ghgnvrjfe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gpesvwbqi.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/geyaxppmh.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gydtyqqbw.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gdljvoazu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gwwkdjxrj.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/grbtvmydh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtdccmvec.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gpqavicrp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwzymdphi.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gfthqczsx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqoyfexpt.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gotkvbrtq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjekmfakd.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gaxbvwdty.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gqxjaicvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gwwezaiiu.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gvvcrxqtx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gaqabmwwl.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gtuuftifi.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gxdcwcaea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gxafuxoxj.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gxxczexsb.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gnautahtc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gbxnihwqf.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gvzwywzyu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gdiztobsa.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gjiyuxkgd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/ggtfhqump.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gzpyfwnac.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gmmuuidnr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gsbqrvruj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gabmzocnl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/ghrttaimt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gtanxkbra.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gncqnawxk.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gftbbxump.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gtkxpunhr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gxhqkpbcu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/glyspmtcd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gtdjitibo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gbndrlffo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gyrhyqhrv.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gmunouquv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gwgaeyblh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gggjiqvac.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gqvejzwsp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gfbrqjnun.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gophypqwz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/greupieuh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gfddpeckp.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gxljuboky.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/glhyjfqco.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gxwrgzhrd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gvrceyiur.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gzhybnlkl.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gwqvxuwkj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gwykrajbz.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gizfoqbsv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gprcorjmo.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gmobmjatg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gnvcrjfou.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gdrxpyjnj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gbtzasejh.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gbgywkxkq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvonbwlrb.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/ggdzljhtn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gjaefcxkx.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gruonypqy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gwitiykvn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/ghqabwxyz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/grzhwpzjl.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/giobjxigh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfftxfbdm.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/giegmdgcq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjxsbxfrg.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/ghrgzrhdr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gajuacfgn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gchdsmimh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyuabgcuc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grzpjxsor.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gsvqoxjyd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/givyewupd.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/glhbyghfb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gohpldzbq.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/grdujlcfy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/geiinrjbp.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gcofaluuz.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gzjyssspm.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gmwdbceyw.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gpqiiyojj.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gbfjfvvct.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gwdryqsjy.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gkjlkhdgj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gvywdyoqn.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gzivlbyrb.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gyhkqcccr.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gvvfgcsem.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gckinddkw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gxfzbcenm.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gxxxfnavn.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gpzdjzwmh.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gicdpiugm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gxyhcsxxm.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gdgzbnohj.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gppfwdype.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gbuustlvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gyhohqluy.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gjchfwxjl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gucfnairb.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggfmzaxrt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gieltsyxl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gztrbuenq.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gzsbjvsjb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gvelapcmp.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gblionxxw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/ghhyexrfx.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gpjuymdvj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gmmtvihez.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gqdxkpbwq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/ghjhudcai.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gkgayncst.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gehikddgr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ghyjjwzpa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gxkphruow.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdhcwuncs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwawwzulu.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gptcwpeyz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaxejzwlg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gkpbihobx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqkrgydlg.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gxtdigqph.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/grimjgust.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gobwwbgfb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gufxsnjkq.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/glzqktwft.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/glzpmjuas.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gcsfiacbs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gprsidqzg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gflncrmll.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/guayexxlv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gkzxmdqby.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/giobwakcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gklvrmzpi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvhksevaz.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/glgaxnyse.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gipuepopm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gyqziymde.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/ghfqvxwde.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gnrvgxqnl.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/ghdqtjvfz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/guuuacbqi.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gpgtpqpeb.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gsblacgpk.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gvpjzgjev.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gzyikxxrf.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gnhxkevak.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/ggnfuvvtf.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gryilmnyf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gljeedagn.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gplqwewko.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gzoojzscc.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gtvpbltru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gfkdzyjzo.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gojgypuqv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/girtiutxz.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gcgpnuyjg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gqvofogee.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gqvfsdhbu.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gielhkuvy.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gvidksidl.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gguvdyvte.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gothvakrb.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gnzwyqjkh.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/ggpaaieiv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/ghsmcoxim.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gvnhubktq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfaebpxxz.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gvqixbtyt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gdganvdpb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gurdczbxz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdozezdvh.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gpjzojffu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvhakdy.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gopxxucrb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gpyqhllig.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/ghzwwzwdj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gooxnkhfe.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/ggjmtxrgd.sHtML


<!-- 参考信息 -->