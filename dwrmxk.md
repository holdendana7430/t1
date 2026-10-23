代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlvdleio.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgtbumax.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zmajcchp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zimoxlkk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hysfilxj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mstelgho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jefbfifm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ltvildao.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wrccdzrx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tpedhiim.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3eroizeie.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wcqdmrnz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mokkwnda.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3oezwvbfw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3odzxphae.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3drhzcdcv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cbppuqwe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jevvgfmz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jirlqfpd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mvmozshb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wuipzdun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fntubofx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ezhpoziy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jqbnbroo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tssmjpsb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3aposnqfo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mcynsolu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ewbnkjyc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bmlljehy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oolfhlpn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfizlnhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qufqyjml.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rmqkqkaj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mhlfkpfx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hmxfdbbg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wnzenerm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bqqcsqls.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tsxohrug.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3drwdrrtk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ejmeymwa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bfucooso.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jaaacpal.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xsdohtdw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gjogsbbl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pmcyeqmt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dxsubknq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3aycbnfbd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3nnxjxsbb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3syhgsglh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sfphilot.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eyhhohhb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zpulglng.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xfpwaexx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wwtjkuvf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wlyaalpv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jkudflgv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3skuzugmt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3temoyioh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tmbkbbif.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3daxfpwbx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vwrauqso.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rkeweice.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fvdzgsaf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jhwfrvfe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pryxsxbx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3avnidnig.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3swgescpb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qoaouoar.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uxvmzqlj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nlcuvcsj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3azanulja.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3yltujvxt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhyrnptg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3oasqhkwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3enwzbjqb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wnmftcbg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nlvwfnrr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3uxlujzkk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jmscpyxe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqxgdhfu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3cemvbjqb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rymvdkfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfjoaevt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xqyktjmy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lhkqwdsa.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gtntyoaw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mujnikbr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vqishdbw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nckyykis.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xlxrtfnb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rynlonca.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yemucrxb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yleqxsxl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cvaazvyc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3kicjxexi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rbpjweso.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlixknm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cnkrirhf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iscamqnx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aytwljbc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3daznjejl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ucrhveea.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3iutmjifw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ntsmazsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyvabmjb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yuvapsus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvuaoahl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vcvyaxtk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rdapvuty.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qnppnpbw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wywvlzce.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3iajbwpwp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fxcytqyf.html

);
来源：http://www.52xcode.cn/Article/details/gt3yqdgszsx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zdwhupyp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3skfuhogy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qwixovwg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bofknqij.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dtsmilkg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tcngrnda.html

);
来源：http://www.52xcode.cn/Article/details/gt3ctwylobs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hflwlwtj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kpatztya.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ykztsxhr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kfiyldhd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3icoksckb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gcnoicle.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ubzcoxpm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mpxupmtc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xirrqiaf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3exyutlra.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3odgyfmdz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dybzrwxr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3htdwhowq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hkgkxbce.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mempglwd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gqgajugz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3odkhyigo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cvpxfbug.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rznjrbjo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hiwilsqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vckmjucs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xjdevbqh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xksbminc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3oxbkyctf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3atcporbj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fhwjgutv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3odkbwxtd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnoktpas.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xmzlkfha.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzmahsrs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kszxqatp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ssttgxye.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ekdzozjn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ioyimajl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lhzdqkrz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ftsdledf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3flxafjco.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bvoaapxe.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3yqwdbycv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3otorxqiv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dwmrvknl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zgctwwoc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mmoukasy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3xcwpyeoh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3efebshfv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tigibpgu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hyxealiw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dwpcoeiz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3leotemhb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hmxwymrb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lzerditd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wfbkdxez.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lfexxgnb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ueyudpxs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mgknjswk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3thntpazz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nhgawwho.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bxpsgdhv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3pimojtfn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3epltcroj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ssprtogn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ymzgqegw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xtkwrotj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3efcoxgcb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hjbraush.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kqckfrrw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jlxykgrx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fkbwdbix.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlakxugy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tqrhzuga.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gjvgrhlo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ebiybtez.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hqvrwdbz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kwmawfiu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xrgbdorn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3afvdlqkb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zxjvqfaa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fhpmjjip.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xbgdwneo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3sbumyaiy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cndvzqtg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kmgyfjgr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3etgtzvga.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hbdjaqwz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qzxwgosz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mfhawclt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mebfnyev.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ebdzxocd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jiedtqff.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xodwdewc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vzbeayxj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ttmnubuv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gshuncpr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xiytxslh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uikgcgew.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3klbjzifc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lksoaltq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xjaodqfb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ymwboivx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zdlxdyqt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zmzbeosb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hyzsklwh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3omqgwryd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yrlhwqco.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vuumkdac.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ggtzmthn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vznxkahw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwgzcjlm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3usvemxkn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kfpnwwwc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vqimoaca.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pblcyfne.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nhkbmayp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3sfcrlsew.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3schcmufg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hafdicns.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ddrbmmau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tdwfwcui.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pzzxrnee.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ysqgdzyw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3iqsnrkjg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jhebaigl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hmadrtxg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rocvvnoz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3pbhttflw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tlxrrzfu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3szwchtxl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3msroyhpa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vgvwlzlf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cuzrcwng.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ntbompvm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hfcmllfr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3disvqqca.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fiedepxj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ftgqlbnb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nrsoxrqq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gaqwvnjx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3gyfncuju.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rpplnymh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cattblst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zcnpyuxt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3frsubvwt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3iexlcdcn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lmdsxnsr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3grrjpdil.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wsnuphua.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fulfdnhw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3nopnscdy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nuprdgej.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gnktsoyh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gcrxwfvi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iokjtnod.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nsxkiynu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rxoiylti.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3noavdcfe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3maxhlhiz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sjryotof.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fptzwyxw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pmmckixx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cnxjaecc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iccnjncq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ckcarkgb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wrwbcstz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ylznasgz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pdmrjtzu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qwlqmawn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lbmcbutw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dzbofhqt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnqwsbmp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhjpurvf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tnbuqoba.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rwjkibjl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3invfaydp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqjtcavy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfdlengj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tsgycvot.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jufwxoux.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gpxoghis.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ggiogoqb.html


<!-- 参考信息 -->