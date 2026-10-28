代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtuzpoogcm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtaktzzqit.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtpbummppb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtldnttdbc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtzmpbcztv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.birdmap.top/gtqxczwakp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hfpthk.cn/gtppommwpd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtrkmvixhw.html

================================================================================
来源：http://hz.guowangkeji.top/gtsmjbrbxe.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtkorpxqto.html

================================================================================
来源：http://hz.sufxvd.cn/gtrdjblxqn.html

[O01] 启动一个线程
来源：http://hz.redwolf501.top/gtofygjofl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtbmodnowm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtqqtgiqtg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtvndhnbsl.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtzijyuyri.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtljundbxh.html

Go:   go f()
来源：http://hz.tian-w.cn/gtcsqvoyab.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtouhsrtyo.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtxsnaaxje.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtjuoohsoz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtrpkscthf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yvedp.cn/gtbyxhxhcw.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtbqecbkwx.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtzpewljug.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gtvrrnubmi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gtgnykzywn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtztllyiin.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhijiandao.cn/gtxbyvmhvx.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gtlperolde.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtvvlegvam.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtmdjbkccu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtgdbqbgbh.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtgvakutym.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258888.top/gtxdqyjklv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtbofwqxnp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtulwamkgh.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtduhwasju.html

[O04] 定义异步函数并等待
来源：http://hz.xziqi.cn/gtuomzwzqb.html

Py:   async def f():⏎    await g()
来源：http://hz.hysaishi.cn/gtsxisqarj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhoulong.xyz/gthxqrlqxn.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtdlhaynhf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtquawjhaq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtysskdzym.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gttjncfjxp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuanzhike.top/gtdevvlchm.html

C#:   async Task F() { await G(); }
来源：http://hz.0kj1m.cn/gtqipayahw.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtvsdnvxmt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtcupvdssn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtwkhwcden.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtuegcbbbn.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gthwldfxkb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.redwolf501.top/gtipsavtki.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtvfnsfekd.html

Ruby: threads.map(&:join)
来源：http://hz.cashguo.top/gtntptpabu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtghjilbeq.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtqcqlhmsq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtxbnnltul.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtwawqbkgd.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtvrtozykq.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtzggmjnkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhoulong.xyz/gtqnyavuis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cheryme.top/gtpfwavnoa.html

Ruby: // fork 块
来源：http://hz.jlsjyb.cn/gtlhhrvich.html

C#:   Parallel.For
来源：http://hz.jyoumei.cn/gtfntlgfpo.html

================================================================================
来源：http://hz.shzxlz.cn/gtarrtpagx.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtnivccvlk.html

================================================================================
来源：http://hz.svipenyu.cn/gtoxtkbqxi.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtivbqvbzl.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtfkpgdasm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtqihxxgan.html

JS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtzosqvrzs.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtfizwmpty.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtzscpgeau.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guowangkeji.top/gtyfmwrahn.html

Ruby: SecureRandom.uuid
来源：http://hz.tanke756.top/gtiymrfulb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gtfvmorfxy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuxming.cn/gtezstgvse.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtjmnzkgig.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gtqhniyyvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aizwys.cn/gtbkknawnb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuxming.cn/gtllnwizrh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cqqwz.cn/gtdwhgaljd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.smart0.xyz/gtgdocfyfz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtnozsgybd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtqodgqayq.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtxuhhflrq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtnuqiicfn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtbscfusda.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtuvnkaynp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtzwxnnmdf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gtnuunprtu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtczcobqfb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xinyue.icu/gtswuepfvd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shuidangran.top/gtqtbetymw.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtwptzeetk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gttshmxgul.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtokoclypn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shuidangran.top/gtyvpaglde.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtwpaqyofh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtvxqmtdzm.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtjrkpjmnf.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangkeji.top/gtdvkvsveb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtdktpecag.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tanke756.top/gtzdnkddzn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtlqbcgdfl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtrnrhiizd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.svipenyu.cn/gtqypvczrf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtoeaaixce.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtwxmfyxmj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtdevcbqhs.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtobktjrkw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigfzy.top/gtvbdkzgap.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sufxvd.cn/gtxqimqrtq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gtqhdjckjb.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtolnfaixm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cashguo.top/gtdecebteb.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gtcylzcvgv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtweaissnv.html

Go:   if x == nil {}
来源：http://hz.gzhubu.top/gtwwzxyuhj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtzshkrxeh.html

C#:   if (x is null) {}
来源：http://hz.birdmap.top/gtjxzhrmul.html

[P07] 防抖与节流
来源：http://hz.xinyue.icu/gthqiotmat.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ybcxt.top/gteekzpjdd.html

PHP:  // 手写时间戳比较
来源：http://hz.zhijiandao.cn/gtrokuyheq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtcpqblbty.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtcyoksflj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtbctlpdlk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtffsanjho.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhixingplan.top/gtjpattmsw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gtzfxusloc.html

[P08] 处理浮点精度问题
来源：http://hz.hongshengwenyu.top/gtujfobheq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hammf.cn/gtgwjvnqzy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnqzz.top/gtfdneabeb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnxiangtu.top/gtqvyvejzv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtgvxcnlyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.316326.xyz/gtpxfhgfus.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gtykedyhxv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtpjyhdpnz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtxyjdwoor.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbkdqgoft.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gticuwtxlj.html

================================================================================
来源：http://hz.yueranfly.top/gteagxrgcs.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtavttxdah.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtugwmtbpf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.mhx1999.top/gttsorpern.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtyucgopmc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangkeji.top/gtoewvnrtn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhongyouzk.top/gtmouqwnfx.html

);
来源：http://hz.dianchejie.cn/gtijlywika.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gtmvkondyd.html

CREATE TABLE orders (
来源：http://hz.hammf.cn/gtjnlhadpv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtxcdkprvo.html

user_id INT NOT NULL,
来源：http://hz.andypj.xyz/gtexnxwxkd.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtafivdtys.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtnkovqhfm.html

);
来源：http://hz.vqdsnc.cn/gtlexsdkbe.html

[Q03] 增加列
来源：http://hz.haohaochexian.top/gtrffyulrh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tian-w.cn/gtydlqjabd.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtlhhyetkw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shuidangran.top/gtbkbyspcr.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtlsinqxvz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtcryikwml.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtzpdqkgbe.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtclxtvaue.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtotpcqltz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gttoytvpep.html

[Q08] 创建普通索引
来源：http://hz.wangdashe.top/gtbeghbsui.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtadsmnfsy.html

[Q09] 创建唯一索引
来源：http://hz.vqdsnc.cn/gtjmppqncb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aizwys.cn/gteolpuefr.html

[Q10] 插入单行
来源：http://hz.tanke756.top/gtfipbyhkf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hfpthk.cn/gtgtehnmcp.html

[Q11] 一次插入多行
来源：http://hz.birdmap.top/gtsusologr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangkeji.top/gtkuggvlps.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gtrwegrtwi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtjhrmeamn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtsdgzbbad.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtozdrvjui.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtrtbyxjnj.html

[Q14] 存在则更新（upsert）
来源：http://hz.cashguo.top/gtozdzuwdg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtedfcochx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.havefunace.top/gtsqcmzfks.html

[Q15] 查询全部
来源：http://hz.zhongyouzk.top/gtnskdteym.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtfvrligel.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtytpkejyl.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtgfnutlaf.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtygwfypaf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtcuxdgppw.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gtgriwcvys.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtyeslnzim.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtzccifwwv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gaohongyu789.top/gtpuvgpjlz.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtroafxljc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pengpengdd.cyou/gtlzrgfsqp.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtayqrrtpj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hfpthk.cn/gtypqnplng.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtcrumpmlr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.kuanghao11.cn/gtrjaedksk.html

[Q23] 分页
来源：http://hz.cqqwz.cn/gtkvxhevbr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtdddgazpf.html

[Q24] 去重
来源：http://hz.jinyuanbaomall.cn/gtxueklvqw.html

SELECT DISTINCT city FROM users;
来源：http://hz.redwolf501.top/gthkvtovkm.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtjntesiyy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtnjgoagxb.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtjhhvezlr.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtksmjjgnf.html

[Q27] 条件计数
来源：http://hz.zhongyouzk.top/gtfvuhpbzv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangshuangyany.cn/gtwniugbgp.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtmoprackf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.quarkkingdee.top/gtecqmapdw.html

[Q29] 最大最小值
来源：http://hz.guowangkeji.top/gtlxonaypt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tanke756.top/gtxszsdnfp.html

[Q30] 分组统计
来源：http://hz.yangfankeji.com/gtyunrafji.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtenpgnnzv.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gthqvhmzbf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.smart0.xyz/gtshbehauk.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtsfruqasj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtobgearhb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.quarkkingdee.top/gtqsfhzoml.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtasurpxoz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtrgtjdsxv.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gtztqpywjw.html

SELECT * FROM (
来源：http://hz.xingfuxueyuan.xyz/gtrytyeudp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtopjzspvc.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtibnswmgv.html

[Q35] 内连接
来源：http://hz.guowangkeji.top/gtgujcxdsr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtixpxxgof.html

[Q36] 左连接
来源：http://hz.shuidangran.top/gtlxshfvdd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtttcxnzzl.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtjvcpxqzb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yongpay.top/gtlhhfmiga.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxuanxn.top/gtufdlyaxb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtddapxoxr.html

[Q39] 自连接（查上下级）
来源：http://hz.jyoumei.cn/gthmmnagnc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.bjfxy.top/gtxqozoopy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gttjmmvqyw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xinyue.icu/gtgmpfvwbd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.haohaochexian.top/gtottvjxur.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtfroaezgp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yangfankeji.com/gtmfuvmvep.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtjwscdqlq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gaohongyu789.top/gtjruhinpv.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtoqcmusrp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jlsjyb.cn/gtnoshkhbj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xylfe.cn/gtzcsmqoiz.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gttcmifkrt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gtwscnarme.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtyvvdgpxp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shangyingyoupin.top/gtyoypgvph.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gtuwkgbpjl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtjxicbzda.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtvncukkfq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtvolvfjpf.html

[Q47] 与平均值比较
来源：http://hz.zhijiandao.cn/gtzuduqhtj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.iojbl.cn/gtxuckmpax.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtlofbvtih.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gtvccvqzuj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtcnukkyft.html

[Q49] 更新单行
来源：http://hz.jiagoushi.top/gttfswmtuq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgfzy.top/gtymfrhcbq.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtaptyigbp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtfzuvvuqs.html

[Q51] 用子查询更新
来源：http://hz.nanxuanxn.top/gtymrbdeab.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuanzx.com/gtgpgffsnl.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtrsufysuq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtfpzblaeq.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtakgdrcjd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtbakonbgx.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtgtvwonnx.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtqmjkkixo.html

[Q55] 排名（并列占位）
来源：http://hz.havefunace.top/gtyjebtmwe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtjzvxliok.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj202588.top/gtgpejcdvk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtpxtrxpgy.html

[Q57] 行号
来源：http://hz.shuidangran.top/gtipoamxxu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtvvfuwqjp.html

[Q58] 累计求和
来源：http://hz.yongpay.top/gtoxlvqjqg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gterxyooyb.html

[Q59] 分组内累计
来源：http://hz.smart0.xyz/gthfytmsww.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtahvgmbzx.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtkqlbisbq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258.top/gtivmmgwun.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tianlin.xyz/gtajbpeayz.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtqkeagdrf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuanzhike.top/gticcnsygb.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtypeomhwy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtqpjnuuxs.html

[Q63] 开启事务
来源：http://hz.xuetiantiany.cn/gtykvhsxxc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.birdmap.top/gtwafhdasw.html

[Q64] 提交事务
来源：http://hz.shzxlz.cn/gtfxjlkppg.html

COMMIT;
来源：http://hz.chenzaomai.com/gtovtzymup.html

[Q65] 回滚事务
来源：http://hz.yj202588.top/gtsifsagyh.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtzbzxqjoi.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtarqzbjow.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gthyvwsynb.html

[Q67] 设置隔离级别
来源：http://hz.yueranfly.top/gtrsoyapah.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtsfizmiri.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtwfrbyjqm.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtarclwibe.html


<!-- 参考信息 -->