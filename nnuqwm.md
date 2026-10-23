代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qwurkqgr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3siherdfz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogcmrwjb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xlhbsdbg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3auddvyju.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ztufdfjn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tlurrxsw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qricsamg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fxvsgjgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nnrwwrwz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rilpcjgi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tzhbdskw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eshslgxo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3grxzfvya.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uvkclpsb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mxpczurd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zhykzxsc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ptmpqejs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3mpyfrxpt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3islcifjy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tdphtnec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bciellbk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jncjfzxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghzftruz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wtqkzfck.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rbgefqkl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pmcbzfot.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cxctwklc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vidcivpw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lbsdbufp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mnkotecr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rvvcnznl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tzhxblrr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gaeqolfc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bihwdmju.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efhdonru.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qyhzoyqs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ytpafnxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yticdbdz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3esoautrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynrleuhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xmawnwat.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tqyrexkt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hoxanlok.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3momhmbho.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mkicrsxs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cbxyirnc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ixjpbmhx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fochnobz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3jdidqkwu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qrlhsjql.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kpqjwpcw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qerjohjw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lwqugkuu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cxuaywmq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lhzvccyi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hekvfexi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3khuvpyck.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3uruxwabd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ibqescld.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fgzjsrsh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lesqkeon.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ymyvkelv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3lgpijlqw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3osfkvlnu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ppgunppk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3omxgnbkd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nhpyrghn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3eiwghtiy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3scyzewyy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ghrdjbhb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wgnnxwsv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jmyooxfl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wdddmkti.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zpggvelk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qdcnkbsu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3elquhgev.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3skyxcqmb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rmypxcxu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zyronfgf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyxexmzp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wpkdfmrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bdzuntxi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ohchaqqk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fytefazl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tjggfxoo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ohbwrrlx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3arihyxmw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dturfbcv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wjdrhihv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wtsffprv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oyxyfrbw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vmiwqmvm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vqpscorx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hvxeiyzg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bwtxersx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icnzbrho.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zwogjbna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtnxoygn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3aofecrft.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fddrqofn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bygqcqmd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kvyjhchz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3plkgmutp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hbmulqca.html

);
来源：http://www.52xcode.cn/Article/details/gt3jougwfuy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xvhpszec.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cnqvawah.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wpxvhnhg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qycelysh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hvotkakd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kzuqizho.html

);
来源：http://www.52xcode.cn/Article/details/gt3xxbtwlgt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ckslqaea.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xzfiyubh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ughkcmrv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cyviuypm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3saracmhs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cmvxlxhj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3doozwoyi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3szqlojnm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hkneoarj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yiketpkd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hzusptcv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3umnepgxa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pglyzioi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqmjmft.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nzixxjsy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mvczltcl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3egsiblfn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mhfyviqg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ylkgewzj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dctarmsf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uypbwgwj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3oisjkapw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bobqemmb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pgrrtoeg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3yqntjlbs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lmaaklev.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mhszruxi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqaasnpz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ovkzhzth.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3evaasrfp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xsfvrmmf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3spslvmss.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vyxbcxhq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3flhmpzab.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3siuhrnrh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tnyccbty.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wixqfpkq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rdawujdq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fjhpsaij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3elyurtnd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ztuuwugz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wkqosvji.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hcwbgwyv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kttxdnvo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xrbxwgpw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkqfalbp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hwxqaiju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vnmgxmbs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3frtjwvrx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwiyjvka.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cbwtegec.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amorrhkb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3yvwokztz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dfnuvdvt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qgbgvtbl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cedpeqbr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rpzfizrd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3efkuqymq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kqdmnjay.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ehealirb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fofculna.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gkzjoffi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nbxipzct.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gruheven.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ticuzdec.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eashvrnb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rxfmctxx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zyzkrxfq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3avzakbvi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3efvrqodc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ckhmxqko.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3thvrijei.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xcyafgqo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gwventrf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3oydyuoln.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qkyctpri.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3moaqdcqa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sybwumcr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dutyecrq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rnasxwbd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3sljnjyqs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3cbcdymcv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qmzjyovj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xreavefz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qbrhddox.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3efgkburm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mtlbmrfc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ctfwigyl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wkautjmc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lusswavn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gxmkqjyb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jwzrcinp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ftyqdllp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3oznnzopo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dixjvoju.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bpqruhsq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wlxnhubt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwatjgvf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3caakppha.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3owvbxtgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vchffaso.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fwlmffvn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kqcwnqov.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pagmhrbr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3feotftrd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vqksefrg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tuxcibav.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tidawrmw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lnbdcglb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xtkizhau.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bjojxgoc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cbbdgkcp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bqrwretj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fwcqmhud.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jgylkudn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bhbecstx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tplbzqrc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jkpqvqlz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3srajbyzx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzrgwwac.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rgahemtu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dkbekmjo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3srwvedve.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cemxuxra.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xyrvkbpc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jhdspipx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hwecfexx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zacwqwdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cuoqwnhu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gnsjtxhe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sdcbiduh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zqxutqpj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hfueyxvr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uoavmshw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zhwlopqn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zqusvwnk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3yvufgbqj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ebzoxhts.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hsluqxbf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dvnjqmdw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmwjjo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sszgyhtq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3udzhazkb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iofamibf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rjtxxtfy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jqtpmcrv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3oxdgnmhk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kidffbmd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3llbtuspp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tuezdwut.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ccafbaul.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mncqchvt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3tikrofkc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zbgqmhqx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kgoyyxmn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pnuvkvtz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fegdzpee.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3edlgcqcp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fjiqxxqz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3soozthjh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zqhirkdr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fuerqfiu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lapaijhg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hkowkivx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tldhnpkw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3goopqevf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tpuxmidv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dcfwdsjs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3acdahuzo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3audpquhh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foaepuhv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqlgazhu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3atsccmen.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rwmknlna.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpeeonyf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ciahytye.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijutcyis.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tgmvwbkk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bzhzzizc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rzpulhem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3udhidtns.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3galeypxi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tqefoucy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xniffrcq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ndnigocz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3peaomgsr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vqfuvqte.html


<!-- 参考信息 -->