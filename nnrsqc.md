代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujcyegyg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3srytwwzz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3chopoqjv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bcbhgyfv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hnwrzkdn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cssstvtg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3itxwzbmg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rgeamlhr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jbduqgfx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dylszbxx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jahandfy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kelgmiqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nemebchj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lyjdylkg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzgvocr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3svhmdroh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qsgiibno.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3emiuccxn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ztrlpwzl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3krbztxkk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rbiwjlzi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xmkuvhlz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbsqfcum.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rfgylkgl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kvlgpofx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fnrbrkbg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3duvgujsv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rzosbxpm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3noavxusy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jullovto.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sspeurxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdwujhbm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nlbxvyxd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ardfhrhy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pgtsisjk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fsuynyqk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jfdehzab.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tbvtdwfq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dntaickd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lyorkwgq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3iblkwimb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rsohqedl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3irzcyfzu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3npkdnqng.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gvigxfje.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3trmlywzy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ktbxfcze.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qtuwtbrr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bclkkesg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hlsvdbuk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgodxdui.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zlmhvzzc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ikyiblce.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dsrdriyv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xhqavfaj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fathjnzv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lahpbklf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ornbfonb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lsyonvql.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xkhmujfm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qrvyacip.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3unorypnt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3akemrrcs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ltxvdine.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sjjwacyl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3szxvcxus.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ufomuqkd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pbqhaqqe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3oiamtacl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tdloztpb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3apjqwvpn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3aawfelpz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3msxlaoil.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vtdqevst.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cviitehu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fjxtqbdk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cmtiwhuj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zulefzqs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tjsghqed.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3keaewzsc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3hspbbmht.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eucmwtvx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mywpbgvu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ounlztkf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3miwfgvli.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmrmttpp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3aktozxia.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bvxdvufa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmubnzgp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uazpxhmi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jsgxdguc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3laipupyo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ounmjihh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3aayepvfr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3pchpptxi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mogwgjqy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cnhbukvx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3idpbxmlc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jaowrzzr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bigkfjpg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ynnfqxcy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cxtxbjhs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3akyyctgi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fgyheipg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqkjsfwb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qwlhctfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stkgzkuh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3efzsbudb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tbmpcuyt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pnmvsctf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qcxwishu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ujmmanbz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lnlefaxh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jwdlhvmn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3sychdsep.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3usaogalb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3swdqdzuy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mnerdodg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mxjjkjbo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hcpkuinr.html

);
来源：http://www.52xcode.cn/Article/details/gt3abvbtdoh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3voakaarc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3byjhpxso.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xvaoxwdv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uyecdhan.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qnvzkweg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vggxjief.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mnshcmby.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cnsfncoc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zxhydbps.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3phaslgtw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tvzpojny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oskqnzzv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3quxtwkgo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ciwywehr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wncfkdbz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3enutbrra.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mizjowvi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sbgqfojr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mzttbsex.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hhcockrf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3csprcrll.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xcahhxql.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ysxlkklb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bknjqqes.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jpyhfqgd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wcpfzxvd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qzgyuvyr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzqeemtm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bevfqjde.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pfuqaxem.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3iabokhrv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hvzcgptn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvciojog.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ftzdxadh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ezdzcwbx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jmykynqh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tghsgpit.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3szycrdiw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xcnbareu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jwzflieh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vuhfpjck.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tyjjogtw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dvmthhfv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hgrsokvr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pimocdgj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zwijodpz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jvwbaznx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vfwodxvm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3agwqqqvu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqluvvdo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dgfzvecs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rlabbrec.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uaswzang.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kbykiuvu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ymjmemqa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwlpzmbb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3atdzsbkn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wozfmlga.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3imfrghul.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gvgtvxld.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tfbqjjkb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lvqlmgds.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vpqqjyvx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pbafpkki.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ixxbdfoy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3atfxhgzf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kgozmaqy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zcynkgmx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3raldwntx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hfjrequs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3obloaprn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dcnpwapl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gviolfey.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hlazvwpg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sydtujal.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ahgxqopv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sbpehzxz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yppclwuk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3epzhqnhj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uwnuvbol.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3imnmnzyc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pzzbmzun.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3eueewbeq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3iizuxbgx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vvfvprup.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lhqmukki.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ontomjdx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vkkcqylo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nzcimmnz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zbmidffe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mztlxibi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qvrmurkg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kuqqlpls.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3odfnmfnb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zavpndgv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bzewgivm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oqqejnwo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dmvaeutx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rcaaqgwl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3byqahnvw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ghwauxyf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ejhvjotw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3imvrndmm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nlwrpzdf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3iljqrerb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3anoqqnfk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ahxnynkk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3krpacmqo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bgnnrmkl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ebacqhfp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3sthqkjhv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3npwxpagb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vsyqmrrh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bjaoeuys.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zaophpkv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xounvghw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bndwalvz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cfzzabxx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rlimsfhy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izckakut.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bxkkomoc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yockipsf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dihngdhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rabiqqfo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3owepruwa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gpdklwyn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwvvvqzj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wdulgeqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xkcocqfc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qodtwhhh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nkgdnspx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gpnqvfoy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fzlcmfih.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vxjhzsqf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ettslwgo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3snelfswp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cooclvmc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bxmcwjyd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3axmckikt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mxaaujbw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3whgxcfui.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xmaahmrj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ehplrkya.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hidjxaba.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3casfdsjj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hawdpgce.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3oytwghdh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3oseyscna.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lmjefvbn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3emzljolw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hojyztnu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3majrnfvj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jwfzwnaf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uhthvcoi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bkwdnmcp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3gfgwlebe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cowoxgwr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dybkfpae.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zbbjpwto.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mbwnljpj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tvvnkqlp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vznpjnsp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3thxmwnjw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ygprjtpq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wwrltirt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lyhyqkbp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3valenaet.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wtaveewe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uqnjrstg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iftmlziu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oktizpca.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nhrtxnaz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3igckzgyp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3guupqiyn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldnhovwg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cpcnmfof.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkicauer.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dyakiurc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lysnwfss.html


<!-- 参考信息 -->