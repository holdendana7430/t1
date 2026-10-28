代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtnhnafjov.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtbruculfq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gtslelppgu.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtphvdegwz.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtvarllpph.html

Go:   go f()
来源：http://hz.jinqigufen.top/gtcffsdeht.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gtpcyzwpwi.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gtsfxlvcao.html

[O02] 使用线程池
来源：http://hz.zhixingplan.top/gttefcbwmf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtzxlocvsj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yonumen.top/gtctichbks.html

JS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtyoqnyvip.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtulfqncir.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhaomingkeji.xyz/gtltieycwe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gthbnpkezp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtfotpczmo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nwbrower.top/gtsueuldhw.html

[O03] 加锁保护共享数据
来源：http://hz.cheryme.top/gtpjdjonnf.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtimtefiea.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tianlin.xyz/gtlgzuqejy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gtpzzbnycy.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gthxdtjxvu.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtnsestlcf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtzlrhhdyk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.vqdsnc.cn/gtgeqrzrbk.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtmezgsszm.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtkymoslss.html

Py:   async def f():⏎    await g()
来源：http://hz.kuanghao11.cn/gtmaqyswth.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuanzx.com/gtzwignxqw.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gttncebbzl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtalqzzpuj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xinyue.icu/gtvdfiykkg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hfpthk.cn/gtvlqvqmaa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgfzy.top/gthtncrjjc.html

C#:   async Task F() { await G(); }
来源：http://hz.xingfuxueyuan.xyz/gtymaqzuxf.html

[O05] 并发执行并等待全部完成
来源：http://hz.redwolf501.top/gtimatzfqz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258.top/gtsvtczvcg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtivurpcax.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtenfelpli.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtednxuouc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtbvhfolil.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xingfuxueyuan.xyz/gtsqwjooex.html

Ruby: threads.map(&:join)
来源：http://hz.ydzc1.top/gtbaatiwqg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gtubzfszue.html

[O06] 使用进程池
来源：http://hz.zhaomingkeji.xyz/gtimvhxmgy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhongyouzk.top/gtjnfyhzuc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtkhzsffks.html

JS:   // child_process / cluster 模块
来源：http://hz.yvedp.cn/gthwljsjpy.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtanaxmrle.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hywenlv.cn/gtsyarorjl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.feifeiyinyue.top/gtyvukvlep.html

Ruby: // fork 块
来源：http://hz.9152youxi.cn/gtjnrtmjbs.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtxzhxaouf.html

================================================================================
来源：http://hz.haohaochexian.top/gtehyasfdw.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtyllgcwhl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlwmhygcd.html

[P01] 生成 UUID
来源：http://hz.xuanzx.com/gtguzuhpjo.html

Py:   str(uuid.uuid4())
来源：http://hz.xingfuxueyuan.xyz/gtngohilro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtrbomojgd.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtrzkdtmql.html

TS:   crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtldtyzemr.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gtunzwfstr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xziqi.cn/gtxepgxwfg.html

Ruby: SecureRandom.uuid
来源：http://hz.ivvv.top/gtbzelvkni.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.kuanghao11.cn/gtkkpfloyz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtaftyprqb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtndgmdisx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtagxcuikw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtqwuvvhck.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zycfv.cn/gtvpjjaeyv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtborhekij.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gttopayult.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtqzgkuxaf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yvedp.cn/gtquudpkxb.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtdbdvohmn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.haohaochexian.top/gtmxjtbblf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aizwys.cn/gtscbqnrgt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gttkfkygzm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gteixknhvq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shzxlz.cn/gtdgdzkvbl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtszmunhvg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hfpthk.cn/gttzayuonp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangshuangyany.cn/gtymiugosm.html

[P04] 求长度
来源：http://hz.meibo888.top/gtyxnrmwfx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shuidangran.top/gtfviymnqh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtjxhtmlqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtyxklewam.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtfuyhgxsi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuanzhike.top/gthicffltq.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtbmeanzju.html

Ruby: x.length;  x.size
来源：http://hz.hnxiangtu.top/gtbiitjiyd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtylyslzcg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.vqdsnc.cn/gtbzuejusc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtblsbxisc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xylfe.cn/gtlswrjbed.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ywan-chungtsiang.top/gtevufahos.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtzoidxncy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtpbcqnujl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangshuangyany.cn/gtpzfqgdsb.html

Ruby: a == b
来源：http://hz.cheryme.top/gtacvcuqbt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dashuyun.cn/gtqufbkcjk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtjrclcldi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tianlin.xyz/gtknpmbfab.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtdccuacee.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.andypj.xyz/gtlgbnbowm.html

TS:   if (x == null) {}
来源：http://hz.jyoumei.cn/gtyaoqgvnv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtvmdarant.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtreawosmv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhengqikj.top/gtqyujinzr.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtbkdcaqoh.html

[P07] 防抖与节流
来源：http://hz.fengsongda.top/gtkbgzulbr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtunxfxpgc.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtpopwfsqr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtexnwrkny.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtutgebtlq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yueranfly.top/gteugymlnc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gtjghpkyeg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtybuemhxu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhongyouzk.top/gtfrzkavrc.html

[P08] 处理浮点精度问题
来源：http://hz.yongpay.top/gtjkdpvsjy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtxrkkjozl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtdnyaovhy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtbclppfnd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hywenlv.cn/gtpslnijrc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtwrdaixhz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shangyingyoupin.top/gtktvvdjsg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.kuanghao11.cn/gtqfvufsxn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.9152youxi.cn/gtrzpmqmfk.html

================================================================================
来源：http://hz.zhoulong.xyz/gttanabcoh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hysaishi.cn/gtpkfibycz.html

================================================================================
来源：http://hz.pycfn.com/gtczgevxjx.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtibldsgmm.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gtkvnrngix.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtklulwgaw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gtvmjuntqc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.birdmap.top/gtdoujqsoe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dianchejie.cn/gtrzirxnno.html

);
来源：http://hz.chenjidiqi.icu/gtpozpgprq.html

[Q02] 创建带外键的表
来源：http://hz.guannengcc.top/gtnmdgotjm.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtzueumdfv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtyrcgimcf.html

user_id INT NOT NULL,
来源：http://hz.yj202588.top/gtsbemcvob.html

amount DECIMAL(10, 2),
来源：http://hz.zhiwuduotai.top/gtzxtzmznt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zdqjudy.top/gtyogbdbeh.html

);
来源：http://hz.zhoulong.xyz/gtqpkhbvoh.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtgxjbzgut.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtjrtmosbf.html

[Q04] 修改列类型
来源：http://hz.guannengcc.top/gtiqprzxzr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gtwhdfytnw.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtfeqmupcc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yonumen.top/gtspgmwuuw.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtljxgfadp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtxaxdjopo.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtjsvkmbqg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gtcrfhjmrk.html

[Q08] 创建普通索引
来源：http://hz.gotoacloud.top/gtgpyqechj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.bjfxy.top/gtanvhbyhl.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtoiixcyzf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtzuauonfl.html

[Q10] 插入单行
来源：http://hz.52xcode.cn/gtecgtnykt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenzaomai.com/gtxpafpulx.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gtpthbdaqq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinyuanbaomall.cn/gtsmeqoakj.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtemlooxhm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtlfdujjkt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangdashe.top/gteuxmtvez.html

[Q13] 忽略重复插入
来源：http://hz.ydjk.org.cn/gtwxnrwsar.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtcbjdwarr.html

[Q14] 存在则更新（upsert）
来源：http://hz.dashuyun.cn/gtyopdsikm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xingfuxueyuan.xyz/gtdpeypebf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtesbytkfm.html

[Q15] 查询全部
来源：http://hz.zhongyouzk.top/gtvxdsfyoy.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gtwogccfxw.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtbdhfmeui.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtyibqtyci.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtzorieovq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gttbrzgtwq.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtyqobzahd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangdashe.top/gtuaruabfa.html

[Q19] 范围查询
来源：http://hz.xinyue.icu/gtqqgqbdjw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhaomingkeji.xyz/gtkdoyjcko.html

[Q20] IN 列表
来源：http://hz.zycfv.cn/gtnpfsjvoe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.svipenyu.cn/gttkfyeulp.html

[Q21] 空值判断
来源：http://hz.shanyushiyangtech.top/gtiocduvkk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yvedp.cn/gtklgdjreg.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtubyccwar.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gtzpbeblho.html

[Q23] 分页
来源：http://hz.yuxming.cn/gtbtephmjr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgufenzy.top/gtfqlqbuwp.html

[Q24] 去重
来源：http://hz.andypj.xyz/gtwpxtmbow.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtlyjyfoxs.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gturajevqy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtguhbxhba.html

[Q26] 计数
来源：http://hz.52xcode.cn/gtivzjawxz.html

SELECT COUNT(*) FROM users;
来源：http://hz.bjfxy.top/gtehyrulsr.html

[Q27] 条件计数
来源：http://hz.tianlin.xyz/gthpkbihxl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtobekuwgb.html

[Q28] 求和与平均
来源：http://hz.yueranfly.top/gtpanyysad.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtvvwsyjjx.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtjeuqinch.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtdobfbugt.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtrhxdxghb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtzjzwivqz.html

[Q31] 分组后过滤
来源：http://hz.ppjwa.cn/gttjwjgccd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xinyue.icu/gtzxpyvbil.html

[Q32] 分组拼接字符串
来源：http://hz.hywenlv.cn/gtsapsvupg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtqdktlfgl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtyjkdxpfh.html

[Q33] 多列分组
来源：http://hz.fengsongda.top/gtcdrxatod.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tanke756.top/gtupabmcwr.html

[Q34] 每组取第一条
来源：http://hz.guannengcc.top/gtcydbtrnv.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtbxhmasdi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gttprttrdo.html

) t WHERE rn = 1;
来源：http://hz.zhoulong.xyz/gtqdgcqofy.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtuuxshlwn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtnajzyqaf.html

[Q36] 左连接
来源：http://hz.ydjk.org.cn/gtzrfcccjr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtsvyacjjm.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gtxegaknzc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtpuuqiqid.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gzhubu.top/gtwiavbuxx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.bjfxy.top/gtmdevbrfq.html

[Q39] 自连接（查上下级）
来源：http://hz.nwbrower.top/gtknrvslvc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangdashe.top/gtqipgfhku.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gteiobglpv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtcjanlwfh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cdnleiting.top/gtixljwuje.html

[Q41] 多表连接
来源：http://hz.shangyingyoupin.top/gtfhyuzaby.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ybcxt.top/gtmidzxpoy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtnqxvidfc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtvjgutagp.html

[Q42] 连接条件附加过滤
来源：http://hz.sufxvd.cn/gtzalkhgsg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtzcukfjel.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtpnjeyiqi.html

[Q43] 标量子查询
来源：http://hz.zhixingplan.top/gtikejfxke.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtsneruhlh.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtakbyocsg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtnionbiiv.html

[Q45] EXISTS 判断存在
来源：http://hz.hywenlv.cn/gthkwlszjf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gttpzdxllk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinghuilouyu.cn/gttjuuxrzh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtgkzdujpg.html

[Q47] 与平均值比较
来源：http://hz.daria6918.cn/gtfwngesht.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtbdaivafd.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtumefafjt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtwwszxeaf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtorjntbzn.html

[Q49] 更新单行
来源：http://hz.hammf.cn/gtieghgizg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtfohiikje.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gtbliiutvl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtwbfrakek.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtqeiadurd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gtxafgsxvt.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtijpfhxym.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gthkesbpmz.html

[Q53] 按条件删除
来源：http://hz.pengpengdd.cyou/gtqpqrwncn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuetiantiany.cn/gtfejpfqtl.html

[Q54] 清空表
来源：http://hz.ywan-chungtsiang.top/gtrfryeacc.html

TRUNCATE TABLE logs;
来源：http://hz.ydzc1.top/gtykvdyhyv.html

[Q55] 排名（并列占位）
来源：http://hz.tianlin.xyz/gtidxocanf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.feifeiyinyue.top/gtktlqeevh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gteiujnfxd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtutcwekbk.html

[Q57] 行号
来源：http://hz.yongpay.top/gtheijsqas.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtdjseqgmp.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtzjcbdkma.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhongyouzk.top/gtyceyeryf.html

[Q59] 分组内累计
来源：http://hz.jinyuanbaomall.cn/gtkkhukurw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gtrovaeice.html

[Q60] 取上一行 / 下一行
来源：http://hz.jlsjyb.cn/gtasdzfspy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ywan-chungtsiang.top/gtqbgacxru.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.haohaochexian.top/gtpghdpnkv.html

[Q61] 移动平均
来源：http://hz.daxiang520.top/gtjczdquaf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtvwsskdji.html

[Q62] 分组占比
来源：http://hz.316326.xyz/gtbbuewgum.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gttpehnbjh.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtmdzjwmyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtjfptbxbp.html

[Q64] 提交事务
来源：http://hz.cdnleiting.top/gtmxdgrofk.html

COMMIT;
来源：http://hz.gotoacloud.top/gtjooodvpz.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtbowplyci.html

ROLLBACK;
来源：http://hz.yj20258888.top/gtjxwkwrgh.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gthmrakmef.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtamlalnox.html

[Q67] 设置隔离级别
来源：http://hz.jinyuanbaomall.cn/gtwuzekubq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yueranfly.top/gtqnxxgany.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gtbhsgxerz.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gtxonvflax.html

ROLLBACK TO sp1;
来源：http://hz.tianlin.xyz/gtlhbfjvxb.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtixspfcyh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gteibjcqcb.html

[Q70] 更新统计信息
来源：http://hz.jiagoushi.top/gtydskaudk.html

ANALYZE TABLE users;
来源：http://hz.guowangkeji.top/gtenpvvxvq.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtlvusvwkz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtfszqbmkp.html

[Q72] 查看索引
来源：http://hz.tanke756.top/gtoafqcmeq.html

SHOW INDEX FROM users;
来源：http://hz.daria6918.cn/gtvpeohltt.html

[Q73] 查看表状态
来源：http://hz.wangdashe.top/gthwrbavfh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuxming.cn/gtjugjumta.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gtqyyzfqfu.html


<!-- 参考信息 -->