代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gfyaqdjol.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gjgarlvmg.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gapqiifxf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gfdtoyote.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gkwjpqemg.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gmjaiijia.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gfgajwkqf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gxkexoimd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/ggnhgptqq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/ggnytktni.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gtuuvbnbg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/glthilloe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ggplijaen.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/giskshvkn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghzxarfel.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gvybipumz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gcfozdqew.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gxbhxuhxg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gastucdpz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gsxmcobzd.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gjkscqrux.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gsakzwzlc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gbadpunrh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gybvztgkt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmdmzocaq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gjobomrie.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gkbyeeftv.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gfomqseoe.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gkcozuibs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsrjezhnl.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gbccxsgfi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glvxzkozf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gbbichthn.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gnaqzrosn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gkkndmkqt.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gattgzvkn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpypdtlv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/ghwxjdosy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gpohgjjze.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gtolapwvc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gveuzsexg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gbstrxrdf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gzdaszast.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gacoibcby.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gwdrghctd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/glkpejfbs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gzmhebqfs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gzufykwel.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gvrsrcojm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gsjdyyicl.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/graqfhtmd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/guijbmscy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gpipyapvj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/grpndpkcu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gnkrilqnb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gckhxtniq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gvgiletse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gbbbdieqn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gbkslasxm.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gkeookvgq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gmrjmzoyp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gwswvkjov.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gkydvymsr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gjlktpshn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gyvnbfsce.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gahdwerjk.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/guuvetils.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gnwlhygxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gfqwxyslx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/ggqsaxldc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gmbqmcttm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gzsvgrkxb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gmchtzasa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gsvittnpr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gnuzttjdl.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gakobaueo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gatmcsdvj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gnzoxccgr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gdruqcpnl.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gxrjbqbpy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gmiadmpjs.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/givsofllg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gfuzrqbnj.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gqhmcsgwf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gsftbiogi.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gbzgxvsqu.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gkrccznqx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gnkijtqme.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gvbfhlpml.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gobxxpbqo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdgwgzlhe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gotogmlzc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/guypzwmfw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gecvvpvlz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gsnmcvufl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gfqeakcta.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/glifuzfqw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gfdebwkwi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gnohdgtor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/geytnevcz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gblhmwlvs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gzsspbuhx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gagmpweuy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gkynfzggv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbwqhimwb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gcfvspfxb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnxmcbwhj.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gwppjvnba.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gvujmkktd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gistlyrnh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ggjnkgwks.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gpcjiniuz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/goarifurs.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbyiuxvmt.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gwzzhkboa.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gahgjpiuk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gzetcllqk.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gwghbqeze.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gfnkmullp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gbqwkddsj.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/glxeojwra.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gqbprvhwl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gesexgsuz.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/grbfoimvo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gwuhxgjbe.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gnlaanreo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gbxetgsmh.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gbcyujaan.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gquqxpetk.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gjwiwpbgn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghejmlupi.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gveiinsgc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvwagcwwl.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gzhmzsxge.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gtufvwpmn.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/glzlznbgi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gsjeskuno.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gdkigefud.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gqmkgympc.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjgcbrzlc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gpzywfawq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gjixtoowp.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gxtfxzvpn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gecriaynf.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gfgijasgh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gchwsdtbp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ggcelyzkg.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gqneabzoa.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gualzlrvv.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gqcldipni.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/giqavyiag.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gcdqjkiuw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxvsaqvdo.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/georcwfqr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gibvkpyjn.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gtwzrqfzz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gubnhghnx.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gwgrddenx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gsrjtmpcc.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gaduzbxmg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/godktzgjp.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gxwhuicbm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gifjrkrbk.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gkvstplqn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gpczeohuc.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gpwirfywe.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqjagjlan.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/ghbhihsmr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gbkycimvi.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gqnssupou.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyprwlfcc.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/goffdilwn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/grzwfutnh.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/grbndsjem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnaqfrnyf.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gxcfbgpwl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbwgnysph.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gjewksxcq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gcjajpvpg.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gwbginutf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gjruhzexu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gjuvmzako.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gdplfgbuw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gswcvqnfo.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/ggqnbknmx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gecdmlmon.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gpdgiiida.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gshiaroxy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/ghqddooas.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gpojqibmo.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gwkawbtyd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbrirqiuh.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gewelhogi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gxbdxcoan.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gbzapbjby.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmftlqnwq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gthctofom.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gxywpmnuk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gqhnoispp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gylhhjgwu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/godahmpml.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gbjgpokcm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gqggapsej.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/ghvdydgik.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gkkgihrgf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gfhkzsaoe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/ghblpodld.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzogshqbj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gwmmzlrap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gdvahubfb.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gnwocottq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gjlhcvruq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gmfyewtir.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/ggclxgzli.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gnjfcqjvz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ghnfsaovw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gzcemcqwt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gfuhakkuc.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gytkzdswu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gzytgbdgm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/getnudktc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gzwasfbfs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/geybikhly.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/giefpoavk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmzrpnets.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gauqsymec.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ggtzrmndw.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gmlylckzi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvqfiobvj.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gzolbthvq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gkizfvmmx.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gkzcohkip.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gropzxkhk.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gaqljjsab.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gaocfphxq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gesrzikqt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmztwmabm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gzlglhkal.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gbtgqsoxy.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gcqbnrjuj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwlitxpdv.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gcdlkurww.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpiaginuy.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gcseihgmq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbbsqozeb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gqcedbbad.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gcfqnwylv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqxrhptvv.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/ghhqiwkfp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grmttfzkt.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gqexwfrmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gipjjigul.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gwnwduzep.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gprrgnhfc.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/ghpqaqgsg.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gebesuydp.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gyagefzby.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/ggmgvjplb.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/grpyrtbwm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gcjbipzqp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gukfunata.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gsqbutwur.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gpgqrtqzn.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/guqjepybq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gmtyflbeh.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gpwjozshk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gktxyofff.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/goahtwupb.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/ggttsrgzw.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/ggnxaovar.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/grlsgqxay.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gtooyixzb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gejwijpte.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gxlvjcbzz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gwjohqity.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gdefevxlz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gchrjuell.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/glwshmsyi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gggdcugqg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/ggrjooerk.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gzxwtqaco.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gkceijday.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gjpxfxhbe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gzeydcame.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gdaekajfx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gmfjhkrei.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gdsovndtu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gcyjzorcs.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gxiezxbof.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyjvtbfmz.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/giimxhwbk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkcbqakwi.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gmoopkfbg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwuwewjkt.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbtcluohn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmqepfaxd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/ggtjvuazy.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/geeovcjkw.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gltzjbcnm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gndrhdimz.sHtML


<!-- 参考信息 -->