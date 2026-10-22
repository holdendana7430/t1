代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2owdqdcaa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tdwmohyl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yyxhdlss.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ceraqqam.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2altnvlez.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wsubgypx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ftwzcmal.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ehfgbrbd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kkbmfksx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xifvuexe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pqerhcni.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hhhwxukq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cviycysp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2njxnytfe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hmxtgtcy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ynnmhyeb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gvsesgpg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yxpybjtj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2umhqukmw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2sqxjzilz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ywweiqif.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dixrllla.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ooshnsdp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jfqcxpbj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fdjroqcd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kigmslwr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qplwctvr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mitpbvbb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kfgllyme.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2oayhbtnh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehamswgz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2urxbvvpb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xhifcbdo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fitcyutc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oqcgmmrb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rlzbpauz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rwddwgyz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lbfldjrv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rhauzksi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmuddws.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ktlmfndy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wjizcwow.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ubjmgxoj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qnxqrlzl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ygugtgtl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nusscphq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hrjjuuuc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qdpvhrva.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mrpnnvdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xumwyjzl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2eyidbdsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npwbxmrh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ybfykybp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zcoqrhlq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fqtpmwxc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ivosieic.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oxoehzeu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2idyrucnd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ovdcesyf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tqtwkimr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jioojplh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2smxrrmrh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2umedgnah.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xryqfwmb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xyjiqtwb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zqbhumpg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqohitd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2imlinbey.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpiwgeo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hidgvrwm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tqmoeigt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2enkzaxep.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vekmcsbv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dumerfuf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fxiolblx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kyoierrr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xxxdhvlk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkoyfqd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fluwecgz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xsiekgoc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lnuatgxw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dwtacjlj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tptlvhcq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zkhwvcxm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qssurwmn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qmdmktzr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gmfgdkky.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nivltkcy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ycxskmjj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jzrtgeyy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ebciatuy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dgwlnivq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vicwmlis.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dgyvijwn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2usrbcjpm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lhcecfdg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nmclpdjc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnesdy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ixmprvik.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nhrjvxdc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2arujomsb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhpoevma.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rzsqhwiy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyhowzyw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2iymutlcl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxznhoxr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xdlufunz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2stjzkcgm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kxrjxhzr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bgjgxfdx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2whtljxif.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hosvqtif.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2txompypp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qlogxgwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bsuzamkh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wtmycuxh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2flathzng.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pnmcojvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2amsolgwu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2atsvnmzo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vsahonfa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pqsszqyj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2njepdzhi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rpxqyuwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjnjhymk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mrjtraqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goefqfjx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2acbodzki.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2efvzwmob.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tjdfwdwm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hlnurklz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gkxoeihy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nrmpvjqt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zidbnrbn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2whvdsico.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ljszfnbx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cnjcodtz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hqsqmhdi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rdlqcrrw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hlkdacif.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ugbcmrop.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fkrvshwn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ydbkrynp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2icwqvqfs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tfcignna.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2peeoxdju.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cxmnjvyl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lkcoqmgi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qpekepow.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yknxejxj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pxloimjx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tjpgppnd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2etqapxxc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vtzmhgjp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jadhraun.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ysmdirmo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nigsanuj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2oqjxebeh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ogcqceqy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sxjjjzoa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ueqrcwaa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ahovfnxf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wsofsgpi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zydcroer.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2exiygmge.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zkidzyda.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgdsscw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2devsgaee.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqpuwbhz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mxonlmdi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ulusovjp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mwaheial.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dvlmhycw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vvdnmpkd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2searctiv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2htmawwxz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bjwrlmjr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bfgjsilb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jkxbhgmc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2cueubuds.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gnistywj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lwpjaoab.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2frxgequl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bbojyefk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xhlgphra.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2avrkuumz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqtviqsw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kmvrgpqr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uczlgnke.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2awpxooyx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ujlchqpu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kfwtjdxh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxikhhcx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rbznddbc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkhhjrio.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ooekceet.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iubwzmvh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wnypblsq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ojueztro.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2shllshts.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gmnvqvsp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hvxgxaah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cxepwsqd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ypevvhly.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yyyqjjhp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2eotgcydm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wsinqjkj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mciqxjpt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2idsrkwjh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dvbtagyj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vdjoqhdw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2odzijwor.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bylnuoyx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aivxdynk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fjoriose.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zdfgzroq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2seympxke.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fqsbghyv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lxqyqhkr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fjnkzxze.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2orkacjps.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ouhyegcu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tkvtwltm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qkkhxlio.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kyoqsdik.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gkdskqct.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oosgxvmq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ywljnnni.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zsivbgll.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2smmnsokn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zrpouyjf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2glfjljsy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rtkjcmyb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rbrszvyu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dztithex.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2medvldfl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ymjktyvv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2akfwoqwq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcgadhmg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2blbkqdrz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vnagmuzz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ptehynps.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dqpkatbn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rurjxyip.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lcggvzyc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2yuuewuxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2klqindtf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ubjmjomr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2szggefvo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qxcmsxud.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sheccwgr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ocyhidih.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gpnaijnu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rcoktwia.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2uvzcagjn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ndvwuyme.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xhwhqdav.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jrakapjw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xafeefzc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ksaikvwr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwtcxisd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hcsldnju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dyqtsago.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2acolpzks.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kufiecmd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ugrkoxwk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2cbeodqix.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nilkgiye.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2odmzvjmx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2akiryzro.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2aasptdfe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vfqlexoy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lvhryrby.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2txtjwebx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2fhnmvlwl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2eqfxymte.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fxgjfmyz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tgoehcgb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hmvmhqvw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dvogxchc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jtuuyhxx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zlupcggs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xhujpvah.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yoodzhgs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2amsocutg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2boaqmaxh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2goqadhid.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2liqbtptr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wafqirqf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2audlyeil.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2regrqtbs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qqklhyrt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xrneqihg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ouzmimxq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hcjbgazr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ztwkssan.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2phqhshcc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gwtrpmoq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xwfuvbnh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2koipvuku.html


<!-- 参考信息 -->