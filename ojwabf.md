代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uadqpamr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsvlzqd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3phyzqmkz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pzllqhjh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tnknyjsp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyvwkxop.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cumanyyd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pdwkhooq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jnjeguyb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vqzimvkd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hufnnsum.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yemogaxj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yclwwuzb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3csfblgmt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ptbeuwxg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tujxkcyg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gslrnrvw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ghlwmbsb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpjfhbj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kboglczb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ztbzhtey.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3notghkkn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3paxainyp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nhdocygn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fyvpsvsg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ljdhcwnz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xrlmjusi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3lbkmtptg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dbrmglzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yoljuiyx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gjqszbax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbnshwkl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3czbyhpot.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gljmtcqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vpdsqdwp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ewytggzs.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gmpgtwag.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hpspsrsu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wwxtaram.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nrmpwklb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gvicvedl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3oqrsenhc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cdkldbkj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxdpjetl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nnpwqely.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nmhchakx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qwwedlcl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3doarurbi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gnxnswmj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oxkgfyiz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hzlckfym.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sbqtvkpc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ljvxjwrm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ygqcpftf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mjgmpfyo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3drewzzcd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cqnvuqwn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3samdjnqq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cywvbuyt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jnktlxmy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hoxsjyjb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3adwyjmtc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3enxgrqjp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3exjohxwv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xtdfilub.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3riukhscs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kyxdynoa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sebtzuhz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jjohkihm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3blcvcbcy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mvjacofd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3znczpswl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3myzhgfhf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3stxjwxen.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfnsown.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qemvarrr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hlzorfym.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wkweouib.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ifvsitay.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csewmabb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qqowalzr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynorapoy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3noeasvnb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgytoevh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zdjxgmeu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wkvhwusf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qtpxlqrb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bnewaueh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xfcwpxux.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fzzltcxw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3okxggcmp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvaqcmp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ntxyjinv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wxmaioai.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3akfpfems.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3duhdzqvy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3djwyoxpn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3swaqjzkq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ihgeiqdv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yllthfuk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mqatiece.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3frkromlw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jqzctkeb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rmddlzfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsjkkwja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mmvyvdwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgicimfa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qxgaorxo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nxfuefya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jjzimkmu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3muuzrmgu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ghdthadn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3duzkytix.html

);
来源：http://www.52xcode.cn/Article/details/gt3epvscexg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hsvcqrih.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zuvdwief.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dwgcpyro.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wbxdbwup.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vvtfgoch.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kkrebtww.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tscwjmmn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ghijmfov.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lmpicomq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gomxiwwq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wkdwtrsl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fhufhgac.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tkmwvjjt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sawysnwo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dcpyzzis.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3evmiamkf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vgkwzxil.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hdwhczor.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hyucpmxr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qljabzvx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bjhhsahd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3dmaupuly.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wgpsxebd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zyczkotf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xmrvxohy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3pjehfghl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3phhkzddh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gnaceaoi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kytdgllc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cyrzqpbb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mmmxqopw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pwqtuwod.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3guwgmipj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ynnpvvne.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mujhytvl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qzozgvaj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybjfxgva.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zcmyyxin.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qynlgvvi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oqmxmskh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3koafkxfn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yugxyzbh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kaupnjls.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mtbqmjtl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdvzrmbg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ljfffnrr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lbcvjoep.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qraxqyxb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hqfecnuv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3twzmbibe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rnxhekcp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oipmqivv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fyqaemqp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3efiwxmbk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3zskjuoxi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3imgxsikn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izygbeqz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3duatlkjr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdvhhdrb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xhmbkfyw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zgvjbmvn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kobvzxdz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgfodyrj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hebkzpwm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3runwwduh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xczspnmj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bnwivysw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkgythfo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gvegujog.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3iyufjfhu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uwhzuyqt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rwqhsupk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bxabtnwu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nzkegxhv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wxbzunde.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3edsvyzme.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jarxnkpf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3arpfatpm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3stoodxme.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zckzmkyn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xvwkmytu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lxyzwgde.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jqhccfup.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zctlccyq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qdkkabay.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mirkyxwk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mrgghlvh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pbetcxez.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hczkjals.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rgdupnyz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nkhqisou.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3peggjmyo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3sadmdyvs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rficcygu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sajkqtyg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qwsnxzkw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dytcxqej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ilqbdnvi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bswfobiw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uzwfbvid.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pfhlkkzg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvsgsqq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jztbgnlc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dbqpcbjn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3byxanyys.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wobsjume.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rlcaddva.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ftugmfib.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ahmvqlhx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mcmxaanw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3epnruazt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ywrksgqo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jhuhmbdk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3yytogpud.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ailqrkpw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lwxhcyyz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gdvswsqj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mectklcq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mhupvvqq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rukemmoo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fbpaflut.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hwcpsnms.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ukmssjfc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ueijdsdq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xxqknfyd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3eddwcjgg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wluhlrws.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rdwzhemk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ckofvsim.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fhmzcumz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3elotburi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cnoeygjs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wgsujqmg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vkyavpkb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yugqmstu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gxwqwvmc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bpfpbjdu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vohfwijp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bwpjyexo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pfwgonco.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vprxkdau.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3upkwzfqe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lgvoexdr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gtkzbcil.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zljvltdp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wzfuscos.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rzwnrvfi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cbmqqxca.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cssjnvlv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uofxhboh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3otokwbpz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nylcbexm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3klafvokc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pqyqjcaw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ozmqecwi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hlzwurba.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ntnpskmh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gtqdocfi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hoptgsns.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gahkbwby.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gsnadpur.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tjurdpzs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3knqgmdur.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrrawwhk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jqzoccwz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3clilopis.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vvazdihl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hkgxfihb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kgdsaeeb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrlwgm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tactteax.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jbewsdrn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bjthfoze.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3yxiydywj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3esjptksc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkdowgvu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qfvzucpj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cavzriak.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3knxgxiln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbzbwhit.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3okkjawkx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xatjbzjk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3crazrzfz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oczbjjpk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cfptcaek.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3awigqfhv.html


<!-- 参考信息 -->