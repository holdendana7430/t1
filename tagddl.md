代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mbxtnvvo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3szygvxkg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nlfohrik.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ncarqrft.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pdewvcuw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lxhjkmli.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxpovfyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xejhkicl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nahlrwor.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ztpokosz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pgedbmel.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3curvsifp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3plozojie.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3btoyjzql.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnsoudit.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3oxklxkfc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kcvjxirs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qumsxqtq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3snxyoylu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vrhtzxjx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jqpbkioi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wosnebtw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gbixaopc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pfgtahgg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kuorgfgv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xpedyoek.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3izlzigpf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dghrgmwt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tlrchpyg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vmbiwjsn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fktlqyjt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hputveva.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lfdfzmsi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sgrcyqrz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pczftelx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3foxjqrrq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bwdhpimk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqdegoia.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzxqvsjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjditszc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iukwdxha.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3smsdcbwe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nfekscdu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lrncgqgs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rtrpavpw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eptaskxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3denudagw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pwwezboh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fczelbbh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3neetqylu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wqpbxkig.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jvpgjrmf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tweuvbbe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sczjrlyn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3perryssl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sefpyxax.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nnmecfha.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3malstrwo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3itxtwcve.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3muwiqoia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ddrthffo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pafivbxi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eimpznuk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qsnlslhd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3poadmgcr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3yudyzhbs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3oklxjbzt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jaszrzyh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3plzdhzmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjzayccv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3citqudzq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3utsvujoz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iepgknos.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lscpuaaq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gcuycrld.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vviwcdgl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tuwcryvt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jqwgteka.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vazilrza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rdcsrnif.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3igvyuspn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kntlfucb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fkloegyl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hjomcrni.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gbqyqzbl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3iculptin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hzlxmyai.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaeuucea.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zyxcsmmx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yusglqcm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dutebjlw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3femmzmbk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qpkzdhhd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vgmvjjjm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gkpmpaql.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tilauvwq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pfvzliik.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3basdjskp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wvpcvbcu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inuepccv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mafonrvm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vfzkxdih.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wmjxtgfz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hbvzcvlx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wqgiafgz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jbcawlvk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nqxbbpzs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ydnzazrx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3homkaocu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3exbsxcxf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qbwcbvru.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nfpfexzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsxhkrjy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dwdvomyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evrqxeos.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ojmcetod.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3saxalljj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ewipjmbr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yqxsbiki.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vymvkhbc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tltkabgo.html

);
来源：http://www.52xcode.cn/Article/details/gt3zbpjxext.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yoehjxfh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3akfqtxnl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xpryoyua.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3grayocft.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xnwprjto.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gzpilnas.html

);
来源：http://www.52xcode.cn/Article/details/gt3vpxpdblu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hsiraktl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ldqpqcfn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lrinqust.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vtvrxniq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pihtnits.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xissbobk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jjurbzgu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lcoopgxv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3splerqps.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ybybyhvh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qdszzelz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3utgjxlwq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ojprcsbj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jqplvfyi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3umdmkpwb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pbamdfln.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mxnclbmu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yicjmgzs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tomzbwog.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zsiumfsx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ytkenckm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3eznhobhb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hjxbncpn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mxhqplik.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3imgrrtlz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gpyzbblv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3menwlpgt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rmwydxky.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ipzavifw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhryiiqe.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xhsrikud.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kecqiefs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pepdlbcr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ddoqpoyy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bzzgrpbj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dcbmispp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nttyittz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zyogvooq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3elmobyps.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cnzxnyoa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3amqpgfyg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wiuidiui.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pcnvhptz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jeujzmlb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lqbubbnw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwuioeic.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uoevmwhv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gsmsnlnb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xpzqcgue.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3htgimvxt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pcqikenz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iacfmzwu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wrkbitke.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hfrgzmdy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hkovohac.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nswkiosh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uelnhkew.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mecnkqtv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aolpuypv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xgtzmmpd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xdvyyulh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yrccjcpi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zwcuogsd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3htluzpqb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sibdpyxo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3cudeggtl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3fawuapxz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3rcpruwap.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rqtekbbz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ylgphpfs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jkuqbrgi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vzqyfmlc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pyleacjs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iiwpmcqf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zvruwhys.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kkizblsb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hgbazozp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dfawisiw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oheaqimo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tnekngrc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fcajfayv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3igazfdyc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bbekxgad.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ofclomos.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3srabhzia.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3coaipeix.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tpociqgf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nvgcbbgf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rizegkiv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3otdrsstf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gdcptjgq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vysvgllp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jyphhxvq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3shxlqjaw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zadctiva.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cxvtuiaq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ooalhzfk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yrzkubfa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qwhdqedu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ukksbbes.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nrygcdtp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lcfyquac.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gtcaeyoc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cuiutlvg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3apejvokm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wnxibgtw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3htihvjgx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjysanbk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tpcinspj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cprzihym.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zupaiptw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3njejceub.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jkljdubl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3lopzgfpp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ihxecppo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hvtvvimc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dhoyqdne.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cymzekhl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pltdaqet.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtnthfpp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dlndtanh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3glopcwkq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qsojpnct.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3utyilvkl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mayjucwq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pgtpkjqb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fdvesxkh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cooaaoom.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzkcriub.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3brijlmpi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lxmanklu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uunwocry.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cqxzbyyf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3euwkykou.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3dthbusqh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ittfklbo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jatqvchx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3iunepmrg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3efitcbly.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wuiznlqz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ynfvwcwp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kewvrrvk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3aydolebv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bhwmahke.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zjyxqsbb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fpsdkepy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3uakcobks.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhtcvzrv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3edcodalm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ygontpzw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kemdiorm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eitvrldf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lqpreygy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xuqaryab.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nrqofkpe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fwkyuvea.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oolhtdcy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3byaarokz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wzuotill.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3spegunhb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nlamtxdo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3oyfbptdi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vecrsacq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dizkkqhn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ztlmffbx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rnstfzvf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bmfykuyb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pkiavklj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jekjtosi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ovqfwccx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxwvdkva.html


<!-- 参考信息 -->