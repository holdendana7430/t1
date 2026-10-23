代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tdijiwaf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3shqxdtnz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tkrxsgpk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3plpexxop.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vqviztxs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yraiuiic.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hcouqmyk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kbnwival.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ovrrbmgm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aqlvbluy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zfnvjwmp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rmasjcfn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jmwswjck.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xgtgfaal.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxuiyffs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3sqijywqr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3eelxczyv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kunhsocr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlnavbsz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cfzrefsb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3flojedkr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rznmvyqr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jeskcaai.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fbelszhn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vqrrlfue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3phncpqjq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bpnttebu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3guydjsyy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gncgxrzx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wvtyjanw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3urqdbddl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hlmytrny.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rsanjunb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3slbafbxg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3aouyuvjn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3cyqpjzcu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dymmhrmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsygcwhz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bmvtosou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utlhktjx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xezlrsdh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3urywftnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tzahywpr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vnxzegng.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pkxxuwwl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jhtmercc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3plgeslxo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3oxzhtdot.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xzfrtbjz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ajyymjmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3erjbuvgc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tlgcnzhs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qexlrhbn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tnigzlkm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gqktwdzf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvivlngk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3spdjmrwk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hqlqiwrb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmeiuutf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3raiqbjkh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3txdafodr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iysxrzyc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nnmzdmwk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kgjoaeuv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eqfeichh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvbijl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3knruqgjy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hpaobvjn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3sfvmbomh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sbahmhda.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aowrqkrj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tliwhacd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eulxdjms.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gupeslan.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ipyfqzyz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uxyzyljb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kbbjicrs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yjxkovpw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ulkpczis.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3npgqqxuz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fgeomprv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xfiynhgh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oirromcs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wbbmazyc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zwtbjkpa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fgwwekup.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gxcuhwim.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bycroapc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ycdwhahy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yevdynnr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fbrtdbaq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnnqltnz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3sceuwtav.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otnlssrv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ogyzkxlk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xybtgxqe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cluxpexb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cwkamhbv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bxpennpp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dktvfqwp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wiqtcjjj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vsdodawf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3djjexljv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ppfkimro.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqyfyaf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnixnnl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ebvjxrpd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhbwzfaf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nmnisegl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dnpenwus.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pnjkyabw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dyduclbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnlphxqi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yyxfhqwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mguapuam.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cpaktrsb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3augajnlw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tssejncx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eayciruo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ctxzqxck.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ebtxhhey.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fpczbwpt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3sjcxcqdk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3unhphrub.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwxocd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ghyxwuup.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gqnoufkk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zowraurz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sedlrbpg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zhzrtivu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tmjpdctn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ukrjjncw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ldqihaba.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eduzxazo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rhoxjnmg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ckeadcvq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wwpwzkwx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3sdxyspwm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yiysmimh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vwrfgqwl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ygkttvcp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lvlaftiz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vsgvuamo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jwzxsbqc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iwkblyst.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xmrjfdet.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iizvfkse.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fsadceqr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mkfsaqla.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mhkoysgf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bpqyrdyv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eednluvt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3rvznovmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wlbpjwev.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ptbnadns.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3icezxlvq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ejtgiocg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lkmuagcu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwpiunap.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3reqoueah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ebsthqdx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jhjqbztb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3lfevetea.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3edlnmnri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wismhknn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qbuucksj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lfmzulfa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dtithnhg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3phdegzbo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3olywsrkt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ubibgiky.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3goakbqyc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3okhbmepr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fxhnbwwi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhlxrsts.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qjiefxkx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rjsonmex.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rbqvgxax.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlubjnsl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ddtudgjn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivgfpffq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wrqcuhey.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ngtizubg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wbyqwdho.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcrenhbn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rcbjvaem.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kxrkdriq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ptqlqfbt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zbrinckd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ehmcjfoi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qpyncmff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yvhngets.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3inatwpjn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ktzoettk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hvsqxldi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rmbtncrz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zkdmbeqx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vveiddhx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3roxxvter.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bevhzcjr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jfdmgadl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lszffizq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3epslgdft.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tllvbxkk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gggxmxqb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3usrdxngl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jmdvesdu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fhfqhpfv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xlmhqigl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ykiboubo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3anpxkoac.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jrumbapl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hskbehol.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tswpgffi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jlhhfqpl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ucqjuogx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qyuditqp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dpuytooq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wndlwgjj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ncjkxivt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ublypqov.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kplxmkqe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ghelyphl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3alcykxmc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mtsnxkph.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vptaylna.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kptdzfdc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pxyjywld.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wouqipcp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hvyqwtfl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jszfqxwp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hmhgudyo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rvqbbwsi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bxbcyhbs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dsvabvvj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3paeuxymq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tkwpeosx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tuerwyrm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3acdwuxyj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nysythhl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iysihcid.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gfoaskpe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fggkcjgj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wxevwgil.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ettylkyw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qnxcwvvd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ecalkodn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3geresaax.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzookeon.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bvsxketg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3blmuunlw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lsnqawyu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ndpegbfc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vsdeaskv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dnlysolr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3porhlbvo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xlcasyxh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3psklqans.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3otaucgce.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jeyosgaa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wovqapui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zgdjargr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kzzrouvk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jactgkhe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3shltvvew.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nicnphrv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3krazlgrv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wlsmibog.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mtggqkbf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ycqpprmx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zeawhaan.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3isllnmbh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zzpuzbem.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bwlmjmsp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3emgzuihv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3iopvxfsg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rwdphimy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qcbxkoag.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gdmeoyin.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bscxyfwx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojbpdcoj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hnimreqk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3sqykqiig.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3svbeagtq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ndwfmnft.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zpweyyal.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ebssxvxb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zbhppknz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3myxuxqgr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dowrbbqw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rzlfjqwz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3eephcrbp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vycwzdyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ttfvzpjq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jdhxhjce.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nrjmryjn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vtfbgmth.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uekwsgrx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlppteql.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhruoxgd.html


<!-- 参考信息 -->