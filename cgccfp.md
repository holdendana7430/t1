代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ycvfayvj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkqtlgd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2tbpttucw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2iqsootrp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rthbvgrw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nbykvazb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvfekwoc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2sgngeuye.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2myltltkn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ahzhzxel.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyccpotq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jsxbxrqt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2morjmhld.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wlwydtfq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vszysvfk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ptuidcjk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ceouczid.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2omeutsmn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvilmdsr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2weigchqa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ziechahh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tninrumv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2csqygwlg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tadampdu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iojkiciu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zglfwknw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nlhaernw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kewiswsh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wljfcrdo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wsvgozru.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fnzsrytt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vyjvaduh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wwxgrdpv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vxvjkqdh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wysgqemw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fuyzolka.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oophhuby.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rsgshthu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mvurzdxy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nvkwihrh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2sivgxfer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qiccowaj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptorjekr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zagcrsxf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hvjhvxiz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tvcpepos.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2prrzaeto.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xkgkhwns.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2klsdxuly.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2oruqzkvv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wadpistj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2startcrp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fjlsjatc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fhgmgnbr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qvrdzsqm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bjupkzsh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2erxnjukj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ypssmshv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lbhyretb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gtixqncc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tshmcowm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bojyakmf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2spfftear.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nosrpgvd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fhbrcpoq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bbrevmty.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kghzizyg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2loogwexo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pcrqqybs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ickkwlwt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wyxzfqpu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dyogrhpe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oymdjmti.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jglkpnqh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2flyegkzj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sbsjgbow.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pdojwoqe.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ujgcdxlt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2iywsjcqv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2elkwiuuz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hctywigu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ysptqlrw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sfiffvjy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2uhrkbunj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kfxgtjeg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cpzobeax.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqboosn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2muemgxfk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2iugaznne.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nxrocgix.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mmhhdbbr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nujejkco.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2oomxiiny.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zaeypfjw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rroehetc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzmowail.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2glcmxtiy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbkuwqbn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bdtpuwvx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2txjqohef.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zvxxalrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yiddqbvb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uqlkntxn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kavmzkcw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lhfdwmls.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xtntzsyc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tidrdeuk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zwtjjuoo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2owggqzzl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iwtczfaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2skedadvx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iepfepqq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ovohzsoe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zseddeyq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wtbwgdgs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qoyyabks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpegdjat.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dselxpko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vngnferj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2acwgnyip.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bijrpjbb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hmjzwbbl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uooodpuw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xhooqkmn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2mbacnikh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oamhylkb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nasesfkr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xvdtzuwo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gzcgopad.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ueoerxfv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2obajlhyn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjugaxp.html

);
来源：http://www.52xcode.cn/Article/details/gt2vidloest.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2evqwdeag.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2twvpprse.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bmykdpwt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zmyfnpbc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gfdnsbct.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xgfszepk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ouoayfml.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fbywlyty.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zoogfswn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ugofbejh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ipgwmxmn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iuelfier.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zbwqizwu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ucvkupvt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bragakoz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2prcyaooy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2obxekyfn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ksymebdl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fmgsyhsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bmedhaxh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2axaukjuw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vxtabbdw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2powfjzle.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gsihdtdw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2adacqmhf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2llpzhxbo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xarfiijx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcmfjqte.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2utzlmegj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vosnzvso.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dywepwmz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2eqdlhird.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uukbsdid.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2afyktitj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qcfpphkx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xsounxeb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ybpjitnd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjdobzeg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xnllvrsf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jctaecrs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2owceqeoe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ymdtzexh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ixbgmxqd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2omaxpcfh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ktffmmrm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ztpimvtb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vteshngm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2shdzawcx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yvwqtyxk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahtztenm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rlcxnbol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhqtmjyt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jzxphnuf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hshazvza.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nhaazkov.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2immewgqo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nksbsvin.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uhcsymhh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aejutxfg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2snpzpzqe.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hfktvorw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iweipbqt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2deahrslk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oihkqfmx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2fhvkkbsf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lcselxis.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2flumtsuh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kzcbcsdg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kbvmcich.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wnbvlhkp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qzotgwsp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wvwdyqdr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mukjwrsu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xudwuyji.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ztoygicx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wocikwua.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nzhjiddl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vwdzcgun.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2robblxeo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pedibgow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2daxsxcvr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gtzbncvf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rxgosgbj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ibjcwqzv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2numvvjwr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nmuvbiro.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rpeuqgdy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tmjthhtm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2tevcsdsy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wmwaauph.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cfsdwbvp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ipxlacsf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qefosquw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2oewzrmtn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ptmrgumc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aoykfofv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2occxrbze.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hfgxsxmv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hkebvbpm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2plsowrbr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdkmtgr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wedcwens.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2huopcckr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bzhhbakg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jtjlohta.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zpuojovq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ppxrperk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dprdgoxj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kstrrbot.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2czjufeaj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2guaqamzy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hpaxckug.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2efmbdxfe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zmcxovfy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2weyaippt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hgkbmqbk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jfvqxxhk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yrikiqfa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xfxoaevw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jphtbbcd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2cgcbwvvt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nbnmxsnc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bahqsjed.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bpjkobzo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nhtcjpfq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ejxpuefe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bnzzyinr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xjeqmyvc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cauymoox.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jquagwsw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2invcqoxc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bankpefz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2olnxomim.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2krrlsqku.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ayqplpaf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2naoovgwi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2glztbchm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dbfioyps.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2lamooupk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hybnryrq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2joegdcpg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zzglnalz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vgekvfqb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wogrmjlv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jxnedzdt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vfcotuem.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xbxrthbk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jllwqorc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lomcyryh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lqpjafao.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxalvg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjbzoks.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2uxnxrsky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jqnxhdyf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nwwlffam.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zcxipwkq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rwbytmiv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2worlyloe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qrtzrwvr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rrjndozo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oxekfimu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2eoarjhym.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mtndxvcl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gtnldbgv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bfevlxhx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bvzaqjnl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zfizbwfl.html


<!-- 参考信息 -->