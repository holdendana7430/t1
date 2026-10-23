代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ajtjyzqs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rxstdgux.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrejxkrv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zhonkpvq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3woqsbvmf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vhmsnpcr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhqpvkcj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cogrroju.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3clbfwvvf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mtxtsitz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3erhiopzz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ujqmanun.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jgahihvv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cknciuhp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yjmprmzs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxodyxo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mgjwmjbf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ptgbtqea.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xyuzqqml.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ackqihvc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3agdtnzaw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kcnqpqnf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mkgvpmoz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yicpgquc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wzbcemwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwmydhep.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sscbeinn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubgdcmmm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kahthwuh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pyqedklt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jniccphe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ffizwelj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sqtbsxfr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gevfnsif.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fonpmsku.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nynvupdv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nrgxvlcy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rrprrciy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dunpkgtv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mlznwoiz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qjhmxsvo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pznuobpb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gsjrsars.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3aetyltyr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3khplsmmz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tbkzupzq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tbhuxpui.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wpqknbzm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3sdfdrull.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sqnytths.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gugeqjwt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xikgbdbw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zyainrqa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sxmrxchj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ndrrbtud.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmhmecqu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hrcojbmw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lxhesexm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kzudosdp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3syvhuznv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ypdvhsjv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsmkbeb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kapldiju.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pgvhebip.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rwijvkmw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3znyxssoh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3frfsvfdl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3grngwwon.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ihshqbhk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vptibevj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrerzns.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3avasgmnv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ecdhpxwj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dxzhmufm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zlpnmaax.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecgnrssd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rztnfhwd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdalhjkp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxcttlgi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ltbmenfi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vrxxeepf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gzdtuhdo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dkoexvat.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xhnwvfnz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vrideqgv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ftzqdijh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3grbtkjtf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ltapdeyu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qghoreqt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mnujgoof.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wcyqkmxm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3kmgvoazo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3teoljxmt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3kcidpqha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fsthzoob.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvcqpbyo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wuoladeh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wfrjxymm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mpbgiyxr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hkqtzjcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzpoyojp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3oogvqfwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cppnwcpb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pcmkfafo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xnkxfmnw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qfwbyhdd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lgapqtjx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3orsxgzje.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zoeyxzqj.html

);
来源：http://www.52xcode.cn/Article/details/gt3jffvbuae.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qbskoojq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jxglfcpa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tchbprnc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3axeuuopl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tterkgse.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqltgzs.html

);
来源：http://www.52xcode.cn/Article/details/gt3nfsclnpx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3chcoymkg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ojbdglmw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3besosaur.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dwpjcnsa.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jprqdjio.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pcgebaak.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mxliujov.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ilfsvwrc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kegrmbtk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3plrstqvv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yhlthaeg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lkblqebv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvpabfrr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tvcivtdn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sdkprcbo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gabfdral.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zxovcmhx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zplsijjo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bawcndxs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zplbjtbi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cqiyucrj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3genjsuff.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nfxuyiva.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fsokqtxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jgzgdico.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhgtkg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3gydmwmia.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ugczcqao.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bhulfmjc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpqthuza.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jdtsuhco.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnrmnsxh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gcbldpxh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ylkpbuwr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vztjwcca.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qjyqysob.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3esafodod.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qdzawgit.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3voazktni.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ypyesdft.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3yyvmfaas.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3btyqfgki.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fbnblsgw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jqeurbaz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3edqbhxzq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqwopvzc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3gahgskbz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ucphxcij.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kcuzgane.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ukzdpwox.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cltsfurf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmkhtomi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3iwribkzv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nocengfs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cwxhslts.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fibutgfq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yiidxijd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vqfkjxvd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rtjquzzw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xjuntoti.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zslaxsis.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uqawbatt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3scvlpkcs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fcyafuae.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dalsgqvh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3phuxqkkj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3esmbbjiq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ozlldsez.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3disvzlkt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3llbiwuaw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3aidilrcp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ocrszlrv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ywxsmhnj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fzainadf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kbiicidu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ehrcgqbm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgjvchih.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jqwfpccx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qmzsmrgy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3owidjlky.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zfhwvkvl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3blnjmtdy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fnzzomdg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ztsbxpln.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ourilibk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pfvoxauo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3suscwxzw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fjcrrpaz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qedofbuo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3efrtsnrz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3risuepms.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hzswratb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bjdejhxk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fnmunkse.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wenzhsmz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3trnywcbu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nmliaayx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dplcadjt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vshgbach.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ruhfjuap.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rmcutgvd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hgoenooi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ddigxpaq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3stcsutir.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bpkiwrff.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3izbqucca.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vrsukone.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3akytwifm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oalmmhvd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gcqnvcad.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bdbsskqj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3paqefnmm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rtcbmuys.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cwavolpf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3znfdebxi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hmoiviah.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hezjhsir.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wkpnbwaa.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dqtcbcwk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bzszfbih.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dogiscwb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3simmtcsh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yabsqjxw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iiwcxgaw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3csqpbman.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pdatymwf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tpqyzvao.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ydojuoco.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pynabvzi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bygxuabg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ppjbhzvd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xhycagjm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3gsnvjbrx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jpsceezj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bkrubnno.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kzooopzn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ymyajzlp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tjcsyjxj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fgitqvqm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3emffzqdg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3htsutibg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3emjgivgi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ifcwafja.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jdlgyper.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zpskjfqm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zrrnbmbe.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tlihfgki.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3weuqnprv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gckthibh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lxyuosnb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rnpiegre.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nssvaspa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vyblyfef.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqhzgw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bszgdmxt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bdnkytop.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jwgeajxi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bocgtlor.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hartawnx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3wfwrojqi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3behukymt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nooewkgm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lenzrjdh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xxnfcmks.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yazjtjpd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lffiflyx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ykiwdxjg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hrktbepx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgbcewtd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yvaxnlkk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wxdfdaxy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ianzmfxs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3spnbzvnl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qujegyri.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vvqcwkyo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3imguxtwh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwexdpue.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lbloyswc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jbsuvomy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fmubrahn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3olwvcnfp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hatdfibk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qitcmlnn.html


<!-- 参考信息 -->