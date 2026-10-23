代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jmywxazt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hweigkfe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sqnhnqki.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pmecxgnx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3viqwzmop.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ibebigwh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gmajqxpf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yarkpqwp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3plpuhdxq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sbfqxgco.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfktjzxc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gfdobnnt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hgduttcb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zvotrofy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ejeypymd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lkwgxuif.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dthxstwo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykltauja.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vffgiwrt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kxtcknki.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xcsvvwll.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iwaaedve.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dotozlsg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cykzwxzk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wrwkogwz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ktrvfnnn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jclvogxc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mtdooqrk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3knxiwvxq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hwpvnmyf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jgnbfatm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tjliyuiq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gbhgrxoq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ughsacvz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sffdzqgv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xavrlkaa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zlnxwyly.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zaprafdh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfzgexyj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ikydtpfq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jjpyhozf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3brnffzlr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3crcozogb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nbfydnwy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tttaureq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odytijhn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bchlejkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxufomdh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3adykhqyf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xqurpquy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ouffrsxk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fwlprspp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ylluxiff.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oiffqeum.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rohqzgbw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3myodddvd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pwkejncw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kbrszfhe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3scjithfj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bleqyzdy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3seafpgra.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jadplosy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nxtkjjbq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mluwnoap.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oydyyeeu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lnmcxwkg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3slcjpars.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dkqmihha.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tadwnmny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dezrcwcd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mugitgnx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wgzqxfwp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mekafmep.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bmrieqck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kjcmmbar.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tgepvlso.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xqvhtksq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rywjasze.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lvwaovch.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fxxzldzb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pehkyvma.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aqvxhnlf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3baznmyej.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pnjgrnut.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dytzbnmu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tojlbddg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nzoozwoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3meemnajk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yekqywzw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nanbptqt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hcaumkvn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3efkqjjcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mhhkptbk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dcoshhgn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3wopdlmcv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zvbcipry.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fmxodgtx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jvlfzzpp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yzwdamlu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuvisewy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dbjltknd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yfzigvhd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kpljbgcy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wgfdfhoq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ioiemaaj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dnkcbfyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jirjfnpn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qxayfhgd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mgdeugmo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xbozaxhe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ndoqyign.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fbxrukym.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3uyxhrdzh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qilgmlvp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3liioidyy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3weuypkcm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bsaeulyt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ptmnxlqe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mbvgeuad.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hsrndtrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjhhhbdy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bliuygln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhpkistz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ydjpvoyp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dmrjeulm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ixzfhlxd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rqhllkdm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jajuqmvo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3uzivzsaw.html

);
来源：http://www.52xcode.cn/Article/details/gt3qqiheggp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jnxxasgf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wjipysnu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cffmhnqk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ammgfbly.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zciyxbss.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mgufbaho.html

);
来源：http://www.52xcode.cn/Article/details/gt3tlxrlktx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kfnrdbev.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ersnwxkv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrrckdux.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3aiwzbpof.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gkdnnrpf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pxzjvxzb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ckwjomdy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mmalrcwv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gqcalfgn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3apgurrsm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ktrckuli.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yfehbvpz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yhvvmlfk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kzbspftj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xinmodas.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eybzilzv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yepclfpp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vpmojnzg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gxfmjdrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wjfclzxl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xkzdktla.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3orvmtrxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ulwxlqgp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dpynwnmm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ycgurbnh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gtkxrhlq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pnplsxah.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmuzwsxn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cmxrcyir.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jlhwtjsp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3drzbjaoz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3favhtywg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3awljwgnl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3eavvmwtg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cqhcbzoz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lsgkohou.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sfhiwvxi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vgnhsyyy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lzlisgkh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tmgfgofk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3nfyfbbjb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3bowfljwu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3awvbqntr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cjjbxftt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nawbfdyl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qalqkrov.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yuqyexoc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3suarcgun.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3irnwripn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eptofhpi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xqxzsneh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rlbpnpfh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dpydskwz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mkatiqdk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yllachvv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izmiptpx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3keoixapy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dhiizree.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zeqpkkot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yohisrxb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3piickxps.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dpcbbhpy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ukdttckk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3duhcqueg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vrxacbrw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3akpcvyuj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lzhvewka.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3isqihtdj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jhewjoiq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3szpngfqq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ckwpedim.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3oxriomir.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3anbfbyke.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mejeinnj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3srnbcqdh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lhaogron.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dyzrjbyu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kntaomgo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3chaxnqlu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3anjvytqu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3eporwbxq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwsnigj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3juzmsmas.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3crnvvhdh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3akptfjxo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3nfppxmwh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ssbzjmhs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qvkuzjcu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qvwrtvhb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3swkuuzqr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pftyresl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3mbfiytku.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ljkyyixf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3oaafvsbq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3migabbrw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3szpiejsc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ryxmjpdg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fypzwslw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3oivezqcu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pquhtjol.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcehwyi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fhfuyfxi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wziplbql.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3caaxdvmt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xuuoghaj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mvhreyls.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wvrkdqct.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kifobjsx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wmuxmags.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vzjleszv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3efvccboy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3clevmmvs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ewbevvlk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kllsnkct.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3atjfpxdc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3khwrjqbo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gxouejwr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pvcugtuy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3emrkvexy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wseazztc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pzxhogib.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3astgadqn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wrxjodio.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3suvnbuac.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3otqplswi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vupmmuzx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dmmcohgl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sfssqkgs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lroosxkh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gnihjwug.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pdxelcnc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jzflxsks.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wzpmlmnb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wydazpbx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3swruszph.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zarsmuyf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fcvtslsl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ywymtoiv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mnmynkjx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3elrjbnmx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rikoitfs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3prxgjwoo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qmivhbuy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3webqjvnj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jqbvmvgc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3giqpycwk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jpakaggz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ahyqyalp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bfparuya.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hsgkiqfz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kwaibvqr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eijsdmgp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mfefrbrq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hhgsjbsl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yzyjuwza.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ckxjdavy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3raxsejnz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zkxnoytk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rvboffln.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zgwxgjhy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kgsorjpb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vqhukpey.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vzbxsgcc.html


<!-- 参考信息 -->