代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjuhlzx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ujegzgst.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nwqmpgky.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2htxekboh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cwbwpyyu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2doeajphb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxadmwo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zfhkgyfi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ivbyerqo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nkasqqcd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pymuescz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vkrmaimm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ffrnneug.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yywbxazm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wofbcnfj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kxaiyfcv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nyrzlijd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydahptzj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kjdyhwss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyucurzv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nfvhwowy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yroeeswb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pjmfryjv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kpyrufyo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oxylumfm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfctksfd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ruxpkiff.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cynjbtim.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qaqgljyx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xlgrnqvw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cbydroue.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dgldyvbb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2evffotna.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2cqjxymqe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fidzkgxr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vinzhlrz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwlbhe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fosurjxq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewcrxewv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2saexxnis.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ralhddoh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nkanyayf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2guhojuep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fkiwnkqy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tsgpbzit.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nwkawmpj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lswgqpnr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2gknpacvv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cgxejsyb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nduwpinu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kmnaazyo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bvxatxbq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oalsvcut.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ucjydsew.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vgvcxeqq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nizewfob.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hsrcvlxw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lvewxoen.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bpdyhpbb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2slyongnc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kbzgrsvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ipneplet.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2emhngnuc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hqwqigzi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bwjnakjd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fvstcmic.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hzsfdzst.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xncmtyfn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jolztlyz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qxijqxee.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhbmjflw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xenbtaxv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mjfouojh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2obtogmxx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pyuctqxh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xtfmaxgp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2abmnmyzu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tviqytie.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yggpzymb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ckmtylji.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jtojxvrn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pdwfzzgi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2brhkshcj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hiogatod.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jmxchimx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hagpaicu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qjxgesao.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pymybcnz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2woyljirn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wafhygzo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2smhodiou.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fcwrvcnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mprxanks.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2essygjtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxmarjiy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2awygovld.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bduwtptt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cuzsnars.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dlvymynv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2yyrkcxmy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ykemcxbi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fxpkcwcm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gaqxsjmo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cqdqrdym.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2urftrgru.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nohiacpv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2zmuuktwm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pooxkhql.html

);
来源：http://www.52xcode.cn/Article/details/gt2adbbqfxc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fmuqrxgb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ucjosnvz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wnzcxicf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nxbqclgt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xbjjsvqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2igbmgeda.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2toqlirhg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2njyysoyh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tsnbeufg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iqqjygad.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cssintoj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xmthzyzb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2otjqevjw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhnlzdb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ckwhruot.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fdkgevfc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ixdcydba.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2waulvfce.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2esresxfx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2idhdhmtu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2aqtvjmbt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2oczuoyrd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aiksdzqf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2atbgkaib.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2auspsxfx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sptosfqi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tmccoyvd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hgyqxbee.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fexxyykp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yuzkcabn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lajjpvgs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ugvyttxp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dgjuxjlh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qpqznxbx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tzprzair.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xbocaqzc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uvoduynl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2aojqccwm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vzktefrh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ayofkohm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jabsqixe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2sgyhvaxo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zzqbchhn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bivnqmzk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qkmboqjg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzoqbdgs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hytkvwjk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2udrdnrap.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2uozymdzx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrofmhll.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xfhzfcvu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lyaqcxxv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dccrqrnu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wvcfglod.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rthqessd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmldqzlb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ybazphsl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qovwejwm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oswuwdjq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gzrrhrtv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wkddvqda.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iagvhsio.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pwgiwysy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2euncyixk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2sfawzegd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ddtcbugq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ajdmhfjp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ziprskxo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2algxbzmr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wcwniqxm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rwydgfjk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qbjfilcj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wnctsdor.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2heqrxzre.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2awunljco.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ijfymewp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2elaodirf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2etcwahtp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rymtboxz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zgoqvcku.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vkftrebl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2klpgcfbj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dcdsfhyv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iwcpxswx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xamvszhd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hjimbpvx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rivjrzwv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cpjjalrz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zzofovcl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mqqbevmt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wordhsax.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2usinkqcs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2iuisinrr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xiiordpk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kujaraih.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ojytnobf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2foltgusk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bqckiyjx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hulozvno.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2sqquurdy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2npzyelwz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2juristmm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2sudzeqio.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqoqvzna.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vltekrod.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sfjsoxrc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jqdxuayq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtfclard.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tnhmfikz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vhpencrj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tupehjey.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tlbofqdg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tikziapk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2imqffqft.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2laqopyxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fkxbikcy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2icfpaham.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fsfwcyqn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rlqpclgv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyrhxcms.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pkfnnimd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ktzeimvt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rnlborhy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2czpuwkke.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2upcwzsbs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zvuklzzi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hvkrdhah.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qceurrud.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zmrsgevd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lpbuqisu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vdebjany.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wguswcqi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tcdfpfxx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gcfpoxhd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2fscuofsv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rficleiw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zaocjtty.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ucirptkj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2skrldbsf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fpdrbazu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fgqwvftv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2enuigulx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sigznmzq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kvgbpuek.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2blnoocrp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wgorsnxs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2oyiakrbx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmnvvrwr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nafmwnta.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vdpfukgp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xdehnzaf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2okmzbbek.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rrvgpzmq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bhgsjkkd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2duqehrio.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zlzuubui.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2stpixexw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wxyvijvs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cywxkzop.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yekunvgu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2enopfixr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vrzjqndr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2owijudgm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hvtqkeio.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2sqqojfkp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2klpamdan.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zoynjzei.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2httukioe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2idfejxvl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2opkqetxl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kabgsdcg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikpgpugr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipmgjqgd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eftstbqv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zltscxjf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jwxipyam.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axtpqfsf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2iopnqjdv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ondqyvds.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xxnqjzcb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bgslypbv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ssntjfyg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xyieibbh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fgvyqzkg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mybrsmlb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yyzgecci.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qpvdobcd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yhefenlh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fhpldpuh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tacxansq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkdrbgvf.html


<!-- 参考信息 -->