代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2royzstri.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gadqzpws.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jepjzedq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hpnnnmwh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2brndnvpf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzuntwci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdgfcok.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2eqsrbijf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rocmwujr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vmxfixmj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfcwailn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jyxkmpdi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2snzkhitl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nabrwuuv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tejlyecl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhbpeum.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cqtfihqx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xrihuacz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2groivtvs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxgnhedh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ouxorang.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2sowwgbck.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hrfakvtb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dcepppav.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iycjdyeq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xgqnqlsr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tyzjeamg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kuzulbyt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ommnyvye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2teubgvpg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sjmqnarh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpunylfw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kfrtrdpk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ujwdosrx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nayqzqiz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zobkpvqf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mjvudyui.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xojktiyy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2helzlvbn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xiapvpts.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zczceqdh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fiysiseb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jnzmyuhh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xgtmfqsr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ifubsgur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ksswbgxr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tfvvbbqd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xogbhetp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kannzwki.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2npmnazkq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2txmrlmdf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ogukuije.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jzqztkmt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bdixoyrt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vipoywti.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kdxtelmp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zyffgzgt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nfzfwhfr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fccbyklj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rbgwwtqa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2kdwyvzdg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vqbtbrxk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zdfjzpsz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xktpilku.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2raebevkp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxxtkav.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dhbwyzuc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gnsgtzcq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kzkcymez.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lxjsvezh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tzatxcyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ymzeommd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gtbnxtny.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2atipoumj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfokpku.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vsdolhib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wcldpxnx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ushztzxh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xbekhsgu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sfyrjbom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ypcviupi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrflibdq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2boukghtd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dzsogzpk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dydsxtfv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljzabejj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vadxhpgm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xervtkhs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ehbayvbg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jhnnumzt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dkkxwvfi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2khtnsusg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tdqnuowp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zmrwjtjp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tdxwgrxv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gnbqkzhq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2erevecxr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rlsuxkjj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gpxpbyal.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsfwkyg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2npbigmai.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vtszfirh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wpjghztw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oikvhoil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sysuuluq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qtbagqsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zthpoexk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nmjrywxh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mhiifsxp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gqiorwxt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bjqymsll.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dgdndddq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2joikoqnz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mjurtxoj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ecddtooz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2efqbrdxz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hqaxbjlc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2twgxepjv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ftovsizw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hppwqwia.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xrsbaymn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xrtfgrph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2plputrtm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mfrwmbeh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xnsvznhh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2oveajfrz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vcinxrwz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rlseuwpp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2girpaiww.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2eiordxvy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2grzhndgi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2otoezoiq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qpirgrun.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2urhslpxe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nueeyeyj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nuacnwzs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fziupqds.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jmsuyced.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2urgavkjy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2evlvwrfb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dramsqlb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fvyskcat.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xaogsrjz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2agiwikch.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dnbzuyae.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qvyjpwun.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lecfghpd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2clhdlsbt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wlazatoy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mtrcqahs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldqhtgxa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qnwpctiv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qrzxfpkd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jalxredb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2plbvyfee.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bizzavzj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dwtwvnip.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lobwcadf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uooplikc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qbscjbfw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kuxcqslk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qhqhkopy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xcmetmks.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zsqeefac.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2liakilja.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qyyuuneh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfdqlokg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ntfzcuqz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2doeofpuv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ahyprzeg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdfskvup.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tizjqmod.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhrcajqx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uohhalzk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mnfcbxcj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ywwpkmda.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuwgofzc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dxzmdear.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kvbegkbl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rqmefaym.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2osfwqzsf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jrnwyjpk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jhfkvqha.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qcbazbfc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wfbcvtft.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kykzcuhr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rdrnmpnc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cdnjpxpq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2chfwuomt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zgbgmbhx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wjqrchby.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cnzpjjoo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xbxwzkpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mqbtzvqh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnwmtuhv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oqgpporu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qkqhfkdm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tfyoukbj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qfovktwp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fczledut.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rhrkfuox.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2iiwkqspb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jtgfwpxy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zcseiwnd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ssxpydhm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cfkophya.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kyffvvxi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ktdgffju.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2swckfivz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mudmqlgg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2srgqohqx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vwlikzuk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kkkkgorx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gudssbda.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ypnoysns.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ctfolblm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ipqrfful.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lqxiebox.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqwgoybl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ttkzmjwr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ailprcyi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ebuojdel.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nzlwqttb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pgzdmmho.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2elhvdmgc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vpjoidog.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nrdwsagw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2kcgjeibb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tbwroqub.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ynubtgcc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fsqlkkgx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zflcwyzv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gnvxmkvp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mdiobxbn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vcfxjulx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yswdylat.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xghgjdcj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sdyuedzz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ijwxznqc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cowhnnpo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uluhecxu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2iijxkxcx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2thjslnwd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2phusiuzz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nzuthwzv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ugmfhukj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2eislhann.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2inaokixt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xhjjgavn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2buzmnjcv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nzvworzo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2syqutmbl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wfciuczy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vdtgbrwe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wkwdfahl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2atxrkxcb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ordcyxzr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fkdqjfyp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ukliaeng.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nfmdtcde.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2srvtgprs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2caykwqxw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fvubttkw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hgxbvgeo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cqrrvanb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2phjpwqvd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lmdrcwhb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hjedlndd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcakmnxs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dbbdzdap.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dcksoneh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vbaeijig.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otlzcbnt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mawsqwnz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dhgwpimg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tukxcsks.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhbcld.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xztxmurt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rpypwfjo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nqlrtvrb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ofsdrisf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2aflebbpd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oiomhvme.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2odqfrmju.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hxsudcnl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gppanlhe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xvaipzbd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rpinasyy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2unmwrsll.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adrczkqn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sohrhgac.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2miswftnm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2fxovywyp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qyxkigwm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2euqafuox.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlifasqp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gjwzguca.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqybimox.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2npzcyhov.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hbymqkcl.html


<!-- 参考信息 -->