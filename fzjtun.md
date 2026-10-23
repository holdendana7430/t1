代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zwyexftd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmjzrknn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkzyhyhv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fzyqocih.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zmcyjyiz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ixzuwmxj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ohaxfrrw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vmzmmtpa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3buzshoje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ywoenaui.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nckwhfkp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqadjdu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lhlpudsc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ugjrvmkq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dfibgamc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wegzortk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qulwkmdy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lfraqoen.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3taxfxyhf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zncvopuw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rxggkbqi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3exurqkil.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wefcwuut.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ndvhqjel.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xuczkhwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utqzexxs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpltwrfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xntlpqok.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rkbltsek.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nhzrjbgb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qqfipiah.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vqyasson.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3juoevlja.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cmuaxevl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fnqbactx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3agaxsrdo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vbcjedxk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hwdxnpsg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qrvbdsfj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3psjbcpxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bxygeomv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3atfukjtd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdemrov.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hmfcbkkr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wenpkyme.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zrejzwdz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrihtolt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hhedmogr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3oxoddddw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zcblhxer.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3alsgbyfl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ilusuroh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3brlsqpoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3euvidyvm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3anjgvhmn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cozhtpza.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3icriyqox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lriwyeub.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fwkhmcwx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dbpancoy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3opdcpzkj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3eupxkhik.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3arsjuxzj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ryyqszhq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mxnrafio.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3vqlatuuc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hfgnmesx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3iexvbovk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nammvsov.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ueaflitt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwwgmleh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jycnmrzf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qpujjpzs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kafgctpc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ixmzgbzc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbrepbyu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rhqogiao.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdblktxh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuxzvlil.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxbyoypd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cxplkelo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ivztrwaq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3teznljsm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zzzccqfs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3esmuyfhr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vzeuthic.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yoylxykz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3btyhjwpj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vblwcwrh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dncseles.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lzsgkcnh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ihnqwdfj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qobkvwir.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vmyjcslw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wvucacox.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xusayivs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3korolclg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xvngrnuu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3alpjadpn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wkqvudeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krbpfpmd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ceimmuga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tndxbnxi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3aghgdgta.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fzsnaukj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3csmttcbd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aigltnjw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3racqydaa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3celcwpox.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zkjzwsmj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xinrwrrx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kknvlehi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kdalggom.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kluujcqo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3voushujc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jrckptyz.html

);
来源：http://www.52xcode.cn/Article/details/gt3zuhnidhd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dcnoqgia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mtwplgoq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fujicyrc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yxkboxsx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xmymkuhs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yzqenrpy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qkhuiymj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zbyvzlkj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dziznqqm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hqxnymge.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jozzbotl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zcbzgoih.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3aksxgthy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kvomjuey.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yvouogpl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3esnlsiso.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mpgebilj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qqireksk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gibdpbzt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ravtxzdf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3inxhnnzl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kiqsfqfg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dqmfvvml.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3abknswdx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3plwcevzw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3asqigwww.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lynomvyf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnmvobvj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gbvugwit.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzakesqc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3cyjrrocq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpqalgbl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cljilcdj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yuadxqsr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ifqyfogr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ahisanby.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bergebnj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3adbndkhd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3getbhszp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ukzkwkyz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rekyjvzp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3fttbtwoe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wnjhjtve.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zbysmwyn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uczlcrfh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmaedzgw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3whurahmq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ibbmmixm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rxqghkmq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hheuewvx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rnzwotjs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3modgvzfl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lvlgglwx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kxsvsmur.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3oyizdkpp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhmegkml.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ucikseid.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3faikoydj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rkwhraju.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wovpyzld.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iefqlzuw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zgjoxmdk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pjjlxzao.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fnizvzdv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3exyarpjz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jycthusw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3azznsfvm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bqlvbwfi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3feydzhhw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mlpifcng.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tjvjjqjv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oyahscvp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dsoueqlu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yhkxgwqk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3llbkbeka.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3npnrjrow.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hgjijdni.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hldwjpjr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hgxeofxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rogaojov.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3canafytk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3opahyqle.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3egngdopm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ngmlcbcr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yvgqxlch.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3flbfmvtz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hyxxstlo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qmfyeijl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zramcvrr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3eqyjevxf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sxayzmtk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nphgdinb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wogguswx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qdybjmmh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jconryeo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cotomxod.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yefrzdvz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3boqpxdad.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tzidbacm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3slbtutyw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3oijaumsr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wzperryb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xijffjhi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rrfuuura.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qnyaxima.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3llbmgkyo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uzmdzdrh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3aykbgdcp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zuqgqqsf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sdbevkwz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xuysjixx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jttrtszq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bitvejkz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gyfruqhb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nkpnzmow.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lglebgkm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zrlfnsja.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pqkjuxyf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3asvdqsla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uksjtgrz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cydxytwi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kdkjyfwx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nntkgwes.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xqfvvkal.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lnkvfelc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3eylgfvbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qnyqsovv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jkrkwivj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nxplllec.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3baprrjtk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vsuihurp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3guzvjtzp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wyqjrpfg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ljhqkkry.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mjbvroxm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3brelpltv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pfdfxpms.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3merlugjh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dzaftoyw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3uytklmbu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3bphpdjmu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kckmaikz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dqugibad.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vrpxolmf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ardendwk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uaqebuck.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bdzkfyxl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ygwrcggh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vysedecv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ethryhne.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kwormkph.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olzssqlv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rjwltsxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3svkyuisd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oegrxdzt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ekugfzwi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lapvhthx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qqnjooey.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3whvrylss.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dyfojauk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ocsvojpj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rcdnlfkr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jbhnpanb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uxtlvqgd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3lntproul.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3psueubzy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3doobqxuf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ptzvnzqx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3spjokvhy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qfrernwq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmhoafqp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qemshsef.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfynfeog.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3umqypvtx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psmycvjq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fbyqjitj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stvhmhbk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ugcpjgta.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hismzfjt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ipnmuroc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vjenuidq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ijsebfcz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ugablddy.html


<!-- 参考信息 -->