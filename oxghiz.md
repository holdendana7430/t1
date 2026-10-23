代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbgefhtl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvmwgyhr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3brompndz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3oicqsmdn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bqhiazzb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3psgrhwhb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tgltjzxd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3puqwsmze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qcqrcipt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lazarejz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3edhvtxds.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vyeyrrsa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvypnu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xnctxozv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yynozxra.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxahazu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jhgeuyvz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vpaywlzb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ngzgytnd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bgyezxsa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qbedoibz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3mpjtujcf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gelejrnb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3etqzvdos.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ailaqxwa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3smzhvpgy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ericvgsc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3keqrkktl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gpusaipg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyfevkdn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jcfhzhim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaslvnwg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zvqpapux.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3udduesnh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ungxaqhv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lkxhmdnq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3klundqzf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eaaoujgi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qkyuqqhi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cjbmobif.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ufepiefa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gmkmnsel.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kagolxya.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3oeeeyyrt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3annsntkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gquoflpe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jmlwrvsm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3padyfwqr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjdalqbc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nvthhzzw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lyfpjqld.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wtfwaxuq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lrnmcham.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xxdpjaeu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3olmdlwtq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3upviqoho.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dshzgeac.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qasdbtyl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nljhyjub.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lfgbqtwv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3odelhhkf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jtcqithw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ofrykdgp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xbfpuibp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pppzrzbu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ddeyhjox.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dcnqnrgj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xwblzwfi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ljfviozg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vafmmauc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nrkdbmcd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3phjuuupk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3grnekhsb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gnefztzy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yfrzjxzs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hcqeargp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3gelyzrmd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xpytchyw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hcmznlky.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxfdgfig.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qheszumn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyncqqqp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvvaizng.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpcrmszg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gnkmihsy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krmugdny.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ehgjziir.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3adasgdhs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pnfjjvxb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3odlxqufw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3taljrlzz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpwlfysw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tdxeohcp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jbkwkrbe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qhrtatjx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ducunmqy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qhpvctlb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3uyrspcak.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hyimrhni.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ijmryibc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ukapskqc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kkvbmysi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tmhsalgz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lzevcmfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsorzidd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3divzeyaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iitfvfvu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3oyxsvcer.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3onpwxxdj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3eeqkptjs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sxcaiwek.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3unbfqpfg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3iopxnvjw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bnaflvjl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3cvvxrcnt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zdxxezlk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ubiuqnyg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3naneuwzj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gksqpfga.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xwqdnewl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ibsbvyzl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ayqzmrfm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3msdehsqu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3kodrpqeq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kaylifqz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3iprluyrd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3amrpqjyb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dalfxlex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3awkgdusu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cvymsquh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cdbyagbh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cgwxtjcn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ovubbmrz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3brbtijwx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ggcadqes.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3klwkwfli.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gkunjhqj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mlocbilj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3aionyixw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ubecbonj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uqrrhtve.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qhthcvyv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3iznxbhcf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dygbiqoa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dsfiotyr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3pgsfgupn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tcvifthh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zebjbzth.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btrmojzt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mwlxlfnt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmrxmpuh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xkfndcvh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xqeazljf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lwxctdll.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3exujcixe.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mwfqwafs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rauncpvj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mgiyfgoz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqktxkv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zvzqxjhp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fplnivkt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xnqwmkbl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3moarafvi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3obtodzvh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wpcoemfe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oxlpavec.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gumkkyie.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3crayfxur.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nkkuffse.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3dzhcidpr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oyzmglpm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cnaustbl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lahqiqfh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sshuwshz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3irjusjsl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3agxnfanm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aiqtmcbj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xrfluppt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rgcrtlun.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3afsejkxe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3abxmfeae.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpuwiwlf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jsvfpfqo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ebxrhdjm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ziagmxyf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xmbguvkz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qbropgvh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ixlzzzfp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kmsoscrm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3viezxawf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jbwjhsvm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pupbcmmq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yysuxodk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fsfrjgzu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pmmqcuiu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3htkdtsgb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3czxzeuku.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3llemhmkf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fqjjggfc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3folrmsmn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bnvtdouu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nyrzhrms.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gutzwllr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qqkmzepy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ulfmojdb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3poygnbot.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qpuclwdq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pxyjxrub.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3txncxuyp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3loeoyivk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ovpgmvcs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kzarrwpe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rafiisde.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wevoqfdm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pcdorbil.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mwunomsm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fjfpmues.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hjeosfne.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3plvuccsi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hqwdjiuj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zsxnvvlm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nocdxxyl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xfroijyy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uyuaclka.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sdgpjnnz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nmiwccie.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kjvopgsk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xpclvufm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rzkrrsxn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3risdyglu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ruokerdm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vhnleyzq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3snghcvue.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wlveotze.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ccoczjsy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rrcjaztm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wqgvcavm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rindisuf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bwvcoqrc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fjrljwae.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixmutmec.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jvruhjrs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rtvqzudf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kjozxiwy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oyedypzd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3sgecenyu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3cxiobcyn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3leugmyho.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gmfuurmz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fqbkdxsj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yxzzfgxx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hfbzypsd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wauowysm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hgqfywxt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mtwbjuwv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3numetxoj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3libxuyrm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hnzvyfgg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ivulrrmm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rpdgatsm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bdlsxmgd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3idqiyshc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rdxgppml.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3welzxwyl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cekkmvih.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qhgmmtwv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jdtlvbcn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yihvrgxk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dbcqpsmx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yytbebom.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vtoladxp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ebgiqlak.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fqxslyuk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3crubtyvw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sufqymro.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bxknxzac.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rolytkub.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yawtfzyx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nvtvewqw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mgdigfgb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qkddfayy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ctzbkyrr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3snkksqmk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dlsunhkm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nziuqnex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lemqlgyg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qfmdnrrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3guvzudht.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mideuied.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubbejhpo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3orzndfsy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfgchtaj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mbczkedk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kqajckas.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gwuhwnus.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqaxnkhh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sskqvnvm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3txdhmvme.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3natrkkqz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3enetnfij.html


<!-- 参考信息 -->