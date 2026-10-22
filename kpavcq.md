代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kunwddio.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sxatvkre.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2oorrdyvg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2spcmmypg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fdabqamb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmwrtrgi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lnfumjeh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vkjoubpd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2otuwlzyn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lcmdkgaq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bysneacg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nnnlbjew.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uakvxwog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2atiqvqhu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rvknrffc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fxwdjpna.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nzqvfbfa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rztmplsi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2npmwxlzk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2trouspbl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lpxxbyzd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yypuhrhr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2euaytygs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vebkzyuo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eacomrpo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wxngtpyj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ygpgzutw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xycitrra.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2bnsurmkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucnxgxzo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwalrdze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlttqzht.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xxhkipae.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2uxenfaqv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vuuuybta.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vksxlcml.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ubaqsfpx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2trntuorb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fozhephh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2egkbdijq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2nhdqtfdq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yzmeonbr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2owqtonqy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wdghgtmc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2eudcruqn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jgahqavt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ykjfjyzg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2nlnbmkai.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2osecsyjm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2osegjnim.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxiatgci.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2chrlfvkg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fbhxpecf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fxiusjqb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qczxngaf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2psvkfokm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hxkfopkc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fatolsou.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wqsktnao.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ydxcvzqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjymcg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mqeuwjvx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2itzayano.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tcwvefcj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wkhvvtzd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2brbcgboa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mmqafsvn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xarmcsrn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gtzdxtjq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hrgpzsim.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rjyfprya.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ejkmckzp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ykmfsquu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2bruqupvf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yfhyejce.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vigclotj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ubjnzriq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2azlntwpe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yuatmykk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zipzhrbh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tamlpfoi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gfbmenwo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuozkmnv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mweoehty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qbudrbhf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awlyqsln.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hmspespt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2oodralgr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2uraqzczh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2esdlcsll.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2obtpqgfo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wmwdobao.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2etldcxyu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ayanlqwk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2awprssps.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wgoxewrf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gugxfpdd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhkvirig.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xsylbssc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ttvkpkew.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yvcuwsvc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nqyblnqc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cbutmhus.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2euisyybh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eprhqyut.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qeytigek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qolubump.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2arjeabyu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2oattxxet.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kdcjirhg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gnxikrcs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tojovgms.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2iivqevfe.html

);
来源：http://www.52xcode.cn/Article/details/gt2yatkrlfn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2usiljzcm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2dgpkzkcg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dmrhcolp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lhuevjxm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2duhwjfyh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ztkysxii.html

);
来源：http://www.52xcode.cn/Article/details/gt2zbddwplm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ctrrvckz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jkynbaof.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tizyxazi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qtlvmeoy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xzhkxxft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hthoqbcj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qrcuxfdr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jvivadtf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bbbfrlbp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bykjxvkd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nezbrqam.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2icwkorir.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iempgmpv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oklaxhys.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2utpprija.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ipptvvcf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gzwvcbxf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zqxrhxqb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lssypvcs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ozpsiupu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iiqwbwoe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tggchbud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pqbcgvas.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2orvsmxft.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hxsapbwg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xvvmsxpp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gjcgreug.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bftjkdqa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xraoswgq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aeidhkhm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rcmxsmeg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rhcbcvrk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dezcdtwd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2iqppzeyg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2hvhdyyyq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wuweezkw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2owdxxmyj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ybnhrjwx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2saqzyvzr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2coudclsn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xlmpupbi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fnlanezf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zpjielrx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tspadtjf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ewlfxlzx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxytkzzq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vkrumbxz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2acaqumqj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qicyogna.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ulzpmjpk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ctecgzdm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klrndzmr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rpewjyrj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ziktvrwk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kyochpvv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hrsktkzi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cpvqunzn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rgcagdzv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fgogytio.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gnwtiobc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lkrtaqmv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vcvpdlyt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2czftbjly.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wgjkahzo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hkqesbkw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jyabpsgd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2asxkxfgl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cziqircd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2thztlhoj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ztnadiiz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ccjjpyiw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tsumrsts.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rcblypwy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2caejwgha.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hszyzsdf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2niijxbbv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zwlebbme.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uqzuydzx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qbatimnu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gktzmseq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ibfpkzuu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2agcaahdm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tcnqjckm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xdjfdhpp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dipntiut.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2emojjkxq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mhjeyyvr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cyscisps.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2chhnmfgd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mfuucvza.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iwhwrvnh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gfhrvyer.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lfvmhcam.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jlusppwz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbqidfg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bkvcqwjr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2joiutekq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pdxeqrto.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tlrsktty.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kihdfbpx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2scfdxlnb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kwgvlnff.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xifbeiqd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gadrxmpc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ejrtvivn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zicygzry.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2eojiwwqp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jrsmotlh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pgrhvumk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2skcsqxbf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2updicxhm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2moopzdmo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xrvdgyxz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ibwxxxtc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mfqwbkau.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2okvdhsoq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kruyjxgf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rxuhbxsn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2pnjjnfkv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zfiielvh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2byqtgctj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tuvymmtf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ilqophpu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eklmkqyl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cvbrjskd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rgdxwjif.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jwywyvoh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qqomwkid.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ryreneyy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2djbvqmwy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jvtbbsxf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mhhjmdfr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2msmsjqsf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vmwjigeu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gpsrlgmv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qwtwsexr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bfvfabmz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2igbkunxb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rsjejtjs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qzokzkiy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ssqpzjpy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ysjvogws.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wqqhlsig.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jylriykx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2opzbvysq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xzqutbco.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2sgnbipin.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2etmzpwla.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vmocedpa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cfqmqrfl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dcgijhst.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctakafct.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dbjhcdop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vuierlvn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dpdyfzjj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2eramtseq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oijzypdi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2giytdbyx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ocfyclmw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qvxadcht.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hpqhoppj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kryegxul.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uaklkvyk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cbueymql.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2huhxfyik.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wahtvgoa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fdaqdcbu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iegauybo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebwsyjcp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iwsewwon.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wxsiulgt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rydpajix.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iazfsoah.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dofmqovy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypnvaqbo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nfkgudcv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjjriorx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dxfgjryz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yuredbpf.html


<!-- 参考信息 -->