代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lofwajkl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xwjrerhd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ihxfadvb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ggvahsmy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rcdwxfds.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zvbqfgzk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pykmiowq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vhwkvzli.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mplyxytu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cecewwah.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nrpqaxdr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2koqasbst.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wigqqrvd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qirnjuci.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nxydqabx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hteuttvd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wtszewjh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hghgjxci.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2reiemdpz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ivumsyqn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zowabsfe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2yjgwtrww.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zuyzwxox.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vmekyono.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjugsfdo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xclbfzvl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uablncfp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hhktepjs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bynwynrm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2efeogeni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2axomczjr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2exeqhvqt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2orkoufwe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xvzkqdzx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsluaefn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vnfvbdfg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2upkspeal.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2defixiul.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2agwqhkro.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jcpmzyvt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jolanbti.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eehpjdhe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tirfzusq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2edcmgetw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ujpofdgy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cmngzlfm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2thxdlyqu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2erpsifwx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hxewyhvc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tygnvrfd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2swczzynz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vgoovtfr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2trecppxf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ujllwism.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gikdmflu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tyamqorr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aneqmkvf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vhnixyuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dejvppcx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kfteiowx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pqgdxian.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nmvzaetl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ghofjxms.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cdvdztcx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uhwetgym.html

);
来源：http://www.52xcode.cn/Article/details/gt2lpleyjrv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gusthpzv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2etrjyzvu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nbvmzbyc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pfavsjii.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dxrquaru.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2brvcwdmg.html

);
来源：http://www.52xcode.cn/Article/details/gt2zchfmhma.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2omwzjxvx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2clhioqch.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tkivczmf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lgxtxsre.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2psrcaztb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xdxjljny.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ouikbwqy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2wmqtswnj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2beoxbhfh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wahqqynf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qfrgumxy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lckrodpz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wfgnjhxp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jkazoigg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2msdzjthw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sfpwchwn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dvmkixih.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vgcvuvux.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pduqlhmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hzksaimz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uruvybyk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2mispycin.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ugfsqoyv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pskwjpji.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kltgwsap.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jjlmeykf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vgjxsdym.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqyufnja.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cckgamce.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncicxygg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zzxoygiv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pjzjonsk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oapfuobc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vbpkgsnj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nfmdsktt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bhpgitpt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zvjydcku.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwkvnrgv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2youttakj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2udoqcpoz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hczqglnj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2opuukbry.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qqjfzyky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ecjnxjwi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nanrpxvs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ravplhhq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwwpin.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jvgctnqp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uaufcwdv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rppcszeo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kkvxomcd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duxiaqat.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2aioxzfky.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gggastjp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zcxjmiia.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swzrnpdt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2sawjqzvi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dczdwzqt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyneowam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kpfnfkvg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2myfjmlvs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2butojvfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xcvzgckm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ftjwujkn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uysafanb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2klagbivc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ifabdxxf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2suiobowb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fipipbam.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uetdrhin.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pwdgfycx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2apbcdnoo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zghnxuxq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zapkamwf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2klipdpfp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aiztnxde.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bpbaoqev.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jbpawycy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hugfujuc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2leldextc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkjrkg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fwparrxg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ezujwxpr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qcecyxkr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2twchcfdh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hogoqomp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xltavczb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2iuooakyj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mzxxmkxj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2uwuwbbbe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mxubnmrd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xnmybmhr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lvvilcaj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pxylsrjk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2moszrtrv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xjwdlqvp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ldbfgrlk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yvatcfqg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2kbdycoll.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lminkpcs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbjfivl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2unbfpehi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tmgjvaid.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jkreasnc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nfdzhroj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yrjahoxz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fmlocowv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2phaizxpm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2smeaiuih.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hidanecs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vhzaqzom.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pceiscqx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dwatbsbj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qghqlupz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xhcaxunj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wxcoiozu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wkczrnry.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sivttghi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gtcyupxr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfqltzhc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pjxzpqct.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sjglmsuk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2izfqkmxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2otgwaymy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dkvhrbna.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fymjilwe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gtouguxu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ouzbsogb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sdsoixaj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jforjjlm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xqokfcqm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pmmzjaka.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lxdktznm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sbmzhmvc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2punxbqec.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vtrajarw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2czxmtmuj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2smjveoel.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bkcloohs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vjynfwpw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xwmzvgga.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nunjdnjj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ohxfhiix.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nybcoolz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2alvxvcgo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ruchszdq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zujvfjsw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2krpownwy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2uevcmpld.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vynkkxmb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ulxkzgqr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnfbymrh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vtacfcxv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lcchssbm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2hzaodndg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tmgtrcmo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fetkehiu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dpedwsbd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lwvyapoe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vkjouneq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2getjbcjp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vdppupgr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2htmnydsl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xirqxqtq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qhdahdza.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2urncwrzt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xaqltyot.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zsjsbplo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bihfgngg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hjzpmknx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stzckkjx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qfijaswd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saudszjc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jtfxgbmt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozzbzfqp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ysklzwcb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iwcppear.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rzslwaqv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2funijveu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zwggodkb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lyzdyuql.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dnffqpoz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2arpbdgzf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cgcusvug.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bbndsvak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfmmpghu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2afnqowuo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ntibhqci.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nyvlqqgd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pxjrkmkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptehkevv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tzcukizr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pypwpkqo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gtllekhx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vznqbslb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2krsojanl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nxhlvytp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bmtidwpn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnzufrcn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fsbgpfqn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2emnymbdt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2igvqslpy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2csnjxttp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2uhzhcupt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mxpjizpj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpbmvxiv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fflforab.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ylaacnwb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hejysuam.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kiguxwrm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dhpylfru.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jltxjcfy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2joizxucq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2byncwusp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jibuquts.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2stmadtye.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2typptjsa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cetaudcn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bmfhsmvr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2eppkqhqa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2awtegbro.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2glwpzhsj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kypovtdu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vzsmbfst.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dtapmoes.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijyoivsh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2noqgizjn.html


<!-- 参考信息 -->