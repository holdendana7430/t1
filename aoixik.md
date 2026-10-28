代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gthqcyyvat.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtmuiyvnci.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtmmuwgeta.html

Java: // 手写递归
来源：http://hz.fengsongda.top/gtbisccdvb.html

Go:   // 手写递归
来源：http://hz.quarkkingdee.top/gttjlbbbwd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtuulhfrrz.html

C#:   // 手写递归
来源：http://hz.9152youxi.cn/gtgzymxrwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtsqfsoilq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gaohongyu789.top/gtzvuscgnx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gtbbgfaaws.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtfoujbnvl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtfzqzqlqr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtcudopuvs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gtalzaeymk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gthvznwzlj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtdhrxoxte.html

================================================================================
来源：http://hz.hysaishi.cn/gtxqwexxla.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtbzzboutq.html

================================================================================
来源：http://hz.9152youxi.cn/gtiryqztlj.html

[O01] 启动一个线程
来源：http://hz.ppjwa.cn/gtmmajgbad.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtumcqhfsp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtqddaupel.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ybcxt.top/gtsmsmgzbb.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtseifkfka.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtxpwbczre.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtbfebkrhl.html

Ruby: Thread.new { f }
来源：http://hz.sweek.top/gtxzewtmdu.html

C#:   Task.Run(() => F());
来源：http://hz.xinyue.icu/gthabxsuez.html

[O02] 使用线程池
来源：http://hz.cheryme.top/gtjwtrqcgc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtnmpvwqlh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtslgumvtg.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtyaskmkhq.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtpcqlixnd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gthkrxniyz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jianghu66.top/gtprnezjjm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtbexlajbb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtroqrmrwi.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtapmgirlj.html

Py:   with lock: shared += 1
来源：http://hz.pycfn.com/gtzoxsevqd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtisqkrscv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtqeulvlnd.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gttzfyuryx.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuanzx.com/gtumytqzoc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtrhqufxig.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gtxcnlmpgh.html

C#:   lock (gate) { shared++; }
来源：http://hz.dashuyun.cn/gttaqaznjy.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtsrgddlks.html

Py:   async def f():⏎    await g()
来源：http://hz.gaohongyu789.top/gtnmbgirvg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtpfivkaol.html

JS:   async function f() { await g(); }
来源：http://hz.yuanzhike.top/gtjfzektsc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aizwys.cn/gturnmelfd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtuwiqthoo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinyuanbaomall.cn/gttrhklllp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxuanxn.top/gtdkmrtzgf.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgufenzy.top/gtkirarmho.html

[O05] 并发执行并等待全部完成
来源：http://hz.yongpay.top/gtbqjkplbf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtgzupjczu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yonumen.top/gtmzgyauzc.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtnlyjwrlq.html

TS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtbemiglpn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.redwolf501.top/gtysuxvysw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgfzy.top/gtrpewhjcu.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtrndtjzvq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtiphddzrj.html

[O06] 使用进程池
来源：http://hz.yangfankeji.com/gtoocycrys.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258.top/gtgojalgvc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtchmtlawc.html

JS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtrputfpku.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtwlhfebbv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gtqaezasla.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtsnkvbhbo.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtsmzadnkx.html

C#:   Parallel.For
来源：http://hz.xylfe.cn/gtrrydrhbs.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdwzikdsi.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtzzkaydjp.html

================================================================================
来源：http://hz.cheryme.top/gtevecggfn.html

[P01] 生成 UUID
来源：http://hz.aibaodan.cn/gtttfrybcp.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gtbgjgxlgj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtztxuobca.html

JS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtlrevtezk.html

TS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtinlquqls.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gtdblqscrj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtatciafji.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangtech.top/gtoegswpgl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtgapbvyrt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangshuangyany.cn/gtgkryhuyx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtkhiocbtd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sweek.top/gttejyqvqz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.c1oappe.top/gtmvvwilgh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjfxy.top/gtvnvwryhs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gthnkoqsho.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtqkiqvqkm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuetiantiany.cn/gtxlvvvseo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtduiazmfj.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtnrrfmihj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.quarkkingdee.top/gtieypybsg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtbghtlytw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtvsosurkn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtmrdhktit.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gthskblkgm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gtplonrwje.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.haohaochexian.top/gtynnzikfd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtedkhibxe.html

[P04] 求长度
来源：http://hz.zhixingplan.top/gtpesnahmr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhengqikj.top/gtphnpmegf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtgwccpgyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtufekdivh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hfpthk.cn/gtopnsrdjm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.snrcjt.cn/gtlvolmjvj.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtetjnhwty.html

Ruby: x.length;  x.size
来源：http://hz.birdmap.top/gtoinebztk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pengpengdd.cyou/gtcctlokqu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gtlcdubdhg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cdnleiting.top/gtytawqcab.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.0kj1m.cn/gtpridfszj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shangyingyoupin.top/gtxjfupeqn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gthdbmvajc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dianchejie.cn/gtawnreacx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.svipenyu.cn/gtupbixnta.html

Ruby: a == b
来源：http://hz.meibo888.top/gtbsltwniw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtkmboxvih.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtaojukaub.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtvkhcfwae.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gttudcxgdq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtxuppfvdq.html

TS:   if (x == null) {}
来源：http://hz.snrcjt.cn/gtdcdamclw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xziqi.cn/gtnbhacqfz.html

Go:   if x == nil {}
来源：http://hz.0kj1m.cn/gtpuqyshqd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cashguo.top/gtwnsltjjp.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtfoblelpr.html

[P07] 防抖与节流
来源：http://hz.redwolf501.top/gtrtzjizsc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.snrcjt.cn/gtmeejnrge.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtkaubsucr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtcpxwuhpy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtilywchyw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtzatninfa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtxgystxak.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtysdxhufy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cucudq.cn/gtdhcuqdvq.html

[P08] 处理浮点精度问题
来源：http://hz.pycfn.com/gtfpaqitip.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xinyue.icu/gtdzggidir.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtrwexyjhu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhiwuduotai.top/gthzzirqni.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtnmrooyjk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhiwuduotai.top/gtedynfpnb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gtbznzinch.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtmetmeeli.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cdnleiting.top/gtfybjlcsf.html

================================================================================
来源：http://hz.jiagoushi.top/gtsbhfpcci.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xziqi.cn/gtxhsflqhf.html

================================================================================
来源：http://hz.shuidangran.top/gtxovvdkfp.html

[Q01] 创建表
来源：http://hz.daria6918.cn/gtkomxqcjf.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtztuctity.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtxlzpxthl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtnfplhsph.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhongyouzk.top/gtinqvaomd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.0kj1m.cn/gthabablmq.html

);
来源：http://hz.snrcjt.cn/gtothnmeya.html

[Q02] 创建带外键的表
来源：http://hz.meibo888.top/gtprtcrqki.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gtbsmsirqe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtqivldfrz.html

user_id INT NOT NULL,
来源：http://hz.chenjidiqi.icu/gtzpirakci.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtcbhvfpat.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gtxmcwntky.html

);
来源：http://hz.chenlongwang.top/gtzeermaag.html

[Q03] 增加列
来源：http://hz.cheryme.top/gtnpdzqttl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtuitkocfs.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtglyersyq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gtvwpahkde.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtzmlbixnc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ybcxt.top/gttiyibbqt.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtdwxbxtow.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.andypj.xyz/gtytzvqoqf.html

[Q07] 删除表
来源：http://hz.yvedp.cn/gtjizwldif.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenzaomai.com/gtdaftciif.html

[Q08] 创建普通索引
来源：http://hz.zhoulong.xyz/gtpuogcwig.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtzdkaupem.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtgpurncpe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtilkbdgqf.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gttyvczpge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nwbrower.top/gtpgkalybu.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtqgtrtjyu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sxryk.cn/gtdicylzhx.html

[Q12] 插入后取自增 ID
来源：http://hz.xuanzx.com/gtbuthddad.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gthznlmppx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gtxgzuviak.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gttplgfbds.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hysaishi.cn/gtowznkrsz.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtkqjifzcf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtonucvavp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tanke756.top/gthphganeb.html

[Q15] 查询全部
来源：http://hz.tanke756.top/gtuorjxjyp.html

SELECT * FROM users;
来源：http://hz.nanxinkj.top/gtoehgkhdj.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtffpfdhap.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtkivyztmj.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtrhygnbzw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daxiang520.top/gtmojtcauq.html

[Q18] 模糊匹配
来源：http://hz.svipenyu.cn/gtbcdxbewx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dianchejie.cn/gtlxvfudnx.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtxqrerelq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangdashe.top/gtarpldejh.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtokrputqx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hfpthk.cn/gtwmgzqlen.html

[Q21] 空值判断
来源：http://hz.zhijiandao.cn/gtnedkuolg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gtgxyovouy.html

[Q22] 排序
来源：http://hz.cdnleiting.top/gtwzrwbawn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yongpay.top/gtkwksfrfq.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtvrfimxsj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hammf.cn/gtnsptgfzk.html

[Q24] 去重
来源：http://hz.guannengcc.top/gtnswixjkz.html

SELECT DISTINCT city FROM users;
来源：http://hz.cucudq.cn/gtxemakyil.html

[Q25] 只取前 N 条
来源：http://hz.xingfuxueyuan.xyz/gtefymxheu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hammf.cn/gtpornyfuv.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gtglbyimdm.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtcibvulwq.html

[Q27] 条件计数
来源：http://hz.yj202588.top/gtmooshhhy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hfpthk.cn/gtrvdusqsl.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtkczkgtbf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtaolyenof.html

[Q29] 最大最小值
来源：http://hz.ydzc1.top/gtubdbybji.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtomgsvaen.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtyodznezz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gthzkgtark.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gthgqqxisi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtxajzdksy.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtfvqktuel.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtqqpdpewl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuetiantiany.cn/gtfcfnrtor.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtnnkianfq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtjcewuvbd.html

[Q34] 每组取第一条
来源：http://hz.sufxvd.cn/gtetmxgfqe.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gtqqjjaekr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigufen.top/gtgoowphse.html

) t WHERE rn = 1;
来源：http://hz.cdnleiting.top/gtmultalqz.html

[Q35] 内连接
来源：http://hz.shanyushiyangtech.top/gtrnciyfsz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtteitnjtj.html

[Q36] 左连接
来源：http://hz.jinghuilouyu.cn/gtymvnhcrp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtzfqtgkkw.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gttkrotcfb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gtljfgtrxb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ivvv.top/gtnysdvuay.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daxiang520.top/gtisgphlkv.html

[Q39] 自连接（查上下级）
来源：http://hz.ppjwa.cn/gtiitzgdhh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtrscxsisj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydjk.org.cn/gtcfazzcse.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.andypj.xyz/gtifmzqmmd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtisboprwh.html

[Q41] 多表连接
来源：http://hz.chenlongwang.top/gtmsfcbbyy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigufen.top/gtzjwtickz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gttezprrqi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.meibo888.top/gtyzidqmwc.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtirtfgmtn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xinyue.icu/gtbexwqniz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ehwqpu.com/gtdxjjfzjz.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtxzfjhbhe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gtecujxfij.html

[Q44] IN 子查询
来源：http://hz.jinqigufen.top/gtadujqjyx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtokarnlew.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtmnmdlqrl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtplocfurk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gthaydwavn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtsvxoqooq.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gthpzkjgaw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtwtaalypv.html

[Q48] CTE 公用表表达式
来源：http://hz.zycfv.cn/gtqwycrale.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sufxvd.cn/gticjdetst.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtyztktvyq.html

[Q49] 更新单行
来源：http://hz.52xcode.cn/gtwxaedqql.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xylfe.cn/gtfnmshfvs.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtdspxuitp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtzklcwiya.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtcrkfuhkx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xinyue.icu/gtdqbdqqxp.html

[Q52] 删除指定行
来源：http://hz.aibaodan.cn/gtqqcjvvux.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hywenlv.cn/gtyygrpolw.html

[Q53] 按条件删除
来源：http://hz.daxiang520.top/gtbizngsmk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinghuilouyu.cn/gtnfvjmjiv.html

[Q54] 清空表
来源：http://hz.yvedp.cn/gtebkgelys.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtcwysbpzv.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtzdatfclc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gttsouhfas.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtxyqkwvct.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenlongwang.top/gteemjgmse.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtffbhiwpr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtblayirco.html

[Q58] 累计求和
来源：http://hz.guowangkeji.top/gtnshmawhs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtwmaxwvqv.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtwiqmwnrz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtetinztek.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenlongwang.top/gtygukpnut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pycfn.com/gtshrncdso.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cashguo.top/gtjbaovcyw.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtlqxprlve.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtoxlzdzmq.html

[Q62] 分组占比
来源：http://hz.chenlongwang.top/gtsiyekjrw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtnnyxaegc.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtektntoyp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtjzzxgcdw.html

[Q64] 提交事务
来源：http://hz.jqgufenzy.top/gtympbopyd.html

COMMIT;
来源：http://hz.cashguo.top/gtzrjpedce.html


<!-- 参考信息 -->