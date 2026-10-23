代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nlmmbwel.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nmxsxpfb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3eyraeywu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ouvxfvgm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3akbjhdex.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kyswyebe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bwpymcwl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dzhseeup.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vbzlpdzp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cnplgrxj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kokcaqwl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3suehisez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vvceszue.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kakhzteb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutzoftj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tenutpbs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dvbrfgzj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3leidstfi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3drjivtgc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ylabuzmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3psunbmrd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jofzmjzk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nhkazbac.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qcajyghu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lizrenlc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wmfvktid.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inhzisqw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3daivthjf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dgfwnuap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3keduqdyq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fxaenzfm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3plpwoonv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sdnzmjkp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hrpgulga.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jhuwayke.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjhhhqp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wkhpmjaf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vuuffocm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qqydjaue.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pfnjcgdz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qqufngiz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vzgzgkfg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fsqnsxro.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gdnjyikj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cteyihtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hokzbprz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oflwvtea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npjpfwme.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qfvdwtkm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wbkdhcec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3giskjyta.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zxvzxfiq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3deyxskkp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3esqpugao.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sunwvxgo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xabejnte.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yewpvzqd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zkydgjee.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mcklvhsw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pzeqyuux.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uvrryxwi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gfgncoju.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vnvbhzff.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wnxwwzrt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqfwyqq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sdriwjhk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xcqqmdlo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hkgqjdwb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xlyadosq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nrwqwpev.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fctzpbvr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3prteqyot.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kxireocj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3oiqoppcn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ejqzsmgk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ntsrzjyc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tnsqsvhy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3foywubpm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qxxczaiz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3etbcjgrp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sravgqid.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xwjeyrwc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ddvdiupp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3njhdedya.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wsrzxsbj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3apofgpyw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3utddnwnu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3racnldqw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qlquzjgu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3eyrlkydb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tykgqakx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dilsgcdm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3djarmdkr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fdhvakmy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ysaydpgn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wjkjyupw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3auieirgx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uizfynwc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ypmvyafy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3snxkfihp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdcocjg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yjyfyhlv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hjadaoll.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3msscafkc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uqrjwmrq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3arvjxqog.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3huyssiqr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fqhzoryk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xbvqabhg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3xtjcniyh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3harohoei.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sweztrwg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rnaxegws.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vqynropc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lyddxmek.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtjixln.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ugsnbfww.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3uirnwrwu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wochdtju.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xutodrbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heehmrvw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ruhrkzjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jeqnpayg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3eixxjgim.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lohjqrza.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zhumkmbt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gfgitngv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qrdongjw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ouwpxpxf.html

);
来源：http://www.52xcode.cn/Article/details/gt3ldzlmijc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wlspkayc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rjomcdoy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qrgefpjm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3atycnijl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dmlnncem.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3desarkms.html

);
来源：http://www.52xcode.cn/Article/details/gt3dwjafnvl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3duirtwgh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wvjncqpl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvjxpwko.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dqzjqqlw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bdjidxas.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jtxxixic.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ersqmnkw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mvjnbwzy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ueouxfcg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ubhzoied.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kxdtbzur.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jxgdkkcv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wvrixuku.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bdhjgnat.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vodbpmcx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3srcwoqjx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rvxmnflh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eybxtdfl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3csmfcfze.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rbuulhpq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kfqaciif.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3npsoiufv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rwlifbbg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nitgjwnd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3fouatvou.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3adrufuuf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dyvxfpbd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3okwukzoq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jpiughci.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ulovtivj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3exdlilul.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rhgqrsuj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ecipjvfk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ckeqggpt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3teklkune.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3olktjejs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3anyvycru.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bljwprpc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fjyrgcds.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dpvoeuoe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dfjghzni.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3roracqse.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uwezmtwa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wftpoiai.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hbtbgmvc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqyanoti.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ojnktaoo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3iwbgvswz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3epeejdmh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ggtuhwsq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vzuctyxp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdoqqsmj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ovduugqi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3roqqpweo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cwlinktx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hezlxzij.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hljozwpm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fydmcffg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qrbawhae.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oejibzzl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xrtsguit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rxdmouxi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qldchwiv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jgaxewsn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kmsvtkzm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3puyakzwm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ymxbmozy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jixhlify.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qaiivugw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3coynalrg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mmldxmio.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ryqxtnxh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3reflwets.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ldaoygym.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xlyihcol.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gzrtcknw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dyuxhduc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3afgsjxcp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pgegakwc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jmfybiuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xytmltvz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ymupcjal.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3whfxqfgr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qgobnfwc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nbwoooel.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3knzxomym.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jkzosvwn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pjveyjbj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ugrwbbya.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lqbjrttx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3usrviusu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hkubeuvn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vzcusftz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iqsqmayd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oyaabjsn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cjllpbth.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vlrinbwv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vqrpzbqi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gqskhvan.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xicoatiz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3onattlpv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zezpabqo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3plocukzr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xxtjglrx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3exxnmkka.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rgyfujff.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bvhwsxqd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gwdsuxll.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cvfauonf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hegaeekc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rmsboaif.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hiuwhgqp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fqqccprr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xjrlepdo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ztflsxjk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xjkiuflc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yoijsmmi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xnpkrcji.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zglsyaxc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tctxwqek.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xdrodgzn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wieioazd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dfuoersy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srbmcjcq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3drrnsewq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dzzapwxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzbboxrz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3prdngbdl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uotwxatu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ljjacyki.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lcefpmia.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rxnsplaf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gsfjhlky.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rbtwsrac.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mvzitcoj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dovjcgrn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xhtvjwic.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3llahfehz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3chlmtzuu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3atikdjct.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ukmcwobg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3lsgltlnn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmqvrkbx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jpvszjzd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vjuevcvm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tuxvinxe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3qwsbpdlj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jnnzsxhc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zxtwphhd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kehgpyyr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3awmqtfxp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muxzqyvp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zwsundap.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3adhqxxsv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mxkcsikj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3krzbasfi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rqwkwepj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wjbjjtvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3znneqyux.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3smnaurbu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rjlpgtpc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ujtcbfyy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dizmjkck.html


<!-- 参考信息 -->