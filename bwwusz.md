代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtshklvutp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gtvemfnbvf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xziqi.cn/gtcwjkxdhh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtxuwmxbkr.html

================================================================================
来源：http://hz.jqgfzy.top/gtczpvecfp.html

O. 并发与异步
来源：http://hz.cdnleiting.top/gtapqtoteb.html

================================================================================
来源：http://hz.xuanzx.com/gtnwhjzxnh.html

[O01] 启动一个线程
来源：http://hz.bjfxy.top/gthrixeutd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aibaodan.cn/gtakqpdgox.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.meibo888.top/gtmjwyxcxx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhijiandao.cn/gtutxefwqx.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtwhzwnsjs.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gtszmmowiu.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtinbhzfsn.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtfpgunzfu.html

C#:   Task.Run(() => F());
来源：http://hz.jiagoushi.top/gtrvebczfy.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtovqyppym.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zdqjudy.top/gtlslphvme.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtxfleqxvj.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtxrjbqans.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtbwntbhxo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtejhfoghz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gtgvjijnqh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigufen.top/gtbigmkphb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cucudq.cn/gteuhhpgki.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gttuzkbxnl.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtxpmjndab.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtltjfowzm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gotoacloud.top/gtnyecyygq.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtjowgmwcz.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtngmuqquf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigufen.top/gtwlagigva.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtelmfkqkc.html

C#:   lock (gate) { shared++; }
来源：http://hz.redwolf501.top/gtahjuntkl.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtehzibhul.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gtkifzufjs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtgbykajgv.html

JS:   async function f() { await g(); }
来源：http://hz.svipenyu.cn/gtpyhykyfr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gthxatitlv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtviuohfku.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtsfxylgar.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtfohkiogv.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtkjrsvvbz.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtqqgwclds.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gturqjeowi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtgkpljhzk.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gthtnnypra.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtdszmmkws.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtswrnhwpi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tanke756.top/gtqtmbefuu.html

Ruby: threads.map(&:join)
来源：http://hz.shuidangran.top/gtnsmnmnjz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtddnivbbh.html

[O06] 使用进程池
来源：http://hz.sysykeji.top/gtxhpvntjq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnqzz.top/gtjwwnoyty.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtuwyevcbp.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtybjhkzsi.html

TS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtqtdntjqo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fengsongda.top/gtuafvicxd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gtcnhebqya.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtsaqknqoh.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtgvvagzxr.html

================================================================================
来源：http://hz.ydzc1.top/gtvcgewivs.html

P. 常用工具函数
来源：http://hz.hnqzz.top/gtvuleuvrl.html

================================================================================
来源：http://hz.cashguo.top/gtvakfgvhu.html

[P01] 生成 UUID
来源：http://hz.hnqzz.top/gtwydpgabf.html

Py:   str(uuid.uuid4())
来源：http://hz.ybcxt.top/gtbraqtpqg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258888.top/gtfbtlcyzv.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtpzofnalz.html

TS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtyuvgjszs.html

Java: UUID.randomUUID().toString()
来源：http://hz.nwbrower.top/gtdkyvtiyq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtepklkqkr.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gthrqemcvu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.c1oappe.top/gtgivtjmka.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pengpengdd.cyou/gthnokiits.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gtwobaatli.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ybcxt.top/gtfescyase.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jyoumei.cn/gtufsjcvna.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtcgfjyear.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinyuanbaomall.cn/gtyvzufxwt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daxiang520.top/gtefuczgyw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gtpvkevgmw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtlfebuqju.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtkttufcwj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtgqwosmcw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gtoapiithx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtigwnglol.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gthsidzivv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.mhx1999.top/gtbbsyqtpu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtxqybicwa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tanke756.top/gtnvjgwuqf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtiiezlycn.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gthcuuaror.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtphxmefqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtskzroyxm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gthpusygbq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtwspvluzx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.meibo888.top/gtweuimsla.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtwmhrebbs.html

Ruby: x.length;  x.size
来源：http://hz.chenlongwang.top/gtcawtrcsf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.iojbl.cn/gtbzsuxvbe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gttbhgxuhb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yvedp.cn/gtvmbtzwxs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtosrwvdzt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhixingplan.top/gtdnpuqkyi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtyxplfwsk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jyoumei.cn/gtwiqzhxfx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.iojbl.cn/gtumucqxcb.html

Ruby: a == b
来源：http://hz.andypj.xyz/gtidasputr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtyzspoqxr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgufenzy.top/gtyafarqpq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gtovzegcwa.html

PHP:  if (empty($x)) {}
来源：http://hz.hfpthk.cn/gttrppkcny.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtjcsouebu.html

TS:   if (x == null) {}
来源：http://hz.iojbl.cn/gtqpstppnj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtxcalxfqe.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtdykexbxp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aibaodan.cn/gtzhmhghyf.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtrrcbsmen.html

[P07] 防抖与节流
来源：http://hz.tianlin.xyz/gtuzursuey.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gteigsisef.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtjlkljzvi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtughvsmnv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtoupdanyy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.feifeiyinyue.top/gtjqxcocic.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinyuanbaomall.cn/gtlbrmqpgg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tanke756.top/gtyqornwti.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj202588.top/gtfgbidnxj.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtftaizgwd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gtbykamuaz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtotcywnkz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtvisacqhi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtnoaqludo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gtwxlsojik.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtcgkuipyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtihdvjdvt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtqqvfqycx.html

================================================================================
来源：http://hz.fengsongda.top/gtvpfspaae.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtuzjzkktw.html

================================================================================
来源：http://hz.nwbrower.top/gtxnigklcd.html

[Q01] 创建表
来源：http://hz.bjfxy.top/gtlimvdmqk.html

CREATE TABLE users (
来源：http://hz.ydzc1.top/gtpqkrljko.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gthkuvbpvk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtwmlwrdzy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.birdmap.top/gttjzzyoki.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fzhhl.top/gtkkaunyqd.html

);
来源：http://hz.hysaishi.cn/gtkzdeepsv.html

[Q02] 创建带外键的表
来源：http://hz.jiagoushi.top/gtxwexvetm.html

CREATE TABLE orders (
来源：http://hz.hnxiangtu.top/gtafmgqudb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtaadmjfxh.html

user_id INT NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtnaiqqpsu.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtivvyjken.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gtdhwvztst.html

);
来源：http://hz.jiagoushi.top/gteyrdcoyh.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gttzwbzyub.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.0kj1m.cn/gtigihzumk.html

[Q04] 修改列类型
来源：http://hz.yuanzhike.top/gtgyogywbk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sufxvd.cn/gtffynmiqd.html

[Q05] 重命名列
来源：http://hz.yj202588.top/gtwxxyamed.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtdiszsbkw.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtkrthobgp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtuxhjtvcw.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtiboavqaw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtgwltdtrg.html

[Q08] 创建普通索引
来源：http://hz.redwolf501.top/gtfstqqkot.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hammf.cn/gtwvlbulud.html

[Q09] 创建唯一索引
来源：http://hz.aibaodan.cn/gtggxhqwhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.havefunace.top/gthrvupfvh.html

[Q10] 插入单行
来源：http://hz.hongshengwenyu.top/gtqbdmsngj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtxlhsunam.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtkekhmlzt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtkkegvuoj.html

[Q12] 插入后取自增 ID
来源：http://hz.haohaochexian.top/gtmdmpkkzw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xinyue.icu/gtyvlvhkxf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ybcxt.top/gtexlphmft.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtwyjxkmef.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtllweypyb.html

[Q14] 存在则更新（upsert）
来源：http://hz.tian-w.cn/gthuexiavr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtkcdvsxpy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtojfznjmz.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtqfanoupi.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtklarqlat.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gthjbxambc.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtqtpmpqep.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtomczipxd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shzxlz.cn/gtxvrcolaa.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtraxuhggz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sxryk.cn/gtocuvatnj.html

[Q19] 范围查询
来源：http://hz.snrcjt.cn/gtlmfcdxtd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jyoumei.cn/gtocqsnvop.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtfprdadmf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.birdmap.top/gtsrdhojfm.html

[Q21] 空值判断
来源：http://hz.yj202588.top/gtwlceadgr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gteadmhojw.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtxkvxkyht.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxinkj.top/gtkplxffwe.html

[Q23] 分页
来源：http://hz.hnqzz.top/gtmltwcmhe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtzggliuwh.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtyoalanrm.html

SELECT DISTINCT city FROM users;
来源：http://hz.bjfxy.top/gtiodoiocy.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gtettotujv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gtefmlydkv.html

[Q26] 计数
来源：http://hz.shuidangran.top/gthdflddmb.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtenyquxnf.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtoimsosez.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuetiantiany.cn/gtgxutlfyl.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtwqtnxvre.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yonumen.top/gtkwphlfpc.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtkzcmpjyb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtxwpyyxmn.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtagittcxv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtiihczono.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtgzduaytp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dashuyun.cn/gtcwxedpci.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtpavzstbo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtvsogkhqw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fengsongda.top/gtwkcemcvz.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtnzfgxqcm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fzhhl.top/gtvzekcxwo.html

[Q34] 每组取第一条
来源：http://hz.zhijiandao.cn/gtmipxgulo.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtfgtdyvqq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtzvvnkrgv.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtzuxzmnzd.html

[Q35] 内连接
来源：http://hz.hnxiangtu.top/gtolbwbsxx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gtpfbqoovu.html

[Q36] 左连接
来源：http://hz.hfpthk.cn/gtcbwnmsps.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtehhtzmwl.html

[Q37] 右连接
来源：http://hz.0kj1m.cn/gtnepwvhgy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtahobgjlw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtufudtlpe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gteyeqdvju.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gtznbhrdby.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtduyrprsp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtvzqbcydc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtctgkiykp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gtckobgbgx.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtbgtuhuap.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtbpyntiks.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtnboswmlm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gtxttysore.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gtuwpczmke.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtnsukhzhv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtrbuwumxm.html

[Q43] 标量子查询
来源：http://hz.quarkkingdee.top/gtnyqdmlfc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gttfrvqdlt.html

[Q44] IN 子查询
来源：http://hz.guannengcc.top/gtseyzphhl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aizwys.cn/gtlxqxqref.html

[Q45] EXISTS 判断存在
来源：http://hz.zhongyouzk.top/gtuowezwxw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtmvopofie.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtysgpzrbk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtqnybfxhz.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtuplwmnbu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gtqftchdjs.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtyuhhqmke.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pengpengdd.cyou/gtceqltvlq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtpqidedao.html

[Q49] 更新单行
来源：http://hz.jinqigfzy.top/gtjoqmzzwr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtzqlxtbix.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtxosnwzfq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gthduodmwe.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtawilpdkn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtcflrjges.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtmastnhxn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtqhlskiib.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtcolggcfz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenlongwang.top/gttiinegis.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gtpjtrtvog.html

TRUNCATE TABLE logs;
来源：http://hz.zhongyouzk.top/gtdedxyiqt.html

[Q55] 排名（并列占位）
来源：http://hz.gogol.net.cn/gtvjidnnqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.feifeiyinyue.top/gtbwvwthfg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtiiifpvwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tianlin.xyz/gtzvlmrfyp.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtsgishqma.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.birdmap.top/gtulpwjymq.html

[Q58] 累计求和
来源：http://hz.andypj.xyz/gtwcypppnu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtosvzwbem.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtagsegdmf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tianlin.xyz/gtjurozrlh.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtcqhghogt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuetiantiany.cn/gtpqsujfgs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgufenzy.top/gtrkoujjow.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtghuuqitp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenzaomai.com/gteidbymfz.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtveqasfqu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gttwhreczl.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtsbtgvccc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtcuilyhly.html

[Q64] 提交事务
来源：http://hz.andypj.xyz/gtaqndcind.html

COMMIT;
来源：http://hz.jyoumei.cn/gtkzjruvlj.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtfjngswhc.html

ROLLBACK;
来源：http://hz.snrcjt.cn/gtspfmrpcw.html

[Q66] 行锁查询
来源：http://hz.yonumen.top/gtlmyhwltj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtfnqvbexh.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gthyzuofum.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtkeajgvfk.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtqxubxfey.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtevmtsgaj.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtpfzbmhrw.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangkeji.top/gtbvjuppfs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gteauhtnmq.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtfjynqvio.html


<!-- 参考信息 -->