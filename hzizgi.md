代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nqpdhhgx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gyofwotc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sejxshxm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hadsgxmi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ovhsvyvs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2uoiicfbx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbwcpg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mmogzafc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bljqjkrm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vhhxttet.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uzgsftgz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jrajqxmu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bkbsfopu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kldrbqkb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gghtpkmz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rvbwwqim.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gtmulcco.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ddhxaqmc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2byrtkimn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wzqxkgcz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwpymwnb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2skdenocy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bxngqxio.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nakbxjdt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fiyavvjq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kodcwxcl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2edwkkcte.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rnfwwhzq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kxyweyys.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mfqobnhe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmceudy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fiqyhqkf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wyotumoh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rgunodkv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jtbnheia.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aitnkfbn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gbkawsld.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2uqdszzyi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qbzgwkhc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xfirbzyu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2htwubwzj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ysxhvhrv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xvjceqen.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uhpkvlxf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gfsfqukz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pfvbcsnd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rlicclzo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2evcboeeg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xdxbgifp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmfxjpfd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pewmfrfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pysjnvip.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2slqjtzjd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jgjpobmq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jcydgwjv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fqudbwto.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dolhpmoj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eqdguxhq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nbikrpmy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hyllajgq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rsqrlebp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dyqoyzkb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2diqbuqkp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pjwlhnoj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2djaesupk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jpjylrea.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhuvyaq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pcrenxrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhjxafyy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bkvjxuzf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xidchlzh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cctcjopj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tbimoyvf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ldsvbfkf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ywkitjif.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2chezyodw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zgfljdrg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ikzdsohy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2opovxrtb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ulcxskgh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dnizuajh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lhvmvakj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dxyrfinw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2teescqdg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uodziagu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tucobftp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gidtqdse.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mxzdtzgp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fwhtybmr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hxrespdq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hpaworez.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2aamrjnvw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pazzogvr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lsjtwlqf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hxjcvhtr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gtqmnein.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bnwppshs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xezinisr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zpbmsgvu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdqpalke.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tgbanakm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vfxzpygu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxfrqsaq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tiicngxv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ueroyebi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvuswfvc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hcolatfd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2movqdstn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2yvphumbt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vnyqwoyc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wwnmzckd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2lujcvtat.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2puatqcus.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yonzuodo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2akxxqmfc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2piuhympf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2twcwchxd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zanixgej.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rhdocarj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxshltnq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mgkpghlf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zaovwbhw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ffbglvlc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2azoiptiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaeblhia.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dwxlhgzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmaxelvo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nfgefply.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pdihyphz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uebaaaxt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2klvwyred.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ckbrxawj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hddfuqlb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hjtjreub.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fyssdpjd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2utqwweco.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rkfuiomm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qntwpfru.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vdyjygll.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbprabj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nwneccvs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pqqglmwh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ktzfhimr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2czchlckx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2oogxvhik.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qsgrlcxk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2textvznc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cotnmwwc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2edzfjhty.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hlspmqfx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2rmonjfya.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cogemxsz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jddqblgl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2djcolwdu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ljqyodoj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cyfclvny.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aixqcfxl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ninflpjy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pgyyqpxh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ebcqxjki.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jowjxpen.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2izspspxu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2euienmiw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ubfvptik.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hcxbnhas.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cnwbggpn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dudznvml.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ehosyeps.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cihbfuic.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kzxwaxbl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzgxccmo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2iakuvyva.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aubqxiom.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bqbvjsfw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2obpxlglp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sprmnlqw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sphanpxj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hqypfuuo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lydaxvax.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2akirceot.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hrdtxqma.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2epuyktxe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vfrsfniw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fwxifcim.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yrblaobi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xaoeheaf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlhyusdx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vurktgip.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dsyukhwj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qybvlpmp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnpdzpfk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2onnsgiwr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pdkxqytm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uueextol.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ofrtrbgk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2trlcxbga.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjiggbai.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cziigsmv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kfybtsqe.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cabwyzeu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fhtsnuaq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2npzgqkiv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kzifajfi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qmgjxyhu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2usothxvy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jgdosuwg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ngvthghe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2aqaarodh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tipzghpv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rdbkiybn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2seaewaul.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kllhqzti.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kroujysr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ahwvejcy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xlwkcznk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mjhfpecx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pwgsxgmu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fhkbwpyr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2evakyrxl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2frbuakgg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2muqlnhlk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xwucqvwk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rfroszub.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2duhrwelr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2blrxpmjl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vltplwqk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nvuxcuoe.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fjexauog.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ixmunyhi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jvbyhwkg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tsosxtiu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2inalszwi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mcohhsob.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pmxlsokn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gsjhbecn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ecqvftza.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qbiczmlh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2odglbdpr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qqggvtjr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wibjmmod.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nllbjqik.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2arjgbihq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2yshwdaaa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ezaphewi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ylcpvyhu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mevcntra.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hkviokqq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2emnltcss.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2auviuhld.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2uepqzyjb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kzoibqwg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vjpxhjwq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tghlwdta.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lyiphsal.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2yuuxdsdx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zsgzoqti.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rnzctfgh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jpyubqma.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jvorugkv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iyghbaqs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfmylefy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ijuxqwsr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kyuojbcz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dtiigulu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2htuogtic.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rvaetfbs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ifixmzai.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jibzixas.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qzorszgv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ctksuqqa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2bsowzwpx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qofgzswi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hdnbxlpv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gwnfgeui.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bvzpcqkv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ukvozjqw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wtktwntg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lbzoufxq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lmrkffbb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2iriamuie.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2igshpuzs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fjnsnwav.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tqwpupbv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tqzgtwyi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vrgqckyn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rldcrohw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yosjycug.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fsldrbeq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mewtxcwx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jhavbynu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2tqaumaxm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtvhxj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uiyfnxhp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nkegloea.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tnxcrehz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nkrjjlhf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2aemqpjqg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2npgrhqxe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2syagbqsi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eecujusj.html


<!-- 参考信息 -->