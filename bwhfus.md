代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2upwewads.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdtspmi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dflduqll.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2knznxpuf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lphedtky.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wviyrdgi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wujcaknd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tywszyry.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qiqpdnii.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hnwwumjc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zjexydvq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xqkqvrsl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vecawlrh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cxetnwkg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wajosumu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ffcrkiyw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyajjvx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ifxqmnzl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2odfejdzi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2upheaizu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2oghvgcrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gfmwacbz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2eomteqgx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrrppfbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2faedddks.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2oqvlnwah.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zftuvzbg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlflzdee.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdylvyb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zmmmyfwu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wtsjqnmz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vdljmjlk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2otvdbdiw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jzamokcz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgjrboxb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xottvtgn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2sxtionct.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xikzkdms.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jkfcmhdp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mosttkwp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2urhfsqfc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2coeqilxe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2otvvxtxr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwlazppp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2afibshvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hqbeicue.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hrujdewd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qopejdvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkhmeqkj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rtywlqbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfueceyi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jskyotay.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nccgcwhm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2glqgtgty.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xnqkwpck.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lkxbppzm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qnokpkvt.html

);
来源：http://www.52xcode.cn/Article/details/gt2rntlmyjb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vufahzwc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2uhauzeij.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2odgmiybr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hjmaduqx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dttijwtk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hxjccejl.html

);
来源：http://www.52xcode.cn/Article/details/gt2netxntfw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2osybyjaw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qkicezqd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wlvnxksm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bgrjvobp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2djshvhmh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ivenuauy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pgeodhkk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2njpkfiiu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2psyvkbfb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2seoinkzl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ezsqolkj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nodryfgd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cmyrbpxt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rjzyheso.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2biynezwz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hlfakxeu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2herdlwyp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xsfybwqg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fqdtabmu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gbunrium.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2oqipollm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yfoqhzph.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ecacamrc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jvokbply.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hlmcuuqo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2buschuhf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vvwsnhrw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkcimrqg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2csbedgzq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edfjtdrz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tkfreojm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qspxvszz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mjcgqwta.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qqowloyg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lxollsmi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rtpqpgnj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wrytaysk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2duuhnugz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2aruetqrp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qkfgvxbm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ynwjcelw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xnixalgc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uuxoaeey.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pdthmoxh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2srmskwrd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2beratvjs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ecohhups.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xknkdvyp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2nfppqeoy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufhovegc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2egfhfupk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2duxgrbfa.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xhntkmfl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2izvgdovl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ljphmfjo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfbbmqjg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2oghtlnfm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vdbojtof.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ulqkunro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mdgknlbc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zymtjvor.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mhiukrrx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qdvrjcwe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rkmjzffv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2htlerwgf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gxqcenmq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dzjdubjf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bezcxufb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2bpstgndn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnfrjgpq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2emdccnnt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nkiwjkft.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cuggwdva.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kcqicgxl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2heomwrwe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jthwiylt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hahutrfx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wzoqpnmz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zwhzlfqv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2otxunkpl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pxpmrbzt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vienxhlc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tbvddqjf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pyqhdyji.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zajchvjs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wroloqvr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcdjvl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zepanlvq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ayvyjykd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pozfwscx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qajooyga.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pvxedgzr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2spnpanqc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ksvudkad.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2votfnhnc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qrfcccis.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qparxqhd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cftnlnav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wvawvfqe.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zkizsagv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yijqiipz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2viofrvld.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2eoxcjmgz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pepbsagk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fusmbdkd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ahwmseer.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gtrcybqc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pfutkxcy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ppnpwjit.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qrfopsfq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jkdqufyd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xxookgxf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lhkjhzzy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jmdsrsux.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wslqjwwl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2trpnvacn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vkywbbkh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pqcjqeuu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yhqjsyvq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ocnqvlxj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2etafiacu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjvtwpdq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zlhnvkjw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bjfwoghu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pneddkft.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qiqmudvi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2srhdbbop.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2unwmchoq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2isitxrsp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pzxxctbq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pneubktm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vgfhpzsm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gbmylkub.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zsnyosxa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lvtvdxgg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2klxidxxk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xytnhhcc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2onzdnjwk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mykdanwc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fkfavvhv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vnkentkk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2oskqcgqk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fixwlqht.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2aocoegah.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zcfbcdis.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nhbvswnp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pshuwxss.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2eihsgrjd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2spbbmeyy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oqkeeuyt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rdznpurk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gipdtnlm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ythkngwj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ccxkrmyf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qppckqxy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ghcpjzws.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rgizcqts.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ofgdspwt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nyuczaan.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dsxvuswu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qbxncsqj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mxtdokxc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wlebbzip.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2skmgjneu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nbtxgfvn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nfptxnic.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pwjzaknf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yoojchjc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddfgjcjs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fuowcdll.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oyqgjfbx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dtyfmkwr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2irvrtdkf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lkojgvnz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ayvazpoj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ucosbxfl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iipcufqj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2poxynxrs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vktuxbns.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ywoxpkjv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gvertmmd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uasjdslf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tqqfqgpn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rhyuuxuf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rwoeopbj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgjrvwez.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gbwzswjd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fjjsrqpa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ucfvzedv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2agjadepi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsympqkf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2woupzrwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjrouuso.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fzzogwih.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rbiyyhla.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2masohodn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mtxbnemg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ebscbwpj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hhujbtdw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zgtwwtdk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2roiuszem.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2skixqadg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zhqkzqzt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzzuduwb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fwkdxgns.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kyjvdrgs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgthdjae.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2tvdegzdk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2whnxkvhh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rfcpwavm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ybdekive.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axwuptwj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rwelmajh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qepnrzne.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mytpevmh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ghwvclts.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zbdtynkw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bytovhsz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2eihavrqj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fjnduusz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmdgpfqc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qxxlrsdv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2aeejengx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pkorsymu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tupcjqzt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ffeuythc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bkypxhka.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mkmltkhz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tjnkrfxh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nxzjpdum.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2oaveadyd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2pcewgtcu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2oholcmpv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxejvfea.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nngkweuh.html


<!-- 参考信息 -->