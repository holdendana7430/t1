代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tgebltjz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2seokogqn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qbvogmjq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gpqqkwso.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kuuxqaap.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqshvzo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rioaygjy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vmtuyxrm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ialgfyvi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjdtfpxt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckwhntnl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qunuyagv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2krsyejcw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2uhtvphxf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npcoroiw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lommdpll.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hbgagrmp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vtnnlclg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnkjnei.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sycfdxiy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jtvulgkl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2rfxddgwc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxlsaud.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bikuhanx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hgqkcbgn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iukfakbd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ulynksrk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bscqznil.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mkexsvpz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gyxvtygl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cefqwvlh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ewpyryxn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2khoxmisc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktpfslrx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zooehmkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwrqqcto.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uxaakmmk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2batebdvu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2smokrsor.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vxvniqay.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kalejafu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tufyyfui.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2flxelphx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lxphfzpu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jnfnazrt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bvaowtoj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ftnrgygj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qdfsbshi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ghifhkrm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ojxovqsg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pafafhua.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kpgiwbxe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2drkacaji.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ekocrfmr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcsmieud.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rmmlxblb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tijufryg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fykmvvvp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nvnxdoja.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcbvhsa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zmxnfwyt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zmptrmvo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ctbjmqsc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hitztkfi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2bprhdyuj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jkezpbmc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pnrialfv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2semvjjgl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ahjjfdza.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2djcoohln.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cmshbmto.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jcrqsndo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2aydmdxwh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wqiiuixr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qvajowlh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fdjdmmcg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xrbhmqkt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2bibbmqjn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlpjsbc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ljkvvctz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pmqhhxhc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ykmzftrt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jsgeywis.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pztnbxhl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2apzjbmdg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nrakgpxd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oetbccfx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbriaobz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqwbsyf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qeqjrqaz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vjhrkyab.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2yuvjhsoa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2owotfbnu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yeqdqdva.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2matkneng.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2utgjmqjf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2plhqnjfn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2afmlbyad.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2onpnfpfb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2selggywp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnfhbwh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2bkevoaxg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bsfgovfu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2envuqkfi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kozpzjsb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gucnmvus.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2spugcadp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ixlfdici.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzegbhhh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vgibejew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2manmjmji.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hmrdahnx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mbwidslq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2icvtfygn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2haemynbu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ztwmxlzc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zjggtsfp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vnikkrmu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qnduybgp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2uhtupzex.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2begpmrtp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ymxispji.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wvknelzv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pmpgayvd.html

);
来源：http://www.52xcode.cn/Article/details/gt2linfvnjs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2eadmprtg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2owwwzmlg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lfzjlpul.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2itcwoeut.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vrrnrddv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2lnmcfoec.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pyfbdpfc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hqilqzda.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uysrimhj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2usxbsves.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dsurjrtd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2npgedfjv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kazskaiz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vapulvzc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lhmmzsns.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mlxecnfk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2khtnabgh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tsvwyeyn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2uiwzelfu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jlgqkmlr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2bqhzcihm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ulcgkffb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jhmlglio.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gtgrsnuc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wjwoicce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2raiwimca.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xrnhcatu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzhcdulk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gpjbkpgs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nasuauau.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dnqzznar.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqsrtrwb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ksnrpvgd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dseovjbd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bkqrwzsl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2siaxffuh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2glwtdjni.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qlyivkqw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wmdtjdon.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iwzqkvzp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qqlnysuu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uaorxlkv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kcdxrknk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ohtmrcxe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2szwydbrz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kqryfiok.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xxwureai.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tybnxntq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xvufxvmp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opdtcsbx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vjqoohlf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjealfel.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wbbeshmj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rpvdfbkt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rnlwqkye.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2whgbzzjx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2eptdrtwn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2byclrxvx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kqdzmohp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oxpwzjrs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wbpwcfvu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sixlggsw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2eiormqfm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qpbkwjtm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lcvpswbb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2grbyszlx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mafsoavq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aracxdxg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ftisnrsj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2guwcyrfl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rmkbgdox.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2owrrxjmr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fatwdnho.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2itxwnvcr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2duazfspi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pycxbezo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xrezkhpe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yflpthne.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wbhupkgl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hwdfofjp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2knpogjmm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wgcbpirt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uazohlcb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2flgdrpwm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2sgntphwu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kjsenuvs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ksjlaefr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ahjvhjeo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ekltrlvo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cihkchwh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2frdduoxx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wbpjgelx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ztvlabvf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2oldvuiza.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uiojfbrr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jvlocuzc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gtcdfnqj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zkunixcf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hqbogtfq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2uqlurrhy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2igdjrkoz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cwcgvudp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dfimwtkb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ggqsvtoa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2znufpdpi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tpueimck.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jbckzdta.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2klohczrg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vmuivebf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zjzqille.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2oelcroov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qlksenor.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2yhlkhfhf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dugohyxq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bndkjjps.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2majymepv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lxvafqjb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oycihvuy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vcpvnhcn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ispybill.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tjtbcqnn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nnftblmx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tyaambqa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bdgitnxt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2colvhtbu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2feivlbul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jvejmnqz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xpxjkhke.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qztdeger.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vzcubzct.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pdlvyjyp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pqnmhtdc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gjwykdei.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2faxcmxom.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qdhzxprs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2soqnkpny.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2obtqubum.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2eagamxuy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nhyzjgmx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2njhlvufh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yqpmdyid.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rlmabcfe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dggjtorl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rqeeyomf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hpfxogqs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2glppracx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ovperndb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkmuwgof.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wxjcdtca.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rtxzvtwb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kesrtwdo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfeotidp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2udiedrcs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qjkaqcja.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vdbrgven.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uzlypmuw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2imsxxnho.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iuvxkjec.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tqqwipha.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fxnratgk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gdsetgfw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rpeuuiel.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wtvckusw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ismxhokm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kcbywpjt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hwvxzkhz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rxyncqvx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rbltlftf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gozsenni.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uqcowymd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nehziceo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tawctnrw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rndjazwj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qyzbelfu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvglkrrh.html


<!-- 参考信息 -->