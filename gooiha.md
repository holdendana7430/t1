代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iiyanihf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3neocxbnp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sohwkmnf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yowzsztx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjmfwug.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ynewpjvj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ywhnbujk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kxszzeyv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jhawbwjq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nxeanehb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrcmdnzp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ernqchsf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3auuthmim.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xwcfkaop.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scuwadtl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hdbijhhc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3utjzcjiw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uzlfbynv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3paoulyci.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3utkvhsfg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tgmwcdmz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3epzhrckc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tezsghlz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3eejrztjg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uujismbn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uwowltok.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tvfxvxbh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3erhnrjgy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kgjgbwbf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xtayuriz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3puxidjds.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jsblxzrv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rhhtyxxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qknjuaac.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ejckpysb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iniyyfhk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rzgjfdfp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3szqhauqn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kdowwvos.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hfvgjxex.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3frdmpwmz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gqmdtfdr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wzdgpnyk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ttccpzwa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qmmnuutr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3oubijtwl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zgpeoctx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cmrtlnez.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rdlqyftu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yepqplmt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlygjpx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qvobngks.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fxjlajdx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qjujavsj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkobznlj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3utkoszxz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3slejemcs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ockpzyvx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sakheqmn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmnsgjp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ceiwgijk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iijgnxtr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vrzmlwmf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yiujecjg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3beknunid.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xppfaneh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pqcvhroa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3duzohmui.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rtuwxtsj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ivdqctth.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dxcopfdx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3csvnpoyc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fgmzvtdj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rjjvtpmn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vftoueoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gcnmxasg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jpiygjsp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3twxatqqk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jhipsgid.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3doqezrob.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jfbsmesa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xdwfkahz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fobmbxvu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsxjfchg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vgzzmawo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqsmattg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpwrmowo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vshybkrp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3iwqodezc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrukijph.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3aozbudsf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sfeogrby.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gpvdjeym.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cfvtxfdg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkigwlwh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3usjbsmkm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jehjbyru.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dabktauu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3uienxkto.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hpyaodey.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yezudtpa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vryqmgcn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zrjjqkgf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sccuqjup.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ofrdwyfm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3uufjjgxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sllaljmw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gkdcqvpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afghuhse.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cdqrhqby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqonsrla.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yvulhyap.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dzzynkfh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gkvoiwam.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ucumjczp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wccsfnzk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rhkqzslu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rorpzpph.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wgltikci.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3akkzzjbe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3navjunyj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lcewahey.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3iiurfzkg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdbpvpy.html

);
来源：http://www.52xcode.cn/Article/details/gt3hmibhyzu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3pnhyqfel.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xagomnda.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fwlhumkl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gjcmvtnu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kbipwqvj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3osuobezk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3oivqefik.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3baptqgzh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3akjjvhsm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xwvbagpe.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bwgmzyhe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sinhrxdb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nximomfg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hagbbdph.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wparpjln.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3szhtbzil.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lvyrllog.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nbqckcqm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cawgtswq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fuebxidf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ryjejosf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hnpjhhcu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rhaxlnvj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3psidswyc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3aljsrlox.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mifcucgw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vicdrmct.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yljgveia.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3olljbibo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytlnkzuz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ivbqsybm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwabmfpy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3enretgvn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hhyfvghk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zpdxtejz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nunylyba.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3smjkhiro.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fgjoaclp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3glomdcok.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sipuepjw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3icgodfpb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ouvkjloq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zsgolnen.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lonujglf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3umbzvybt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fziiyttp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dffqorvm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3shoaudgy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3srjnkpbu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3npstwrxq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mnskoafq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bapkrgfk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fyqtwsal.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oikgabaj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bxecriha.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pozqtubd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lysmgrid.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3atywpeze.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3izexadlb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iiawwfhd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydaqvjsa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rwbcmsig.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rnsdwxwg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hhevewtt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lfepsbqg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jannkuwl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3weggqaxy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tbumlhqn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3supxkzzn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zicftqol.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rgwiazji.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wxvtwagh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xhkthrvw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yobfrpbw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hkwuvwnb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3afnduwcz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gqffxmxf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eenfxjun.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jiympgfi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xuzsknjq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fhoptfkd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qmujtujk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3thpurihj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3opeovpmt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wvacczgc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iegacyth.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yyvqddsm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fjdnrwxo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ecbzwwiq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jcdsmzlt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3egzkplau.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tghfygkp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vkgstxaw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3aysnkmis.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ajoqwrif.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hktngqia.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tkuhhqvi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hcnbjyxn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xmfstbcz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dlogrmdq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3tyqvevbl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ahiddnre.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bjtdzrah.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xmezsnvr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3obehiazr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fxomiizp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hiapmwyy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3usmbjtgf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3aedbbmle.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wsbmxkdm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3oqivcmqx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pmpjjpov.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qcoenynj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wdqgwgbn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3egoqmqyc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eikwmrif.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ppngofut.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ajlkkcsq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jurpqhik.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aafczuyq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yymwuvof.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tpgegrce.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3sfabzndf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aptewdan.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3likfuwee.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kspssorm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nfvcbrir.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lzyyqjay.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pkbokwjl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3mqfhonkl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3srcelinf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ewsdiwbc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3niqqddgn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zddjwxxv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lrmbvgmk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3giwuwpgy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zadpltfl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jgpppmpf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yoinrrzr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3thsibzih.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qzpsppyq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kbrvjgjn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3whliutck.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nhoxhplr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3eiuofycq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tgbmarpc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3uqguzlxp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rcvrrhhx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rtidbwod.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wytpphnw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xoywoftn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mcjvtmqg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hgbmidwh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ahubtvse.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3stmbpjqi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dbfivsry.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cglxitdn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xyjizqbb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3aislnoti.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vfwzyksu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kguuangp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tblrekwj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yywotywk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3huheogjj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bclrhtjp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3arxsbmek.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yyfarpwo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3eidmwaqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjpitmbd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3otyvskie.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnkzfcnq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qwxjbfws.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezyhfbqs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oqqijcws.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uiszojyq.html


<!-- 参考信息 -->