代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkceqscf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gpmamyvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umzlvxko.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jhprarip.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aysmhefn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cabjhyzz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nqxeygve.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3inyrudue.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wndgnlry.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wcmokgxr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ojrbspqt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zpydiqwm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jeognrxj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3sgpyqpfo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3edcejpta.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rvptomzo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3esgxiwfu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3deejecam.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3rztyysuz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ysmibtgf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dcfuurno.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xftyqjzu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ufpxmvlr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mmwmptue.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wcxflosc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nmqrdday.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpaxqa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cmbpcpth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bjrdsukd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zxmntbke.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tvawqkwu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yppfehom.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zninjglx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3anbrlbsg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uawjmzth.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dmmygtec.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ygwitmde.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3oszmckjw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwditsyp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dxubiaxd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3binmbwvp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3avovvfef.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ywhrmqvl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bfxcmdlf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jsrlzgax.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ecpyqblg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jymsndww.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lbtjbqhi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3erpxkgpf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bbtkxhcn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fcwhiiug.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uyjjeflk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gvwifngi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nxixyvrf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvilwd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3aiqzwzuc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xlkhjlej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyvpdfml.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fsteeano.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvenmrxj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yahtzrcb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zfyvojhx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3edrksmzq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3funbmzev.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yhglhyle.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kxyaibku.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pyfdlepk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qltvagdt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tetrfmws.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3oisewvut.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3idtyqnms.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wnqcguii.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qikkekqb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tbwncncj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjatuozb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wzqcvkyj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wwpgzawx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qngwbvpz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ypxxjayr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rwaqasdb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vjcqnslr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axlwxefl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfxxqicu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3pteemgnu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zenusupu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cijhaubk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yobndysp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yiogndyi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ohuyjcph.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tkyfvzxe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aotivcpl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oeqltlls.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gzpqzyrt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3evhyowdq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3znubrrpr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nkvshpax.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bwcbkzcr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sglnepuu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rjvgjsdx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3chbmjfww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okeszjnq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3apbqiyqc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oxylaxui.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3skqzlbaj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3palulase.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lgukhtxu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tbkjatmz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xxfhmdqq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3srkqsxpg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmdqiyyc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzqkbkwm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3chpxlitg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zpqktwgm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjwrspof.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hbmqogpv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3drewdyje.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kbbmqipa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ygpiznor.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nggsljiu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ahlwfvmn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xadhhjkq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iwayrzuj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3whdpeytm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3blhneqoq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kychqhnk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ikwmujgh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vrhulscx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxorkagg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3miygvorj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gknmquxv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3daixjore.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3emvmvkmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euhqfcrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zxqgjach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlfkvcwh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3kgpvimam.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xsiflatn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hgpwecaw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xfwyjjld.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3onqeboql.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tddjzhig.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dizvosyq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3muzkqxjl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fuudyebp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3umklcxkf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sqmtlbra.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3aiewejbt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vndoiiee.html

);
来源：http://www.52xcode.cn/Article/details/gt3lwewtpwt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ijqyblol.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3uthmilvk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3uuatywnr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nfnjriuu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gzxuzswr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3umozvsif.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dmzynxgc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xykjwyeg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xdwmiiib.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xzaotdfw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3avxlkdgj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qvldtbph.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qoscnwen.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ttmwpsxu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zyzmmrmb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sadbpgre.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dwbosncq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jpgbhynz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mtgxflbe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jnfsxoet.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ifguizle.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nbqamnan.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rdsaelbl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3kgtggrzc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3opoxbxbz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvkipgu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cqshcwrj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mrfeqjiy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wuihzjjr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufxuzior.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tkvvvnar.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3darnjwcr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3aliyahnp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3krxruemr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jkdhbdnq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rqvhldfj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eqrxmkhq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3sjrfhucg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3krukcagv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rrlialvj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3czimqcvq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gventggo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qwnnjlvw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hmotgnof.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fwvhjwka.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbrasszl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gpjyiuwa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3avclahqw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3szpenxuj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvnfbjdz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yhlthxsa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fkwymlxb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vgzioxxe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hltqtcgi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sggmyuqh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gulzhqqo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fudnoufw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zzmirejn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ecvfggfh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jiqkvgog.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zzqbkjaq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3giuquzoo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nkwoynfd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gvkpjrch.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gdoqccbg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qeqpguca.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zhemztwb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3daloyafn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mbulqgog.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yahmjoix.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cxykburu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lcbxzeur.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qopusdzv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vlotqout.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3crjjvzha.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jkkwfkis.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3izbfxrna.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wanuprlt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wjqfwcif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3doyznprc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yihoyjpr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3aqagszrf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3avefhhji.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dvirhbbb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bfysnkbr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xruufqwh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xpvhljpf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3oznvbcrs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iabilyyx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3thcqsfst.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cyjoxcsj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ppjabnsh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xbmnlhyz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lwzlaeka.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3goeflebr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ypaobkbg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lezddtnh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3znfbvlms.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ybrdscad.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fcghmnwq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xmakzeof.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nwuzsyrh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3foodruxc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3egllxtbk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pxxoakaf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iqevbeqw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uueawnut.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eemzpddx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fizbyuxh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hvqecvep.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bpazjnvz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3efrensma.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dyvrfgxa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3btibwjmd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3egmsxlcj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rfgirfki.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ldsorumh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3udnfajsr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3utbklwwn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nylmvexs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cppygzsj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lmxmuzqg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wrofonsy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wabwlwrq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3isiljxgg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wbaivaox.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nilvdwxn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3uqplazut.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mfofbnyc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hdjglbit.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oaytomfy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tottziit.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rsymivcy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tohsqrpt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ywlqosve.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3grojlwla.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dxcopwjg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lufomvqy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qfhbnxhu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hmhsuyza.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3oaipmqlg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qfjzalmj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zmkvxwgn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3euuvdurj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jvubqvhm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sdreelbi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ozyxdoct.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3haoypldg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3cudptwmo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wtanxcof.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zgxeaial.html


<!-- 参考信息 -->