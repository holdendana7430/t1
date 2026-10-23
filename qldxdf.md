代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sxexlywd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yduztsqh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dldjkpjt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lsxrcmxl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bbmwnjsb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xacyqkqe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rybhmfik.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ufcohpvr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3flnkpvlu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aplpnnzw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ottzdpto.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3oytxtejf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sdwautqi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lqwuqvdg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhzsgzkj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ibtvdaph.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xwdcqjwh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3reysrasm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhxkwue.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hzhtivzv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lcezfagt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3owmimcit.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mapodjfl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgyinue.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3uffqkbtn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dzsroqzy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vxidruts.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ywelzwlu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gibzfmnb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ascbocsp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lqcoktgb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hzslcmma.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3puwqmjqq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xmmtbnal.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wsibvnfr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gxwywcuv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fqsrnfbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gswtdfsh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3axydogkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kubwctso.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rrgcwxgr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3grrdbltf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jonsvztn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3plcbqzet.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3easrakpz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zlsdaoue.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3swnizjrd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fogiyiqw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kceoweph.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3necyahqk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xvepdmgp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3psqwomvi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xadonxqq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3datrbgnf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwicfsa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uokvztzp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ymxshvth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zldikqup.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cczweqhr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3pmcbxbkh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zoijrtyu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3molosspu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pllimdxw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3odjezlhm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3eymlosmt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvjfran.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mwqoxfff.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ztcjplch.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3grjqcviw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dzckvted.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xesdmzcp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hvoywokk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nulismqf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwiypfw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nqgcksqx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pitokmlm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3boibpdke.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pqunxmqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dcbmfxfs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zcwuufnc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jvspmgrg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bmmthwew.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rydskdzh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wycxahco.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vwpttfsw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3etcofzdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dfwlfmgz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3krdpwthc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vuvydlmy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3awubyadw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guqnougj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wvfzztyp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vjtmnxtz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3onwvlged.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zbngfene.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sdjnotbv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nyktefju.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ujflvyqw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eqjydcmd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vrysulbk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jorfpeyx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nucnpjju.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3schcxqnl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gsnsjxmu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ccifymwj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ejpmcpby.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rjifkgdi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rslofiyp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jleawzjo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3txjbviji.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3uourfjhq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3csmwsgsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbuwlfla.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3haadkkxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amzcezbl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ixhuukni.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fnvsavyf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3khjtaxfp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wzxufnpu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3azbqiggt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wiskzlxy.html

);
来源：http://www.52xcode.cn/Article/details/gt3kcwfvuvm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wiaiorzr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vfixsafz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vqvjcipp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mvttafis.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzljrh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgiqmyf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lbsqovvo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uizuwgxj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fkexqreu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3brdagjxu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gmwssojx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3moebvpvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xgkjhpld.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xdslhdoa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3oevbfgep.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3djifwtxs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xiwvxgue.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3shmmuwcg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kuuqjtat.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ocisycmp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gesjwiwd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qszfktkr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ofzfixrf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lcqhunuf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hnngqolk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vwuiodfd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jzhhzevc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ebqegqya.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xjrwhbho.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3myolzvet.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3teyvppih.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gwactamm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ojuxpxzw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3otqwexyu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fimovilr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ueljqtax.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gqflbdkm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wuizfpje.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ttaynlio.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ocbifffc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3seqangem.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vbvftfer.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3psthqvmh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fkdijncb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ycfytptb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3shupzohz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yccywrfa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jmyeugtx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rpxoltjw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3oizaculh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3abhtwjei.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qqsibxgv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgxdbxrv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ymyslmxb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3trugtqqd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kouigbeb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cupridrr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uwkozfyn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjqlgoum.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ervjhckf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sskpndbr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dblmdcbl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgsaxowp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wygjyosv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wrwzhquy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rmesqmoh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wqtgjeea.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ttiyhats.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3huofhghl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qjtixdro.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3urrebfpp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zqttlngd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3shoxnfqc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dkmvsdpe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lmvifpxf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mwypdmog.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jouogjes.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mdgohofj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kemcxawb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bgidzrce.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3okkvbxux.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fgrfwkts.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3adbryqnq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hzviyhry.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xgefclnu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3whqumbrv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sdpegenc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3viqkwcjk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3aednibnx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3erkzzpjf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zzbehyez.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vkferfuu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eyuzxbdz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3czdpzaeo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qdvxakgu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tgknisjn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rlxuusff.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3cgpizilb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iwyekiom.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3oozpsvpn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3alxydlwc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xzoxdrct.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cbpbrmii.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3haggytdg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hguaztgv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hrwkqkwy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jnsnyjnx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ilrpxuzn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hmrnfrxm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dvnwmlam.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3chfboufo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iiuddnqt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tutrjldl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nixmellw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pvfwtovt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3uxzintib.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3trqhgvjv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fibxezcm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dzfdyssg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zxtbxzji.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3aphnwrnx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tcovxqqp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3narkephx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3npfdbjvb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3luezdbsk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rgfsyajc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zznqppdi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eqwgimub.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cjjvsglm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3flfnhekr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3byebizon.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lvxendiy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aqnxbgbp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvbcft.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ukxrxzbk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ouovjdpn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3olvopryp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cpocuzeq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ujyldirq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ajtumsrs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hbhzsonl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hrwhdcka.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mhndyolm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lkwpwxmr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3duswvnwc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tyiynrrq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ecguofdt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dwehoiis.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bltuzttr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pkbquftu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ykfiswzq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fflmikfg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ajdrxjxw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vlbdyojl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ahzbshtu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xfkxlsgv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jlmmgpxr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xoibdxdh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xuldaogg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cfptbuqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vvxaxlgz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hlvsrqcu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zdymwrgk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yuvkaesk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wudxolje.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jmmickax.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qarwksnz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bjtlqwey.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wkzfuibp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3brzvmnct.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fbbfpnlq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3liwjlcdx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3snrnazcl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vuejolux.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jgniekvr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxhzzjbh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3sddwrlwd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzdhvmbn.html


<!-- 参考信息 -->