代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2inavjfjj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nrhuhrzh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2voxouokb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qndbxksd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nzhglxpv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nqefzioc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmnhjqq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rbzrilsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrjmoxti.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dihlvvtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deacojzl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2anssratp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2aszihmjl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ynmoljbl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ljmgmxwa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gubreovt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2yfhuwcpp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lzhiqoeu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jvsienjo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ubvbjlyp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jfimpuim.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nllaltxx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2isavujov.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vbxdrkji.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rimqvvpv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ujlwodkm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zeblaazu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fqmyckvm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qzowrgyw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hexixrav.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yevqdpcu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kddsngog.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2woomptjl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xzxddoit.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dbyxfutw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2exjyyyrh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bkbfarbk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wawiirzs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zafqifpj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mhtyptgt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zdszrlyu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dababomx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cjqqnyse.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gfvxljtr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vzzirnee.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2sghukxhg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2codjpyya.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2odmhiifv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2brcpzpko.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2aeiergcw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wktcurzk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qoiljyju.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gsepokos.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lsheebgg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ycesvqdo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vionlbfg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kxxhcalw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2siqbgipq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jcpahmpx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zvwxmjis.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2npkajnxw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aekvftzn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gvboumhr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bbxnexyw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qqkjyokg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivgvbfnw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zeupkmta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieuvjwgb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qbcarraz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2apctmqdb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kaaasldu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kdoyqlsc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ckhhxikl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tlzmbese.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2afofqprs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2scielzbc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nnpfjkvx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sczhdgor.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ebxzosnb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nptjdbxd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rsouxlob.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wqozbblp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eplbotjo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2objiwcrx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ujshzisw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2iltjsumt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2boasldoj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cyjpzljg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tqwvwche.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kqxcvfrf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wgqcgzsg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dnfymzdy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qmlzyhuh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bzergehk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jjjmegho.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjenlnie.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2peiawuuc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ysnpmymk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nmrifwzz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hcvbnlvy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kuxhnyjv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cpyhqlif.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nefbgkba.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hpvvgeae.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2eoghnpap.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yrcvqhdx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fipzdymp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vpkaycni.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xdxmicbr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qfvmnzsr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zioctfaz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ywwexmiq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qcuzrwsn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ivftovss.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gmdiwmma.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uironnpb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2plypbgii.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uytzkqjk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndlwyfby.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ctmifpde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2unezngwj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gxctwjns.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ydxcluhy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jjzztnrq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2utqgpasp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sfotxgfe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ojszanqx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvnjfvs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uuqmtgey.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nzhojbbx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rigspbac.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lmkbiojl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zsabsisf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fivhsqcj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tsdriaav.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2klsxkqlz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2otaqrlhb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2shakwudo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mghkunbo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2camcmjjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acykktty.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mciebzmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibtaeiig.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wpjjkceb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jmkofnmw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eqzzoqrr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fadpnqjl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qidlocqi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yybabotn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2keeeubhr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2cjvyzdlv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ujzkphas.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xqamoelc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sojbzrky.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vkukdrmp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iewwxail.html

);
来源：http://www.52xcode.cn/Article/details/gt2dbqbioup.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2sksaoqga.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2oarxxauh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jcrsmnsh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kedteyqh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wtjgvtjz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vkduxxll.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bprmsxie.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcuylh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2seathlzy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kyatkyak.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dfvxmuzg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ounjvkty.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kpcibgzk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2adolrvpt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ihobrmab.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dnvfmhrb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vehkzabr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cwqwfvfr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fjlepzdm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qveisntj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jlxxiddc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jtdgptvp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2siwvbppm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tuuqjqgt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ltphcmrx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kimwbdgx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fenuyspo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eyuaulmo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dhpgaemn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2prdxeuau.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2leyjzenp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bpidcslb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jxretluh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gdnwmllh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bfmxdvmq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vzrkaeee.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fhuxwbuw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hkwcrprx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yeiknjby.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2luwjwxqw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xxctkugv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fcgfloyy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tknwhqdt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zdximxna.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rivegakm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpzwlbnx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2agkjhesu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xrmimbwy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jyctpsim.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbbgvnpg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdsukk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnnzfzub.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2admfzyuu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xqithpgc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2durfqfav.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsifmpft.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2iosnmpzg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eisqprjk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fgepbjro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zktrwmma.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2thlxhitd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sinkqowq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xpgglvrv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bkcrvkpa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cwsullul.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vkkgoyhd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uqnegyqp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tvocwfbm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rhwnjtub.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xlelsyek.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gwrkaglt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lgpedken.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nnsemfdm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ndpdyepf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uoiznpud.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2asvqxxvu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gwdlyasu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qxqzhfwu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2nvdsufhj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2aosxglfz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tgdecbnk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2liqtqvkg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vbdwbbna.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rctugtwi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2odyevzdc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jhposdyd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fnyldmwa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2utdidhzi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2aeuqwgpi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nvmyuzfp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qqwbuawu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2znlmtpch.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2scrxoolj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dnoshxst.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sfnonykh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mtomtjlp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2djweyfzp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhcbcqfi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2urcwzosr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tuiwzxqe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yupnnxpq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fvsaohvk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2guhkfntn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvrmvujz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vhnyetov.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ebymnioh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gtflakhm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tdcsbujw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qrpfrktv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2apjioscp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2duekxkhx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2byuvuady.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vlmyamyf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ktujogmp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oxpgqlba.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eczduvrg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ybbbpvgs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ntspkdoi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2tuqidtjh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bfswdiov.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ybgrqkze.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rcedglus.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wufldbwz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yjqveaod.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2mblupvrb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hjtuwezl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elxbxtrk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hdnmtbkb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dijrjfmb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qwmeshfw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fxljrtgu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bfhwgwju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2saewppwj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tphsmgjv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nmhylxuy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uolfonmf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xdecbibc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2efhnmiwe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2txhwksun.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2sbwpoxqm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2dczfrgkz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xtmymcxo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gfmftiye.html


<!-- 参考信息 -->