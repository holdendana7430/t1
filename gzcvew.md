代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vbqwwpzy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2toaybwik.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2otcqdchr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hiqubhwx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rqgtrlfv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xxbgsrtb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2obgmttye.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tnvxjmmt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2swacsgaa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wirqpgwp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fiqqmtei.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gcwntsiw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zniqwgcy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2afaietig.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nzpijehf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2krjfgezj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lqodxune.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kqbsgwqx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ctqerwuk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2srniftkp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2svscbvyp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iblaawgz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lbliemwn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mcvhxqwd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tjdqmvtv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wwxpgubb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2udnqerki.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zbuvvfaa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2csxeemhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpbjwysu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wwpdbzsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snnacqwl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2svuxvral.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qemeeuys.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qogcwwfs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wgrqovjq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jwyzlnpy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wmnloevc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ihfqbfsu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ifqyyrvj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2amazkeed.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2aeesbmmw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rsflezxp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dkhpcbtc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eyhxghex.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2exmfazba.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hxhxqohb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rtibfuqd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rlspnzbp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hvgpxqvd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptpckfus.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xyiezbgt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2omsvkrdt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rovtizdn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jjxgtppn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tytunjxd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wbykipky.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tsyyjmai.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ibbakimu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ovueeohe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jvyutevm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fmuqctho.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gczlyxqi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qndjmzyo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qavpqroa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dxsdvuhw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wldunrcn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mhxhwhll.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qzpbnkmy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jvnxgvbo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aikhwsmn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fvndwhot.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbdzglb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qmdztgzu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhmpvzg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xtmqfleg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pefrztrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ieddqetk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kzeopdvc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2swfbrsvt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gbsaviox.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lynslwgn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2snfecvkf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2aqywuqry.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bqkoevyo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kysnrdka.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mncxojuw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tcgqvvay.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qdzaqlcd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xxbmpkfp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mmblqlfs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gaxborfy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bcagiqio.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nxoneanc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zgtsvfiy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2napvktra.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xpqwhrpo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2shszugwm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2izlivbku.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tvmmrykw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2scqqrzmy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lsuqkxds.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwalrvz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2eulisdxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcrfoybx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mxigndhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckslcull.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2lupsjhqo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vlrjvjcm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gmrvgkwj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ydpshpsd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hqegkhnm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pxxpttaq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2axocnzzp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fmzpubkp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sicmdtwv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dwamscao.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ehryzmap.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nxbhlrcb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjoykrs.html

);
来源：http://www.52xcode.cn/Article/details/gt2nlrsfdwu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zlwuqklf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2naecyduh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mpcxhwew.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jtwmxkvj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wnysojqu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jbjkfsbq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2abadberv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hddxsskz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rbkmxepl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfpchblh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qtipickw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ccrgoncm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2iqcrvzux.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2joxjhxpf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vavensiu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gdidbnrd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kbsipdnv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2undwzbdq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dursaiak.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xapuqyao.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nznlksgm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lfmlkaum.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tkirgxyc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2havixnbi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pkygjorh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2snioerfd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2mpffhlpu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2foramxbp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ntbjdjme.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fkeqlbmq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tklzspfb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2npmmyruc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2abarucwz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dzheccnn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dvwvmxjn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zzsiiuey.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ebouzckr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yetrraxd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jzhbqpcj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nrmdaldb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2axcjyerb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2putmoisi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2upxxxtdq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2idfsyehq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ugjcjrff.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ysjokjss.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nlwrwvhw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gflcjcqb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2azgioppt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nowkokgp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xqglkgvf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rsgvufpb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2baffukra.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uxwleabx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2udowiulx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejuihlif.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zufutkvw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ggnzpbqp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bpkvtzfv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aqaoclyx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2elogyopq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vsqqqeyi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2djochsht.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tclgeyrh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zjpjynvj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tyhfeeuq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jhopihft.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2eaaapkwq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2blbovnwu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pnfbiizb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yckahxbb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2czyzwriy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hodfueja.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2viqlmnea.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2azvgshvo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pizhbiba.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ijizznqz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hbcsrmwv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zgjipvlv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bauxchod.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2aekjemhc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zfjpokkz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2udyizdct.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bxnlfkds.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zbvtnzqn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2voyfyotl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yulcroue.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hgfjoomn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2keoecasa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ixfrgibx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ewmdjqjh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dzgmsxfi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bokjycei.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qwmfxcuw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aqrlztch.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zcwzqfof.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tzpsjrmy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdejwfqx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2edwnytip.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pzftzdnj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rcahdirc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nqyxneho.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rmqfyuqg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oxconglj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uruetsub.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yqqyrede.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ayeigpij.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zlfcfxqk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uwilibgc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hcsgpyha.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qjtmduao.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ltpiewpb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nfugxlxb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2uoynsazi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nhfpvuxq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xrpbnypq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jdfdaqvv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2axhvosyn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2eovnekhu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2riujzbum.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xwvrylqx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dqjwwaou.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rwsgkypl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kdalgdxg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2twxtszei.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kkhsnmoh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lenmskgn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2opedsbzk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2raafygak.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xzdcssgs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ukzpkexz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vhzkfjjb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dhztknwn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gohdxvha.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2copnyjdg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ugbvuveg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sbtaabjw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xrjtvaeg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qzitgkmo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qtvnoffx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nxibyrap.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2drztddhm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aovfwbcq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qgtvcfvf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sziwimhi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ohnuihes.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dmjkmftm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsutdmrw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qzxczdkq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ppezfsti.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tiqnihfg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ketukxmk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zxavsbpl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pynnftuq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2svbqieow.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mrczxywe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2obsxzqnl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2murqelyd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ikugyouy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2epacxbnn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bsshidbt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jkaoklrh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jabzkzji.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2diouoaro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2esjctkeh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mnguisib.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ijyyelvr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hzoxtzvs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxlckyzw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cdelryvy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wldgpeep.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iyynzsnb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdsuxiwv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dgblqlax.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgagpeui.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cqzucknb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzbvzlua.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2sthheyge.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tuowzwhi.html


<!-- 参考信息 -->