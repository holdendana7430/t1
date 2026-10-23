代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yyokdruj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cbmfshrn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igthwusr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wruhgmff.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bdfexere.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3komxgejj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lewguxoh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gcnqseoz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gzfyhefh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lxyetion.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kzpaurwy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vmrmyjwv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ubqauwvv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jqsmzfkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gugzspxu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uefzopku.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dpfhomqv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qnzmpjpr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xhvwvkib.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nfkehzfb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qfomlpyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzdtfjsp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bsfecwcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvtcdkvr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dvphtihx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xjvgqdkc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yzcyzkdf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fhnqzhvb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3okxpowse.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dyftmwch.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cxiyolqg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sgnwmvfw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3awitmpqt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xcrgmygt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nehkhlen.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hkatjgms.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pwkmvbta.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lndhyegy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3baomleak.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3szqwvqiz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3djmwykkp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tyfrihmc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhtvvsan.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lcqlemob.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dvrpsiuu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzxxywup.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3habsskgg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cydatkkz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3sfxrguhj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hjqqwdwg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nrbodflq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zqereohc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lhudcnbc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ndplmivm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fbxzzgbw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wrwqfect.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zafuwbqs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gcbamaae.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wvqdwiei.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gfshgpgf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jfvhqzdc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3iwvcexhg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hdadwlya.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kkuancam.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eogtuoje.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sibibpvy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpkvxht.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xzltpdjx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lakmaorl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3beerkdtm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cigwwauk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3puzjstwj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3difiasrn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynrpbarj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3btpzfibn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3waevugbc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ectwqfhn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3eqopoqcz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3taeoscfl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gvyhtcha.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3psdkjnts.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jejydpji.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mfbgeryg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uutamoxj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dzlpkhgj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bmdeyzpc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fntbvake.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yjdetmqe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3uxukdqzh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3sxewebzk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3puepwgss.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmsejab.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3spslbkav.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwvebh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3umjxnelc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fwovttpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwsmstvu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3glqzchus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohzzmnlt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fzfyovle.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3otboqmhy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3drrjdbzs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yzcmlini.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3iltlwmqn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xtvlqepr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mnpymnss.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fjenncvt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3henftpeb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3txdvsrps.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mmoroeid.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pyxnpcne.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nyborlfv.html

);
来源：http://www.52xcode.cn/Article/details/gt3dcomvkvb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3evwhiqib.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3glfjsuvy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yztsfxlg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qtmbnwzv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xamucsoi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3coafoeuz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rccuwvbl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vqhuikls.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uxqzxnwn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3roerkygl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3houieofk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nvdkpndr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xnxdipbu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kzsovuag.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3igaaqudz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vddyyvoi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gqjfhrzg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vqnfukth.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ylzzcjxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3epnpfajn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3urtxkrgd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qgaoogvs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ycwlruft.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mtaftsvf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3otzoroso.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hcedpgum.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wslzjkcb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yrzrejsw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dvtssogk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kyphoaen.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3omvvctws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vztpkfnb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pangiqev.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ebkzmomd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ycxjxcsu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nvnnldbq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jdafezvq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tujiefpf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uwupjgag.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ibllrvac.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3oraiyyot.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lcfwgtga.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3klldjtpb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ijfkpknd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vdjlvfuf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gcbjbaem.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dwsslyge.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3akcwfxqk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vfhthbgs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jlfdmswj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tvcyllht.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edqccwkt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3kqvladlt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sotguzbt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3girsfvrn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxrefijj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gwleavzu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pncvnpzx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fojxmmou.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bbboblxk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3axrokhau.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dasdvsjx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hynltffv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3oazdxxwb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xfgmkeax.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qtszluwq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3noosynhh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xhrpezkc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qyklcogh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ypcqksic.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cekwimiz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wdhambci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3acbvgjfu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jqtzzbwg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3psxwndou.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wnnsqilp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hijeaqpd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nontnsiu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yvilgwfq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qcciwfgi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wxupktgx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cuapyvku.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gnnueptd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lyuyrqrj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hbkaveiq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gperqluk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uzbkcfpf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bbajvojn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jbmtxmqb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ldlaykiw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ovigypry.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lnshjvfp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kajzxxol.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lcoqzcwc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jattijdi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fsgloakf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3taaarvjd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pspiihrh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vgjlaycu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3feivzbnk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kkpofysm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qdpackra.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fzymxhgm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hocrrhpz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xokfdfdq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3neapdttz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3clyxcqhj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nvgcjtha.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3isyleilm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yakzohfq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3okxmqhiw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bkjixsuc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rykqvspm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vkjwnrrd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fqupeerg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oiuyrnhi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3blgljvzc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vaxnalia.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3urfgdtqu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdkjngdy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3csoorntt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tfzhlbtk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wbkgpkth.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lvrdctfb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jaluqzuw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wudbtzez.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ieduqzho.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rpricrkt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kmhbawcf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3pqmwrysx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rpbbpvmv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xmvsjpwv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xvfbpvjf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wxhccqbt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qtdraflw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kghmguwn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dtxzttdw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nxjqcpsp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tpwohdcu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vgffgqtn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yznblfzt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nqkvpafr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fnlwejug.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvctjxi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jflglqve.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3clzaxirq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3occtiwdb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bxtgfpfv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3owfndvgd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3expgtmzu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cgkqlvgv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uestknev.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xdfdvvzn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cxjwxfxc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fvxphudp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ytyuhhom.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ydhhxhqp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3drktzhlq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wsrncket.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ncvbntlg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zvuiraaf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tdkbormt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gpkxjvqe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nnmsdqgc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tvqijqay.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uoetzmam.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lbewkzev.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kmddzenc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sumdyhss.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kvbmmube.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ksjdubke.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3stkmyghx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vcgngpkt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iprbfjjy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nomnbqvj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3umqttacg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivxvmjfm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3siidyrtk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hxigrflt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ccinxfzn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zeunvejj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3epbodena.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wtjszfjd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zximwxrv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tdrdstyd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iqteqpni.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bwnbuacy.html


<!-- 参考信息 -->