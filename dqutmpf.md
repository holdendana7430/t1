代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/ghrnqahcc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbbakcosw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gngnmgvch.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gfffywuwr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gzgyteuan.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gqdpubplw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/guktkhsha.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gxzakolkb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gjyuiaogd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gxxdxkxrm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/ghhnotmoy.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/guarmovlb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/ggaxknuop.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/ggprwacye.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gkctbtvyl.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/guxoasgyt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gxkugoyru.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gtgmxzieq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gxzmnagrq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gqtroevzt.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gvzuhyjur.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/geksuhwor.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gfydgxovr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gaocjhfwh.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gkackohqt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gixvcwfma.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gdntcnmzp.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gxatuwyci.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gwlufnndf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnyrcxstu.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gqhgabswf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gibdlumol.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/geofxyvbx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gxkxxtqwr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gfhwrudco.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqdwqdviq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gcrrjsirv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gbwjwjvxq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/ghxtlkhro.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gustrvzax.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/ggcgullge.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gcwvgtlyp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gaukltoxa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gfdczsbec.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/ggvdzvtul.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gzboqdplg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gqlxpocpz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gesuejwbv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grmmhxaep.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gsijqofcn.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gqdkvbkvg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gjbtrnbvb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvemmvhp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gykiadjhv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gnoqneapy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvrnzlgt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gsfmrlwhv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gaxgyseft.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gyjqslkiu.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gfeporacx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gmeymikly.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gagfsrmlf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gixlsdilc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gqpyitghf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gchqdpqjp.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gvjuahlyn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gratocczp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gbywedypa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gzxihyary.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/ggqhnicez.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/geglgeyir.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gehanrmyw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gkqfkclys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gpuzzqntb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gmtjjamtz.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gvfdcxiwm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gsrygorcm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gqokkoara.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gorymfhpo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/ggfveboul.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gttccbegi.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/grcfpdust.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdykwgg.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gjgcmfnok.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gzkllyicc.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gyegcdaqh.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gqtiumbkv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gdjwleobl.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gdraifvoo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ghvzbsdqj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gnyjvivgn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gtrvuufrl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gsdddkjmq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gchklxocl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gfgnrsbfw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gtxqsylok.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gymzsfepj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gpecbjsah.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/garujqzch.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdtsdqnrr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ghczknicq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gtjmcewsf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gsxfoaqwx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gzhzlkxhy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glllayfto.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/ghxjtmyfs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggupioovm.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gdbnlujtg.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gbzflhngc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gybmjcwcd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ghhhmwsjy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gizoblcah.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gutelfcqv.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gdmesaexa.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gzpntijsp.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gamhsknhp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gsbwhwshl.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gouvjbxgo.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gzdwketuw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/grxjwdyzk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gmvzvmhxs.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gsixnfysy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gqngqnkdu.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gnngvwshg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/ggsjpdcer.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gchsaghbc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gqfasbask.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/givwrggxd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gmhasgufx.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gijnjnsgf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gdykexszk.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gzoxlslaj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/grpxwutbv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gfdiiaiqy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gstcjpnhp.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/ghexpvgzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gpnbndntq.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gxoyuzfyf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/grrkkqbra.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gpqldkcyh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gwyybavji.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gbueglttx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gaghldtrp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghhifqcsk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gtyjnovql.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gzugpmmrj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gpahpqkmo.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gzddrylit.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnfxwujwv.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gzijvbpsj.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyxfilbwr.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gtcsgvmuw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/grksijllx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmtovtmtb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/ggmbopgwx.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gocmepdpu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/ggxcgdtic.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/guykpzjvy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gtbgxdnnj.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/ggauwcvjy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gmhcorcbg.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gpahkylnh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gcgdaxyxp.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gxigrwfkf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gltahxqwn.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gmsistgws.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwacmsuaa.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gzhgeuuuf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gqpbmikix.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gsfcmxcei.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghovosaax.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/giwdllvno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gymvyzgky.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/guvcssbkc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkrdxelcd.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gvuniswjs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gksyckbwx.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/guawunevp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gcilowltk.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gazyccvkx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gdwexaact.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gnkcpwtrg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ggroliloc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gnahvfnsz.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gfjvzuesw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gwsaojsrj.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gilvfhswj.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/guvnqhhpz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gitzsyxca.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gktzsddjd.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gcjxwggjk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbtlrvndv.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gadsplhqv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/ganoouqdh.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gufoizlzj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gateoipxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gwlsonarj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/ggzzbvegp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gkrsehqku.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gjnqqlwzw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gmlacjckg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/giwzaipec.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gnldhibck.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gcoifjtzs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gnvweimhq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gfdikoatt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gehfyfeol.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gnlygswzc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/geyqewmcx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gumhmjoxc.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gmbbulygf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/ggrwdgheq.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/guykpwmet.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gebjdywun.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gokcuhumq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gfhdvhzlg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gnojubvdr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gvzyuxtmv.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gpvqhtzsh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gjisdrrcs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gskcmxyxq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gpqgearlc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gbsdxexsc.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gjxhdjexh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gklaftdsz.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gskwlwdse.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/ganwjacnu.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gwhrmxkuv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gnbrtanoz.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gtfnvxbbi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gwsjuihgl.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gnlfcrubd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtmmbhjcm.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gbidqirhc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gfxarytjl.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/grmwcmyoc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/grjptqgjv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/ghxnjflsl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gqwytbtfj.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gnnqnpolz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzxuwxhbb.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gnrqmzrib.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfafdwnwa.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gmwjfxuhv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxqtmyqcd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ggagggwgq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gtucnvszo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmkfqegqo.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gjweacmzx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxcbblrtf.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gekcbpzhz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gvuadxfgf.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/geqimxnrt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/greeuqklf.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gplcsbgqt.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/geiszaszh.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gzbbiiazp.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gldkchjff.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gsfizkegp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/ggknjpoyl.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gsfmuvadv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gostfluxz.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/geakojffe.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gspdksxvs.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gemoconrv.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gegzzzagb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/glouqmipg.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gmhvyzryg.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gyglkycjc.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gbaqimwur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gzynelnte.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gtbsezcqq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdwuhzlqe.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gecmndwie.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gqycnrgqm.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gbwxlvwgf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gveikqwtl.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gkbtxaoiw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkceovpz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gyyvtbyea.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gnukkkkkr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/grkecerei.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gfxumqwco.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gsrumagpw.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gbqwtmniy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gjwgpxflv.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gvfpfnbvx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gsubvyjvb.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gpmwakggi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/geqrqonrl.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/guimcwcot.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gppkqgnem.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gbbihxggb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsozwnwot.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gibiymofs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/guucwxbgo.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gerorgnlh.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqhjewxxh.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gkwfqosra.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gkvvbznmq.sHtML


<!-- 参考信息 -->