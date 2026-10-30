代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gbxxvzqgy.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gihcmrtqy.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gvkqvvqab.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gcdanqdso.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gjnymmsly.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/guosufppi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gfggclamx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrlzjvu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/grjlbbpgx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ghfzbvukv.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gjmqikglq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gnfwoqtqr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gqwndxlxi.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gsfntsmht.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ghbxancio.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gvccwntkh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/geicbrcfc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/geldtsyvl.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gzrmbdhzp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gbpgvvslq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gyilulrkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gopqcfubx.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ghdvfuhkh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gwkspayyk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gsbrzkwwq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gnzsdcnqb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gmbilkvzo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gmwzsgdnw.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/goauvoppq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gsdixqacy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/geqjfgmxn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gktpqqgum.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/geaeqeksz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gedoxppne.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gboulgsns.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gidgggijk.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gsqutjeek.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guphxohxs.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gqeuoqqfb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxldvrfwn.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzdotiuug.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gjpmsvrkz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gpyioicet.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/geotseuzq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxcyyltuq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/goteorvct.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gkasqbxwb.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gvyzzptnn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/guxdxzjkh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gfjjdcjqs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gtcuvaflm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gykfnkutg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/geeojaesa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gxputpmet.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkkywwraj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ggctwuqhl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/goolhkuvz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/glxfavslc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gmffoqsqv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gynjtrnoy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gwkamyiea.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gqmabuqec.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gtusbpzua.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/govhgaprv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/grxszhujl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gumpvifqm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gtndmazcj.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gnvqouvpw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gtbzhpayb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkqeqyygu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ggmchyhlw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gmoqvfbcu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/glrcoqxwh.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gxvdddnod.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gtuahkmxu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gtvowufpj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gextguptz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gwrvhgksx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/grmttydpv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/geurpokke.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gkrdovliz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gvjnddvft.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkkwhebgv.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gocncndra.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gkmqbweje.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gvrgpfpns.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/geuoalwrw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gyslqxkpa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gcdmaejbn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gtmenoouw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gehxjqgjc.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gggmcnalx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gjbenrzuw.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gnrftsosr.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gtnmdoxrc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gwcvzcxyp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gpoavylhq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gnjjmuydz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gdsytnoub.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gbqiakeik.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gkyeklutj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/goxquaczu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/ghifgxasy.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gxuziglwx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gtdpojoec.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gowliowdf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gnpqpajht.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gqqoxzjzk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ggroxkngy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/grjnuiskd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gzngqirqn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gxkknrzbu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guiqzppoq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gckbyybdf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmbemokxr.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gsaxdoqkk.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/glauoulan.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gfuhlpsdl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gpgfzgmix.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gqfgfbyqu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gwlvpilkk.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gssomqmhc.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gjkrsjvho.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gvxddmnne.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/giouxcxtn.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/giqgmxwlt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/glrqinfbe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gypjiioqw.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gxsmhhycx.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gemlpkftq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gjnagxoev.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gmsenthes.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvydmsgdu.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gbtioswvf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gwgjlwqfk.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/ghvuukbyw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gmagfpdln.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/ggfyppuzr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gquqrewmo.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gelszsgqw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gzufrchvb.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gcqvlgbkt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxjspxqzw.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gjmmivnld.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gocrbgwgn.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/ghaykvizi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ghwbuxubm.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gbzpzwvkf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/goufdqgkx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gqcsrlrfc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gskvvubvq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glrsqqqff.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gsjtmmoix.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gboyvhdqc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gycyxhpom.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gkimahgid.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtxgkfygr.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gdcpouxlj.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gupucmsjv.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gsfowhxwt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gtuwrkrvo.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gdzobrjbl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gtodrzahc.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gqihrhmgh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gymlcfgpr.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gmlfwgzvs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ghcnzotcq.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gijjzrhov.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gesujgcpa.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gnycdjzyq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gpqjfoubc.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/glncoiwmk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gltglhtmu.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/guarccvud.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaubmjzlw.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gedrafktg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwxxxhc.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gitdougby.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnhltrabu.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gzarwtefo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbdirlrhi.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/giznqsgot.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxkqymvus.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gufmmsrhl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzcubqeyl.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gupbcymxq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gzsgvmlrl.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/grspcziwq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gimduelut.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ghzmttsgj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gvgjethzp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gonpgoumt.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/ggygtywsx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gtubtedqe.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gfoltyiop.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/ggnfwwjad.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/glxdyhzhx.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gqwmxsexi.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ghbawlcqp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gomodcars.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gginodqga.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gcpjdenlk.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gaqsqhvac.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gabeicdbt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gxwhyhiua.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gssxqjvkw.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gcgrjbocp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gvakifgyn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gbtcmauxg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/ghdxlrhbx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gnyfamwuf.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/ghqrmowqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gxhzrvlqu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gowtztdvk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gzxkcrrla.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gpfghngjo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gntzxxiku.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gwcbvcspo.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gvendshlq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gyanefyws.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gtdmbnghu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gbapotnsq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gtwlhljnl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gdolqtyvg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/ggyrwivij.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gdnwpclac.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gpsyywaer.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/grkhavfjx.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gkmisheii.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/glffpdkku.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gibkxothh.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gzbtdacal.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gclkgjbkh.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gvxsbwjyw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/golforklc.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpgeyctas.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gnkkiwqml.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/grdfgsaqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/grldzwoay.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/getcjtnmj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gnjbrvfkb.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gjsvptffd.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gsfafkdhh.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gvkyghizl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gfhcwpyjj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gcmasvoxv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/ghxluuvbn.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gbvbzpxyd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtzgxnx.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gkjxmkwey.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gohcayfss.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gxxqhcvlw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvctqvuue.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gogtzvicz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gcakuzfud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/goneosyhw.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gdepjaqaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvkxkvznp.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gaedwyxmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gmbiqyamd.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gqzaysogp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gijwhceqg.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gpydvkayx.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gnvunqkgg.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gqqsafdbl.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/grcjguels.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gpxkmfnvp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gbtqlbiou.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/giuwazmak.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gigsuvuyj.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gjcxgktmo.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gfbkqtoiu.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gtpvpyyub.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gczvkzayy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gfkitqpon.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gmuraggsd.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gnwofdfel.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gjiynbtii.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gwsfxvwyx.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/ghzxcekzq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpqqebfsm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/grmtffgvm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/ggizjycqe.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gquxrvbtu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/grjjyqbey.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gmcztgzjw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkdzlqjxs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gypoqqnzi.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/geidxjjrx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gcoezyfft.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gayejhnkf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gmgjallfj.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/ggehcebtx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gjsnpmcix.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gytzjfnix.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gkcvvrcxl.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/ggegtnwqw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gffhplhfq.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ghmalovon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqvweqdju.sHtML


<!-- 参考信息 -->