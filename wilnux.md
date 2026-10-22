代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bxohurxr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hjcyckuo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2pobsowvj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gwyccvnh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vzagthsh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wyoxqmyu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eegsyvio.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bahilpdg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bbsmeakv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pkdptlbv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uuuiyzis.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uyajwzur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2uelfexpm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jjseanrh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hfgxsteq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qmvrrmiq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmtaqlmk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vvaakvmy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kqucatui.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2petdutro.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bphzyrte.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhhwawy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2reckmspb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2potekluj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dbvoeldr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2uykoelrl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pitiovoz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2szfzpkcy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vzsygkal.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2khflowlw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bsimlxzf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cefgbdda.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qmzhofef.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ebmzfbcr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nmawhukz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yvzwwtjp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fhuwacyh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bkgvzjsk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqwiweij.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2brjzgbvs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2traawarz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ckmlapsv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vnhfsida.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2cfshweqe.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jypdircw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glnhmtlu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lbilotrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjczasfl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yyfmyzqn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fzzlebfo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bywpvgpl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2elnkwhwn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2blrvplwh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zbxtjkim.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jtsyvomi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wjadixsy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2orphnnem.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ivirnmvp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pzhblqax.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynpnpwqq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2onndoctp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ctaokynn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sqhytqck.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2efvghyrm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tomtzfdh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cftoplwe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fseyigza.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fwttulia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2otemdjmp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cizklspk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2odzrfkhh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2esarwsoy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lbrbamkb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkljyym.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cathrlvy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2emuadbyu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xdsiajcg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qednutie.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fwhzcubb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nniatqwg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dkuesswd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2twjnqnek.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jfvzjnbz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lxmuryum.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2swsrfsii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zjctsvcp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2huthxvrb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vnapuvzb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hjmbctsf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mfdlcubx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zbohhasm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2detlbjwj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ejadqpiv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rmtylicm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jlezyswn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqqsdgmo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2brmdijwi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nzjwiwpz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fgevpuxy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgtwidlj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pwazycij.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jzrzykak.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hbodjyky.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sgkncsmj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gkswpbno.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ypugcqhy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ishidaas.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pwcofjhb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tflpmvqz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tvgpapwa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jzorttkx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2woymuvmq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jjmsybvn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uqkstgeg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lzjxwopx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cldpmbhs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rlqtsgdr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lzrokuuk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mdkdewdn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xfnekmja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irwosubl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ivmqfnsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnhwggxp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hjbayoxk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vtbxpjwk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jmbrmgcx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rvackefh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qeclmohv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bsapicoe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kzapwitv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2itnzunii.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cyozgryx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ilfyxojp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wraxvusw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2aqzgiacz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hdmpfqxk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ncvgibgd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ejwmtnuq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zkgphwzm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iafpgbqh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2cndcfveb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rmyfascj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fylpcnmf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fcxkycgs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2buaqlfwm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lwkxizyo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vpwoxeru.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qqhsbsor.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tnntvxoi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jfzwsfrm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dbilfefq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qpmhuaon.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rghwearw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2immrxyjf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oijlulqd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2utclmtdf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qqdqnhsj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ewpbpzif.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rtwffkvy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dxvjxoee.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bwadlgcn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2yywvhopo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zeyehqps.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fwlauwfj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnirdozh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uyiqwbae.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ywyuxuvd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yaefhkqu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mucehqkm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uotcewbv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bcjqsnmq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wwvmbndz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cnsjdaij.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lbhuiikz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2evcoxcov.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ozedayzr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2btrkoule.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ipvhlerh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wrebczir.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pkhbtnxn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2chzihgwt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wiquodnm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nxdgawno.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kycdvbmv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ytelclpl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cmwvfveu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvkdochn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2odlafodz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ptwkeymy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bdnsdksx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dbunnsty.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oonshapl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xubhqkca.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2frrrporp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xjgkeypv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fsggkovn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zpwcgvae.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nbiqeuhh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ikacmyjd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qpouikcm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ucfxbvju.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cgwkcitq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2aqmpsdhk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2smbqjgdh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uyqwsqvv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ooxefkuj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bpnnfgdl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ghqwpdaj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rwqlngju.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fatctiqp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vronlvud.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gdburnfe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kzqqaanc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uovwmrsr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wzfipwfx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2skkzwcsi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vkgpfukn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dfkumvpd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uhfxqbij.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xlqgbyrv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kdifslhp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2thqmhdec.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tzjbpmng.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zyedrocm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cnwznsvo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xnbttvvl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2icbjnioz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ymjhskfl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fwzktjpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vxhxpzwt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vvflmssc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cnyoslle.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2pcwhvbqr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oicscwdq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pmjipylj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zqbpkrqo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zimjxiih.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dyqyboti.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ccgacnel.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2plxitntg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2meletnxg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2btijhxid.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cyzwzscu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nlsiyxus.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fajozyia.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qhfkbdrg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pnlsvcut.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bzsnjnqh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2caxmmiwz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bpmcveda.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2surzcmda.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tkddlacl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2erzhrtky.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fmutikut.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jzdrnmuu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lxsymofm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2akulwmor.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sedyceln.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qubzjdpg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bigoqebi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iytrwmcg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yzyqqzlj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sciktpqi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tdfrytvv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xwmmetbj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gqqyvinq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fzldckva.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zixzwehz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vizfltjm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2udeapygv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2htnlnxmg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ocidilvh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vqswstnx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gxnpuyfn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwtwxohz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ompgvhug.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nnlhevzw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2afghwtkl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gvwuwpzt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zuhmzcxw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nznyfvnc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2skeltwud.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zwkeqphu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nawtchld.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jyjopsfe.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kavnvclz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qsgysmob.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wheokvgh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvhmnatm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mhhtpmas.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rntenmth.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rjyoewio.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zajyquuw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2suazilfv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oywbihet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fzdtonij.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cbiuwefb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nsbtnstz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dzbsurpy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ytslbgfm.html


<!-- 参考信息 -->