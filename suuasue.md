代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/ghetzbnmq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gedgaurnw.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gpctikiok.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gnjgiyzlg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/ghltkzwqg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gjevhgfaj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/ghlloyoog.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gkyylsilh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ggodyicyz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gqlasgysb.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gkqcmmrya.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gnjkxjknv.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gkcqzonix.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gtqafcpxk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/guapgujhg.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdfictkgy.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/goylxiiyp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gynyfrasv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gsimqkzcb.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/ghseetslf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ghfhacicr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtxiimrhb.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gusiverft.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggmedaelj.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gjlpfbsyz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gzsyrltez.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gjoixcenr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjrcuonnw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gvjurfilb.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gountyypp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gwubxxynv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gqqkfirtr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gywcbaesk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gynvthwfa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gqhudkaqe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/ggvrfhrgi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gaggasagf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gangnziny.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/grmzebqwq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gnjmtuidt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmqzylei.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gdvvioxsa.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/ghkwmwivx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gbqpncuml.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/geptmwnkj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gjgjwfvbv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghgchnpad.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjtpankpu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gdwnjyneh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gzwamfnzx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gyssilqgs.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gkhcixbns.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gysgkaqzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhhvkjd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gutohukwb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxgekvaur.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gecqilpyz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gikmzyjow.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gstzzopxs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gpwbvcjqn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gkzdsajwl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gxnyxluma.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gfzotpqmx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gswvtwwca.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gppllrnoj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/getlujsxl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gsxcfumjq.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gkwjcfksm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gkdvywsfb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gudkitcty.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/goawzhujo.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gmllpspdp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gytfkfpdc.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/glplkjuzz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gdhjnipsa.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gqhufzmya.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gkvbtuxnd.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/ggciucgpr.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/ghdtpzraw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/geibaankv.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gzfjqnyfo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/grmyewhhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gyeapsghc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gmxzclotx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gdhbjrvqz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gamkkexng.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/giqmapjof.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/giurvsrho.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gaivfjmvz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gljvrpppc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gszucemnr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/glbanjssp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gpbjjsjab.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gwccckrpp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gnsgxpcto.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gyiyfyksh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giykhqtkq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gqukdulic.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glpudxdpa.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/ghfkfhfpz.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gvtyfdptr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/grzddbvdz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/glhdzhdef.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gwesagbpc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gklsztswz.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/giperpnlp.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gybljnxhe.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gmsdlwynd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gooyhpnfe.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/grycxhwqq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/guwpokxrh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gbjnwnxlw.sHtML

);
来源：http://baike.fehbvm.com/Article/details/garburegz.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/ggiprrolz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gwtmpxxmj.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/ggbplgfbt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gzazmrjmy.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gtkgidgsq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/ghzavcqrm.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gjygnrwko.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gwwyeadyi.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gjgkzlpjb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnrryndnk.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/grffvuqdb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gzghaeaqi.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gcntrbafq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gwaaskdjp.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gelhiense.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/grqoxgfde.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gijijwbut.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gcwtvcguy.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gywftxtpt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gtzmwtcfw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gkothctlv.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gxeabudpf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gorqihbkd.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gvtbgsmuk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gfvsjvvef.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gtuwuejyb.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gtiozpdjm.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyrnzscms.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/glvsgalts.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/guufrgszi.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/grocziyfg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxjcfovxj.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/grlcrvwbv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gfilvfdui.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gvxlmeanh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gqaybkqmo.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gnqjcxjay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gznaznccp.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gnfnwdrwg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gjxsniyrh.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gzonkuewd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gwoapgrma.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gkxgkpeyc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gngihtftg.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gdfwatixd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gzwqtkvgs.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gutgopdjh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/goewosqtj.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/glufqretq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkyzdhgpp.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/ggkvlwomf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzwcnwhlv.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gooiqtzbr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glghwfilp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwzjxweju.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfywbjnmd.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gfzoshhjl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gopafgsxr.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/goinrkggk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/ghgauknvb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxkqkrrfa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gcbfcnuzs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gskxcwaqt.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gbafavufo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gidawpuxj.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/glavhgqfk.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gfacwtbsz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gbrhgjjey.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gmmknqsim.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gmjafpwhq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtvrxhuru.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gsbcikqyy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gwrqgdflv.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjkcinccl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gjkbrlqej.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gropywmmj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gyxxzrylf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gbuketgsk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gqbqfunwe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gprzgahig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gmbxeyvkp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gfbgwygkw.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gqzcgajaq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gyexmewpx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gxviwuqcf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbceslzo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gmtgjybbj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gfshbbdzk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gxwvnploj.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/grygiadgz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gjjnajpdw.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gkkpuzjhf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/ggsaoyczu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/glzxzkuvg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwszngvl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gvwbdihjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gkarnbzot.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gxwhxtwsr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gfcvawplw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gokvtloma.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/goirxkmzl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gmysnlqog.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gkicqired.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gaphciwbg.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gphwpgejd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ggzprutyp.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gwcfdrlsh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gzhjebqpj.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gttobprpg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gwfhizsvn.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gyqjvcezk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gxngyefpv.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gneydscau.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gyaikpusp.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gpynkochw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghzaomusd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gwvdwtult.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gcclrgcpi.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gtrlhkhwp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxtiwxest.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gdqanswba.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gliuyodzq.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gpdexhtjj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdgkwgdrl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gvmehetxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/ghkeocfsw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grthvsvbl.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gulcsvuxl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guyogejae.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gmkxbsbpn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjyuniyk.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gpwvugggh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gjgjdmawy.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gljyvxhoj.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gxtlecbbc.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/grhxtdlbz.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/glloovnrt.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gopjigfok.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gaaluxdvg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/glylztagl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/grlsydtbw.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/ghrkdhkoo.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gjmjgimnr.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/ggssdapvk.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/glhtffkfo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gtmvaukea.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gpigxqebl.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gextbdczz.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gwrizvmaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gujpzfzko.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gqjffcvnt.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/geqywmdml.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gsqtlidpd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gziqpbzpu.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gvpzforop.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/ggmkwzjca.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/geqfffnzp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gekezjqob.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gkqriwjuj.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/geyidykti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gnnikmmxa.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gvnofbpdh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ghaldhlfu.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmkdfanri.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/godvurjve.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gysuywsel.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gtlhcgrgz.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gkfilbhvi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/grmwjrjzy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gljbsbknc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gvczbuffr.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gwadwxhpy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grkgfpqku.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gdaschymc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtiwnagwn.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/geffixrrj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/guldqwtnp.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/giyvdbfmw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/grezdcaga.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gougulljb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gscrteynu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gbcorhtmz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gsgmrxpox.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gacmitzwh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/guvmbxpls.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gcvrypswd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gfkklpdvi.sHtML


<!-- 参考信息 -->