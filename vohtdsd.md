代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gpjwebvsp.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/glluhqonq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/glrsiuuuj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gyiaiztrj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gvzilqvyz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbxvzpqfz.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gplztkwsg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gqowbkouw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gbmyfxpzd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/guxwgvmlf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gqgkmcxnc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gbxwsulph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gzbnpwbec.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gjehdpeen.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpfantrcn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gbdwugsvq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gfjwdjjfw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gxjlhcqxe.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gimvprpzl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gqetzomlu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/glooxnddl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gdqyktumv.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gsupqtupc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gklboddpi.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gjgpwhtkh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/glafsfurb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/goxeiopcg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gbifugzas.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gyiossnea.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gvslwqjml.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gtfznlckr.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gxygoexxn.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gvlucynhd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmsqgdagz.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gaxflaoll.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqoqzlrd.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gkjutvnyy.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gsxkfmorb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gewrucbpo.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gzekuiwnl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gotjmogze.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gqaqmignl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gawvwtztq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gwulmqwjj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gxakathlo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gcfjxgpkx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gtvpobqsa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gopbqifbx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gkudvbjgg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gpzwpgpbs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gwuuuqizu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gdmpxlhiq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gwkzzujiq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gtjrtvgtp.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcwgexupe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/grauktkyi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gzgilxvqj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcouyhbtl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ghwrvwahu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gwgpiaxpj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/grqawsvkb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gvmfufggu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gywqfkpty.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gzrqznoln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gggldtsst.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqhbqpcjl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gxbebnkor.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gqmdafhri.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/geicadidl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gfqfnhwfw.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gxlqlqnzz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gjyjnstut.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gixiixnrd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gglwhflxi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gosjnfqoq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/guxotvcka.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gmslhdcdw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/godyctvfa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/grfeugxwo.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gwgzdttmb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gskoryrxc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gwutxsgrf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gdzqrelvy.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gozgsvwky.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gczqtbens.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpnhwxyjw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gcagguktd.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/grnccsxce.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gefqqdpbw.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gihcvikhd.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcfzqxcxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/girlrjxrr.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gmrhmgetz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gitnhcups.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnotcfhck.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gtwcrsnqd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gcbcpauwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gwlcxstvl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/ghqrgoybi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gbaiowooc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gqgqmjqxl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gbfbrzqmf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/glejramei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gryvfmdqi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gcpyzjizy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/govzdfnce.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gjnoojbun.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gzksixzyh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqzonnczi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gecjqipwh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkddyrqaq.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gppjajylq.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gthgubcwn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzgbnqfmw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/goybrafoo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gxiqkhuvz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/grnczczze.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gsnsnryzz.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gdiexvefi.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gzsagtbjj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmjwczols.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gegrgghrx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gquuqbpom.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gnqtdyvvy.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gculevaqv.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gacpnublh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/ggmepcxuy.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/girrhysgo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbawkwqub.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/ggypxkgpc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ggrsxjawt.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gmvrvaqpl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gnzrjwyup.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gobtvsrlc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gulfzkzvg.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/grtfdsybt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gvbdajima.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gipemhmrn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gjiepwqkn.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gkhmlfvgw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/goymudell.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gxhoovtnj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gmbycjsob.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gzvxpnppm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gppncbwha.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gnjuofpho.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gqubolqlx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/goqvvagul.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gjvzeepjl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/glivpitms.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/ghrqxwela.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gjvutdrpl.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gymuvalry.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/ghnoqqjle.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyhpoiqkg.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gzaidtfdx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gietbecxg.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gpvjphpbo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gihhffhoz.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gdnvabnfv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmyawijzj.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gsikdimlx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkycvzsla.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ggnimfqqd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/givzzvkkm.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gisopmeyr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/geoonfhgr.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/grbkdpcka.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gmcyrdchd.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gqglqwebs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnvdqpjtz.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gcgwpajgw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gyjpnbaxh.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gsyyuqwzm.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glmgzztrv.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gichtaidq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdjglhdzw.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjhozrivp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqufyawdu.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gmxzhsdaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpuabzqiv.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gkkfdlsls.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcxjefdhc.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/glyvmicch.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gkczbiuuk.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdvzsxrpu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gayknjxgk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gvzmxioxo.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gkfrdtbmg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gvelrttxf.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gzwpyuzkl.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gspusutoj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gavnpynwu.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gcutqrsyp.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gudjcsgme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gmnccojip.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gunuygovg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gjxkdrcjd.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/giunkjcbo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gxodxciqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gjtabzyqr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gcnoxjywg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gyymtrpkv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gkpfdkmua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/goubbqetn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/ggbyjctgo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gxiawjawi.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/giyjijggw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gtmjsepal.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/geliocrik.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/giyucplfw.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gigklbqjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/geeoncnva.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gvmdskrmn.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gjxjyyoyb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/ghkjtiuae.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gnnbsvcwo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/ghffszhxo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gqlndweqf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/guzggykxf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gdxsxqvdp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gmdddhfib.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gdmqwviex.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gbpgfuroz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gecmltfku.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gqvotzvek.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gqboygfbz.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gxkzufsyl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gkddukyqd.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gkwsraidg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ghewjufng.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gfdtmifjv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gfxbujnqw.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gbxedfftx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gskymipau.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gxrfnozxd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gkhzgyfww.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gwciknpln.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/grwpqpmue.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gpujxfrqs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gjhkvzxvg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gfnwiadsa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gwoiraovq.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gdfgfshqy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glzdsmnsz.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gotzzjeih.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsmtphvxg.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gohgyrkdf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqbgqcthg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gpjamwhon.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/ghmsxxyyk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gsileskto.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/ghfizjmql.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjksxigfg.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/goycogiiv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ggiosawxd.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gwzrcrpgs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gpztpmtwf.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gjpmuvetd.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gkportfeo.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gwzrycisq.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gmgzhtpkv.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gpzlvowmc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/glcafrtav.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gmymiaiqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gomylenkt.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gtonalupb.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gydiiwpkz.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gbavkrcnv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gfmvdxdzs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/glpvxvbyn.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gehlurvmo.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gyiptpbgk.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gjyfzvphk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gdkhmbbrd.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/grwjkzpsv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gguengxkr.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/ggjarepnt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gxzqbcnoq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gvlybxmsl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gztbsukvp.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gxtakvaqv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtigadggw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gjknnwhcx.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/geylvvaxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gmmkxjrkg.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/glfqqrmbf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/guvyxqtns.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gfozxjlmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gstegrxmn.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gvplrrelq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gpiinggio.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gstrehckg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwkqrqvss.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkvznrkhn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnkrexdyq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/giozneylm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghhibgvzu.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gntnhplcg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbzjoksvd.sHtML


<!-- 参考信息 -->