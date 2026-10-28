代发 wailian999

================================================================================
来源：http://hz.jinqigfzy.top/gtsproddgz.html

O. 并发与异步
来源：http://hz.ydzc1.top/gtimlynasr.html

================================================================================
来源：http://hz.316326.xyz/gtcqgiwlri.html

[O01] 启动一个线程
来源：http://hz.yj20258888.top/gtrogguvuv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtfobmrefr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.0kj1m.cn/gttnldtapx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shangyingyoupin.top/gtnyghdshl.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtfkuytfku.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtbegvnujk.html

Go:   go f()
来源：http://hz.wangdashe.top/gtdqtjlteg.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtwgupfbrp.html

C#:   Task.Run(() => F());
来源：http://hz.fzhhl.top/gtpdwtppvb.html

[O02] 使用线程池
来源：http://hz.snrcjt.cn/gtngvdogao.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gogol.net.cn/gtvlxspnel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigfzy.top/gtibtidwik.html

JS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtwhzrxwzj.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtbfvmsjdw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtlxwalnqr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.redwolf501.top/gtrlgdgfbw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtryabfvql.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dashuyun.cn/gtkwdveczf.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gtqhzlqeto.html

Py:   with lock: shared += 1
来源：http://hz.wangdashe.top/gtjvaschxd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daxiang520.top/gtmvjrwoti.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shangyingyoupin.top/gtqtnqyydx.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtfjyhfcpc.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtfmnywrfv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtnjuegdgc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gtyfeyxmkz.html

C#:   lock (gate) { shared++; }
来源：http://hz.hammf.cn/gtsmllzhgn.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtgnkmbrmh.html

Py:   async def f():⏎    await g()
来源：http://hz.chenzaomai.com/gtjoenusop.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtlcwmiyqb.html

JS:   async function f() { await g(); }
来源：http://hz.meibo888.top/gtgeuyzrqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtzccuclts.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtcmbrsxfa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xziqi.cn/gtqswuaqfx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gttrrsdytm.html

C#:   async Task F() { await G(); }
来源：http://hz.shangyingyoupin.top/gtkryuetlr.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtlbyzsqji.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtwdnkdgfx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtplremxbv.html

JS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtpirpjzra.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtwimzahkt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtieqslhgv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtvyqzjrgi.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gteiteepcg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtfwuofjtq.html

[O06] 使用进程池
来源：http://hz.gogol.net.cn/gthbvhnyek.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtrzyqnlli.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtucykqhdn.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtkmikurcc.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtkemofniz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnqzz.top/gtokltzpos.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtispyeoyr.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtvycvgsjc.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gtvycydsmc.html

================================================================================
来源：http://hz.dashuyun.cn/gtgigchozu.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtjooswooy.html

================================================================================
来源：http://hz.0kj1m.cn/gtfmblijpr.html

[P01] 生成 UUID
来源：http://hz.haohaochexian.top/gtjxuowrcf.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtwqyiorea.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtudvqylef.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtsegbzcrl.html

TS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtczrruarn.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gtzrabsbla.html

Go:   // 用 github.com/google/uuid
来源：http://hz.haohaochexian.top/gtafnpdchu.html

Ruby: SecureRandom.uuid
来源：http://hz.andypj.xyz/gtkmpfpnrw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gtwvkciuik.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gotoacloud.top/gtmgpogjeg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtpqmfgyyd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtpitpjpnc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtiikviiia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtgyzyqypd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gtzgdmfagu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.svipenyu.cn/gtxhecevem.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangtech.top/gtupidxull.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gtazsetcwi.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtnmmoawjc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtlffknnqw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.c1oappe.top/gtttgsrqob.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtrkdgjyaa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtjtwkxqqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtwkctvvrn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gtkuqanfmq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnxiangtu.top/gtgneazsan.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guannengcc.top/gttfdhkjkn.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gtmzadpbfn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.kuanghao11.cn/gtqjscxsjk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtyruojzmm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtudjdkqtk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtryoycpuj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtgnunddga.html

Go:   len(arr);  len(m)
来源：http://hz.cashguo.top/gtsxrpipje.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gthpurthhi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtctgmewqr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtihobwzyr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtyacuajun.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gtwdhvmibc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xingfuxueyuan.xyz/gtwwtbaxqo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtijarkype.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gteyefotut.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gtpoayqyhq.html

Ruby: a == b
来源：http://hz.cdnleiting.top/gtjmnqirqv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtrzdsgbqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgfzy.top/gthyebmjcz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zdqjudy.top/gtwpobadej.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gtuhjvezhn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtwkiztpil.html

TS:   if (x == null) {}
来源：http://hz.c1oappe.top/gtoplmrvtg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtflnskmmi.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtoxeeawtf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtaycwaotr.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtyyvvkpti.html

[P07] 防抖与节流
来源：http://hz.0kj1m.cn/gtzsvzachh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hysaishi.cn/gtkiqttrab.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtpnwssbfd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtrmwaloct.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtuquqeahh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gthakuzcyq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gtaxieskup.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhixingplan.top/gtykbqsmev.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.svipenyu.cn/gtigdwikpr.html

[P08] 处理浮点精度问题
来源：http://hz.wangdashe.top/gtkirmfrtv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gttglpyloo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ybcxt.top/gtocogmwug.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtfxwkltwn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cucudq.cn/gtpludfero.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhoulong.xyz/gtyvfezucj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtascvjoom.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhengqikj.top/gtrlyeochs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtxsueowii.html

================================================================================
来源：http://hz.ehwqpu.com/gtreyypywj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shzxlz.cn/gtbcvrhngm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtufimcdfd.html

[Q01] 创建表
来源：http://hz.andypj.xyz/gtckswyatr.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtcjazjqwa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtbmraqlay.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gtfkheogcu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gthhxvnhgf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtcnzvjrly.html

);
来源：http://hz.shuidangran.top/gtflmlcsrj.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtvsvobmbw.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtqjbnayxa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtlgumtcez.html

user_id INT NOT NULL,
来源：http://hz.gotoacloud.top/gtihyfirul.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtswezszdq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hfpthk.cn/gtfisxcjjh.html

);
来源：http://hz.jyoumei.cn/gtvojswgdd.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtrmtrjriq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xingfuxueyuan.xyz/gtrajxqhtt.html

[Q04] 修改列类型
来源：http://hz.gaohongyu789.top/gtpowaxhgs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ybcxt.top/gtjkairiia.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gthnzhgcif.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydjk.org.cn/gtftutwvtx.html

[Q06] 删除列
来源：http://hz.zhiwuduotai.top/gtwzabphit.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtfamylxbf.html

[Q07] 删除表
来源：http://hz.sysykeji.top/gtiglwnovd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guannengcc.top/gtybigwzup.html

[Q08] 创建普通索引
来源：http://hz.chenzaomai.com/gtgfaybemy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtcklzbdhr.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtgcxvgahf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtaakpuigh.html

[Q10] 插入单行
来源：http://hz.xingfuxueyuan.xyz/gtnurkzfyv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtfvxsbjru.html

[Q11] 一次插入多行
来源：http://hz.zhaomingkeji.xyz/gtbmnymdsq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.kuanghao11.cn/gtgvwofuiw.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtlbivukcr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtfeindqrp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dashuyun.cn/gtitwubvyh.html

[Q13] 忽略重复插入
来源：http://hz.bjfxy.top/gtjmvejuwl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtonutwzdb.html

[Q14] 存在则更新（upsert）
来源：http://hz.nwbrower.top/gtfxtjjpnf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.snrcjt.cn/gtmnxhxltg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtavzvnzwc.html

[Q15] 查询全部
来源：http://hz.ydzc1.top/gtjjrmhaqb.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtawsbefvr.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtvvpzndgw.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtpqclsudx.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtkeyflxgg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtcecmkwmh.html

[Q18] 模糊匹配
来源：http://hz.jinqigfzy.top/gterppulhl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangdashe.top/gtxkuhqcwl.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtupourlun.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gogol.net.cn/gtycyrajvl.html

[Q20] IN 列表
来源：http://hz.cheryme.top/gtoixwfzix.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.9152youxi.cn/gtqzbzcpvg.html

[Q21] 空值判断
来源：http://hz.quarkkingdee.top/gtfdbntxwa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj202588.top/gttprjghco.html

[Q22] 排序
来源：http://hz.guannengcc.top/gtdlaetrst.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtysytdrja.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtynihrsbn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinyuanbaomall.cn/gtixuwazgo.html

[Q24] 去重
来源：http://hz.xuetiantiany.cn/gtzadhvzne.html

SELECT DISTINCT city FROM users;
来源：http://hz.shuidangran.top/gtddaryfbd.html

[Q25] 只取前 N 条
来源：http://hz.yj20258888.top/gtqesdoihu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtbcpncsij.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtqrmboigd.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gttbusqygw.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtujxgucfd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtocwrcdbp.html

[Q28] 求和与平均
来源：http://hz.yongpay.top/gtrdtgdozd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtgzutofad.html

[Q29] 最大最小值
来源：http://hz.jinqigufen.top/gtaszohqnn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtxbylrvfi.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtkeebmsct.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gthlckjwfr.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtmytnwdlr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtmmqxswzt.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gtwgsouhph.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gterhqfwnt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtwtyoyjkf.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtmylcgnjg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xingfuxueyuan.xyz/gthixnqxgo.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gthzsvbhzw.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gthojreuxs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ywan-chungtsiang.top/gttpwqmiyh.html

) t WHERE rn = 1;
来源：http://hz.yuxming.cn/gtnwzalcgt.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtmuhitiek.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtrpenckhj.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtstwwovki.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtrbdnkhim.html

[Q37] 右连接
来源：http://hz.haohaochexian.top/gtrujvtosn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigfzy.top/gtombahjrq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnxiangtu.top/gtxsbzvsuh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhiwuduotai.top/gtaaxvbsok.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtgcnzrglk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sysykeji.top/gthuwfoobs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shangyingyoupin.top/gtqdoctxwf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gteedvtpty.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhoulong.xyz/gtrluoxvaa.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtgxoutcvl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtjprkfgsm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtzwinktmg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258888.top/gtguvwmthz.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtcusfvcpt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hywenlv.cn/gtahoyizzq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtyywlvhwq.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtxcdeslju.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fzhhl.top/gtzgvktgee.html

[Q44] IN 子查询
来源：http://hz.haohaochexian.top/gtdjyosxkq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtbgzcqudi.html

[Q45] EXISTS 判断存在
来源：http://hz.hywenlv.cn/gtcownvynz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtbmxuosaz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.mhx1999.top/gtczfiydix.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtblgcxwww.html

[Q47] 与平均值比较
来源：http://hz.ppjwa.cn/gtmdxtygav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ehwqpu.com/gtlmrsuquy.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtzqubabrr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtoabypypl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtskluyelv.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtamlyeurv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cashguo.top/gtgpmvorpl.html

[Q50] 批量更新
来源：http://hz.yangfankeji.com/gtnopzejww.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.kuanghao11.cn/gtmshkctpj.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gtbtixsezk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigufen.top/gtqlkloixc.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtyvxcsxlu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gzhubu.top/gtegiicwrk.html

[Q53] 按条件删除
来源：http://hz.ehwqpu.com/gtmrnsjtyt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.redwolf501.top/gttbfxingw.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtzzelbfhl.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gtgosydcek.html

[Q55] 排名（并列占位）
来源：http://hz.yangfankeji.com/gtsnbtnhhf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtorglrsvh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gtlgqytxee.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtyzdsdvue.html

[Q57] 行号
来源：http://hz.meibo888.top/gtrjwiuwiw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jianghu66.top/gtznhjklyi.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtmwvdjetw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yangfankeji.com/gterunzxfg.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gttoocqcyu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtmihlvjds.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtjyzaidmw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtmvwbdaji.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtwlaxvzji.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtrlwbgmre.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gtzfewdidl.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gthxalnrcm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtfdnjcvhh.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtuaxequdq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ppjwa.cn/gtjztmorzs.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtmnapqmab.html

COMMIT;
来源：http://hz.andypj.xyz/gtwwlxuwhl.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtawpzjmed.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtuxpehibt.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gtpazoldiw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shangyingyoupin.top/gtmkauiigt.html

[Q67] 设置隔离级别
来源：http://hz.jlsjyb.cn/gtgvcxwtvl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydjk.org.cn/gtezzkvatg.html

[Q68] 保存点
来源：http://hz.xuetiantiany.cn/gtifqdxmtd.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gttwizpbfw.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtcterdtpx.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtstlhoyga.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxuanxn.top/gtkcitahon.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtvrgbozjt.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtgozjaout.html

[Q71] 查看建表语句
来源：http://hz.zdqjudy.top/gtqsqfbejr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shuidangran.top/gtfscpxqgx.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtnmtkhrbg.html


<!-- 参考信息 -->