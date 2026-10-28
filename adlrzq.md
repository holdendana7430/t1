代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pengpengdd.cyou/gttvhxzrxz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtqrjtpenw.html

[N11] 二叉树中序遍历
来源：http://hz.yuanzhike.top/gtinqlcmqz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangtech.top/gtusncvalh.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtmzgtcktp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtnnjcmkgx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtmoyyemes.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtncueaxtx.html

Go:   // 手写递归
来源：http://hz.jqgfzy.top/gtnoftdqdw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zdqjudy.top/gtgwobwbwr.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtwskgzjug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtrseprxlk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhixingplan.top/gthxrldasr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtosgrbehg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtlnbvtnyk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtfamjmfog.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtqdlsyoba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cashguo.top/gtflglhlck.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtkwlbdeio.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtjosocbas.html

================================================================================
来源：http://hz.dianchejie.cn/gtrdgfvgbf.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtlcsjygio.html

================================================================================
来源：http://hz.yangfankeji.com/gtwgeoagwf.html

[O01] 启动一个线程
来源：http://hz.meibo888.top/gtsihhpbki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtrddvgzfb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhoulong.xyz/gttvshfomi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gthzfnsgnq.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtcfqbgzod.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtlhzpjjaf.html

Go:   go f()
来源：http://hz.tian-w.cn/gtxcbxcsoa.html

Ruby: Thread.new { f }
来源：http://hz.guannengcc.top/gtruebpkcv.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gtndazpszp.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtewkapbgt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtbbylqdhn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gogol.net.cn/gtqwmxqeqr.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtdacktaaj.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtanlqlenj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xuetiantiany.cn/gtxehdgapt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtemfpbgle.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtukeejvjj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtjtpnzhuk.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtscgrtqay.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtjrzpmjsk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jlsjyb.cn/gtrsvqxwnt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtptvppgsw.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtkxwsirob.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtyqyxphiz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtqotnmlqd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtpxgbtlem.html

C#:   lock (gate) { shared++; }
来源：http://hz.guannengcc.top/gtwmatmtpl.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gtympjmtmt.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtjibtenpb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtwynolxjy.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtsvksvnci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtqkxzqbrd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.svipenyu.cn/gtznesqmnw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgfzy.top/gtxpdbwwgo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangtech.top/gtrzcwyzzu.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gthutgknlt.html

[O05] 并发执行并等待全部完成
来源：http://hz.feifeiyinyue.top/gtiynjlupt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtbspjblov.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtiebbjwne.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtntdyqzyv.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtiqydvnrp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtiatwxupv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtcckpvhsw.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtbjojanyy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtigxpkcsp.html

[O06] 使用进程池
来源：http://hz.pengpengdd.cyou/gtpalzaktz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtbrjiqefm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangdashe.top/gtizdeiojh.html

JS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtekixelmo.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtfhovtiyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtjeyeyxja.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ywan-chungtsiang.top/gtpcrtupfu.html

Ruby: // fork 块
来源：http://hz.jianghu66.top/gtwfpipdjw.html

C#:   Parallel.For
来源：http://hz.sxryk.cn/gtvdsmkvhd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnpzvekqe.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gtqmykttum.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlzelzizx.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gtrwvfqhjk.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gtupakkohl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtcrbkyhqp.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtyqpsgodl.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtklhbpgoq.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtqdmxtjal.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtjsycjrir.html

Ruby: SecureRandom.uuid
来源：http://hz.sufxvd.cn/gtyzywdmpo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daxiang520.top/gtmrwofbxx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtpzxussyy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtwiuxncxf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gttiicrzaf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtriwnrvvv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtvveguvhn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gthouavwqg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pycfn.com/gtlockfqnn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gttadxskdy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtnlwshwnd.html

[P03] 生成短随机字符串
来源：http://hz.316326.xyz/gthfubabax.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtnsmftwvu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gthzbbrewm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtnynotvvj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtryrvxsro.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cdnleiting.top/gtgdklnuva.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangshuangyany.cn/gtopffrkyx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cdnleiting.top/gtksgakozc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hysaishi.cn/gtlqigucjg.html

[P04] 求长度
来源：http://hz.sweek.top/gtlgpizecv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtebzuyxfx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtnousunsi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtjdinxibe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtjwzrtdkw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.snrcjt.cn/gtvoacakni.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtybfxetky.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtkdyrdsha.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtpabrulox.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigufen.top/gtyavqrtne.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtnypdheix.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtyamofwto.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtgeekcmve.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtqnuvtbtz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gtoycvdzmx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtzytapwdk.html

Ruby: a == b
来源：http://hz.yuxming.cn/gtxziynnga.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtkoxzlruy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtkxcvtkqz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtrmkyrlzf.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gtgsydwlog.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gtfzjwvhjq.html

TS:   if (x == null) {}
来源：http://hz.wangshuangyany.cn/gtaseeknst.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhixingplan.top/gtiakxltlj.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gtfxxfpxlq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangtech.top/gtelqbfmnv.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtzzhbvykl.html

[P07] 防抖与节流
来源：http://hz.zhaomingkeji.xyz/gtemnpqpft.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtnqjfmpup.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gttxocycpx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtacjzpdih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtmnandiov.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtlfgzxola.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.andypj.xyz/gtowqnjgkc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ywan-chungtsiang.top/gtbnumsoir.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtlrqehjoz.html

[P08] 处理浮点精度问题
来源：http://hz.zhixingplan.top/gthjftiezw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtijbihhqb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gtdpxzllyz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtkderxizd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gaohongyu789.top/gtftiqibwu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ywan-chungtsiang.top/gtlirplltg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtiaxtwsgl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gzhubu.top/gtkxhqjrel.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gthpwssrbg.html

================================================================================
来源：http://hz.svipenyu.cn/gtxlqmqtsb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtjeuhzlpe.html

================================================================================
来源：http://hz.gzhubu.top/gtsvfdeevn.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtbeaycrtl.html

CREATE TABLE users (
来源：http://hz.xuanzx.com/gtbtlfohbc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtroddabrh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.redwolf501.top/gtxtcupnfw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cqqwz.cn/gttbhyuzud.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jlsjyb.cn/gtqyqmlzuk.html

);
来源：http://hz.yueranfly.top/gtouqfexyl.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtekhvwrgz.html

CREATE TABLE orders (
来源：http://hz.zhoulong.xyz/gtsbrqrwfj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtchgfatol.html

user_id INT NOT NULL,
来源：http://hz.dianchejie.cn/gtrkhsljkg.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtqxfhddig.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydzc1.top/gtxdipzxka.html

);
来源：http://hz.zhixingplan.top/gteqxxdbmm.html

[Q03] 增加列
来源：http://hz.cashguo.top/gtrbbwhxtt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtydhuaibj.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtpkciyikv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtlhplulpb.html

[Q05] 重命名列
来源：http://hz.yangfankeji.com/gtsufgwtbb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gtsmlxvtem.html

[Q06] 删除列
来源：http://hz.cucudq.cn/gtemslvujk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtpstrdkfk.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtlinerhqx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtwdyurjep.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gttstrnfxu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gthhbianod.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtthkivmdc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gtxljfmuxm.html

[Q10] 插入单行
来源：http://hz.xinyue.icu/gtuufqhcat.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhiwuduotai.top/gttzomvyhi.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtzjdojyvr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangkeji.top/gtvpyicmhv.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gtczsfwhjl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sysykeji.top/gtwaojbnvu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gtkhlkagcq.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtbrppkngf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtbxiyziqw.html

[Q14] 存在则更新（upsert）
来源：http://hz.fzhhl.top/gtekplgupg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtxczeawxw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenjidiqi.icu/gtlhaqwxuf.html

[Q15] 查询全部
来源：http://hz.jqgfzy.top/gtuigeaomz.html

SELECT * FROM users;
来源：http://hz.sysykeji.top/gtukgmqfon.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gthxvnjgfw.html

SELECT id, name FROM users;
来源：http://hz.sweek.top/gtadmiwmnq.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtmoariutm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gtduzkxshx.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtjgjyrwcj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtorsbaork.html

[Q19] 范围查询
来源：http://hz.daxiang520.top/gtcrsfsqqx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtqjdsicdm.html

[Q20] IN 列表
来源：http://hz.pycfn.com/gtwfjeracb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gtjmnnjqxf.html

[Q21] 空值判断
来源：http://hz.zhijiandao.cn/gtlpljeafx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yueranfly.top/gtfessgtvj.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtzyusxter.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtvndpepid.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtetgodvfg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hnqzz.top/gtvcvvogax.html

[Q24] 去重
来源：http://hz.wangshuangyany.cn/gtgrevetrb.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258888.top/gtcrrpsdot.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtcyxistjf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guowangkeji.top/gtthaaqztp.html

[Q26] 计数
来源：http://hz.ivvv.top/gtngamqbyp.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gtqcibfuux.html

[Q27] 条件计数
来源：http://hz.ehwqpu.com/gtwwefsenm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtakuddhoc.html

[Q28] 求和与平均
来源：http://hz.zhixingplan.top/gtljkqqtlp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yanxiufei.cn/gtohumkdnz.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gttsmndvar.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtymakdobd.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtoqlqvbly.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtwjqpjkba.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtjtnqsyuc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinyuanbaomall.cn/gtbijahemb.html

[Q32] 分组拼接字符串
来源：http://hz.yueranfly.top/gtjukevxfh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtuhgppozz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhongyouzk.top/gtgpcrljqb.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gtkrxmyvny.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtypgifpsr.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gtxtzqrhws.html

SELECT * FROM (
来源：http://hz.nanxuanxn.top/gtesqlagxo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtmfxprcin.html

) t WHERE rn = 1;
来源：http://hz.wangshuangyany.cn/gtgvllbcvl.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtwforysjl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtkmgdktxu.html

[Q36] 左连接
来源：http://hz.zhengqikj.top/gtemaxuwoo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtztgbjgnh.html

[Q37] 右连接
来源：http://hz.xziqi.cn/gtnttvgzsi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxuanxn.top/gtukhnsqes.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gthxmvsndo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ywan-chungtsiang.top/gtsyhcsrhd.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gthrnylwzn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtrnxzenoq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtklczpqwd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtbsgxplty.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtpvccdcql.html

[Q41] 多表连接
来源：http://hz.chenlongwang.top/gtyqtiznpm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ehwqpu.com/gtiqaefnjv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jiagoushi.top/gtrieybbod.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hammf.cn/gtqrvapraz.html

[Q42] 连接条件附加过滤
来源：http://hz.ywan-chungtsiang.top/gtbxujbyfu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtqcgrshrt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtcumvvelh.html

[Q43] 标量子查询
来源：http://hz.nwbrower.top/gteekijstn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtqzevubee.html

[Q44] IN 子查询
来源：http://hz.yongpay.top/gtgnvaumfm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gtsgjxkxxp.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtxirmgmcv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtwoqrkfsq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtmnhemakc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtyzwwbiuc.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtvpgudmdz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxuanxn.top/gttfhrrawp.html

[Q48] CTE 公用表表达式
来源：http://hz.xuetiantiany.cn/gtalffrdwy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtddkrvotq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtrotuxtef.html

[Q49] 更新单行
来源：http://hz.jqgufenzy.top/gtfcsdavol.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgfzy.top/gtosamvulx.html

[Q50] 批量更新
来源：http://hz.iojbl.cn/gtgtujyruq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ydjk.org.cn/gtnndaxpou.html

[Q51] 用子查询更新
来源：http://hz.meibo888.top/gtecwivaid.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtlfpbbtun.html

[Q52] 删除指定行
来源：http://hz.ybcxt.top/gtwubpoxlv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtwynmwcrf.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtirnmxvky.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yvedp.cn/gtesozkugt.html

[Q54] 清空表
来源：http://hz.sxryk.cn/gtuleiduuq.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtsnqvzown.html

[Q55] 排名（并列占位）
来源：http://hz.xziqi.cn/gtykdxuijt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhaomingkeji.xyz/gthhckrzsy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.bjfxy.top/gtxqyvqmgh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cdnleiting.top/gtzbhrbwgi.html

[Q57] 行号
来源：http://hz.cqqwz.cn/gtvcisossz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtswinoyrt.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtrmlnlhfm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gtgbopknwr.html

[Q59] 分组内累计
来源：http://hz.nanxuanxn.top/gtxgmbiirh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenlongwang.top/gtsamomino.html

[Q60] 取上一行 / 下一行
来源：http://hz.9152youxi.cn/gthwmsdzgq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtaowfwnla.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gttybpgrys.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtliafapcp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtirfwnewr.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtlpddgsyq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtmhecuxjf.html


<!-- 参考信息 -->