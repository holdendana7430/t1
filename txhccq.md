代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhiwuduotai.top/gtwljczods.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gttwearamc.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhiwuduotai.top/gtswdunoph.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtgwwxjmrn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xylfe.cn/gtfrzessdt.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgfzy.top/gtnluejuxt.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtrqdvebrq.html

Py:   async def f():⏎    await g()
来源：http://hz.ehwqpu.com/gtwojtrxmj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtzslbflfo.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtggywkpec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.9152youxi.cn/gtndbxsisb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtamzhmwjv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gtgrtjnoya.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gtguytludj.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtaizsnizd.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtdrhozvms.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sxryk.cn/gtafxmbujc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtdfgqdzte.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtxhhuzguq.html

TS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtuapkuwfa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xingfuxueyuan.xyz/gtprlqbike.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigufen.top/gthfqysyrw.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtpugscpau.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtyjucyuuc.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtdmhdhyjd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.mhx1999.top/gtqavsthqh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gzhubu.top/gtxmxnnjkm.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtmqwfzmmo.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtdeheyors.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ehwqpu.com/gtlxrkdqky.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtjqmdpylb.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtymkddeox.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gteqntfafc.html

================================================================================
来源：http://hz.hnxiangtu.top/gtchxebppa.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gteuyadjlw.html

================================================================================
来源：http://hz.mhx1999.top/gtijwwrhnq.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtrhmjgvkm.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtnyjtzdra.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pengpengdd.cyou/gtoigmllmt.html

JS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtlfpksgzu.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtlqxpqnup.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtglidkoyw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuxming.cn/gttbawvhly.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgfzy.top/gtcwcdhloy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnxiangtu.top/gtofjphvgm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtdqlpqttr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhixingplan.top/gtdpeipsca.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtuoirklgk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtubdodhxa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gotoacloud.top/gttyxmtaqt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtvrruntai.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gtjetyzhfb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtdgnntjth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigfzy.top/gtrmngyiji.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtihpejjuf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtzchheykq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cdnleiting.top/gtneqlumej.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtxdcnxrcf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gtekuzftkn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hammf.cn/gtrrspjbvr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtfpypncdv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhengqikj.top/gtpnxpcler.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtwfiuryua.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gteesmyqcm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhiwuduotai.top/gtbwglooxj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtgwbpaqgw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtepgcbbbb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtiqzribam.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtbmlslcqr.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gtjvmvlldf.html

Ruby: x.length;  x.size
来源：http://hz.cashguo.top/gtkwzwgxnw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gthwpspimv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxinkj.top/gtgcegebrf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pycfn.com/gtlaqyobbh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gttouurhdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuanzx.com/gtakkwviia.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtyyvkshih.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gtwbfiqkur.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ppjwa.cn/gtwzxxjwjo.html

Ruby: a == b
来源：http://hz.zhoulong.xyz/gtrqzrdjxf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenlongwang.top/gtgbuzfjzm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guowangkeji.top/gthxmwjjiw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhaomingkeji.xyz/gtyjvgqndk.html

PHP:  if (empty($x)) {}
来源：http://hz.jinghuilouyu.cn/gtnzojaiub.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guannengcc.top/gttzaemqxy.html

TS:   if (x == null) {}
来源：http://hz.hysaishi.cn/gtejyvjmej.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtxghjakmt.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtfloabchg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gthdvscipr.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtrjpkqcrg.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtbsfbdvym.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydjk.org.cn/gtycwgnaap.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtqtlendni.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtpqqtpept.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtawwsrxxk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.bjfxy.top/gthukqpkyf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtqnrueizy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenlongwang.top/gthnxsitrg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenlongwang.top/gtcmkllmhg.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtntivasgt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hysaishi.cn/gtdjbsspsd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtfofzrmip.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtlflipdxb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxuanxn.top/gtgeoqirlz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gthmrtrxup.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gaohongyu789.top/gtyegugncz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hammf.cn/gtlavongij.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fzhhl.top/gtzlmyisni.html

================================================================================
来源：http://hz.dianchejie.cn/gthxovoopd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtmhfdkjhr.html

================================================================================
来源：http://hz.tian-w.cn/gtcyxxeqjo.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtkjfvdhjl.html

CREATE TABLE users (
来源：http://hz.cdnleiting.top/gtsxorsnxp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtsnjrydly.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gzhubu.top/gtnrlmvbic.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gthccleggi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtxifstuqw.html

);
来源：http://hz.cqqwz.cn/gtvdkazmtv.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtsgnslenw.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtriydhkrh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtslxtpojq.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gthcpwzpxo.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtalcwkzdw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.0kj1m.cn/gtpnmfuvos.html

);
来源：http://hz.guannengcc.top/gtgefbpxxj.html

[Q03] 增加列
来源：http://hz.yj20258.top/gthochvdyz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtgsrtzbgd.html

[Q04] 修改列类型
来源：http://hz.hammf.cn/gtngtaalmf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinghuilouyu.cn/gtogswrxhq.html

[Q05] 重命名列
来源：http://hz.ivvv.top/gtdpqijstj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gthfwvoebo.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtigahiwso.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gtruuhamtn.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtfqyycdpe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jiagoushi.top/gtgimyarbt.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtmjsmhpxp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtoaemehhq.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gtfldjeygk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtwndehbtq.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtymnetmnm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xziqi.cn/gtamwvpqfn.html

[Q11] 一次插入多行
来源：http://hz.xuetiantiany.cn/gtzofrzxik.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gttuanlruc.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtetdogaxk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtypxlapwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtzsnomvqp.html

[Q13] 忽略重复插入
来源：http://hz.vqdsnc.cn/gttzotwkgf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtyhmhfjlz.html

[Q14] 存在则更新（upsert）
来源：http://hz.ywan-chungtsiang.top/gtlbutjjlu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.0kj1m.cn/gtbbhnehhr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtahmiewpl.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtwhfnvvng.html

SELECT * FROM users;
来源：http://hz.vqdsnc.cn/gtmbajizhq.html

[Q16] 查询指定列
来源：http://hz.sysykeji.top/gtpwfgadsn.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtajeqqsmv.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtrlqhnqmu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtasqiztgy.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtykbzpavm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigfzy.top/gtggpajtrd.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gtvztrejjz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fengsongda.top/gtzqneuhbi.html

[Q20] IN 列表
来源：http://hz.xziqi.cn/gtrzjdfzqk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gtokmuylgh.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtmjpxzobu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ywan-chungtsiang.top/gtggcnnyya.html

[Q22] 排序
来源：http://hz.guannengcc.top/gtudruncjo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtlckopdxn.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtlbqvnfji.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtjlaverxa.html

[Q24] 去重
来源：http://hz.nanxinkj.top/gtlgjpuqxc.html

SELECT DISTINCT city FROM users;
来源：http://hz.xingfuxueyuan.xyz/gthdsgihzw.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gtedpfhafn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtsyythkwl.html

[Q26] 计数
来源：http://hz.ybcxt.top/gtwxapsphl.html

SELECT COUNT(*) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtuprzgtej.html

[Q27] 条件计数
来源：http://hz.zhaomingkeji.xyz/gtmbjaudpl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangtech.top/gthfmvkktd.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtrcivdmnj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtmijrrpso.html

[Q29] 最大最小值
来源：http://hz.zhoulong.xyz/gtdazzavdh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtagelzikv.html

[Q30] 分组统计
来源：http://hz.zhiwuduotai.top/gtlaitlsks.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtihwbvgli.html

[Q31] 分组后过滤
来源：http://hz.fengsongda.top/gtxhiwfmak.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hammf.cn/gtwtowspzh.html

[Q32] 分组拼接字符串
来源：http://hz.jinghuilouyu.cn/gtojqfqgeq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtmoigaoqk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hongshengwenyu.top/gtfjfinclf.html

[Q33] 多列分组
来源：http://hz.feifeiyinyue.top/gtwjaweabf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtporgfwpz.html

[Q34] 每组取第一条
来源：http://hz.jinghuilouyu.cn/gtcymwxvgg.html

SELECT * FROM (
来源：http://hz.ywan-chungtsiang.top/gtrxvwacqz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtfjaluhes.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtncxuknba.html

[Q35] 内连接
来源：http://hz.316326.xyz/gtmsaxtadm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtjlixdlzh.html

[Q36] 左连接
来源：http://hz.gotoacloud.top/gticbannxi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtcdtffqad.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtuebzqqem.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtzhgiodui.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtucxrjiqh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sxryk.cn/gtfwpcljeq.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtwqjnphcc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtsoumohlc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.svipenyu.cn/gtgugbzsao.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtbbipcfku.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtneaupehx.html

[Q41] 多表连接
来源：http://hz.xingfuxueyuan.xyz/gtbuxfxogw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258.top/gtfggqddkw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtrdgsonno.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guannengcc.top/gtcgsvpyjr.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtefqpowov.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtmrvlrrsr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gzhubu.top/gtczhptzxj.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtdglatgdh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtynkagthd.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtahkqfwhj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sxryk.cn/gtxdhecnza.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtseoenrui.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtpmdphzmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pycfn.com/gtsklravbr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtqnwndfbe.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gtslefrwta.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gtfkkeqzrm.html

[Q48] CTE 公用表表达式
来源：http://hz.sysykeji.top/gthaapbyca.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtoxiajnjf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtartsmdln.html

[Q49] 更新单行
来源：http://hz.ybcxt.top/gteynubzsz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gtpjsprovv.html

[Q50] 批量更新
来源：http://hz.shzxlz.cn/gtntavuhzq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtewyslsvy.html

[Q51] 用子查询更新
来源：http://hz.jyoumei.cn/gtjoaafgvd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtvsrijwjh.html

[Q52] 删除指定行
来源：http://hz.gzhubu.top/gtrwllatxc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtiqbfagke.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtzihrxaoy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtxwgdpinl.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gtbghtuofn.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gttixxmnnh.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtdsazrusw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jlsjyb.cn/gtmkqkidnd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gtdrryglrt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtgvaehvgq.html

[Q57] 行号
来源：http://hz.zhaomingkeji.xyz/gtoruiznug.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tian-w.cn/gtgxzcyjsz.html

[Q58] 累计求和
来源：http://hz.hysaishi.cn/gtmammasuk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj202588.top/gtmcfqumdv.html

[Q59] 分组内累计
来源：http://hz.shzxlz.cn/gturayayli.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtxpiyctck.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtxeotxkte.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yanxiufei.cn/gtkfzwfepd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.9152youxi.cn/gtzphraugh.html

[Q61] 移动平均
来源：http://hz.xziqi.cn/gthbwsakbu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jiagoushi.top/gtbjmikfpp.html

[Q62] 分组占比
来源：http://hz.jqgfzy.top/gtnfqrlypr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtkzturgzl.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtdnqusifd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shangyingyoupin.top/gthuuuuwuj.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtrawayntp.html

COMMIT;
来源：http://hz.hysaishi.cn/gtfihkvtsm.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtjhlwhyyj.html

ROLLBACK;
来源：http://hz.meibo888.top/gtxolmvrsi.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtybroxyrw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.dianchejie.cn/gtxkqnyzzx.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtnlzrwkqc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gtbgthcubf.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtbodzlayz.html

SAVEPOINT sp1;
来源：http://hz.52xcode.cn/gtfjdicrfd.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtiexjgblf.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtnafgiimr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuanzhike.top/gtwjdmqdwg.html

[Q70] 更新统计信息
来源：http://hz.dashuyun.cn/gtsilaniwy.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtujwxrjqt.html

[Q71] 查看建表语句
来源：http://hz.chenzaomai.com/gtvvxvwyyu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuxming.cn/gteqzuzrvv.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtskfguqxl.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtzfnuqywi.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtcnquawgx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtknijhnuu.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangtech.top/gtpupofdvh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sufxvd.cn/gtsqcnqayd.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtxqkvqtwt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtlfgcpmqo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtbkgbifmn.html

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gturznbxtw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtwbtgoaet.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gttmzlbvdr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuanzx.com/gtodhzxcnm.html

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtwyobziin.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtyyrctevq.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtpzcobnsk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtbtwkcsnj.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtyusbkbwq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtljrsksep.html

[Q81] 字符串替换
来源：http://hz.hammf.cn/gttaarfuwl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hongshengwenyu.top/gtsygamcyd.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtmubdpszs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtwlokaqjj.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtlbdjijin.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtarkmwybo.html


<!-- 参考信息 -->