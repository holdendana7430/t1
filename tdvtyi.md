代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtjyhqjipw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtmlvtlids.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtsghwaqua.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj202588.top/gtnrcoelsi.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtmxdwevun.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtyyliknca.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtidoygrfd.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtyrzdhyiq.html

Go:   // 手写递归
来源：http://hz.iojbl.cn/gtecgwrhoz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtwjdpgany.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtewhajhhv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.meibo888.top/gtrqusezjd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangtech.top/gtwfxvfpyk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sufxvd.cn/gtosdmuaay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtwxaywynb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtjfiiifco.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtddknfjnr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtsbdwvjrz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtnygvuhrh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gttlgmpspw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtutqpwviv.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtefidqnyg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtijqtyioa.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtthkpcmkm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guannengcc.top/gtbrdhrtnr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gteyfkvxyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtmgajqxop.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtembmxjpu.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtcykkdyro.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtelwsonwo.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangkeji.top/gtoqjzcyap.html

C#:   Task.Run(() => F());
来源：http://hz.birdmap.top/gtwxujcfzi.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gthcwepros.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtwracujpu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gtorbueulo.html

JS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtdaylfziv.html

TS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtsufbjatc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtvyxrtszc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cqqwz.cn/gtineznemx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sysykeji.top/gtbuwhvpsf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shuidangran.top/gtgdbpfbet.html

[O03] 加锁保护共享数据
来源：http://hz.havefunace.top/gtpuiddjtm.html

Py:   with lock: shared += 1
来源：http://hz.dashuyun.cn/gtixnxozdg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangtech.top/gtccxbhqep.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gteohmwzdh.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtauquqngm.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtchtryaeu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtjhpbxmsv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinghuilouyu.cn/gtzpvveyxs.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gthnbtbxdb.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtawnyoocw.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtrhenefcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gthjgwtojt.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtkieoysfv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shzxlz.cn/gtnflxchcf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtizozidcw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.bjfxy.top/gtmurwsxsy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gaohongyu789.top/gtbzcjdtll.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtecisrtzh.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhoulong.xyz/gtreswlsou.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ywan-chungtsiang.top/gtacjaxmhg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtvopmwzfv.html

JS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtdbaeusev.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gttlcegojs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtcumjgqom.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtlrfiaeci.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtwpezdgxy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtlnimboiu.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtozmqgjoq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtshvmklam.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.52xcode.cn/gtvjunstns.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtgipeayeb.html

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtyxnclurn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258888.top/gtpofdqlqi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jlsjyb.cn/gtrborjdyb.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gthnxdvnvw.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gtaqiwmoas.html

================================================================================
来源：http://hz.hammf.cn/gtreobgqhn.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gtcfcthelr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbrplfsgm.html

[P01] 生成 UUID
来源：http://hz.xziqi.cn/gthblvfilw.html

Py:   str(uuid.uuid4())
来源：http://hz.xylfe.cn/gtwpvysuio.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shuidangran.top/gtnbwuddbl.html

JS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtrawmtbfr.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtuyumrmpq.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtznlqylpx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtpnkjyuaj.html

Ruby: SecureRandom.uuid
来源：http://hz.fzhhl.top/gtwtzadmcr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangkeji.top/gthncdwyzy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtrorezipy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ivvv.top/gtotmkgcqa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtgaewqdzg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gtilqekdrf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtjmpbqekr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gttywraxit.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtkxwnpygf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtxsuezrco.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtblxollay.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtyhnsyjwp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtykvoctvs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtakjbmsaj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtgmevsegd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtanlvynoz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.bjfxy.top/gtfnqhcmrm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtdqlcbktj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gtstsxpfam.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guowangkeji.top/gtcsvsquzd.html

[P04] 求长度
来源：http://hz.ppjwa.cn/gtxmwdghat.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtkqfprrnw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtmexiebca.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtgsodhgtf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtyqklcfaq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtsoifiuor.html

Go:   len(arr);  len(m)
来源：http://hz.shuidangran.top/gtbmqkprhj.html

Ruby: x.length;  x.size
来源：http://hz.316326.xyz/gtfxhjokiz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gtwvxjkdhz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.quarkkingdee.top/gtgnfbpxzg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtavsorrnt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtotrafbbz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtjuucnbgo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtzjjaauyl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jiagoushi.top/gtkwktkzng.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtscxirhvk.html

Ruby: a == b
来源：http://hz.tianlin.xyz/gtmpcqxqex.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtxdocxldt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xziqi.cn/gtljsyhkfu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtgnxdtire.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtxyqcfooc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hywenlv.cn/gtbckzmfnl.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtaenwnbjn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gtflnzfcdx.html

Go:   if x == nil {}
来源：http://hz.xingfuxueyuan.xyz/gtcgaavktq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xingfuxueyuan.xyz/gtcnaentav.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtilvzkbxp.html

[P07] 防抖与节流
来源：http://hz.aizwys.cn/gtwoumewkl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenlongwang.top/gtfkkezgqz.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtsfyztkip.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gthvjemfza.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtgdmamzqk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtybkysvve.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtjwgcuzul.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yvedp.cn/gtrapyrlrm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.smart0.xyz/gtlezkwlkw.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtafajamup.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sufxvd.cn/gttmybnnwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yvedp.cn/gtnbqdkpjb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtrvpfwepd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnxiangtu.top/gtddoletuf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtejvppmzt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hammf.cn/gtgdhrecga.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtmvizayiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtuzlhafzp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtuoxhgerc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhongyouzk.top/gthplfhcdi.html

================================================================================
来源：http://hz.nwbrower.top/gtnalfkxlp.html

[Q01] 创建表
来源：http://hz.nanxuanxn.top/gtmkgzwhgo.html

CREATE TABLE users (
来源：http://hz.jianghu66.top/gtktkdwggp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtczqoytkz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtowhgprac.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shzxlz.cn/gtvzkxintc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxinkj.top/gtnyxiuorc.html

);
来源：http://hz.feifeiyinyue.top/gtvredturp.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtudmsfuju.html

CREATE TABLE orders (
来源：http://hz.havefunace.top/gtkcawfshf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtkvqnqebb.html

user_id INT NOT NULL,
来源：http://hz.zdqjudy.top/gtgezvxfor.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gtgeepetxa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtgwbbnugc.html

);
来源：http://hz.shanyushiyangkeji.top/gttjndxguo.html

[Q03] 增加列
来源：http://hz.yanxiufei.cn/gtfjzvemao.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhixingplan.top/gtejwcxsps.html

[Q04] 修改列类型
来源：http://hz.cashguo.top/gtpbpgyrtw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhaomingkeji.xyz/gtmuabyxch.html

[Q05] 重命名列
来源：http://hz.jinyuanbaomall.cn/gtwsieiliq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtnmusnmrc.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtpagafuvh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guowangkeji.top/gtyfullbtm.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gtgfctzqrj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.quarkkingdee.top/gtlilthitm.html

[Q08] 创建普通索引
来源：http://hz.9152youxi.cn/gtksmbwazn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.c1oappe.top/gtqriuqynq.html

[Q09] 创建唯一索引
来源：http://hz.xuetiantiany.cn/gtnmwtfeif.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtlppickqm.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtjarbtrqt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gtzhhkrght.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtdzsoanur.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ppjwa.cn/gtqgasxdbi.html

[Q12] 插入后取自增 ID
来源：http://hz.jianghu66.top/gtmfrpyfay.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tian-w.cn/gtihprhdgu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtzrkbvnni.html

[Q13] 忽略重复插入
来源：http://hz.wangshuangyany.cn/gtoqmymnlc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zycfv.cn/gtfpekelcc.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhixingplan.top/gtoabtylgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangkeji.top/gtafiigdrr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenlongwang.top/gtatwprvec.html

[Q15] 查询全部
来源：http://hz.dianchejie.cn/gtqnbmtpwy.html

SELECT * FROM users;
来源：http://hz.yuxming.cn/gtnrlsvjfk.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtlrsedlmr.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gtqfinykae.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gtddxhvlci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtycbtzkkb.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gtircqrgzb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenlongwang.top/gtluuwnxfn.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtckowwtqm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gthtmzdbxo.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtbhiwupcs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258888.top/gtgbnhpgsw.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtjzxvukbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuxming.cn/gtaltubjgu.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtbepwgonh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtfpluxnit.html

[Q23] 分页
来源：http://hz.ydjk.org.cn/gtsyvsyqkn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ppjwa.cn/gtcgvbndpd.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtpzmaxgmv.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtlxfykjat.html

[Q25] 只取前 N 条
来源：http://hz.cucudq.cn/gtpxapoymd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guowangkeji.top/gtzlnyoreh.html

[Q26] 计数
来源：http://hz.0kj1m.cn/gtqmeqmnya.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gthbquwuut.html

[Q27] 条件计数
来源：http://hz.gzhubu.top/gtdghnhhzc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtuijhvzny.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtyvdyvrly.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gtpimpqkeb.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtpnufayrl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtupqmdxjz.html

[Q30] 分组统计
来源：http://hz.cqqwz.cn/gtbadyaygq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtnwcdhzez.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtcvbewiuk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hysaishi.cn/gtqmpsnnkr.html

[Q32] 分组拼接字符串
来源：http://hz.dashuyun.cn/gtmfurbplz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtvjvrlofz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtykjfjxed.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gthhxpfcsa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtfdetepwo.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtzdxcwicf.html

SELECT * FROM (
来源：http://hz.yvedp.cn/gtzskpjplg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtrjxxwtjf.html

) t WHERE rn = 1;
来源：http://hz.jlsjyb.cn/gtrxcklmfp.html

[Q35] 内连接
来源：http://hz.gzhubu.top/gtraukosvx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtopycvlon.html

[Q36] 左连接
来源：http://hz.sweek.top/gtebrwqaym.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtqodbkrdh.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtgbndwgxv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtydgydrra.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jyoumei.cn/gtorqlxabg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gtmtzkovtu.html

[Q39] 自连接（查上下级）
来源：http://hz.xylfe.cn/gtztsarjxq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtwsyxaufg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtvbkxfugx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtxgsyvzgd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtulyvvxdf.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtoqklsptl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangdashe.top/gtkpvwiosp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtajwokjkz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tianlin.xyz/gtxaqqvntu.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gtelptoqwy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gttfmdhxvy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daria6918.cn/gtfqltneln.html

[Q43] 标量子查询
来源：http://hz.guannengcc.top/gtqalxpzgl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigufen.top/gtihwcakhx.html

[Q44] IN 子查询
来源：http://hz.nwbrower.top/gtubsxujjm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtmrhvamgq.html

[Q45] EXISTS 判断存在
来源：http://hz.shangyingyoupin.top/gtrvitmtyw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtkmnvgmqz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shzxlz.cn/gtomjgikaf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtkoxscdol.html

[Q47] 与平均值比较
来源：http://hz.chenjidiqi.icu/gtascawuqv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtkcvfebkx.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gtmvkwqkxq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shuidangran.top/gtlbzpnbrc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtbezeacil.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtiudmunzx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.svipenyu.cn/gtjtrgdzmy.html

[Q50] 批量更新
来源：http://hz.cdnleiting.top/gtaetxzcfq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtvlktifzy.html

[Q51] 用子查询更新
来源：http://hz.yj20258.top/gtspokweim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtccykkunw.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtcpcozykd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtkgscnncu.html

[Q53] 按条件删除
来源：http://hz.c1oappe.top/gtozccwcux.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigufen.top/gtanxjcpol.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtoiuhklbz.html

TRUNCATE TABLE logs;
来源：http://hz.cqqwz.cn/gtppvkjxhz.html

[Q55] 排名（并列占位）
来源：http://hz.pengpengdd.cyou/gtplwiyrzo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yanxiufei.cn/gtwkvsbulh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtdtdoqekn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.316326.xyz/gtgnzplusj.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtiaxflvnp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ivvv.top/gtovnadtwi.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gtcsznyypr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gotoacloud.top/gtrfmqyqdu.html

[Q59] 分组内累计
来源：http://hz.ydjk.org.cn/gthpdewiey.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtyhzooice.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gtsliyubou.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtvwefdtec.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.svipenyu.cn/gtknvzvwqo.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtaxnhtxxy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtmfvqqfnl.html

[Q62] 分组占比
来源：http://hz.nwbrower.top/gtwnacgwdb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtwijrkqfs.html


<!-- 参考信息 -->