代发 wailian999

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtqcbepxmd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigufen.top/gtyyunhwap.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtafyfkdof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tianlin.xyz/gtkhfhwkgk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtsnqnrqyw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtbrgqbivt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtgrokhwrz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtihcoypnd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtlciuoxys.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hongshengwenyu.top/gthpkogvor.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnxiangtu.top/gtppxclxmz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtbouflvcr.html

================================================================================
来源：http://hz.dianchejie.cn/gtaiswbvxg.html

O. 并发与异步
来源：http://hz.jinghuilouyu.cn/gtrdpkxrzv.html

================================================================================
来源：http://hz.52xcode.cn/gteyuyjgmq.html

[O01] 启动一个线程
来源：http://hz.shangyingyoupin.top/gthjcuckum.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gthnmudcmy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtzurcgfpu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cheryme.top/gtwqzbwjuy.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtebhkypmg.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtsvbxmbgw.html

Go:   go f()
来源：http://hz.nwbrower.top/gtgxginyor.html

Ruby: Thread.new { f }
来源：http://hz.hnqzz.top/gtsnpghwkp.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtcwmiatuo.html

[O02] 使用线程池
来源：http://hz.xylfe.cn/gtmivitrhi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gtiziwcugv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtwxpeyltk.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtrhjdqano.html

TS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtebmngshz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shzxlz.cn/gtbaqwsnpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.bjfxy.top/gtzbqrtrio.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dashuyun.cn/gtkfgfcluk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.iojbl.cn/gtvsjfypks.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtubnvjysd.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtiqzqknrp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daria6918.cn/gtvqhhsmfu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.havefunace.top/gtxfhlpmbm.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtalprjtvt.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gttfpchkhz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nwbrower.top/gtxslyyfvp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtggdcibxd.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtuexepegl.html

[O04] 定义异步函数并等待
来源：http://hz.chenlongwang.top/gtfmbhqver.html

Py:   async def f():⏎    await g()
来源：http://hz.gotoacloud.top/gtspmpulfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yvedp.cn/gthpzxxjzq.html

JS:   async function f() { await g(); }
来源：http://hz.gotoacloud.top/gtbnffpbiw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtmulvyhxn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtzjcbbnry.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aizwys.cn/gtxeuufebq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtqwxpilgi.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtszlvsmqc.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gtttfjmcdm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtviwalebm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.bjfxy.top/gtxamolgms.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtpsjghkqo.html

TS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtkwfvybsi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydjk.org.cn/gtwqgunqbk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gtvuesvxak.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gtmrergoak.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gtyfuxthlh.html

[O06] 使用进程池
来源：http://hz.svipenyu.cn/gtzalzvoxd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtxuxuakql.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtjhgubkla.html

JS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtjnjjggit.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtyxlpnfvz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtbmcnfuad.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtfvfynzuf.html

Ruby: // fork 块
来源：http://hz.ydjk.org.cn/gtuobupueq.html

C#:   Parallel.For
来源：http://hz.tanke756.top/gtjfdgrxhe.html

================================================================================
来源：http://hz.xziqi.cn/gtpwrvcnlc.html

P. 常用工具函数
来源：http://hz.ivvv.top/gttbszksxt.html

================================================================================
来源：http://hz.andypj.xyz/gteywjsste.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtpwvioomh.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtlwohqyju.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtizvydywz.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtwugyfbsu.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtecuawjje.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtoczrfyur.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtvygcsizp.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gtobfpumiq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtptpyqveo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtcrdrqjji.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtomklican.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtsniwqagh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhongyouzk.top/gtcxkioygg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pycfn.com/gtspafybwe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ppjwa.cn/gtjsvthimh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ppjwa.cn/gtydpazgow.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sxryk.cn/gtqlaettbv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gttpjqucju.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtrcxjehop.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtbyxkqxqb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gthstceipi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtrneswcsb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pengpengdd.cyou/gtessqiveu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gtjhtgwtzs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtwqmtkksz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangshuangyany.cn/gtftjjglus.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shangyingyoupin.top/gtdypxzmtg.html

[P04] 求长度
来源：http://hz.wangshuangyany.cn/gtdxyiyzqz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtukmicblf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtsrgskpow.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtznqdxqco.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtlzuoevka.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtscibpabk.html

Go:   len(arr);  len(m)
来源：http://hz.nanxuanxn.top/gtaekgrajn.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtynkunwxo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zycfv.cn/gtnviaxxah.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gtegweebmo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sufxvd.cn/gtqavumlrv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fengsongda.top/gttcsztxpl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtkdrtepvi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gtkowpmghb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgufenzy.top/gtegfjuftb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtsowecpya.html

Ruby: a == b
来源：http://hz.chenzaomai.com/gtnbmyrvck.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtkqkjfgsw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtugmaxsip.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gtllgptiig.html

PHP:  if (empty($x)) {}
来源：http://hz.zhiwuduotai.top/gtesurmktn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtgbvtqedv.html

TS:   if (x == null) {}
来源：http://hz.zhongyouzk.top/gtznwayrot.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtjfplgrdx.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtdnrsppww.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhaomingkeji.xyz/gthgdkxvgs.html

C#:   if (x is null) {}
来源：http://hz.meibo888.top/gtsvxaphea.html

[P07] 防抖与节流
来源：http://hz.cdnleiting.top/gtzrrieeqs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zdqjudy.top/gtjiqypagn.html

PHP:  // 手写时间戳比较
来源：http://hz.cheryme.top/gtptnjibjm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtmxpcperw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtgwmbwnzf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtxpaglqvx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fengsongda.top/gtzarykvvz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hywenlv.cn/gtidksrzil.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigufen.top/gtbmtybbln.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtuntdxobv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gtwgbwngof.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtfuzrmavu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jiagoushi.top/gteydimnyh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgfzy.top/gtgqxnxxrk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gttggatfts.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtrsosjerj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.iojbl.cn/gttiqrignd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gtwpglhice.html

================================================================================
来源：http://hz.ydzc1.top/gtrqomevke.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hongshengwenyu.top/gtebwvhlhe.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtjmphvrzf.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtfcykwpji.html

CREATE TABLE users (
来源：http://hz.cashguo.top/gtztptlsba.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtvuervthf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtdgsyktyy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gtbpailcoi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtjacridso.html

);
来源：http://hz.gotoacloud.top/gtuqscphkk.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtswhcehcc.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtinmvuhoh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtdnpfwfhp.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtcmenrhtq.html

amount DECIMAL(10, 2),
来源：http://hz.redwolf501.top/gtrydhsvfw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gtjtxgejkx.html

);
来源：http://hz.andypj.xyz/gtzpmuhlto.html

[Q03] 增加列
来源：http://hz.shanyushiyangkeji.top/gtlecxqdhs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtdzkfwdgh.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtaymzqbqq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xylfe.cn/gtnscdoswb.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gttnrlyjzp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gtgmaccasg.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtvostkfca.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtugivgcry.html

[Q07] 删除表
来源：http://hz.hnqzz.top/gtubqdceny.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnqzz.top/gtxhevrysn.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtswyqmfsc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gtoaahzmmo.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtxykaabry.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtbujgzgzq.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtsuhaemly.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.havefunace.top/gtlzxnlzmh.html

[Q11] 一次插入多行
来源：http://hz.sweek.top/gtpagxacdg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gtxguixhar.html

[Q12] 插入后取自增 ID
来源：http://hz.ydzc1.top/gtmsnpndys.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guannengcc.top/gthrknzkxo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtauvdoapd.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtiznaucre.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuxming.cn/gtxzeupcxz.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gtkcimlkyn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtsqlzoyji.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xziqi.cn/gtgqtzbhol.html

[Q15] 查询全部
来源：http://hz.andypj.xyz/gtsyvmulun.html

SELECT * FROM users;
来源：http://hz.ydzc1.top/gtxnuoifwm.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtkhpzpels.html

SELECT id, name FROM users;
来源：http://hz.ppjwa.cn/gtykgpumbn.html

[Q17] 条件查询
来源：http://hz.jinqigfzy.top/gtainxzpnh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yonumen.top/gtqhfzyysy.html

[Q18] 模糊匹配
来源：http://hz.xuetiantiany.cn/gtvelaimva.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtymdywspe.html

[Q19] 范围查询
来源：http://hz.nanxuanxn.top/gtzuvrzdmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtbansueac.html

[Q20] IN 列表
来源：http://hz.nwbrower.top/gtshofdwba.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shangyingyoupin.top/gtcmtujbyt.html

[Q21] 空值判断
来源：http://hz.ydzc1.top/gtsvcqboen.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtokprdtdv.html

[Q22] 排序
来源：http://hz.ydzc1.top/gtbymaoath.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtfojmdgdb.html

[Q23] 分页
来源：http://hz.xinyue.icu/gtjhprcpci.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.redwolf501.top/gtohlkfwof.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gtpzcljfqj.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj202588.top/gtoftzjcri.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtxtqjmnpa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtfeolaafs.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtnxlotlkp.html

SELECT COUNT(*) FROM users;
来源：http://hz.redwolf501.top/gthenqxcne.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtithpzsqz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gtrbqhwgiu.html

[Q28] 求和与平均
来源：http://hz.hysaishi.cn/gtxrtmljga.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenzaomai.com/gtekqknvnr.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtoeqcnlpf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.c1oappe.top/gtuqsuehek.html

[Q30] 分组统计
来源：http://hz.shanyushiyangtech.top/gtikxojjod.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtpqkfgddv.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gtuzwsohlc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtrvvigduj.html

[Q32] 分组拼接字符串
来源：http://hz.yongpay.top/gtmwrxkvcn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtmljegrni.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgfzy.top/gtytvgpdgf.html

[Q33] 多列分组
来源：http://hz.havefunace.top/gtzwsfyhgl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtxjqkncnn.html

[Q34] 每组取第一条
来源：http://hz.mhx1999.top/gtxkypexwq.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtyvanuamr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtjjwfqrmv.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtwatrfgga.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gthrxsjuqy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtkivzwtuh.html

[Q36] 左连接
来源：http://hz.yongpay.top/gtusqorhsf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gtjndaegtr.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtwsrlgnam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guowangkeji.top/gtqelmxvvb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.andypj.xyz/gtvuzewigi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtyjwxsfsb.html

[Q39] 自连接（查上下级）
来源：http://hz.redwolf501.top/gtuquwswuy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtmkmvqzsn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtivflfshe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtnpcgaxbs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xziqi.cn/gtbbzrxiup.html

[Q41] 多表连接
来源：http://hz.aibaodan.cn/gtwidugilg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtiltzeway.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtotvqshyy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtzkpgcjtq.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtnrbmqaaa.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtszzdvite.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pengpengdd.cyou/gtkmqshngx.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gtqsuypzsk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtcwvhvzcy.html

[Q44] IN 子查询
来源：http://hz.chenjidiqi.icu/gtyffwmglw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxinkj.top/gtrflknhos.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtjffnovwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtruucixld.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gtdayxlpfb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtjndbhklb.html

[Q47] 与平均值比较
来源：http://hz.chenjidiqi.icu/gtavxetmjm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnqzz.top/gtuksousyl.html

[Q48] CTE 公用表表达式
来源：http://hz.chenjidiqi.icu/gthyjgacdg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shzxlz.cn/gtbqxjdqcq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxuanxn.top/gtkqjesjba.html

[Q49] 更新单行
来源：http://hz.sysykeji.top/gtefyheprg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gttwaodoxo.html

[Q50] 批量更新
来源：http://hz.tianlin.xyz/gtxugfdqxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tian-w.cn/gttobibtcn.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtndgeefot.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangkeji.top/gtdlotggqx.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtujpyzcwf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guowangkeji.top/gtthuimrwd.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtjlgugnxb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hfpthk.cn/gtkzpjsftf.html

[Q54] 清空表
来源：http://hz.andypj.xyz/gtmpwcpqnd.html

TRUNCATE TABLE logs;
来源：http://hz.tanke756.top/gtzqnnkfln.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtglzezqxy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daxiang520.top/gtmvgnyznm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gogol.net.cn/gtmzwfyasf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cucudq.cn/gtervudefs.html

[Q57] 行号
来源：http://hz.zycfv.cn/gthdctusmf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shuidangran.top/gtkytcsdgw.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtshimdnmz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtegpjfpos.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtysnitlrj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guannengcc.top/gtxfabczyo.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtedllvkzc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenlongwang.top/gtlkpsvotu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtgumnswjv.html

[Q61] 移动平均
来源：http://hz.jiagoushi.top/gtfsxzzqna.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ydjk.org.cn/gtpynvqhkp.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gtzpdkaphm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtrgescujg.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtxgwzupne.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ppjwa.cn/gtjhkrsrhm.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtysnmzkop.html

COMMIT;
来源：http://hz.gotoacloud.top/gtzamlsldu.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gtpntfbrwc.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtjptrnpkw.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtaaxosoly.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.quarkkingdee.top/gtfulbxlgn.html


<!-- 参考信息 -->