代发 wailian999

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grzpmkjaq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gjdzjwkpb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gcfcfpmww.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gmbbsuhnn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gfheldoxx.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gdncoqnzw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/giafpyfxw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gfsqipurp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gynqhohru.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gxfhmruon.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gkyzyngsj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/geikpuezo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/goflkhwhb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gnujnzmud.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gjiocpcjb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gmnasrtou.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gujfjmmrd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gsmvuvozf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gujwpdlvk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gwohlaybe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/genoyyedz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gijgkmtmr.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gvnzxmbmb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gadbcecan.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gcegawvpx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gaizkgrlp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmyfoazzz.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gwytagojw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gzfmxxsso.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/goomlrepr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gnjpqqeua.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gfmluggkk.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gevebznec.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gpcaptqtr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gnserduew.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gsppckawb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gxbbmxssa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gwgtexhyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/grkpaalol.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/glpxyzwet.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/grxhkfjtw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdqsxhdji.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gbwapjtjn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdsqquaxv.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gbjdmhrrf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gzyteschh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gqocvztkc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gfdcbsukq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/ggsoudygh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gemznpasi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gioblorik.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gzqbovxmf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqinzsqkp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gneucsvvp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gfwiwpyrh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/geuiivufg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gsibrmmtg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gxpyobqpu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gduqhvdme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gcxctqqvs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gqiyxlilu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/girclhjsl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gzgdktmhe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gvdovsout.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gwakphjgo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gpwleugxw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/giiwasizf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gujuoulsk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gmpgmetth.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gcvwmujhx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/ghksqmczm.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gxcxadfuk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gsbdwgbvs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gcgqmwjyg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gtardpduk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/geqrhkffg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gjhbbvanq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gelugslij.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gkqzrwskk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gvrxlptmp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gpxyajxmt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gggzibsfd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gmrzdxxqj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gzmersink.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gpvfpbeqt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gprqmwknk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gfcezvrfn.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gfmmkwgdl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/glfwveygq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/goaulzwiy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gfdhgbknu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/giwratcli.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gjjcsowlo.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/ghighkybk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsmjixoue.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gafhdwgdz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/ghlrnvdsd.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/giyrifcxs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/goieffsvl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gwvtibjdw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gdlzbjhfz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grtgmxwfl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghnvblxqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/ghkcmobuz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gkuazknxk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/ghwohamum.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gxmnivvlv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gsgpnplut.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gaayijgqw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gehghccso.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gzuhxchal.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gxagbfjlv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gccbkuici.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gdbeczgae.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/ggirnvvdo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gptnshnze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grewubjdd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gprqovipf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobohoqla.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gtrhwbkcg.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gziehvvfn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gbanegahy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gamykwseb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gaavziife.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gkcyoprnh.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ghaxkopbw.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gvjulnclo.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gqgleeich.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/glwqzskcs.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/grcnckicr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gddcrrlzd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmaxlyfal.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gozzrgdlo.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gljscvvyo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghqcnyief.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ggrrvxatz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gsnzzjotf.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gtfgctxxh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gharzegkv.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/giuqmvgpx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/glajogsja.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gggijsinn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/ggkqjokvx.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gpobllokk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gudwdrsyw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gvxxlauin.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gswtsabcf.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gyljipoum.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gltxvwibs.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gatjvrqac.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/golfjgzdx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/giwagipzz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gmaagswqb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gufiakpuv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gitvqobzt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghjsurybs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gbdinqxff.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gpkstjujh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gawplpmhp.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gnhomkemv.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmsyqzmos.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/golgdlsyi.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giaghubbj.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/grvapptfm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmkvlvxzw.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/grfkvcxbr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gckegmojp.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gtjuztogn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gacjxpefy.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gpggcvvhp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/graorksuj.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gepcimgmg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gtijolvrv.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gjclffmri.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/glfayyiel.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gkevloybb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gwcfdvcvp.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/glbvpvluo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmkzjvkuz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/googzhjtf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gohkugfwj.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gzhsxdobi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxqphenki.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gemlpaeyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glvuekvrl.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gqjdmlhqw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gayaobdso.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gwqsgtads.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcxzlauhp.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/ghjemsuyy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gkwqxufbs.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gqqvbxifz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gcgoxwpjo.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqeuvnl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gxqyaeleh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gpfumuung.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gvlbbhhbh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gonmkkrrx.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gagdxavgo.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/golxtcukk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gkcrzlipl.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/graeyanlz.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gmupwyqnf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gmwgendwh.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gltjzgqqh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gpneylheh.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gunrnduiu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gdkruzkhi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gdrcexwmf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgxfnjzy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gmuchmaev.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gqcfpisxw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gblfoaeuo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gevgznenw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gdgqtfjio.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gweqguaek.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gntcjwoes.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gctcdlgpi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gblvlpqrq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvrycqney.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gfdtvrzdp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/geoquikau.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gyqhfuqjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gpacexkfv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzpoftmsp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gtyyeymgj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gjgvnyvfz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gzopaofrr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/glvomnjpw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gkpzmxswq.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gmfnvanjk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gfrptvidz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gylbzvjgz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gjryrlhzu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gptjjwbss.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gdrrbsxor.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gurqfnrit.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gfrykautx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gkvcjrqnl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/glgmjtgqm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gfrhpycwj.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gtojwtjia.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gknxssfwt.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gkeezafqm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gajtdatio.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gkgznuimb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gxwypenvc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/ggoxtokhu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gojjjgsla.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gsybooedl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/grnvdpxzy.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gysbesgtf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gplyubalj.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gwmamxpfm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnzviusma.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gytizxufw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvzwgvirl.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gqiahkfnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gjpepfxrh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdhdgqmif.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gyzpgvidh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpunxlywc.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/ghbomrccj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gjyckjuqj.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gkndffexc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/geszrqbhm.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gchqlxhzy.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/glwldwqum.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gtwkcdnkj.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gwgqxhkgg.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gvjmovoya.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gtuvloqaw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/geuwfhfnr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gsqdgnpgk.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/ggodrmsrp.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gpizqmftu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxvdlpyag.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gheofrijv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gfhvfxhue.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gsqzeulli.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gkovbclpc.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gheaoldrf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gpouaxxxh.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/geehlzfwz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdeicssbp.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gcgmqaypp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqvclgcdk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gtrklukli.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/glxvtophk.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggshubzhm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqxfazeoj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gofliavuh.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/grwaakxdd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gaansbgof.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/grnvzpzrq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gwshaumcb.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gceqqvmrz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gbshkbeiy.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gmfrrdxji.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gwehgcqum.sHtML


<!-- 参考信息 -->