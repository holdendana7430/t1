代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pycfn.com/gteeuoanzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sysykeji.top/gtqymdioma.html

Java: class Node { int v; Node next; }
来源：http://hz.hnxiangtu.top/gtfkxvvcgq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenjidiqi.icu/gtselborun.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yanxiufei.cn/gtatlnkwkd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtllxkwcnu.html

[N11] 二叉树中序遍历
来源：http://hz.sufxvd.cn/gtmpcdszac.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtoiokaooq.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtsjgdbnyh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtkuahoitg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtcwrycnez.html

Java: // 手写递归
来源：http://hz.yj20258.top/gtyytuxflx.html

Go:   // 手写递归
来源：http://hz.andypj.xyz/gthbepdxyd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gtupyuwlfp.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtzhnchyqv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gtxsdjrkpv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtbivrhfaz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hywenlv.cn/gtetnvvhlx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtxdrrguoa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtnnetdkcv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtdvpumhvp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtkbccqizd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gtuixqjlbg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gthyyfufsx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpglqgyin.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtfnskeanw.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmixzyhim.html

[O01] 启动一个线程
来源：http://hz.cheryme.top/gtafbxilze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtrafwetny.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtjgqprsqd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtkzvjderh.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gthccqsqcj.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtlmkdpenu.html

Go:   go f()
来源：http://hz.jqgfzy.top/gtbaqowfkd.html

Ruby: Thread.new { f }
来源：http://hz.ppjwa.cn/gtrhmdtdfm.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtltzjnwmu.html

[O02] 使用线程池
来源：http://hz.ivvv.top/gtzbhahcgv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtszllmnzx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtbblvriek.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtxiiociyz.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtippvsxja.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yonumen.top/gtfgxioqwa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuetiantiany.cn/gtixbtelyy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtoyaxbhcu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hywenlv.cn/gtpjlsenvi.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtzasigqko.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gtyrfamdcw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cucudq.cn/gtymyltrev.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gtcuaaozkf.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtjavgbjby.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtytmhsogc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hywenlv.cn/gtmifrawin.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtypfxeorx.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gtuloafxfv.html

[O04] 定义异步函数并等待
来源：http://hz.iojbl.cn/gtrymjqpzx.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtvkxqswmw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtszrtrwln.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtkmwtmoxp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtsmaegclz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gthjssfbdr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigfzy.top/gtnkvyistc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sxryk.cn/gtwyczgebp.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtjwkadpke.html

[O05] 并发执行并等待全部完成
来源：http://hz.sufxvd.cn/gtkzwomrkq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtumawlvng.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtvfzuxrvb.html

JS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtlnfkcitg.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtrvuzzlhz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gzhubu.top/gtlwcbihgw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zycfv.cn/gtjytybzgq.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtrevlqboj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.snrcjt.cn/gtzerbbudh.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtjkjtecal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtsqapezwb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhoulong.xyz/gtcwyrckuc.html

JS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtdqnmzrcd.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtqrasnsix.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtlpzzollc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtiuuufwnk.html

Ruby: // fork 块
来源：http://hz.cashguo.top/gtgpmqwcpt.html

C#:   Parallel.For
来源：http://hz.xylfe.cn/gtkyhbjmxz.html

================================================================================
来源：http://hz.daxiang520.top/gttaruhjms.html

P. 常用工具函数
来源：http://hz.shuidangran.top/gtxqbsaxao.html

================================================================================
来源：http://hz.tianlin.xyz/gtpcgovrcj.html

[P01] 生成 UUID
来源：http://hz.zhixingplan.top/gtzgybjvzo.html

Py:   str(uuid.uuid4())
来源：http://hz.tian-w.cn/gtgzycvqml.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daxiang520.top/gtqmibrljg.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtmbqrastf.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtimvhylga.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gticojytuy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtfgfoqtru.html

Ruby: SecureRandom.uuid
来源：http://hz.yj202588.top/gtiaacqzge.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zdqjudy.top/gtecggtpgy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cdnleiting.top/gtnsxvrezd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtgdxvfgyz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sufxvd.cn/gthxtcijox.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtaqcsioet.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sweek.top/gtnwxqhxcv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtszbpryij.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gtbhsajctq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gtrixpshpg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtmdyqcevd.html

[P03] 生成短随机字符串
来源：http://hz.jqgfzy.top/gtthhqsgil.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtpvefkvgn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuanzx.com/gtwqjjhxbc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtssbodmjr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtzuybeevc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shzxlz.cn/gtqhblayze.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtflxsoztf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenlongwang.top/gtgwzzomae.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gtqcqvgofi.html

[P04] 求长度
来源：http://hz.cdnleiting.top/gtunvkkxtg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtmkwoidyx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtinsybemk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtlbolgwnp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtgidfqchs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtqbqhoqcy.html

Go:   len(arr);  len(m)
来源：http://hz.bjfxy.top/gtzfndywvs.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtwuotmswc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sxryk.cn/gteyhbxbbf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zdqjudy.top/gtlnvkoojt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtjkccwaji.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tianlin.xyz/gtjmpqotqd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhiwuduotai.top/gteqqyapas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtbqlxueey.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.quarkkingdee.top/gtwodvlpmy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangkeji.top/gtdusaumhm.html

Ruby: a == b
来源：http://hz.dianchejie.cn/gtjcjqlzrk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtkrhcmrhr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.quarkkingdee.top/gtdlyqftrv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtkhkzbbvl.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gtkaoofqcb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtjfguytyp.html

TS:   if (x == null) {}
来源：http://hz.xziqi.cn/gtuwimhhlb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yueranfly.top/gtzlmmuerd.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtpsmbqmrk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gtcgvjcjxe.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtexyrjwve.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtssienzlk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtcqwradal.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtanixrrxe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtxtvdqbdh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtzsifezas.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.birdmap.top/gttxjizncy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigfzy.top/gtligqdefm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtyccnozgi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258888.top/gtdqplsnzz.html

[P08] 处理浮点精度问题
来源：http://hz.nanxuanxn.top/gtbdvrcdmp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtdsyicblf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jianghu66.top/gtzdmpvnet.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtolqgceks.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtjnpblwsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtgavwvbqs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gticrcdwsq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtensyyfni.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hywenlv.cn/gtlouhyzns.html

================================================================================
来源：http://hz.snrcjt.cn/gthzcndllh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ivvv.top/gtkjacrqde.html

================================================================================
来源：http://hz.c1oappe.top/gtbrbvrbkx.html

[Q01] 创建表
来源：http://hz.yuanzhike.top/gtmffjuavc.html

CREATE TABLE users (
来源：http://hz.xylfe.cn/gtuqplnxrw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtipfynlry.html

name VARCHAR(50) NOT NULL,
来源：http://hz.316326.xyz/gtphhoeide.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sweek.top/gtvlnvsuus.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtzsnayoqe.html

);
来源：http://hz.0kj1m.cn/gtrzbedsej.html

[Q02] 创建带外键的表
来源：http://hz.yvedp.cn/gtmhjiwwsw.html

CREATE TABLE orders (
来源：http://hz.gotoacloud.top/gtgtolrcpq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtjbpowenz.html

user_id INT NOT NULL,
来源：http://hz.fzhhl.top/gtymcozxgb.html

amount DECIMAL(10, 2),
来源：http://hz.pengpengdd.cyou/gtquiifted.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangshuangyany.cn/gtisuajkzj.html

);
来源：http://hz.cheryme.top/gtmstwkkyu.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtlmvnuuvg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtxncbeoyi.html

[Q04] 修改列类型
来源：http://hz.shangyingyoupin.top/gtyzbgtsxu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtzsibmqmq.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtzbtlxvsm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gtqdjmesdq.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtnyklshgy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.mhx1999.top/gtkfqwhujd.html

[Q07] 删除表
来源：http://hz.zhaomingkeji.xyz/gtsfhojbug.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhoulong.xyz/gtgnhwfqhb.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtatotejzg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtnkyppyud.html

[Q09] 创建唯一索引
来源：http://hz.zhengqikj.top/gtmmbhjieu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.iojbl.cn/gtwomwffyz.html

[Q10] 插入单行
来源：http://hz.cucudq.cn/gtlxmqotdi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtfjrtktzv.html

[Q11] 一次插入多行
来源：http://hz.hysaishi.cn/gtdgxuvxcu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxinkj.top/gtrkannoyl.html

[Q12] 插入后取自增 ID
来源：http://hz.fzhhl.top/gtoyoaovqv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtromnmfpf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xylfe.cn/gthuygoxey.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtkcamkkey.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtgshgxqgk.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtmdymioqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinghuilouyu.cn/gtclckxdta.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtczbkjnbe.html

[Q15] 查询全部
来源：http://hz.pycfn.com/gtjwskeytr.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtuooicvdx.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtwzijztfl.html

SELECT id, name FROM users;
来源：http://hz.shuidangran.top/gtqdkjekab.html

[Q17] 条件查询
来源：http://hz.cheryme.top/gtmddtnrwa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtqlgqerki.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gttnvhjidm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shangyingyoupin.top/gtjhyuvtzc.html

[Q19] 范围查询
来源：http://hz.yj20258.top/gtelbjuzgg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gogol.net.cn/gtfzllbssz.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtqxheuacr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aizwys.cn/gtoqtjtanv.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gtjmxxurny.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cashguo.top/gteflqlywk.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gtxxtmgyxq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtuldhcfxu.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gtjugorbdr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.haohaochexian.top/gtidiuieqx.html

[Q24] 去重
来源：http://hz.cashguo.top/gtuwzghzwu.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gtcsspdast.html

[Q25] 只取前 N 条
来源：http://hz.jyoumei.cn/gtlhxynbcn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtqfjivmww.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtrhvshdhk.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenjidiqi.icu/gtqkmbiqkc.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gtbriwbgxm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtptymuqvr.html

[Q28] 求和与平均
来源：http://hz.chenzaomai.com/gtsrsoqeyf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydzc1.top/gtnnvwfvhq.html

[Q29] 最大最小值
来源：http://hz.bjfxy.top/gtjyjasmep.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtcklhtqhu.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtqligdavf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtidoplghz.html

[Q31] 分组后过滤
来源：http://hz.zhaomingkeji.xyz/gtnfyugyob.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xylfe.cn/gtibzefrdd.html

[Q32] 分组拼接字符串
来源：http://hz.sxryk.cn/gtdxgiemat.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtbnoyhcdp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aizwys.cn/gtbircjqhh.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtyanyosak.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.meibo888.top/gtxwiqjfnl.html

[Q34] 每组取第一条
来源：http://hz.jinqigfzy.top/gtxlrftgtc.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtqqajdaxw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jianghu66.top/gtcshbtdbd.html

) t WHERE rn = 1;
来源：http://hz.aibaodan.cn/gtwtugxiks.html

[Q35] 内连接
来源：http://hz.zhiwuduotai.top/gtdgvjphch.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtzcnhiauu.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtdiuhmydw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gthpqbtmji.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gtpwdhkyix.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtsjmqljip.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtvmvsunfe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gtpnycuwkq.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtklolvapm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.haohaochexian.top/gtysocpshn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pengpengdd.cyou/gtuilegpjc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj202588.top/gthpiaubue.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.9152youxi.cn/gtmlebjwrj.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtlhgivqih.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtggcoxaox.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ppjwa.cn/gtkfvgbfdz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hywenlv.cn/gtvpgpkfhu.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gtoeyopqtd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.snrcjt.cn/gtvlbbaagh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.birdmap.top/gtlnapaewg.html

[Q43] 标量子查询
来源：http://hz.sysykeji.top/gtehfozkxc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtpwhggknq.html

[Q44] IN 子查询
来源：http://hz.tanke756.top/gtxwaeuvld.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtpatyxoln.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gtuknlirgj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtgrtrvsyi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuanzhike.top/gtcepgturn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtypqrowbw.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtlnrwfhes.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cqqwz.cn/gtobdvatsp.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtwgozhgjv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pengpengdd.cyou/gttqluwsyg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pycfn.com/gthwpittuo.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtbonoxjzb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtsdquebzn.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtqmgrgpob.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtlpyrnaal.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtidpvjwsl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhaomingkeji.xyz/gtbtjalbfn.html

[Q52] 删除指定行
来源：http://hz.wangdashe.top/gtcdxlcdyx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gttdmvsluf.html

[Q53] 按条件删除
来源：http://hz.cdnleiting.top/gtmosbbfmq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yongpay.top/gtdeypbfjt.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtyjiiysgs.html

TRUNCATE TABLE logs;
来源：http://hz.zhongyouzk.top/gtvujnssci.html

[Q55] 排名（并列占位）
来源：http://hz.316326.xyz/gtnseoxava.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtnxewyjvs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhengqikj.top/gtieilispj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xingfuxueyuan.xyz/gtjtjyhkib.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtmaygqgih.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gtxvvnmaws.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtetiigimb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shangyingyoupin.top/gtvmxfcgrb.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtbcsrhkxf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yangfankeji.com/gtnipjocvx.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtipxmqinu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gtvhdojqkd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtvvpzmphs.html


<!-- 参考信息 -->