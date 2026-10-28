代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtrjcrjgph.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guowangkeji.top/gtkkkaaaro.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtuijtqihs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtrpbogzuy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtpwxhwzvk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.0kj1m.cn/gtycwtuelw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtnahrxhui.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtuyofzlwe.html

================================================================================
来源：http://hz.haohaochexian.top/gtaibfdulu.html

O. 并发与异步
来源：http://hz.cqqwz.cn/gtiyovvjzd.html

================================================================================
来源：http://hz.sweek.top/gtpkmxckhh.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtkglaiphn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtorokebje.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258888.top/gtmksrhhkf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gtcqiiqdwg.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtrtbfndqx.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxinkj.top/gtmzwygvhf.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtixoawycw.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtfdasfzhx.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtfohsqvub.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gtjmvzhkjk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinghuilouyu.cn/gtjsgzaldx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigfzy.top/gtofbfusqo.html

JS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtwvulqrdj.html

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtqgxoqwbu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtoscjawer.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtyudqsyem.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinyuanbaomall.cn/gtnmfggoow.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinghuilouyu.cn/gtxmzzbpwk.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtkdkmduue.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gtjwbmntym.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258888.top/gtuisvwlgh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtlojypbmv.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtrhecodak.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtqxjbkhvs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtzmivdrgi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gogol.net.cn/gtmsynkynt.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtomxubmkb.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtxbnrclsq.html

Py:   async def f():⏎    await g()
来源：http://hz.redwolf501.top/gtrciehvlc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtnjiwtbey.html

JS:   async function f() { await g(); }
来源：http://hz.tianlin.xyz/gtogglzxtb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtsolhhdvz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtaxnpzapm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtqgjxzulx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxuanxn.top/gtxliagfye.html

C#:   async Task F() { await G(); }
来源：http://hz.zhoulong.xyz/gtfuuklpmk.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinyuanbaomall.cn/gtxufbcauy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.snrcjt.cn/gtifryupzj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gthowsabxg.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtekiqbjut.html

TS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtoljicxie.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yanxiufei.cn/gtzmudyqgo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gaohongyu789.top/gtqjqabsvm.html

Ruby: threads.map(&:join)
来源：http://hz.ydjk.org.cn/gtpbimebzy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtxgfvqzno.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtuhbunkry.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gttpgjndmw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gtgfegcvta.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtuijfhgap.html

TS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtufchprfx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ybcxt.top/gttdwpgfxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtwguxstgx.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtpseegtrm.html

C#:   Parallel.For
来源：http://hz.hammf.cn/gtaxxwxane.html

================================================================================
来源：http://hz.ehwqpu.com/gtgugupctw.html

P. 常用工具函数
来源：http://hz.svipenyu.cn/gthemiwycg.html

================================================================================
来源：http://hz.jiagoushi.top/gtpubzhkee.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtnhsrbxnu.html

Py:   str(uuid.uuid4())
来源：http://hz.xingfuxueyuan.xyz/gtaeadeorx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtgxnkurak.html

JS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtbymwfhxm.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtdhhhwane.html

Java: UUID.randomUUID().toString()
来源：http://hz.pengpengdd.cyou/gtgeizbgzr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenjidiqi.icu/gtsfnkeepb.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtaaxcecqb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtcyiernjt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenzaomai.com/gtlgqzehtw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.0kj1m.cn/gtacbzeawc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtfxqtkvvt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenjidiqi.icu/gtsvgihpiz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nwbrower.top/gtspmkclgj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gthuirpwjh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtzeysgefi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sweek.top/gtlxnkozcg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tanke756.top/gtrxtqrzsb.html

[P03] 生成短随机字符串
来源：http://hz.shzxlz.cn/gtnbprfoyl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtupvrhvaj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yanxiufei.cn/gtugwnlaoo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtmcggzedf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtebbewdfr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgufenzy.top/gtbjfssyxr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sweek.top/gtbhjdbknt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtmwstqhsn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtzrdotyxz.html

[P04] 求长度
来源：http://hz.mhx1999.top/gttkovmskj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aibaodan.cn/gtplimdbgb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtdnhrsguc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtiveibqko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtylmvrgjl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtkdwqqply.html

Go:   len(arr);  len(m)
来源：http://hz.c1oappe.top/gtlurnragk.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtalumwxuk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgfzy.top/gtnfsdkdoi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ybcxt.top/gtqewdzqsd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yangfankeji.com/gtudverqrf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gtfpopgydz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daria6918.cn/gtpnmqalld.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtiatihwwt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nanxuanxn.top/gtyndkthot.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtmttmcdzj.html

Ruby: a == b
来源：http://hz.meibo888.top/gtgvhwytax.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gtipnslihs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtovyszhjd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtpvqhvzie.html

PHP:  if (empty($x)) {}
来源：http://hz.chenzaomai.com/gtqwqigzdz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gotoacloud.top/gtnqxcmpid.html

TS:   if (x == null) {}
来源：http://hz.jinyuanbaomall.cn/gtdidsrqwv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtrsovdvao.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gtdrqzlgue.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gtuvkznxuf.html

C#:   if (x is null) {}
来源：http://hz.xinyue.icu/gtovoyajzt.html

[P07] 防抖与节流
来源：http://hz.birdmap.top/gtrqhluzzd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gttclrovin.html

PHP:  // 手写时间戳比较
来源：http://hz.svipenyu.cn/gtqhxlrcob.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtagevwujx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtqqrjrlhh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gtslvurroc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shangyingyoupin.top/gtdasqbtot.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenjidiqi.icu/gtbhlfpsxz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtedhkmctg.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtjntjbsek.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj202588.top/gtfkluusmr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtlghlsuzt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtemciwbgw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yueranfly.top/gtqpwggmni.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.316326.xyz/gtihjkdyar.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cheryme.top/gtodhggwtu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtsazebhel.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhijiandao.cn/gtbolqqfwe.html

================================================================================
来源：http://hz.cdnleiting.top/gtpraizmsw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtybxrrzqw.html

================================================================================
来源：http://hz.yj20258.top/gtuofirnfo.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gthiyjipei.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtwtydzgvp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtnernqdok.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtyuoseiki.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgufenzy.top/gthpzlsryd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtydaskauf.html

);
来源：http://hz.nwbrower.top/gtunactucq.html

[Q02] 创建带外键的表
来源：http://hz.52xcode.cn/gtacgccwem.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtwpmiruli.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtzgnbvzoz.html

user_id INT NOT NULL,
来源：http://hz.tianlin.xyz/gtsrbcriwb.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtionamnxd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtcbqnsvqb.html

);
来源：http://hz.yvedp.cn/gtzdogqfjs.html

[Q03] 增加列
来源：http://hz.haohaochexian.top/gtayqxheln.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.meibo888.top/gtmfrsjcdp.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtiypapqbh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnxiangtu.top/gtlyykvxzg.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtcjaqfpok.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtqmbbfiwc.html

[Q06] 删除列
来源：http://hz.andypj.xyz/gtvrddkkzo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinghuilouyu.cn/gtutbsygbd.html

[Q07] 删除表
来源：http://hz.52xcode.cn/gtysgtxpyd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtxnipvjye.html

[Q08] 创建普通索引
来源：http://hz.gzhubu.top/gtbfqurvuk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtktrujrno.html

[Q09] 创建唯一索引
来源：http://hz.yonumen.top/gtusfrpsjz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtbmaalxtv.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtdvibkbpj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gogol.net.cn/gtdlipqovk.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtrqgpenww.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhiwuduotai.top/gtszqllgav.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtpaemnlef.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cheryme.top/gtdpvxtwbp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtsysbaaza.html

[Q13] 忽略重复插入
来源：http://hz.nwbrower.top/gtwhabwlfl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtadiglwzn.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtijjopzon.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtxnyucnmk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtkmnubjkj.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gtucfnuezd.html

SELECT * FROM users;
来源：http://hz.chenlongwang.top/gtrzkppobd.html

[Q16] 查询指定列
来源：http://hz.gzhubu.top/gtzuoggfxp.html

SELECT id, name FROM users;
来源：http://hz.shzxlz.cn/gtlbmttgkv.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtljdokrfb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtzrlnoyqp.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gtadrtuhlg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gthufnnojy.html

[Q19] 范围查询
来源：http://hz.nwbrower.top/gtmcdrkbuf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gteeebprwf.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtyrsopjep.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gtivqjtyns.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtbmozhlut.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtdgbnfsza.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtofdimswq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtydwpdnqs.html

[Q23] 分页
来源：http://hz.xinyue.icu/gtuwrhfhpd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gtkqfdzdxm.html

[Q24] 去重
来源：http://hz.chenjidiqi.icu/gtmheknsoq.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtppvvsmyz.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gtwrcfvpiw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtmjrrgmhw.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gtpkjjtzuy.html

SELECT COUNT(*) FROM users;
来源：http://hz.quarkkingdee.top/gtgkuhvekb.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtcygtplbr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gthnqrqeyu.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtjvqhffku.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtbdwyuzty.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtydfgrpki.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gtdclresro.html

[Q30] 分组统计
来源：http://hz.smart0.xyz/gttliqdmql.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtyfndeswm.html

[Q31] 分组后过滤
来源：http://hz.fzhhl.top/gthdqiuizm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.fengsongda.top/gtpnklhwfh.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtgkwevkhx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtxuioohim.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtaumrqfen.html

[Q33] 多列分组
来源：http://hz.zdqjudy.top/gtvymnivoq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtgzwqpngy.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtjngulgvz.html

SELECT * FROM (
来源：http://hz.chenlongwang.top/gtyqhfdgju.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtgmdzprev.html

) t WHERE rn = 1;
来源：http://hz.gotoacloud.top/gttneqjdlz.html

[Q35] 内连接
来源：http://hz.zhoulong.xyz/gtwgbisidf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtjpzoasqe.html

[Q36] 左连接
来源：http://hz.yj202588.top/gtpgfharvk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtvzzvqzuo.html

[Q37] 右连接
来源：http://hz.birdmap.top/gtvimnbexd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258888.top/gtauvjdpib.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.vqdsnc.cn/gtadqbgszv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtovqglgsi.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gttjwdvnih.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gthsaaedqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.kuanghao11.cn/gtubndzlnl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtxijslfzj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gtmovjobfw.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtihpsllno.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pycfn.com/gtpdjwmnys.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gterffxvjd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgfzy.top/gtjnnitcko.html

[Q42] 连接条件附加过滤
来源：http://hz.bjfxy.top/gtnitgxzqp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gtauemyamd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gzhubu.top/gtuinxhitk.html

[Q43] 标量子查询
来源：http://hz.zhaomingkeji.xyz/gtshxpvefx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtfhemojvt.html

[Q44] IN 子查询
来源：http://hz.tian-w.cn/gtqrbbwskl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zycfv.cn/gtbcuhrfil.html

[Q45] EXISTS 判断存在
来源：http://hz.yonumen.top/gtsbdzqyzf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtevbdcyeo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtinqhqkyy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtzgjtzdmk.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gtaejyhjdg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtnynsexbe.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtznqvixgc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtsqvwxgje.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258888.top/gtksbcoshr.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtxzcgftam.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jiagoushi.top/gtveuiyipk.html

[Q50] 批量更新
来源：http://hz.wangdashe.top/gtjdsgwlyx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gtvcpzvzlz.html

[Q51] 用子查询更新
来源：http://hz.bjfxy.top/gtwzueepoq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtbfpjidoi.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtvwuolxrc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtvoquhkqd.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtpskvmhwd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtirgbkeaa.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gthstqupzx.html

TRUNCATE TABLE logs;
来源：http://hz.fengsongda.top/gtxgqxywyj.html

[Q55] 排名（并列占位）
来源：http://hz.mhx1999.top/gtkjwieqbh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cdnleiting.top/gtkdpafxfk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinghuilouyu.cn/gthfnxqqwq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtgweqqpbe.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtyfikwviz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hongshengwenyu.top/gttcjhakov.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gtsmozxytk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhiwuduotai.top/gtohocjngb.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gtbgtqvibx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydzc1.top/gtqowzmhco.html

[Q60] 取上一行 / 下一行
来源：http://hz.nwbrower.top/gtleridqsu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnxiangtu.top/gtxfjgwgzj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sweek.top/gtfafqpwic.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtelvoixob.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtnqybvnql.html

[Q62] 分组占比
来源：http://hz.jinqigufen.top/gtqbxvfmtb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gthzokayxm.html

[Q63] 开启事务
来源：http://hz.tanke756.top/gtxwrzcqej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtkoyxpdoe.html

[Q64] 提交事务
来源：http://hz.aizwys.cn/gtotmnawgh.html

COMMIT;
来源：http://hz.guannengcc.top/gtsjkhrpko.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtzzfsehvx.html

ROLLBACK;
来源：http://hz.dashuyun.cn/gtjpmlnoxe.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gtvnroenin.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtsixcwyvg.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtpduelhlu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtjeodwvrc.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtrejwrfjm.html

SAVEPOINT sp1;
来源：http://hz.yueranfly.top/gtekytptbm.html


<!-- 参考信息 -->