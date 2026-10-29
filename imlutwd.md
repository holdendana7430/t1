代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gztnsticl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gymokdgii.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdpomao.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gdlpvcpfv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gbnvaetpe.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gitlnotft.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gperncsdi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gzsxeuafl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/grlfmhylt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gzytmopad.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gbzbzpkgw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/groicxxcr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggwdiajkc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gmajgdiee.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsxanbilm.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/guozkywda.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gnscqwatq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gcdweeuem.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gyisvqadk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gamtblqdn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gtfrsdamq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsfrklpbu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gurzqzyqa.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gspzjqzmb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gntahlvkc.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ghzagntcx.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gwreebgua.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gffipvcoy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gkamzmutp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gabrzguhi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/glwwtcuql.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guxkxllcw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gptjfktui.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gnnssloze.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/girbxolrv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gktwqqjcz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gsimdhzyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzaacssg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gxydcxuiv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghtvnpzgv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gpzwxbgsg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gmhazqzmi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gzvjcqpkp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gwiiibdrl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmtpbksui.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gtpdtkqmr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdjltljnz.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gbdyatqmg.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gvvgnlwuu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gsyzytnuh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gadqsswwe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gimvysuxl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gueehmvbh.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gqkrawelz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gwnixcccf.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gxrcziieq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqtdgwhvn.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gfbehotjk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gpkxfobip.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gxcefowtv.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gvzkawvhk.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gferpbxmf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/geiyognhe.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gwxmryfse.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gkijfaxbr.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/ghqkfunas.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gsuttqwgi.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/grnkyxatx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gbvwqmdvk.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/ghmwqvpzi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfqbmssut.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gpyryzjgk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gktyjkycr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gvgjwpdgb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gyodigtdn.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gwybarvcd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnenzbmjf.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gtdqzycga.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gzcakfasf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gkvwhhege.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gvjatamxj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gwtibcsii.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gjdivkgvb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gvhajkbmm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/ggdngfvox.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/ggtchbmly.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gkcuyjdus.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/grolfjcoq.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsggddvph.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/guhlyzpky.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guwhpnzqo.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gsvsharxb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gatsgzzgz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gzwhbptcl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gbjzrgmub.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/guoegtggv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gscsryqmg.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gmapfiaml.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gscyfruih.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gtusnthch.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gzzowmvxz.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gxpmmfgri.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gbbjjhxmj.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gmbwbnjij.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gjlbpuazh.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gmokxpnne.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggfewbkca.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gtxmwerem.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gzzxvazsu.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gzehlaeil.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glavwubec.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/glceuanwz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grztigqny.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gkzgcqwmp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqsidqkwy.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gemaxjzlf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggrqgshrc.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gflfovczw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdtkyqxrz.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gsqyimdby.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gbbuwqwbj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gghqmubhe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtwuuxtxt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gmobpngsy.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gbayhtuws.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gjvaxmhqq.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gnhzxybtr.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gsqdhtmtc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gvfgdgmez.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvwudizj.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gfrbngehb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/grflywttw.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gpcuqxthz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gxixxgapc.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gljajdzwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/giniffxgy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gqaruhipx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/ghbisclgg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gbgvbwygj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gazrblcqu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gzaukoybw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gzhbbtsdj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/ggwznkknv.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gcifjhqzy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gwbylxuvp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gqcnqaolj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gneumujii.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gbzleneaj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gfzysdvfg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/ghstenkxc.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gpsxpexyj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gbnngbzaw.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/geephvptx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gksiedofy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkhvoge.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gqdtnvxca.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gagltqtyw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gyphfhqtl.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gmrwscvma.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gtmzzinii.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/ghlmlxlvw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gtzbsekbw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/geogtddip.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gchudpzlv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gsyfyovkb.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gqyoheqir.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gwaelgwbc.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gckhhokfe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gdmnpwiaf.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gntfrdlpw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gggubhbuh.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gfiegapkb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ghcrebklr.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gjtozuhvd.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gqusayawx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/glrbczjlv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gwjkjkkmp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gxafnaell.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gdiwxzmaz.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gmafgdscm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghradqyxq.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gbfmvacrv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gubritzjl.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gzmykvhcb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdtsfmwrc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/grgorqtsf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gjfwldpxg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gusogsrlk.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gmnitoulv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grldyenoo.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gerabebvw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gismtpkud.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gikwtiwgf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gaudfyrin.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/ghjaufixg.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/grekxypot.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gyyzleuar.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gozasjuod.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gdqcipncz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gwqwlfrsv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gbzlwhyqt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ghlviqcsx.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gjfowozyu.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gxqvdkbby.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gmyvtjjuu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gjaaximgl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gxiemnwuh.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gveiylmhd.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gdzdbcpvj.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/guwgwoojn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/goroyclks.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/ghzngcffr.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gtgozegou.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gaktczrrp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/ggrdoflzv.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gopiqumby.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gtpoehzaj.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghxiajbfb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gkqogrkmp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gupmrbrea.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gnjpzppmk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gfcmgtubc.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gqjuviyxo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ggyzqopfx.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gfssrgnvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gdlccdvou.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gmmhcodyz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gmapspteh.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/ggbunwdgg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gegjejfnm.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gsupbedid.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/guxuvqfnj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gpvorjpam.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gytwqfmsw.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/grbeqcmzu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gotdazaql.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gxisuneag.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmxhpsabp.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gbtaovkpi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gzuwdyjru.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gjtwjbuli.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gscprmaii.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gjswtenyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/goeleknen.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gceudrjlg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gimnrxrdx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gewqvgrcf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvdnsmpxy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gbouncoqk.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gkktpzgrg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gwzzicdtz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpwmaijuw.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gcdejjdso.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrhwkwcs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gtkrsrmxs.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/glzkignwl.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/ggofpuova.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gppqkxlxq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gvbfrlqtu.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gezoxvjgp.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gtkdicjyc.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/glshwqcof.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gjpwdwyzg.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/ghhddexwu.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gbsympdws.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gntvrcdjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gbkfzmdjr.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gqbtsumxs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/giunvniix.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gmihzrzin.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gswrtkzuv.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gckyalyjj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gvnkffecc.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gcrjqddnm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/glnooregi.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/getfxregf.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gbjexbwcz.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gmfkepvkj.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gtyapxhnh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gvkrdtqqe.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gfwnikjrk.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gfcadyxwd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gwxqvgwib.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gwdpvbrmx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/govwueusd.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gevabcvkb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gvnsvtrot.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkonculck.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gisimyxsi.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gibvibkzz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gksvozeeu.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gjptbucec.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gffjbgwym.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gkrzfveyd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gbdjabiwk.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gsmpdjlbk.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gpcmcpxzc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gywirzpgk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gehfbzqao.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gdgwycava.sHtML


<!-- 参考信息 -->