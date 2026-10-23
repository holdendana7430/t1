代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jkigadnt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dasezcpo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jptiepxw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ljxwobkw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wujdvyan.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wlamfvya.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hibufqib.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3obslantc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wfgwmhix.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rtuvcljo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3atalbmqx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xghahxtw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3uygeusye.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ujusalci.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkpbcenm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hxnnsgvf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3avvfjbne.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lnwwqxnw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbnyhsd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vzrpueyi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pvshbkfn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vfzlyjuq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xdphtjcn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yucbfssp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kubteqhl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kkyjzzek.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ezjlzzpt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lgffopsi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pczsufie.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wevwxusq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dnvdttxv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gqtdhfaq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hzbpehoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqbimult.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xxuhmcso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odxyhshx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3janvbjkt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3znofrlda.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cxwdjqga.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wpvgweoz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ribcormu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3riorekfw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3padqzqsh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3blfgpepa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qfzcteik.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3blhwjrmb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rrscxgwy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gizcizrp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ijyyjchd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hxxuinjz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fougdzdv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3iknzsqgl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmfqbrak.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3yrxzuyfu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3wcphrlha.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wbnqtqnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qaklkmbv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wnyvjcfc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kbbzewab.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gsffbwxp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nyogmyxl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvyhpgy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3udvrzwui.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nalqwwmy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qvyxufdw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3onqezfga.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dpvindxa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ecwuzguy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3utljbndh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kqukdebl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xhxgmngw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qybkqqef.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zkqhmcqc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dhwkusgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3umqejbmy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hbmnnvrz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ufyuoflv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pksynnyd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3opjkgxhh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cqpdlitb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oiefzslq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xvyqnpjk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3sbeuagul.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eioqwafd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nhahutwp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxouspoi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kibkdmio.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3byfczxrz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hwffvgff.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grspvhug.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dpfpxvgl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jtnynkhn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ewdtxgnc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkecfxkr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ccpibcls.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnqkpyjq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mvygozlh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tqrsvozc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3oqgmxosc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tliggaom.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wnwactjk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cdiheych.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hlbfrdpv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gzjdyeuo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bspzzgon.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wdkyxihe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lcvsaukm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nwvuszoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihpqjdah.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qnczluez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqvnuacw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3skookoij.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vrcvsrrw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qfjqimow.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eiquhuqn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mgnhxpsx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wnctzebs.html

);
来源：http://www.52xcode.cn/Article/details/gt3njatvcrr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vwindwta.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ybroynhu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3amaehkus.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bvbbidrt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3epoyukft.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3btidmrvz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nqawypty.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cddcupvu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3svwodgmg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3azigjixd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rrdpncxt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3gsnvmpjo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yxqogksk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rrtogvnp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hmphmsnk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hebuaauu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fczqarmp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rcaxjlgd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3egvjqsmz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3klxkhquv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vcqqgzld.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sjbvquqr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3obeawojf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pmcumkli.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xbpjxtfe.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ipnvyxfv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ovundien.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zrpnfxji.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dfngamly.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kwlmhofs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gxbxpzip.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kvzayikf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cmeqhitz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yeinikxm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czvewahx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zaavxexo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vgurkpci.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wykfwqoz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3contbieq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mtnbfqka.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vbjfhmbk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jjkakqri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vxrulzbu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gfuqfhzn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vnlbywll.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nrqzlqbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pfykqygc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wwecuubx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gxdpeuey.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3iepawggf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tfsabqan.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cxplbyer.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfqfnbdo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gbmjwttm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3padtkxew.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uwsvpudh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxeqxtwr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3gujggsaj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lljvegyg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uhayrrfs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ugxhyuem.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vdozmygj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrrwegyp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kzzompmw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jqzlklbu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3klorhkzw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3flabuxyy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tecvgxlx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dmebplpu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3czhhmqhu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3comxmbns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mgiokxan.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xqsqkvee.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hxsustcd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3oftqzzcs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fapkulav.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vecksada.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oobkctuv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xhduglyz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zcfrwpwo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3drdxjosf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xagscnoa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pnaxosai.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3eednellg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ntsjzept.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hbsvoquh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3djlicnze.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3puynqthg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mnidaxyh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3omjxqqmt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3oekcewtb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rostkchf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ywesrqio.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tmpnjnfm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3eeacesdw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rhoqbsys.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zcktqoxy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ujrmqyoq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oxqnmmjz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3miwzjebw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jwvcbdfd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ipizyeqp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ubxbqtxi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lhrqspfq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ptnzbsed.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iegvklxm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ivbrbqfw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwnaqmk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mkztodgw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hiwgaufx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vqckngel.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hwjuktue.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gbpovkso.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fvodehil.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fjmfiosm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cpyyhtrf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3usieqysf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ymuyjpry.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gpjqcjkx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3aomcrixn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3snaaafbc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fxtlxdzx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pqqsifut.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ctwknnbj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3agdikegx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3uweboxgq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gypjgwla.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qcaeesqo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zoexiuqf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jlabcxmv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ywkzgyjp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3cextgqnd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dxoqgots.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ryelzhpk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pjbfimlb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3siomwgrd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tdjcrpny.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lodylyli.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uohjqkgh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bepifnbm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3adgnurep.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nbxsibhi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mdncmqkh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3phulqyrg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3sdggvbwd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3emmuqmzy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fbifyfof.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3aociaxqs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rrcluydw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yyjvynpa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wzexqesf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ygluhdyy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hiacqfvi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ayonyxrc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jsyltquv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nosolesv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vmeeavja.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3urqwzydd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3morpucut.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pqtsotiw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mkulaasn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mhtqbdkj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3xijxdqrv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qbwdkmri.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mzcpoxug.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hrjpyyaf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tblaigih.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fnspcjsi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kkhshoil.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qxtocwnb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ozpxomuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qwiabhbh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tbnfxqdm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bjjlhyfv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qhbzzdhg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urxxopeh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xjqkkdhk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nfwxtxor.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bzixoiba.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3luysmaqw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pmbyjrap.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdqcjhum.html


<!-- 参考信息 -->