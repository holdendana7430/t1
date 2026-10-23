代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3knfghzvq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3krskgqpx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bndhlacx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kekrpobm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3grcowxut.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kaylfcoj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3didavlhe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3couuhgau.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3iidqucqh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajbigjjm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tinekihv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yewtleov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oizhtuch.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3skyiezpf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfsimryc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tclzdmxg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kxurbpan.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3knslwnwe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gueoehpm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xcqfojlm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vlykgxpb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wdnibqkv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3knyatelx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3reyhbxyk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lqhowbuf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3geeyenzc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cjfyyzyi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ohgorqhl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wtqiswkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zhffefum.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jictouti.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yudwwadp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ohmotajg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hykztvsd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3agauiksv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slhimpav.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gsizkldb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vmbkfptl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ihpwffzp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gyratpcz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mkerdgfi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sbjynobn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3geyoljzq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rboqglaf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cbyyukzq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fsjjsvir.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zdyyqqbr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ksjmzawk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3segbwwgt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lyppkpxs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wbuuymgl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3aosvqiby.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smvopwgl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3evufsitz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ikqvdeza.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3reouvtfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tcizuckn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frbdcnss.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ozhuqqfi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lbunwonq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qlzmqudx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kptqfoqy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ilnracme.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xiuafrca.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ccdodlys.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijsnbjpt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cfeoxfrc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gkxlqhii.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lygttssf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ffwwjddm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bqfhloqj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdtrzf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3exsjvvrp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cdeziehr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kaduhwml.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wighnurr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjtacbk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3llgjglsn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tskcsgrp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3yaayvrkb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kowrujms.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3noplbbqo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ecokctai.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxqqufcl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3usmjkfrd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksuyavmk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwlnnebr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmfvufgk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgfzfek.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mvohuway.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zfrdmiep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tpetcamb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xdlwahrw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3beavtidx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yjyvtjmc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3etjvghks.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3taygkwgo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vchldifg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zpmjihyu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zjwrdrnu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mrpkaqjr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhkyfcqm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fwoxrkth.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ncjoaxab.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ufbogmio.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3canvwruj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3leeshbzc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ehqwygiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkzybxtv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3inlheasp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcyhhmrm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mktukkae.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vibanttj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oeyioztl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3penwsene.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ngbqwpxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3uqracakj.html

);
来源：http://www.52xcode.cn/Article/details/gt3zoqmmrre.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3docyrkhl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zzbtajhn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xlfxdask.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cufzwuep.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yjtziuik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3oaijyanr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3enqscgcx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3iszflcmv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fsjqnnko.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vystmpqm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hvaoqddb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3arikmozh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yztjobdx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gpovcgjl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uirvfayr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3imjnqgce.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gigcwxem.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wvwsbmzr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mpixmqtd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3crxigelc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3supngjth.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wgcfnquv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ratbipie.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3majenvuz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cncthjdz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ieahllab.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3iguomfcx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gxglljmk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ufuwmuck.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3owiovcjh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ymupfluu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cywnebgt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vesqsvqx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ezapyjsm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvnbnxzz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ppmbigqp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tzklozsr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukqfvzsi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3loclskic.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qqgjxiai.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3grsbhgwr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3usitxrtc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kepsmkzo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kdqyhzxb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ooebfczc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nhorrkez.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kswxkiki.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ygpqhjto.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kiuespsv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xinazzyz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pajwwsbp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xcpdwmtz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zedvrdhe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lkbzmiho.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3iizqnsep.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lcreyvnx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ywiyygtt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zemdanuw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmykwlbk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nqjvkyjt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbybhfbh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3apbyhfya.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnaztmxt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3acorbrib.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3brireyyv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pwuqubgg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ftolffus.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3csmnhevg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gkfxbhvh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hcojkumi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ciyqkcab.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rpsywxms.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rrvwwlyr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ofalliho.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3cpcelmcc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gfivtdmx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3oiqjzyyy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nctvhecj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vusapkgu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gdxuefkq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jeugqxxs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jvnhaxel.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3loolubfz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oqqadsec.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fqtowfqq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yguxrkra.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3njrvfmyd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hxmrgqjj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bgzifnbn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uvlhpofm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hnmmnwhf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3guzgbicq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kupznxbh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qcobnvtf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3udsqxvae.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3aiqmtzie.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qnwjxlrb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gifowiis.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nbhriles.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zhktgnwg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kiefvggz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3edthzjua.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zwrrxbfa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vgtvhquc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xenmhskx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3feclkqcz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3slnbaikx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sfrvwntu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uggfwkao.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rljlvqnl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fjnaiycr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uiicdnmh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3refnetzj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ientzmqd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmhggtvu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3baugcdbu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xqnqkkte.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nnbpukze.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oqlbkyih.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lgpqgmwo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bunpxcpi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lzraqqxn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kybcfody.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jepkuvid.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ixfovsic.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ghwkvasv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhueljfw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ddnfwgih.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lovaampb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rzwzkfuw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mxvxxvmg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oiyyxqnq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3utlpytxm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3auxotnhq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bzecyxhe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pskzmvsa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tsxoaqgs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cwiroftu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sqbjvlyy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bfrtqlmd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3scbmuhmz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3etdcuxft.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ycjpgozs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gylwtltu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zrdkawul.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hstmjvra.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yitrppat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jtfhwxte.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3aypkqqwv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ifvywmnn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ppghpego.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qyaiiefc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ljtqjngq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3htzrlpby.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yiboefsu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ulhmcxrb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zncgsnkd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xtgktphu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3albnssiz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rtmqvcsq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vxheejvp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nkkvveeh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gkamljhm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qykndgbj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hkjywgkh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yarbmuzl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nalpivtu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ngmuztsy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3srmzjioe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bmjnqrum.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nbhwmlja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qkuxblfm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wvdnvfva.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3twtlqjzh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ehfnjmfg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ululxdzv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xcwkhgoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqubrdrw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3avrlyyzd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvfqadrh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3anwleefs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wywbltdq.html


<!-- 参考信息 -->