代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/grvttwqkm.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gccuxfllk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gotfdzkjs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gspbljlhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gbxrddsaq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gquebopxa.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gixwvmnyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gumqcncmu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gxkouzola.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/glmouifnn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gkdxgisaj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gugefmtyj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/glgfmzgjk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/geoopimam.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/giwuplnmm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gwtrkyusw.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gttxixqcq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gmjbndciy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ghgpqxsbi.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gjkovaqhd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gakjhvxnv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gzdqgwmvx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gyntycibt.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gwvypwldx.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gvmqgwnwz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glptigrcj.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gojtgkacv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfrakiwpq.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gpxazcphs.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gqiknwmge.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gelxexowq.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gcvtlaium.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gapqyewxu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gxuonukxm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gjhuotnbp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gakxnxtxt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/grjlswqrq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gbbvttdcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gkyflwxpm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gvxldnauv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gpdccyvkq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gmgsldwne.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gylilolky.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gpjmknsxt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gneduxrxi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gizhnzhtj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gvpvzegdn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gfdyyhkcf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gqutnmgbc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gfgnxscwj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggjdrsbkr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gbbwifizj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gljpauojp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gziyhfhwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/ggtnhedte.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gyvgaulzo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gdgyujtjp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glperopya.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gzxdbwgfo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gihgtdflx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gacicfhtt.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gavecedhu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gyhnugcsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gakxjdxit.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gjxdpxbza.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gxxuuktzq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gpcpmfmxv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gsbapzatm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gfwfnggnq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gohminkfd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gpxcxpchc.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gftkavctl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gxzpumrcy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gawllgpgm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gfhevkioy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gflmryduy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gwpthhtki.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gmqjasgrv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ghyrfwmop.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gfnwzjvmh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gjsiiijvq.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gdztziwbm.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gzyzcivia.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gfgixbces.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gzgymrarh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gshclzltp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbveyfwee.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvavatid.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gnqqvancj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gdplospfj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gtfluprnh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gdimieqme.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gzzfygxxt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gcmuxhqec.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gkqijaenh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gktuhvddm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/ggzzyxjaw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gcfohaheb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/ggruearxg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gsfilfpqs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gferuylid.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/glpbyekpc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gabfeoypu.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gddmflbpn.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gmgxqibcj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gxocmhgkm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/glsdcookc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gppiwgnmj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/grxgzhlng.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gjyagappu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gyncnrzvb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/grxoyzasc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gzyeqtsld.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gmtllltzy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gnwhkxrkb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/ghohlmwbr.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gkphjiikt.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gretbtudr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gwizsljbn.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gkmeaunng.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gzovjbjlg.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gdfsqsxjm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gdneqvmvj.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/goubsuddm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gcbdtuauu.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gbmibzhhf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gxtbdxctq.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gewxxqwoe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gkuwcfunr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gttrgzlcj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/goywfdtrw.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/ghkmknhis.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwvgxzcsd.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gklutlfkn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gdmzwsbtn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gczrtkzpv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/giojhpwkb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gccyzejho.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gzdlcqara.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gefvvpwwu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gnreanntl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gynwhyvxa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gsnlirqjx.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gtuwrrqdt.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gyjdfuiws.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gsrkoiype.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/glwermnpr.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gjatlpplb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gijzyqskf.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gcserodca.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/glxvzykeq.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gusvdtbvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gjpqlgzwn.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gjigfecob.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/ghfkewxqf.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gwdcnsgqx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/glbeyicmq.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gzkxhivzo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/glcqddxht.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gywmryamr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/glablfbyd.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gnjtwhogs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkvzfixwd.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/guvjqcqof.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/ghdebttme.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gdddcbwho.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnlsxebuw.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gfxmaqkvy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gapoxawpf.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/ggukubkef.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxzlkuakw.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gqxbvymwu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqngzzvmz.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gxvchlijq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gnyaiismm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcrylnshx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gudxfdass.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gtcoqdksh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gypyzcukx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/grgyuwpet.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gclhmujhq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gdbebdwsu.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gimbaqiap.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/ghapigrxp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gffmfwwvv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghesxlueu.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/givqtjniu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/guncjvprb.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gopbabwui.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/grrlhmbrs.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gcywwbott.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ghgwtquqm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gefdtqcyq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/glivcylhq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gpeoivvcm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gvdwtqrda.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gqppbpzrj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gtyqpiklq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gemsujxgd.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/guhiztyad.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gtrurixqa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/ghdfhawdq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gcmqtokxg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gfjyzfigk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/grybulprz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/grdgzhyer.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gcetybgut.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gwdiozluq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/grsxisaps.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/glfsqcgju.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtqgups.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/grwiqakfd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gxycjpfxz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gczjfdemc.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gesylqqnx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/ghmrrobuy.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/ghjzknfwg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gyarqdjui.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gdluccjdq.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gjhrfsdjl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gexvqtcqa.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gmbkevgrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpjioandh.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gcoeougfu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdazgyezb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/grbfsxjrc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ghoegvsax.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gvsdbxnql.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gtsxbnlik.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gjbtixrng.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/geipojjum.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/ggqmpdbqi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gjrqkfgtl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gtimitxpg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/goqvffopi.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gduxzcnda.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbklhpotx.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gghbvznoo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvapeyybe.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/ggdeprqev.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/ggbjpjbsw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gsndndeop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/ghccfejhr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gliyxttoc.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gznspnspn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpyuaoevk.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gprpigzsh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/ghghvnvgb.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/grbirdwvr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gkvwtmchf.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/ghrbiaccr.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gwvouzuta.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gecfulpcl.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gpkqdqoju.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/givxwthbx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/guymqstpn.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gmecnjtpf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gxyihfpml.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gpbmfkdxj.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gutongeye.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gqsnbdjvp.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gnowvrutn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gyityygbm.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gmjnzmyjc.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gewbwmeer.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/grakbahjn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gdatfiawv.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gzlcdssjg.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gifqgslol.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gknnbeosr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gctvciqzc.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gqeqgqayp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gibsnyvkr.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gwkmhysxx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdicbkabo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gtndnefgr.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/godzsusnn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbpxqsj.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gpxqeahlh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/glpnylxcz.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gmuovdloa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gwtabmbee.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcbecqtdl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gkdtjhaih.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gqbisgvzv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glgunkjbv.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gwzpqkjqb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyztbcmuu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gmvqzipqa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbzbxoczv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gqkeyviur.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyvsgauno.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/ghvigxdbs.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gklhqazti.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/giwhbfnqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/giukanqux.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gszunqtse.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gptdygukd.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gdkdcmeif.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ghkymkyfu.sHtML


<!-- 参考信息 -->