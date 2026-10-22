代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yxoueyfk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bilpbsxt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2itooxzuu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2basqcjvg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ajodhwsy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2srwoukby.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2piuxpiur.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2naewhbej.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kfumeiae.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zyebvzyh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhniiedj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2eusdchay.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zlqiayyx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zwffzder.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrdmnfmz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rikoukow.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2smzvuxoa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxwxpihd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kyctkmds.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hswltujn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2arlifadh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jksezkfm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2phbozcly.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qgdkxyak.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nlcmcetw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wokrpxsy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zpiyugau.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2khnyuctl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrbkayr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jwcijjyl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vzpvpdbo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yxzcslot.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jnhuemta.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2udvggpov.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdzcqmh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2klbukgae.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wbldtily.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2muzaiuvy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rsvydxzy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zjcvdddl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2raiipnbn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2msjornxx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2peohqmwm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nsirxqzf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lcyawmwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scmyuots.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jabyuzyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fukrsjau.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2aykiwqcb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kvpcuujv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xykpqkmp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wcnoszvm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bwupnfmo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lyxncthk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2eyvmrvcr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mxqzrxvs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2urcmcmkz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wkwcdbpd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jstebwxh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lnadcpeb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qwaejggk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pugtrtnv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2djqsrlit.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kxspoubp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wlctrncu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ygdugslo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqmpryjp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cgbfquxr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hzlpmsqh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zmtchbue.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bsiumaif.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fukknkwy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2sejpkshp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgedchq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2suvjirny.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2iacoqfua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wobrroya.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vgmvjouy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wjijyyba.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uwatpryu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2frttzyhd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qjzgsgun.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dgicsoil.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rvbmbaom.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mjwujbkj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2svalswho.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kccxcpsb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zudqnega.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwralldk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2yhlbheep.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2peuakmqd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cbgfczjm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2iujbfrmp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vskhgiwb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2otkqxgjk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qemekfrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wskiqffi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hqshehax.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ruvgzbwj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zupszwwj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nrwgghfp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkorwozr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2eglujegs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rfmswhny.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fxtnlpzm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pnmqyrjy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jmvazvru.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxrprtl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2onlbsnyj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2caxpwzzz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kinocaxo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vjnibzfq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hdxtkggz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tdbjgfgz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rtrhptxw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bonygvgw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2aisfetno.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vxspvzit.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2guzrwbyz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vbjvpefy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntqdpkle.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2spystljv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuvhoijg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2monahgbx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jljnxvxz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ulgpemfl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bbdjxhzp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2nvxsswjx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vgopjibh.html

);
来源：http://www.52xcode.cn/Article/details/gt2xrxsqswa.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2xlhxpnya.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2iysdtlxp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nsfkodbf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xpjizdhr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ptbomflw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mdmceqyk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kzrruhra.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kbvcccjj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qcgrqinb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wgcvhezd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gtswliqs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ywtiowee.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xikivaxu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ppqflogb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fhwrnxfc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2smwwomye.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cqfaaikv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2brcqtscf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nvqmhimc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ydlyaxjk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2btcbekzg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qodtawgc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2srqjtevg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mytwskfs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tqtbfntr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nqxctenp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ftvfmufe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wywubtlq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ibnhnvot.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mjxsbxon.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kvvxsips.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xkvylbxv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sfufxvsf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dgdwtovt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zcuswenm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jskdtwrx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2basnfxqi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jdrgxhlw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pzmwwggm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2poaspato.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rabyuvnm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zehoakps.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bigvrwcn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mgkrotvh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2iydxqsri.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mtdfzuja.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tpcholqq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2enpzhszw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jxptafkc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2eaxaryha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mkrbdxvm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2daefpwne.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ifzjbvrz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ndmaawam.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sjdyjakf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nqzjqstd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcsfwhxm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jiwimmjk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2alskupsp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2evegvsmr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xywqypoh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dgnjhnoh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwixhpwp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cfuwffxp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2thvizfvy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nhjdlufd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dbmlccqq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2quwwogmh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zvjrjskb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jsqylesk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ywjasgof.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fwmnqksd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2famlbqjy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pjmouzmi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bfllcihk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rrkinfri.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ephcfdpc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qaoxbzlg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2myqwugfy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpebqxy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gkcblnej.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2psvoumwx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lihpxngz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iljarkvn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2eweaxwrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2odtevxxc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2peguqrgg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2yojghmfs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wrvtwjnx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2azwmfnlf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qalacgfe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2uvohibea.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lguffehg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hkhefiov.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2natddxad.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2krannfds.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2izfayvci.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pgykhlkr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wxqndaah.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ecradmgu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qrorkbgq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kgyjyamw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2iuhwsqvp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2frvmwpld.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vgbmqujc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vziyelpn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zaglhekn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ythpvejc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vedjczsx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2escuokzi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uwwxkoqi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ghnehcbo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pflkborp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iriwhsxk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2azdrnmuj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zmjyqvpn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wjiungly.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kbbmhhsx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2awemksue.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2szfqsfpd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sceztiru.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rggumrsa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xnbzivsl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ktqjiiin.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cibobafu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ztrnzmlq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oonqnlan.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eshgdffn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jhsixmxg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2gvsvorow.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yrrsemyq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rssvzqda.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ckpsviza.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2febaadex.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2iupdomde.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbbxray.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fwtdqohm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lpnvvsye.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xmzyjtwr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mrpxlvib.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lszhxseu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rsusgyxo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2clyuakok.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fjgrnoqz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2djgyocdf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wrjtbxno.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2anlnyvrd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qfzjzale.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2eifajmfd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eaxbdjpq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gtvonuqx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tvtzdhkz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2bglfzqfc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2rcelqawu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltuzvepw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bsbxdrez.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hnupgfon.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ckhlrhnl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zccleqik.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2oovimwgh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tfzrenqf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wfgnndnz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2otusrihk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2drmrfxho.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rtldreui.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2upbxyywb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2uvprdxco.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ldtpvopo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nwfvlifm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mpdohcuc.html


<!-- 参考信息 -->