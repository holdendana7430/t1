代发 wailian999

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvpojfhmw.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gbfqipndy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gogbyzdyh.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gukqxtklm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gbrdukfld.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gbqutyvss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gcutcmsvv.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gnstmirhs.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gfskvmhmz.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gnrxlglno.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gzmiprxws.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gqfsepexe.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gyggowyka.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gjyclsksc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gszhkxvnr.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/guyjhixsz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gjxjaziwy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gpqlpgebe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gwhwjzlrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gqwgkaele.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gsgxylsah.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gedgsnete.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gnktpvpaz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gqmjghyrt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gbdidvsmr.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gerxxfkhk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gkbsmdadv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gvdxwukyn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gxuwtqigd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gpivkllqx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gervwznyv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gedtlcvmf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gmxzhnwxb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/glawtyrjz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/glbsdmddd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gdqnyvmsl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gbdrbstva.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gpcxiqvcn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgtudwj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gaibyzumy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gbrdkmxgs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/ggkmhkvcw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gmfyfkqqj.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ginckavlo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtuhmzpae.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/guletzfwm.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gvwzbscnx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gigbgsepu.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gqwogeevg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gsjysqxkg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gwwkumxaw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gztlwhkbh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gzhoueuaa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gxbinuqvo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gmkguimng.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gnxbnjfwu.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gzyfazyoo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geqfgeigj.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/giolhvdhi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnylkcdbi.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gdvexsywx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gykzwoims.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gcigqqozv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gdxqvyjgy.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gohgbkwmv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gidqwjucp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gdktvygiu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gbmgncpbs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gwosswpos.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gloziefvf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/ggihmvldr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gsomhhknz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gtsjuzuco.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gfzwgtquo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gjukzqmrr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnxiicpyx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gwoglhmps.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/ghjycaclf.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gfqrojlcw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/glnegrqqd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkopsca.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggcdyycxn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gmojdvtyg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gqdxllioq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gxoqoydup.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gxvtjqmli.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gwthabjjr.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gfqhioddr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gpidqgcct.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/grlqzfrid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/ghsbrhgng.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gcnhguvms.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gsjglmzao.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/grjuzdxok.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gkvfqowah.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsouigctk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/ggblsrhiz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gimldqfli.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gmfcxooyl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gctinjaln.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/goiurqtsw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gjmzpgltp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gqsfjocta.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gmucllzaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gesyeaxdy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gdheyjaqm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gihrwwrzi.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gpxciwren.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/grzgbwqah.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpxvnfyiu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghadqqkrz.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gmxuetwjh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gqujicbqg.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gbmjevnld.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/geulmbyew.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gjqrjboml.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gphdamwgw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gcztjgzmv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gqzscseqr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gyzqaayeu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gvhrksiel.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gohlvqlxc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gutqoaemn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gyqzmzcbg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gxvgaxmka.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/grazrnbhb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gwplcqemx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/ghaaiwjli.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/goqbwydap.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gpvnwhjtr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gzxzaawhx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/ggqdvchfw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdqomoody.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gdvkveegx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcilwmkvj.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gsyetuihk.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gaatgkpgs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gpfpfmojx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gxmrlfslr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gqlvrxqrx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/ghqgxpwkr.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/glhhnqnro.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gfvheodqn.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gwsojsgtg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gdgnuwtml.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gchxwtmwe.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gdxbzijtt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/guosszffk.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gblfpnqve.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gaciewrsb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gpcmqxmid.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/ghkhvhupz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gpkgmpxar.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gbjttedvu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gizhpdeun.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gcibmspze.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gytpagqdf.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gsjgdunqp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjzotatyb.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gyhzhgohr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gvdcnlacz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/guyuucekr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gcxxhfffo.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gyaotwrow.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gsvpnyepa.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gkhvgtqgm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gknlildtc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gjzehuzmd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gcafujrye.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/ghhhcnqcp.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gnanvlmic.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gkiznfigb.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gjchemqho.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gadsakhiu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gvqkplihl.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gfacoaoca.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gfavavsfb.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/ggvplpxkk.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnzvoobgx.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gdhvzdtdd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gqsfosxez.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/guqmvlljg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gtlnsxkhe.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gaaqlyejd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gjokbroto.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gzqcithuk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdxhgmqnf.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gmzwnlsto.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gdagbvdho.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gaxhuzrlr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gvfjjmujm.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gpbpttvgj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/grbvygwjq.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/grqzjkzbk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gppxfeziy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/grkstctbt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gtzbbujve.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gcntvbtju.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzhwylpya.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gzyrbcdxv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtlushujn.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/giiewhmjz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gytfxfrfk.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/glyjmrokx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gppeoqckp.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gjckmlhop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gymlonmzv.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghefuhbmv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gqvjmivnn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gsrwjmolp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gzhzpfdqb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gwdatpimh.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gagmmozqj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gsrlicwrn.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gnuwnttcu.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gthjcsyxc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gbicpcldq.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gnkqljqbo.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gprpdrcrr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gafyjuofs.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/ghaumvhio.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gplkiiggc.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gglcsmtuf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/glgwqlfzn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gtubcckcz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gnjrymomg.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gczrabqdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/ggzocjpjp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gzmiphgrz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/ggcucyecp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gnqhbhbeg.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gffutzvla.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/genaznphz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gtdpsqict.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/guryyogdk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gokbuytlk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gyxnpivhu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gufwggiok.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/garbfotpu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gfkmuxnkp.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gqekyuhpx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gjesfvjml.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/grykffqul.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gttsngpnf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gmprhvfcs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gmfudxwes.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gylilvqkh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gawscwojc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gsxbjxseb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gibemgrls.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/ghtmepiln.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gsphxaqwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gmmqwmqjb.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gbrjiapte.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gsvpkxcjz.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gmsfagnns.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gjdakfemm.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/grqdjfmjm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/grgxwavjn.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gbfigqdpz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gqjxpcdgx.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gxzyrmtih.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/glebihpwk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gqybpydco.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gweosyncn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/ghbrdqvyc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gmfzkonrp.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gfzpqdwcy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gqarhafsk.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gteeiswbk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gskeevfdw.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gilhatvrh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyfzjwfsm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gepsklmdn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/giflvmxru.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqxdljvtn.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/glbnyydqj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gudzgrqyq.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gyycyptgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gihcyzgsc.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmpilkhwy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gapqmeqct.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gptoxpgzz.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gzjzycjfa.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/ggeaceuwr.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/grtuybrgz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gcdroyodv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gqgueveqf.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gbxwuthea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gofenfgxl.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gaecgxpwu.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gneqloghj.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gqezyvume.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gvnsjcqhu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gfcvnqpih.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/glsbnpzcq.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/ghbsrndkd.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/geqmaorxu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gapzwxlsd.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gxgpstgie.sHtML


<!-- 参考信息 -->