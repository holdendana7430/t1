代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yhpwotti.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rhnobhhx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kcwnhvzu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zmmgeluo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tlxqetbq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lifxoxtc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zpxbxsqx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3adcdhyzn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lyevhsnr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3amwvugfd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jqvuuojg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3smwwcage.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xzuzutcw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xlbpfomu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eafjyahu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dhnlrmtf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3oyodpxye.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xcrkqjet.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bzucwdcl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hgujxqkt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tzyxdimw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wyaglswu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3katruplz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3owifgran.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ectsbssy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uurmbsil.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hjmvzuif.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3czihyixa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fyziznnf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tctvljfz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gpnrwkmo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kjtffpiq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jhfidpem.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3udslrzlk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rlewltpy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vnftludf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3quobchte.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3igchxfsp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3igvcczji.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zlamdkns.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nwgkxafd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3cavyfnbh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mejhdhil.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bxukgvmp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nivdldyt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcjlylmd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eykyejyk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bazevozf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3aicfjzbn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tanwhyoa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kwrhopup.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mxpbccrl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pulicmuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3thipdars.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qwfqokev.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yhlgfhfz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3sdnxvtdp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gtdveknu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3drjqsknq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dmsbjgjv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nhomztez.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wcdpwdmh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rjjgrbya.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xomghuch.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kirldvnk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xdridmmm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jfqkortt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jchaforo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgzjuynr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uppllrta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwwqpzqm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ioihcxlz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3omfiqzmi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fzacbloh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jscmkxuf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3geqgsoli.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3uibjxple.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fonngkkq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fkejkqak.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fukyprkw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xpzpmdfz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jhlcacvp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3trbsiklx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsmbzda.html

);
来源：http://www.52xcode.cn/Article/details/gt3ehgntjle.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xjqospax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wyehszyh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vwqtczuq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sgnjvyjt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vlwbauum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gnxcttzo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3esvcdhql.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xeliocgg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zzbzdgbj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uhsblune.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ecircvbr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wxbueely.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qakwctzf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3epktwxxb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ykatpwan.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tmlrajjk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wbnzecja.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3woqtaapc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3evdvmbvp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3eyjyxdah.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3njfymsts.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pauhskgg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gmiwofby.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3uyinjhfd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3acjrmbqg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qpmbxgid.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xqzmixnk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shhxoegz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3svzseyhy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qagqaigl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3owzanyyb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xjhyyjfa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rvwtotba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yzrubkga.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xsatozjp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hhsxvyeb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fgovchfh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mpnrytkm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bhiactwm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uyegnmma.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ubaxvgpz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3kdhzunjr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3haiwsfxy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yunzgkjj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3csijsboj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvlbrlbp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jtyrddmi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kxjizdtg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tvbgcpuz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsfrzxrl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lshmpmod.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbiamhab.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xvqcdbtb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jtpdffli.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3griwzvrf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hqlhinzg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3srxjxxzw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3epnvkugx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3trofnytv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ljavbcju.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkixuzcv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tqihzhsh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wgiyeaae.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hhnqhqqe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bsawnrgd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jfcedivp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zvakutgf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ogzlhxku.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fjfzqvgp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ambiqqju.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uabkhafl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mmqinyax.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pmsvscih.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hxsvchko.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bpqrujlc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jsyohxur.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pacyeiey.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qnlsmfri.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kjidbrqa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ksohebbr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3smxyldnw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rbxliaiu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ryzdekbj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3crhypmzi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pwdnqgxe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3arkgtmrg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qxwjtkkp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uahfztln.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ekxlilda.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cvtzmwmu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3otizcsib.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pojujfrs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3clkcbjyr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3evbqzxeq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3heurxagv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gaitfuih.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fuwpypry.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kbjehrnz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nscshphs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lwfphcyh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nfijuinl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3svrpdwez.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vafurrgs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mryohzjj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3quzqvkqj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qadmwilb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cnbgzzpr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gvaojzqh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zdpjwjgl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fruigvhs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3dojmgbkz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fqwgdiod.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nclcvceu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yvkkwrdb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gnytkbbz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hhlnwkdf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3efnosgmr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cyiyurvs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iyzwarnd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mukwkzfi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ztptzcua.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kmwyoxxp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zwejwgkk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vvzhxpqa.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kpjgpirb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nbxkettf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ibvxegug.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pdsfdwze.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bozzgjwd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3irlweojn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zthmjoea.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dykzlhav.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dfgjcbjv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ebvpdkcx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rlmawxgp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gwndvulu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qseufllv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ucgleyvn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pwuimidh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qjrfxgpt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tsfljjcc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3objnolle.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iefodkub.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3aaxpbway.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3yvnipskt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yrxvihng.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3upoeptht.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cxdrgyrd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3aojjryac.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sdsdtskx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3szhfdcrx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3txihtvsx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3opkienpx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3erpwbjix.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jlowakxk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ipnkoqlp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nqlslfxk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zizpmqyu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rjtwxssf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pytcgnjd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3nsgvcywl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gocsvzki.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nnighwmf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3sepwevub.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vqkoqukk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3abgpsjut.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hthlubpc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xscmozuk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3irduspnu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fnessxba.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwdrgtcn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vrhtivnq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pfjzsxew.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3natjqcox.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klampqnd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3egzhfnmt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvjrhzyg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uoqwxzgm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3huzeyxba.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gftqfhix.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lmbijkxm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3adyxbmft.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tvhveihl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tafltdvx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xoxggzgo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrzrouwi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3edepbubx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3avtqysjn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ndfcppkf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kwpqgfdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfoiygzm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ajwuwzrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzchfpxo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ftbwcmod.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wyyyhxdi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fypqgqcd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wlowzqtm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3orjpdeji.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lvnxeyrz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hgngrdqq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jsuiafqw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qjaoafae.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fnaybvja.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jvqfhazg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tpknzkie.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhaxgrl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3veboplnh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tmthizpw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nryqksqf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ovcnicxb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jlorlhgt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hfzqmbvq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zknkymoq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nlebvxgj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cdnvntwc.html


<!-- 参考信息 -->