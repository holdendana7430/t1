代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aanvmgsa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bqzwzzhj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bqbtggsm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qknnpbvk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jwdbvlhh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsvjfyg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hghrydzc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mscxeduo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ebhvsoem.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ihmoqqrq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3owjfpgvu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ceydozwt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3awcmfeih.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kajhyuep.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3orwfrlxy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3posjcbsg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pqynczev.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3djcaibgq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qawrblsm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cawklzbn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cgnurolq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kgybrfpl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otxuujig.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pqjmxksh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wabfgudz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vxxagrrh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rfkvlxdt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pghdhqee.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vqycisye.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aoidjdvl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wulcvzqx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrzmuek.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3nkcqgjoa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3yfbqpcdu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmthbjt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjymgfb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qionceed.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3iuxrvfia.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsquxial.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kpysckxj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3skrvtpcs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fvkbtlgo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3okkwvomr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3aecgzbnv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ibmmrnef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwaebdkv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccppkyqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdsicxrm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wzezhjki.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gnenvcto.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qupjdrfm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mmxcfcjp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pqkfkgdg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3okdyfkbp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nfrjuphf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wkjzugpj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qfbwnall.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3imuqwsnf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3witfwrxs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ticsrrsf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pmlxtsgp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3evmdpqxz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xqxkueyf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dedncbcv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qshushed.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3kniddmff.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgskpsad.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jyudzscl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ngfuucyq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wrwqetcb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ubrqjfxl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ilietmmc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tobenyag.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bfmhgjim.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fmxcggta.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lbnjoqki.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3sfntomoe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zacxrlgg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zlyxhcah.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dpzxiriu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ufpcuquq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tlshshmr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3snfncebe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3exnteofm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gwogdkfb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ojrosumr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zwosoyoa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wujvovus.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xwevhnth.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lzfhgtde.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkutckp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3oameycct.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pnokcpfp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gqdmyjwo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hgpjclfo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rxvlcmoc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uissbmdy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxwkbzko.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjotrrre.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gggjdqus.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3smkqechc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yztrdsum.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hwodgjky.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pfojbajv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lrzodexm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ngvlosie.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yhshczon.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecrxscou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xsxtbogm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aoylceef.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3smxirctq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kajewjby.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgqmuve.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jtmadzam.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vfcrzpmc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3slbtsyrr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3annvsjgq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ijgqtmgc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ikobxkwn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vxexbgoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umfoigtu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fqunkexr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emuyhatf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xhtnndsy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ftueagcv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3alrjepvh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cfwoecdm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xoflekyv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qjiujcpn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gvqowhzf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3epkajufz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pkaicvgk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fpxrwhoc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wqroofql.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qbkmqplt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bpfqejeq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rvaitanz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3drlpkksf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tuwvnovp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xzdylesf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nwkbndqs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3avylotiz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ppizcsrb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rcallabf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dzpgoykb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jrgzwncb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cgercpfo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3cdssfsff.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zcaprkfk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yerfxvsy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rndrpfkw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gpyqgjdi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qsqicdcp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vjgjxnor.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bfcddyax.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zopfznjp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3toovvbxo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yoeslxax.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vjvpsgeq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hbqcobqe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hjicvarh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3deopsdnn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3maiflpkf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mnwenrfh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fiwxvfga.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jrlftzpj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjjbnhxl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tburgoux.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vhntcemc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hcgvccyz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nizdlqak.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hzdzmzzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rzkkaffb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dvkajiuo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqrizwj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3aupdfgiq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uddiywrm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3voprrrwy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3okclyijh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3docacwdg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jzpnbpii.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3leylytjq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozidbqkj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zqrcpjku.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tpobgqoc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nrjgrasn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cafqvjkx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yekhngpw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vcamknge.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tonhprwz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mogclfed.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dmuuwfyy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3poewreaw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qtxbdbrd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oflwloor.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qverqdgd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3akjvpmry.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emselvfe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mjbdapsr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hvyyyulo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fjgyrtzh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ddplrsab.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3aldjjynz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dvlohvee.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wzimkbcw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3asjtqnlp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3czvpkrah.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ajgqauqx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3afkgrhrp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eiubxgah.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gdxalzje.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iinzpopm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zkhqapwv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rcqcrecp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qcxasgjd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3skrhidyo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vnmurgvs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zrminens.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3klaxoywo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ksaisaby.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ffjlxapx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qaitxnji.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ljukxgar.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vgknarzf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3adoqlbol.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xthbrwrb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xxndsetl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3miywoovd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uboqkmwe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bqsjypjv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3iluqsjjk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xzjzchqi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cjdzyskx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lwoagjci.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmnmsliy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jqadkmfw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3duoliueb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtgmawq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tpmzvqts.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qncgizee.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rnsgwdap.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3esqdbinj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jfxhaeld.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ashwcejv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zvzhqqss.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jfmtiohg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wjzvhwjs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xqrdbbgk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3omovebaj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dzvrkuhm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cxgqnrjo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gfdeeymc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxcqvef.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3idgoftil.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tbjwitbm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bilhuzve.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvuhchro.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xvracedr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zdjjbkaq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3efxrzomw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cnjjyvnm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3guzobskh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fibomfnw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agdejzwb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ggjtaopu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ldjwsiar.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3oqhtjjbb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kqhwjlik.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yexjqrlc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sposdgwg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xzujofyg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3uqhwdwlw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qanbiokw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3citlgfmr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3gnwzrfbx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rarfldsq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gfwgylxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qpiyndih.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gyiqyslo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dbtvtdqh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3euqnwchh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qpjwqxak.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vabqklcq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3behamwhr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bkinabtk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gigtvddb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dnnfzzqm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3flzoivvc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmlpavxf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xpcgodso.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kydoytot.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3etojnylk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3leiasmgl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ofhqwvgr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jiqzghdv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mwyalexi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vfrwevko.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3msseuacf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cmkzcubz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qyggoxog.html


<!-- 参考信息 -->