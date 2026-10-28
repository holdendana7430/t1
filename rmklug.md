代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtzctbzywl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.9152youxi.cn/gtsfyskjtz.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtbnohtnnh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ppjwa.cn/gtiesbvqpb.html

PHP:  // 手写递归函数
来源：http://hz.ydjk.org.cn/gtvzejwney.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtybxqwzus.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtouqhnlny.html

Java: // 手写递归
来源：http://hz.wangdashe.top/gtzfdmqvfn.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtmgwwyyxl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtvrupulmx.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtetfnfgsh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hysaishi.cn/gtqtezvnae.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtagtjkukl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtohsmkuia.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtbnsomxzf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtkyetlbid.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtbyrpbzju.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yvedp.cn/gtttdiyhol.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.vqdsnc.cn/gtbhndpxdf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtxhkpaevh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtakarcjyb.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtgdagqwij.html

================================================================================
来源：http://hz.shzxlz.cn/gtgdtsgwwc.html

[O01] 启动一个线程
来源：http://hz.kuanghao11.cn/gttuucaqfz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hysaishi.cn/gtovvyqyxc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenjidiqi.icu/gtpinsfjwg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydjk.org.cn/gtlepemvsr.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtztgfbdmd.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtviyppsyc.html

Go:   go f()
来源：http://hz.hongshengwenyu.top/gtawfhleom.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtdahabtjl.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtxmpqndqy.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtjqybqrie.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.haohaochexian.top/gtsdzesnvb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtbaywnvqk.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtokoohvid.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtixtpahmq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dashuyun.cn/gtvkhwsjgt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gttmlpzckc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgufenzy.top/gtulvdmpud.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pycfn.com/gtchhalkgq.html

[O03] 加锁保护共享数据
来源：http://hz.zhaomingkeji.xyz/gtbekjglty.html

Py:   with lock: shared += 1
来源：http://hz.tianlin.xyz/gtktzzixvt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangshuangyany.cn/gtgcxbjvpc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sweek.top/gtzumogjmh.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtdrimubbr.html

Java: synchronized (this) { shared++; }
来源：http://hz.nwbrower.top/gthwxigysi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yvedp.cn/gtjanujydb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtbahmgiyj.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtrvzmzfom.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtkhyexzej.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtgdmgumcv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuxming.cn/gtoizxipce.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtacdtfyuf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtuwatvdfi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.mhx1999.top/gtupevweyl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dashuyun.cn/gtcivogeis.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigufen.top/gtfjmcwefg.html

C#:   async Task F() { await G(); }
来源：http://hz.sweek.top/gtwwzdszag.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gttoubglcf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aibaodan.cn/gtajhuvylz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuetiantiany.cn/gtsvlwjozw.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gttktfxnez.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtfdjayqee.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtjzyzmzzt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gtazplelhv.html

Ruby: threads.map(&:join)
来源：http://hz.yj202588.top/gtoctlzdzx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.snrcjt.cn/gtpnryejcm.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtlbpgijhn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtvygazczq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aizwys.cn/gtocdolalr.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtqfwlmxaf.html

TS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtffnyeisa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gtzblhqihq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guannengcc.top/gtflplgdaf.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gtferojdun.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtvagfshbs.html

================================================================================
来源：http://hz.yvedp.cn/gtkyrvdqvy.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtodlztzgv.html

================================================================================
来源：http://hz.yuxming.cn/gtlijnsdjp.html

[P01] 生成 UUID
来源：http://hz.hysaishi.cn/gtkjuzxilj.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtunjslpdq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtktplgxzs.html

JS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtxeqghuil.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtqjzjjlra.html

Java: UUID.randomUUID().toString()
来源：http://hz.fengsongda.top/gtiwxpydsl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtqroaqpcg.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtlwrmyrcl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtwayajyvf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gtkaimmclr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydzc1.top/gtmnjqbroe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtitrxgccg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtycapzpsd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtmdcmunsj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuanzhike.top/gtyxkpmblh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtsyqovvaj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gtjxqrflii.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gtkrppnflt.html

[P03] 生成短随机字符串
来源：http://hz.snrcjt.cn/gtcjlkhyas.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gtrfrnvgnd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtxkvyvnle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtgkgzfznt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtghjunbqi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hysaishi.cn/gtfrqzwksm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shuidangran.top/gthtdjqleb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnxiangtu.top/gtgcxxdklr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtdgoqiqce.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtgaxozinw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj202588.top/gtzbtuexlu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtvthmgakq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtrmqvmfla.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtymyjyfaw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtebhsnnny.html

Go:   len(arr);  len(m)
来源：http://hz.ydzc1.top/gtasbupjuh.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtkxznkylt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtewsvbywe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtzkueyrms.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgfzy.top/gtsbibhgsp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gteyuucpgm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gtalfdjout.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gthtpflhuj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gaohongyu789.top/gteasgsnww.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ivvv.top/gtfqootqyc.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtgnxfublt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtyqyfkmfq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gtibsaqjgi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtzzmvyxky.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtlaillpgc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yueranfly.top/gtwcxgefub.html

TS:   if (x == null) {}
来源：http://hz.yj20258888.top/gtnoqclfjx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ehwqpu.com/gthkjnvoqu.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtnzqouvyj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangdashe.top/gtwqqitzeh.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtnxusdiqj.html

[P07] 防抖与节流
来源：http://hz.birdmap.top/gtjhhelwbf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangtech.top/gtuubblado.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtdvcthvaw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtzopfyumh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtvcvsdedy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtvolqppdj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtqfvpbosn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtzwibrljn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtsulfwqlb.html

[P08] 处理浮点精度问题
来源：http://hz.hammf.cn/gtzsbpgzol.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtudnoeske.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenzaomai.com/gtoxtjthgn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtmtqcgell.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dashuyun.cn/gtbejtbdqf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.haohaochexian.top/gtgpswkoql.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yongpay.top/gtvbcxodfb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangkeji.top/gtsefgmwcl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtywbvffdp.html

================================================================================
来源：http://hz.yj20258888.top/gtwrlsxlhf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ivvv.top/gtimwecgbn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtsnsggdmr.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtomswpbdj.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gttrxjjqxa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtsrohgapx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gtfrxonwrl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtvgrcmygh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gtriwxizqs.html

);
来源：http://hz.shuidangran.top/gttghkokju.html

[Q02] 创建带外键的表
来源：http://hz.hysaishi.cn/gtbyfjgxir.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtotaubfkc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtdaeqxxvq.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtsikjnbpg.html

amount DECIMAL(10, 2),
来源：http://hz.nanxuanxn.top/gtpyilxlrb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pengpengdd.cyou/gtksrvoyba.html

);
来源：http://hz.yvedp.cn/gtamfyivif.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gtkeccehkg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtacxyczrc.html

[Q04] 修改列类型
来源：http://hz.cheryme.top/gtsdhmzgmk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jianghu66.top/gtstattnpz.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtulayozru.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ivvv.top/gtpufsvunz.html

[Q06] 删除列
来源：http://hz.haohaochexian.top/gtcmtgbmpa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangkeji.top/gttlpwwdsw.html

[Q07] 删除表
来源：http://hz.yonumen.top/gttgfeyczj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hysaishi.cn/gtwlmnzpdg.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtphsiamzy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtlrfkapkh.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtyqoyoqpe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.c1oappe.top/gtnzvmduse.html

[Q10] 插入单行
来源：http://hz.wangshuangyany.cn/gtyaawvuim.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtfwhjrlwd.html

[Q11] 一次插入多行
来源：http://hz.xylfe.cn/gtqyhkaqel.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtoohygvhb.html

[Q12] 插入后取自增 ID
来源：http://hz.svipenyu.cn/gtzyrcjstb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangshuangyany.cn/gtrjpxokgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gtegmizywi.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtctfwhixa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.kuanghao11.cn/gtejrgbdzu.html

[Q14] 存在则更新（upsert）
来源：http://hz.dashuyun.cn/gtixwgyris.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgufenzy.top/gtjdlnuiug.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtylydqato.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtpmoggpem.html

SELECT * FROM users;
来源：http://hz.nwbrower.top/gttqikveti.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtcobhfoit.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtjldxgnfz.html

[Q17] 条件查询
来源：http://hz.ehwqpu.com/gturjgmzyf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgufenzy.top/gttpdcdalv.html

[Q18] 模糊匹配
来源：http://hz.xziqi.cn/gtshjzzaui.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gtcjpmwnmq.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gtdwekjdpg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gtvbmhsmlo.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtwqkislgo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtvdpzdmqa.html

[Q21] 空值判断
来源：http://hz.tianlin.xyz/gttpozwqjf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtgowquton.html

[Q22] 排序
来源：http://hz.zhengqikj.top/gtvabceypz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtuljwlrhd.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtvhtdqprh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ppjwa.cn/gtwkskdfeo.html

[Q24] 去重
来源：http://hz.yanxiufei.cn/gtdtrfmlew.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtfdzqamhm.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtxsfvbsbm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.vqdsnc.cn/gtlhwbdfot.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtixosjtho.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtwvdqliwe.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtiemstavd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtvtjenxfr.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gtpdkfedzv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gthtkbbvne.html

[Q29] 最大最小值
来源：http://hz.sysykeji.top/gtmbvufzex.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangtech.top/gtoolzhmnh.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtzsmmjhpu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtoxnvvuyt.html

[Q31] 分组后过滤
来源：http://hz.yj20258888.top/gtvkzhhlsi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtnlmvgzid.html

[Q32] 分组拼接字符串
来源：http://hz.316326.xyz/gtcmpyzvaw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtigzbxrzd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gtwdtthcsf.html

[Q33] 多列分组
来源：http://hz.shanyushiyangtech.top/gtzdhuirru.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.smart0.xyz/gtuehkluph.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtmnsshrrc.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtapcxwpye.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtuvilrcfg.html

) t WHERE rn = 1;
来源：http://hz.cqqwz.cn/gtdphtvisl.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtchglmmzo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gthpblfwht.html

[Q36] 左连接
来源：http://hz.yj202588.top/gttmwzgsbp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtidwiktuv.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtrgiwndng.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnqzz.top/gthblegxoz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.snrcjt.cn/gtmizvmqfo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtsqkcidfz.html

[Q39] 自连接（查上下级）
来源：http://hz.xinyue.icu/gttrxxjzeg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gthewrpndr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gtybudzism.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yongpay.top/gtydxyysjo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daxiang520.top/gttuhcvyjk.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtyoznldqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zdqjudy.top/gtpziynrrx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sysykeji.top/gtjopczril.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtfxnnebwn.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtmnwudewg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtowlaksna.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhengqikj.top/gtqrmwzwxz.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtsaxxzmll.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtvfontzxw.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtfvimrild.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtgcjvrxvt.html

[Q45] EXISTS 判断存在
来源：http://hz.pengpengdd.cyou/gtaxecgmbx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtnzsstwij.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hfpthk.cn/gtkiqgyiwg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtmdndaoqe.html

[Q47] 与平均值比较
来源：http://hz.tianlin.xyz/gtmmepozgv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sweek.top/gtdsixvcja.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtrusgkudn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenjidiqi.icu/gtqdinzwqv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtdfolxwka.html

[Q49] 更新单行
来源：http://hz.zhijiandao.cn/gtblmrhgjz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtzobuatvz.html

[Q50] 批量更新
来源：http://hz.cqqwz.cn/gthljkpybo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.52xcode.cn/gteynojtfg.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtglsotoqu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gtrubvwjzb.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gttbjthmkz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtkfefpewg.html

[Q53] 按条件删除
来源：http://hz.daxiang520.top/gttccplmxy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258888.top/gtbxiajhdx.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gtcjxtmzmx.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtliugzddh.html

[Q55] 排名（并列占位）
来源：http://hz.wangdashe.top/gtfbczinqj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.316326.xyz/gtbxjmuags.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtitvvijja.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jyoumei.cn/gtbvuflrqc.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtxmxogngf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yanxiufei.cn/gtmgxmcijn.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtiwjwnyqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.snrcjt.cn/gtdfymwtsb.html

[Q59] 分组内累计
来源：http://hz.vqdsnc.cn/gtzwxvbpfo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtkxayeokp.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtsknsscvz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtwcvnlcgm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangdashe.top/gtaehdozgd.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtluxiyukt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtgfqhzbhf.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtycbqlqow.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtcswpqgyi.html


<!-- 参考信息 -->