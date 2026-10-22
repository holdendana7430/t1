代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dnpbxtyz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2klnuyilj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bjlhszil.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2jxrtmgpd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2godkwsto.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2iniyoycr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ngohtwfq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zlxzxgvh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vllnjozp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zgwfzgwh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ibuwqlax.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hahdjjht.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xndqdvub.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnfirygg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddwxyckx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yxskagcw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ixosxohi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2wtcclujz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vmsaypse.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gnuefacz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2emgprpuw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tvpswrto.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtdmbdf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dlzhnbda.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gcnbtnqy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iuunstoo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kkmwdpjv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vmizbfyz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2awojrjvu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lkzvqqod.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qdyjzvri.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2febnzzvx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xsbsakui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csqguwjn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2urxonzwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asyeoiqe.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uziyxohj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ripzvqlw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jozwumnz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2srrmgdko.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2coinznrt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wcjqxqxc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qynmqeih.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2szcbxink.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2obpylhvi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2muzslyvk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wwsfschs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lqgnbepc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zgdfvhys.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hhtprssj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zmvugxpr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2flnudzol.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2janqhkgq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ytlyejfp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vufkduzx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2viztvhfe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xhupahqb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qbnschqr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fovzwuhu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tmjtuxxb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ttwprhpy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2knlotgkf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2balenjlj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ladkjjvj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2iimpvocb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pjkaspxq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zipwusdb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hjhgvfth.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bdqnsing.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2audtmeto.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2waymwtyt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qjhkdlwl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mxzxyiyj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bbvkmhxx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tecehhbz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cwuqmirs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nsajiaen.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yxcyclvp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikbllhia.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xkwdtngy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pyvqmxlj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kemhptbt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jtvxyxqt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zoxlltgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lxzedmci.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmwbpkak.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2auyxqgdh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2chvyhroi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2numexlgq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzaednyl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vwbhuzhq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2upfdqngp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xkrjxwaz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bmzuawyv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bqsxuizk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2difozbga.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bxexiyve.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fnfzccwn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ahutiquv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vpuosemx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2szmpqhmi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2damgwehs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ukrgiyln.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zjjudirg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dgqdewow.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cwqyhwuw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wkntwloh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gaknuatd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slhejeqn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mjgwbncj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lznxfslz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mazgncqn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2cmfjvyps.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jfmxequr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bnedjsqt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2unxzaeib.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kujfrdae.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gqgyfzrt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rtonekop.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zopzknsa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cbgccrnr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zrdzmrhj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vmimhpgv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhthhbh.html

);
来源：http://www.52xcode.cn/Article/details/gt2tmknrhcr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dngmjtkv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bxqjekpd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2etzygtkl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hildtnpz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tmzdybrb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xinynsbp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ckhkhvce.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2akydzwfc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nuxtaugq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lexblvjb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tmstvvax.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yfhgftox.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2epjsodyr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fyirknzc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qcljxwbc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tpujnbgk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wfxgjnpv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uifgpxvm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2eskvdotq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ouekxlss.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ngmltord.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ywfsvjac.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cggpolmb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ojdlrwqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kpyhxvfx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2piuesqbj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2oiubmizn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phubccif.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hdfklmqw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brhfynmb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lbgizyqo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zavgoxdx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lxcmsrqn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2auldktrj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ixtmzwpt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xssaaxrs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2biqngcfo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uafbsnqi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2spvkhzds.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gatgknau.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zzgwtjps.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wzpgdurx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jwwgcacn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfpwrkm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pnefzcox.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhikpuek.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ctkmqhiw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rgodatrj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xqgkjyrp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2joejefwd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2lmqgqxba.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hxuukkij.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sgjvekvq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bghwxocc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yzwwxsjf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbdbqyoj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mgyugmoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2procqzob.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ebzfdlwh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wjypdfqi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yuohrlgp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2adlwkqfy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ukumxlgm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qkmrqvho.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gpfcggmo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2benoareo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ttmfgejk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xeaseqen.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezvhawhq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tcfdfnvn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gpjmuyse.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xydbatxq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iloqkjpo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lgtlmwzq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yuepiyqn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yecwddiy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vvbwqfcm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2trvthlgg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vmvkonal.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2phjbhbnq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hhpnvqoq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yiyftzue.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mlfwemma.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ydfcggue.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yczvicyk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jvlnvcsn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2guaxzwuw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zntjqhlq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2etcwgagx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zqxlmzsi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rsdgsmrf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rozlwagt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2etytisbo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fsjzptag.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hazrszwq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fujrdhyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mqpitfyp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lbaibhxv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mcrirgsz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hfkpctzm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bhydpntw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jnantdro.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ywepmygq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pvbiyuin.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xmwzcouv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pzrdtwgt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fnmplqtx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2chksdwwt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vcjcmedc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2blvjghdw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2abhnoivb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qwufcgfa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wkjxawxf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kaojcxul.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2knrrvlhx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dpadgbpm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2onwisjvd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rhgapdkw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xllxxprz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbudmyix.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2aiwrwbdz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzseceb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2iboqobdg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2npygypan.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2shorhaip.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2aqjmtgnc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tmflqlqd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vnfcbxqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vtumrxvg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2uzzviocw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ipircqve.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2snszlnrn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wyntbnhj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2orxjzyyk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mmhnzhws.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qupramxn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bwhcvxdo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2npdmybkk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zqeodxmb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jgqyqsjy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pnywdvat.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2okoqozki.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rnadjgrr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2poyungbs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lhkbfjbn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2glzxylqc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2reuayggl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2evegurhl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fdiftfji.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nriupcnp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pvxfmvwt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbrscpzy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2iltgfpit.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fwrkmpps.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yvstpdvu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hhntsose.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2utvtigiq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uzzirflj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rjcuevcu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ynsegfjp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uhmhnche.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2izuvaati.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jxyvdsjh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pudbmgsx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rmlbbxjk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2woaofvfu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jfmwmnii.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bwltzfoh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uncctnxn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bwaczxzf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aidloaei.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmhfujku.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oosjjchx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2neddbxsm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dkdprcde.html


<!-- 参考信息 -->