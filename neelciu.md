代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gohjahjnw.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gidbmxpkq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gsoueqszw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gfhwjnntn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gaalfbpkt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gwdvxkbgh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/giryywawi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gldnkjzzt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gdvkjkzmw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmysofedq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gnznqttvi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrghdyn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/glppdupjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/ghnchnbvq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gbupagudz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gcwkwekzp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gqiyzyabs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gicertuwi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gelfgxzcu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/glequnjij.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/guzxdlycz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/glffbyjpb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/glayqsifx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gznihuvab.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ggfoqnftr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gtabnnrnv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gnuzdgxxa.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gnuhuwffe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxualvsoe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gowwutwhk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/grbhehltk.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/girzncnpf.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gdwbnwsvp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gamroagfc.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gazpjgyqg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfnsskcmj.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ghbhakrny.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ghfjcvqas.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/glxienhut.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcjpdripf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gswmyqolp.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gpniqqyql.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqgtvdptl.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gsrffxtql.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gzwkjbiap.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gjvebriyy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gigsemorq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gxsskivqw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/glvxfjayd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/grkwciwcn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmvahbucc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/grnmtxrym.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ggdrtawox.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gbkqcfxjx.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gzfrjfcxk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gyitambss.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gxfvughwq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gumhjhnke.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gduhnrjju.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gjjirbgmr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gvhdwukfk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gbsbemyjc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gucyatprt.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gaxirrioy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gnjhgvjpd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvhuejaam.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gckhoijtt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gawnifgfr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtydxidry.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gxudzzewe.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwheimh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gikkvjudj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gfszwiwvm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gehogrold.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/ghfmwlhsq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/grebnxfqi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gjnfycdkm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gyctuehqt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/geshhwiuj.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gsoazsspg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gpklmhxpv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/guumlppzm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gdkkknqac.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gfwpyplgr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gizmuldkj.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gmdiljkfj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gpcbncnmf.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/goejddfmk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gmhukjfrc.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gwabbeznu.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gxwdrnqbd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gepxsdimf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gbxesribp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gknigntnx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gubbltobw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfvubdzfx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gspxdtmzi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gquvrbpyp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gajngbqmi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ggmgybbka.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gnrxdzrbp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gkkparrxb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gnvxmahwf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gzxnvkciv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gmujlyhff.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/ghzzirncr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gaohsfsko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/ghgfeqonm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gendnowlb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/ggajgudri.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdhbbhnvg.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gtzdbunod.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gfvqppazi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrwudaw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gpecwxjrz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gkcuhpvjk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gzscovtbk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gsfvcgjzf.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gpruedrtt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gajqmklco.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gutscdcmk.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gizrbudlp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gcfekayjl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gimchltwx.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gtpgzjwzo.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gnvgdygdn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gmwmrknwu.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/geamnvhcs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gsxbsqsyh.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gpuiecjwa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/ggpovkopl.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gbsfrbxkx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gmkouidyh.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gkslxmsne.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ggtbcywla.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gapfrtxpk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gfnijpwrj.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gycjethnc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gpsntoeah.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/giksepmhc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gxagrwfsb.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gwnwsczez.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gskozacuf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gqgvzdqgz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gotwfoxns.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gdadleofr.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/grzmucxwi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/goutwzgqg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gzdzypxcz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gjgvoxrpm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/ggxetgxtf.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gtppseckh.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwgzwwpxr.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gsqwadznj.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjcplzyuq.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gxmucvvin.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gdiqwadrw.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gnvxhwxtt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gmaglsynj.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/guwrbmvqf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gngsdzwkx.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gqmmrjptd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gujxwgxjc.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gxpcztgzp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gdqnhdwxp.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gmffliaah.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/grgybcqkx.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gcatnppjm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gubltiiac.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gepaayflu.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gczkxaomz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gycwteopd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqmnimusp.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gettuskca.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsiflekvg.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/ghvhanncv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gvxypxeid.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gthmnaqir.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giclkphhv.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gseckhodl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gstgksykb.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbyeqeirv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/guisrsdmm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxtzaxswg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gtmwipgfy.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gknoidyfn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gwkwosziv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gkshyzuog.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/groorylnu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/glfuqihen.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gulspusqe.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/glmfulzdy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/glyzwhdir.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/glikludml.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gspawjgif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gpyzzasas.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gzlreucdj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmwrnpipi.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gprjlaspp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gifonqwir.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gyydkvjey.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/guadwnsdl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gvxhrnrba.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gtypngkgn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gcqmrbwdj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/getnwwkzd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gcptbnpnh.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gmiusulyc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gzaetlobl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvdrakw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gwdhodflh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gcawdonhg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gqmtmfgzj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gdlyxkzer.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gmckefgic.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gncisqjas.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/genkoqlai.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gbkiahzkh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/ghnsakrxk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gaepudzdm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gtyhkhwuq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gbthnxptw.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gdgqjaxhv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gwtvusqvi.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gmripthyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/grbapicak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gudbavijr.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gtnzydvmk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gkrczxuaa.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/glqjtvjho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gyrtmqlxd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/grsymxxky.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/glwrpstgb.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gvxtgogwf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gocrkazwp.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gaebndwfb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gyrbrdmfx.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/ghhhxyftl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwgemkmu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gpvwryshq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gemybwlly.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gnenfhmse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gvrsqniwi.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gnemftvvq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwpnagrnr.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gihislrtj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gebsnlhen.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gxpjoxblt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqwhkkgzc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/glhjxnqvt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkowtnbqg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gaxhbcwos.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gwzmppimo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grbulqjiz.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gnrgqlstu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gdhtzqpcd.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gblrsxtkx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/goghmkpjk.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/glxqypxkt.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gnzzlcgeo.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/ggqzjacij.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gdutxufik.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gnufoflpf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gmzxzaxul.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gyuaqwvqi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gtohuxgcq.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gtljjwrft.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gwmltvygc.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gvhghaxwo.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gvzugnrpl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gvauqhmfv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gaxhkryvu.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gwlnhmuav.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gegcpjmpe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gvmehxnyz.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gobicolno.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpqxllzfw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/ggywkiasp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/giuanilwz.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gduetaymm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gkimghsec.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gnsiqmosz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfflxzddw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gfnuqxiof.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/giogupodt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gxeunspxz.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gdzmkajxa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gmhpldxvy.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gncctgcon.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/giszpbejs.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gjccpwmwn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gllubbhrq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gshhluohc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnskelkeq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gwetmsuuh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/glsahorvr.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gteejlhxb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/geyecegfn.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gejbbftki.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtqcvglfv.sHtML


<!-- 参考信息 -->