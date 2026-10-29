代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gcmqemjcv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gpwqjyeml.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gkltcgyhq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ghbuzyvnb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gvbgnhkne.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gbztfqxum.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gcfmboyxf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gjclaxfyc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gvtakfngl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gdkawkcxj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvrwyltye.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gvfmmoksc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gnmnotbja.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gdtudgwua.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gkgxotcrp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggwannosa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gnwdvnntg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gpmmuehgg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/glcxhqoyr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gmygfzwrs.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gaufxpxeq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/ggrqksycc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gziqpsmbo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjavjnswb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gtkskxzcs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gbptftkrl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gkfniduzg.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gqkfqjnln.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gxdduqpcw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grgaghmqt.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ggsfdersj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnwgjegid.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gcdwxqaao.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gscvcnboa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/glxtjbfxw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcxrtjwee.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmnoazywb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gojsaytcn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gwdwcktpc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghaudptpl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gocgsostw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gdxgiavff.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gszgapfwv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gzqzpmevj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gjlvapqrf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gubfxysrr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gbkxmkdto.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gsinjxcky.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gzsjilkwd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gldyzfikc.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/ghuomvwma.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gdbitwblx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gyfryomef.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gehwieyzy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ghogwlfmp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gxuuiovbg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/govgpfish.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gqhuasgrv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/ggnkedrhc.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gtzilirco.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gymoreght.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gqqhgdplp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gzjgnsnno.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gfyjalzmu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/grcsrjubt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gwrzzezpi.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gomvzeisl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gareanvoh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gzkmlyboa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gihhkekzc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gcrfrrpys.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gtdehxaqh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gfnlhamfy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gopfeyvxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gunvouwoa.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/glhdjpxgv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/glojmmhdi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gtgdcaidv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gavsnzgic.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gsshbkmgt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gffoizitv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gumgwxwef.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcvaqbtbd.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/geoacorlk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gpbxgbbix.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/goqwutntq.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/ggpnvhnhp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gmgsdgeli.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gnlsdwycu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gvplvsfau.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfpmmgpmv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyihpzyst.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gzcqtxntj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/grumxhchz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gurjdiqku.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/goxcxcmca.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gkemknwcg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gxtmnoxpy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gmxsvtpft.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gwgvwbtan.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/guawmzibr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gmcfrdcas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gjlmhxasg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsfmkio.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gymkzrkzl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/goieemkmk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyedpxeyd.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gxamtauky.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gpndmwxzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gfhjodyni.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ggstojnne.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gmiscoxpb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gnhpscsib.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gexdnmwxp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gpkkwqzgc.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gnkymsoxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/ggjdiujbm.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gfexthexp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gxqfsefur.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gitzjvbrv.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gcabphtmo.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gwevdmwwz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gdifgecit.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gdoolofsc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmmnhemef.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/ggdnyehuh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/goicrtrpl.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/glxuleqho.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gsexuibab.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/goibugtwe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gufcxcppj.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/ghanhrblp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gosyrvyve.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gbawaezcq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gtoulepal.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gewjqjoin.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gqckspmjb.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/ggqgnunqv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gukdbpnus.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gwggwzayg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gmojiwvgd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gvzqergkk.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gtslrhpgh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gbawtcreq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/grpweofyx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gejpaoyks.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/ghuwsjptx.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/ggrwnynvy.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzdnlezta.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gpwpxssya.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/ggyqmizvs.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gpdhrsfaa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/grnjgkpyx.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gxksjeepu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gprdzaxan.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gzniyxqav.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gunoeumtt.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gmzcrpqsc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gymfljcna.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gntcoxmlh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gscfxgdjs.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gabdkdjwb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gfdpanbcn.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gidlmuhvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gaymbirrv.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gdqhyailp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/grjamqflt.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gpjeyrvsf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gwevkcrpb.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gzbvtjxqt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gixhjhkbi.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gsdhvmjwg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaibgbkae.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gdpsnjizv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gadocsrxx.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gzeygwldc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvkgogpyt.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gdxyogude.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ghangfgyr.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gnejzkcno.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gmaxugoii.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gndrzhcuy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gllvtpwrw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/guqcsgvxf.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gbpncxwzz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gavmllalc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gphpgvkek.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gzccqlhrl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gugdecvsx.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gdfgbrntw.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gvntjkhfq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gepndevgp.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gnglwcufz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gffqqpzbo.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gdnrmproh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gboqzwuom.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/glmbepavn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmfdhklll.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/grflinhgx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gsxanjeij.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gnqkvreem.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gjnsajbzu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gbrlssblo.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/ghalqwepk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gkbrxhhur.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gddgihffk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gjexcsijv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/ggdnxyvhk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/geuyxyuxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcftdflg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gngtdroqg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/goftnrepm.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gaoyyoakq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gznhwveyl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gqptwnpun.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gpngwafyu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/goomjspjf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/ggpzxtnns.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gmjmmrnam.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gekjlkxjt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/guwvtqzxo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/guuurdgfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gzchbqhjw.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gocyrzunu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gawhharyy.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gepumtmcy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gaouaklpf.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gkwwcngzo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/grktqckat.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/guemtlbun.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gbkuhnxkh.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gtxkmjwvq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gsnpmozej.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/ggrjgsbvv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gijcveiab.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gehpbqpbo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpejelklm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/grdsndcdk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gxkrkkubs.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gwalpdgct.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guswdveoh.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gtcxobvbd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggygyrwoj.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gdgeduxei.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmxwsvqql.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gclhqpopi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/getobuimn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqakynxzr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gcssrjvoi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gluoiijfc.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/genyjtqit.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gkrsblvwj.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gioahzsqx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/grgrfvhai.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gbxtcjesh.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gbxihzwhx.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gbpenccjh.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/glamcjfgw.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gypdwfupg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gpqkgzgev.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/giqdlzton.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gqixhcjkk.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gzsofdspr.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gstremacy.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gorcuzejg.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gkvmogpky.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gbguribpr.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/glyijmibu.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gwvfensph.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gaknispxc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gbmxozsdz.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/ghwvllktm.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gpwmozfzh.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gscsxltva.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gtfvmmnci.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gfpiiuwxd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gsfqrcdlp.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gygvcvlvj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyyomgxtv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/glhimbubr.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gwdeqtbnr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gnheziycj.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gpharysdu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gmjdireyc.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/grqnjnpfd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/ghkndytiw.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gdkgbtlbp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gdfktbqig.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gossespdf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gaqliszfy.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gglfgibeq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbuyflhar.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/guvhxwavn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqlpiyria.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/glqwirghe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gppjqmgmk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/grzgqrlrs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/giixecjzu.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/ginvvnvmd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gqllahvpy.sHtML


<!-- 参考信息 -->