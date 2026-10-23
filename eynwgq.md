代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxmesrby.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrlmmgbf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jwyobvms.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3icxljlpf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tcbxqcor.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pjgutazm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohnoyjlc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xfxxcqmo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sinhlxnh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ypbxuids.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gqskludg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wnxolqdb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3itesqpxr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmfhay.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ipcfdspc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dnatfsip.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3brtfuxgw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rtqwzxym.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nqzumwvi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3sgmctibh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nyklverb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nsabalar.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3odetrkii.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dsenhlzy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jkuozwyt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kaoytbll.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cwcyhjsn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzmbqy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hoombcfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjbajsbi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cevhzstf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghqmgzkj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xshnsrry.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bheqgjaj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nmzlcrgs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bsuljnez.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3agcqicif.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hruswayq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yculayen.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ssguanoe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ihcbsszt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pnipdsse.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yweukhni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlcagdhw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3abtovjbi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3htjhetqi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3clbeqlit.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pjvuglel.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lydkeesd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3thlrigpu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsqkjydw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3brkiuasx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gacxbtzl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ahkrnoef.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kjklhwwa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3orbhlmkn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qgjirjat.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zafwooob.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wyikqpxu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3psmdnqbg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wwsqngvk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sviewdlo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dmxknuiw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kqzxryic.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fsluzbpv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ullzpkxb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ysvrlwre.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ftruwpxt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3opkhyyrb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3btakcmjb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dgcwcank.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pztfdclf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fkcrsehx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3azjyxrlq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gpfnklqr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3crvuzxwh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3inrkvrtp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wokglcjz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ldpypgcj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxdnznht.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bkdruxcf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehupmxoz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogcofvfx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jmxkgbxz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3sgasloms.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3sxsmqhrh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wmvmwlzs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ptxrvmgy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nbkwqzrc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yvudibrm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zwsnkvkt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsbfqaxj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ueleixpt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rksfshqe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3llutlxjh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3boigjerf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhzgnsk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vcgsvqwf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iuonujbx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3trxjcybu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wswuqyme.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tnmhitdx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wassharw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kjruhykf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdviommp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jqslvyse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edrtkzkp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3geizryip.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ydizcctg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ysdrydwi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yhhvpyvo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rbtxiucl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bbktbjpb.html

);
来源：http://www.52xcode.cn/Article/details/gt3attfbhvh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hesjsbqe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rvvpkkpn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3skdqthdf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hmvxrggg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3acsjdxmn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wytvudst.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3derjfwzz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ijzdtbxf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ykchbmzj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3duhuwahk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cyuucefb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wxuobycy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3oqijpkfb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dievvouw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ooyiarpg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkpzrz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3atremzcs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cbtndxsq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3icetmccg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3sblurqfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3savukghm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kbhbwngh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zfexpzkn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bgvvxjqu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xlwpmrhy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3valayfav.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3iodjqkbl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3edodtnhc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vfnipeco.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3btwqefcn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3rhcdhtjg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wswqstwc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3febbgcyl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hmffzdie.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wlvygyom.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jmjhtkjl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wfobxyhc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ydpzlgah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3uwurhfsf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3yicklbwy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3scsozkwr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lzrxlqto.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3emwxrzic.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ozzhvrfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ptpqhkyi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uxrrebre.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hkheiixe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qfeiknnx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3uibjtewb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ocavueli.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yigxgiwp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nqdyonjq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cajamjji.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jfqehxlq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tbakrelo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3gzfdhsle.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjbykzpc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cqdbkliz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3odyayaiq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3skrdanoj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tswvdrxs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kysjrhhe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tuqlzmjh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bbakyzon.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lwumfcjv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rqrfpvic.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jkcxuhot.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cqzdfesh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3imhuovpr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qbvgnfjv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mgwqkmjq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3olzxfodf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nyfdrhrn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3aqigvcfq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pdhhbfxm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xtkyovnk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bupvejfu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3heqqztrg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxaeuxmu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cwbvcixl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dsuosfcn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3imrkrnlq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ltxdjdmj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lasjcxqx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hxlnigec.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xwgnjzqq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xuufubxu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fwaqpyby.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dpvzlzew.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ibzjzbqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3klcgmuhz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rivljxyo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jmfeoxbu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3awyvioew.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ahubhpfp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wgshgipl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3awsoqpkk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cgnxbzya.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qvecttvi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qnrnvvii.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gvsjbnir.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ycbsgiqx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pphfylae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xgbcrcdn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3oavhiqwy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfaizjr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3evaehwxx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hhbyaaab.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ysyyjwwr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ffkchgzl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kfujkhoj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sgsvmxef.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mrjygaah.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jsrkfzca.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vgmfqjfh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3imepcdoh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iilgztnl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3frjvwbwu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3piebhxrc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bhlkkows.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zjshobwp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lziwmvip.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nivyichf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qrjodnjy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vhoduckx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nvxildki.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awpbnnck.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zjwcolsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lafogvwc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3agugehos.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vuebrlvf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gfopvcwn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3saubrwpc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dmwxtjvo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mmilllcb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fnfwdnua.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nzxpgevm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pwrsniau.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tnmfglpp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wsedsera.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wrwwxrld.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qymrqkpo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dehvjnxi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vldkfcch.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vfcciety.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sugzbbzc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jwyvbosr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zxdtpwgf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fjprqalh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3npijseci.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pjsxmweu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ojjcjarw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lyevftia.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3nqgsulyc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3sbdatulq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ownearbo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hedetmyh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dluukpya.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3erhjacvk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3cmwardej.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3whkyddjc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ecvylrhx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hxfvawts.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nkuylblo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jpzxcara.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3paanraih.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3uzhjcjle.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tdxpphdu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iqkgkump.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ltenleki.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nswcuzwe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ilaaawtk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jvmfrcrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ynoswsok.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xhcwcthp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ievyhcjz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3urkdlhia.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yypsbecw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mjjrokpa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzsfmpsf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gyjtholz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xujhfxlu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jzcmwfsv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nkhsacvq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3obztowwa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tytlevwl.html


<!-- 参考信息 -->