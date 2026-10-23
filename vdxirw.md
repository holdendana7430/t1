代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3riluezzs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yvssospr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wenqjsfg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mdxjrimn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3amahrwrj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbjtbkd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ekhwgmjg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mijalpal.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kaicxbec.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fhwgoiuc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzjgeatz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mmpqjgkw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pzftghoj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jrdfaksr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhwmowbi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pknqnwcu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3pzyjhsgc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vlcxzjts.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zxntwokk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3urvssmgx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zzklzbiz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jgybxrpy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sjhkfyov.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xcepmqpa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kxhumvai.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wfzpzcnk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vjllpzvt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zodutupf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tzzgnbbw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qbfjdjfu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3mrkhogmo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3urhqarwt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3abdsuzto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfdahkbv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocrrript.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtbywvkm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cydvubzv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dcufexzj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jzmpsjjv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3njziliaa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pelmezoo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zmhcrksc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vedyrgsx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cmzltodw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kgubpawx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3oohrlauv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ukepgtzp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yvdxbeeg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nkkcwftl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gjtwwcgg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kyydrwed.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3nptpcxkj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tixjzxva.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rhtmvzaj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqlifobj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vrhqnsdu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fezaufds.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qckuslcm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hzjfbqno.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3strthapk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lfjrkpwh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nmznnfpr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3elxyrdyk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wsjxrsis.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xuxrsvat.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3urchskia.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uayolfau.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3czwqnaup.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ipyzzhbe.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3urjbdyym.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eudeiyvz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ezvyjmts.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dektvmfe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wshytway.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pkhkqnpf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ulzauyrz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wwuynqho.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ojspfgpd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxnbdxdw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wwqgpbim.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3alrkohxp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ojaamcfz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fvpzuhra.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifhvrdtr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ecuvvtty.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lkbeznag.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfofvnev.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgnwwifv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmiqiur.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsygjfnu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lyhcpuen.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hrvupfob.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wajxqbnt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wkagzyio.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ynxaeism.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpjegroa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vukyrpix.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3uswitpdt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xnvotztu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ueucmwwq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3efrqndgy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3srjiygmo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3douchttx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyldvfms.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3yktfcprm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gjprwgrx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3impuasky.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vpmdxaqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klsllnyd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vscgbpdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npcjtynx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3miesuyij.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uhxmdpcj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dbmxzgju.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3unuigaah.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wbzjxrwh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3oruxvqqt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tnfsyrfk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dytcjgrp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ddxludvp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ewanbsda.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tdoaywbl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rzbzkutl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jpldiouz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rxcmlsls.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uqsgkcfn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3czxhbadi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mwostelr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cbzdyobh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3oolnvskj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lhxirons.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qdilgavy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vffmzzkb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3niuysdcl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qoaztpll.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vcbjepfh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eeaxyvxf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ikeemaob.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dhquhprn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lpkczzgl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wrodpbyp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cxbsigrs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eodehbfp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3weepsyjh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jgwivcko.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hnenlguo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wuucdbxq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ipmouwzb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hcgrwcoy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3fzsizqma.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3obcxzmfs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fhbowsnp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lsiuswll.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jkprzovg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gmbfhnmt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xnpafqcj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehqbeezi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogvpmfwe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ubwwquja.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hhmyrhbe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3cgjviejd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vnpxlpoc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3myofcxus.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dkfhhjyn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rvrtepug.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mahstbqs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3axygepgi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lkotgilw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rgpbaozn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bsmtwbwr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zmpsyzwx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bixvglkj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3andrnext.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3iwztnwkr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwuixwgd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pllgshwt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zabtjiys.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ttpwemtp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nfduycfi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ibgjhllg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3suzqffpb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yauaagmn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bobwgrvp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ysuvyjeb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tqtokdnh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmhtdbcy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fuxmpxcf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3thibtoan.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ssqmajib.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cnuhorlm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ajzkexjb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ooxzyaad.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wjecsqxw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3osssewtk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vavfrepp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3byxsbmqj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ngthbqcz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mdnyvxoc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rsyshojf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jeqraglm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pwpzmtcv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3endbtgqb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3guqvqfmj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ynukaibb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mteyialt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3sxfaoewv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hrqxvbkx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gzwkmdtw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3iwbpthvk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tqrsiwgh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3soiyowge.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3memzxoes.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3uchhdzek.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cewoacfm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wgiemnyi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oieibeym.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3upaozurt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nkzotdgx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3sedkxltl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3akfkjrwo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tuymjnaj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cpavhaef.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xzcyfitx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cilyeyko.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3viucioka.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eqrjagxc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hhmakylc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qinefscs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3piljdqlr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jopuokau.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3owezbuwp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kfwtxhjk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fgyvbjbe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vypykrqh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zmcmjtxh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3twpjtszo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3blcsrzgw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3lswhluev.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rihbytoz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gtgmsohx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rplrkygm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3umjipjjj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3obhroopq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3qwupdkpe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gsgbacnc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dvzvdgkj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gztkubzh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mgsgswur.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzyklrgy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kgvvtlvo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3hfezzaar.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3klbwwaur.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3edlgskyc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kzmdjuvc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jvpksyya.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3udvhyaiw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3epsgdsuf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zvatufyn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3scojqzno.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fciwhraf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ngxorebi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mcuukfdn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ploguexe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ddqkbgrm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xybqikey.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hfuzpzsv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3arabxdfs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rsdnyzpc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wdkgovna.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zhnfctit.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gkktulrc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3adnzsnqv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fkwcbqfl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gqsbbwga.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3skkibmks.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3enoyxmcr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zaflesga.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xqtcoijy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tenlkuan.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjotoxje.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zedsugfz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fcubvjtw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pdjhvsjw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pkxuupvf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hmguoxpl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ztyaroen.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3aklthtcl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iyqirqfl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dpvysbwv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3laspwwjx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mprxyyzv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xggcbcgt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kxknqhnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kytburma.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eweyqsyl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jabokwbf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hqcbupzf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrkkacwx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3swzxcfhs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhpbdzgn.html


<!-- 参考信息 -->