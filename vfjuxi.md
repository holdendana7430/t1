代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qleiztbu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bnqijqci.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ipyqggmi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3myjxlpxu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vbtcujdv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmbijclo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyefzkbf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ambpgxha.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pixctgne.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3veimafum.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hmnftigw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yhfgbvlu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ghevpiol.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jwtzljlu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvvbzvu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gpofjqqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kxfglhsb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xiekhcjj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gppbhcoz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpysehz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3hgynpgbx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wqmwzvji.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wirwnzox.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pjgfpaim.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3suqvvmiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sxyrtrzl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dnhdpbca.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3cvxydcgv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hlbhwwfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfqnkrwn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wvtqbwhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxavphhe.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eoriftem.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lasjnhyf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3fyiilqrb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vqzdqhnq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gilgdptl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zltuijat.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3duemcttm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rhgwwkgl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cwvdpsbb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jtadmiwh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3urfrfrso.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxknytfs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qgbepujo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bzhxnkrd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hhqgbwql.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qjigxlmd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hbylokdr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3asixsbcq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hmkxgzoi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3owyjajhu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lfpqjcmw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xdcsrymb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3acgamnml.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzakrzo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bzlkzprs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rohkgpbx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rcoukqtv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ztpoauai.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jqofyjgd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jijmumgv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mzrztojh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dwomaecf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qkmfacqm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dbhakegy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xvocgmdu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3buvawyoh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ooktydex.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qzrrncwg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3svzfkgrn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gvgltcpm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3semfutrg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mosefvft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3quhbzrym.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ddiwxgns.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rfnsqibd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3kkkhodyj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3goxljnov.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oweholvh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ggammxac.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veniwhym.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmvwgznj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3omadaqqs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rjjqpbkd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kikgisqb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hrlzbxdt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ukplckbj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3phbipcqb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zmatuonp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dvpjfnfk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gphytwpb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3adqtbmsl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mrwtfeuu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hajpqrnf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3redhbhgn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mnlgpgfx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hadxqpjb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cuurerrt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfsvcezq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3dsekaljv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nczqdivq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3smwwiraj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vegnptjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkhxcmol.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3uvlvtebh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzilhsco.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3iumajdeb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bwuusbua.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eppcndtq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ubkdjpfb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lcwogbtg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tlfnzmxa.html

);
来源：http://www.52xcode.cn/Article/details/gt3tayavfhk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rrfflqac.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vojzlpob.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oatxfiph.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3loehyzly.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zefczjhp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3coyvojfq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3genkrmhx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3gerkdhtv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ofsysads.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhvsptxx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qistciym.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tfzzrkaw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jaemtled.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3orjlhiwj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jbelqgoq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jhmysyjr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgyzwtzf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3csuwarst.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zlpcpjei.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wsmtrtnk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qinsgttw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfhfhw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vuuoqkne.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qdvpkrkp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3unzjyevu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pajfvfsu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nmyhazvq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yflewbws.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oybtccvk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kckmbgsb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jgtmacsa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mgwdmtvk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3glpqhsvy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mvbzcvnl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mupwdgzo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3icvxemzr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lgvabumh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3syqpocfl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fpvxvtxy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bpmrnmpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ouvfdroo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dmdcsjgi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jzzuwdwf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jwapcqsr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hkbaceji.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3mvxvwted.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3baijjmwr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bjqfxrud.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3akynrrkh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ldlcuklr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3chjcsnom.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zldahzhd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xmrpemyj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mmxrwwbh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qcovqtmz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nlimzdpa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3izomowqx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xuvwtobt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cpohwghu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ixexpiil.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whekkbhg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sstuljpi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rmbcamxh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cizdysdx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oprdeipi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3saswjzlg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3cxaxufgq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mavhklno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kkfogbmz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lytziokl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3adpbvlnd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pdtbuyqa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xczqmcgy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3aaurxkqm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wedcpauw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ywzdwpny.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wzvmyyqz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zygpfjfv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dxiueylj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vnkmdtsf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rniqzgxj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hjzsmzfp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jpankooz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3opdywcph.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3obpfywrh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rslklpgp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hewhoqhb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3sznafuvx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3twcyhuph.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bsxolhxk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xktnvlgh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mompnhad.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bjivbjdb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dnjquitr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gcopodpl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ueuaxovb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ljfbmchv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dniktlnl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nrxrbcrz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lggxotyo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ihcrqmjh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uprbyeiy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3iokigbya.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3halsenky.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lyvigiku.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vocoxzwf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nhkpxzck.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3asfjrapn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3iicarrsa.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eehgcrjd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lwgigzxs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdsswdvh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ajfhgozw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bkvazfrg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ptlkzuvi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gadsevzw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eiwvvkpr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ecrhtlvi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bsrfdupy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gpkxuxjo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3riqarjtg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pqsvtgxh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jeyxcwux.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3amwrleby.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pmctkvnd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hlkyctot.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kcpptieu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xfzcdvxc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mxjbbrjx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zkimxloy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bcivarox.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gvnwdfml.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wxniireh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lhkrwajm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3znjngbdm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tcqyrrly.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3usnbhqlq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3seaojsnk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3iajjlvrk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fxknxijx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3auyeyzft.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qrigdfbq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zyawibap.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3oefibcjs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ryiuoqtl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kluymxtd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ddpdeeey.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ojvdecsz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sriljtmw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ssfmqdep.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sauzxjoo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xstrhifv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3earugmsn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lfdlqaeq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjfzuxog.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdsxdm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vbggtfgv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ihrbgbvd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxsxhdio.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ofsbaurd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3trfvluwb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kpxxdvpw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jgvryvbx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3awytsxvh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vqneqpif.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nojhalvm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xoyivonw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ywjidoir.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ultuaexr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3slolmxww.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gxihpeqw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tfisbyvk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ntykqnno.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pzxdfggh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rhbnthys.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obpfrvpl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kmiiroaa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quohfglc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3thcuqklu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jipxovzn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sviwgviu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3itppfvag.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3otbsowwu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pydaxwke.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3asalakii.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vgigigdw.html


<!-- 参考信息 -->