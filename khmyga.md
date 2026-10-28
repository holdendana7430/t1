代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xinyue.icu/gtoqkgrqnk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtvxlbspun.html

Java: class Node { int v; Node next; }
来源：http://hz.aizwys.cn/gtscvcivfj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtdsckhmua.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtogroynru.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cqqwz.cn/gtmkyiraal.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtvkljlixh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuanzx.com/gtidkdgdll.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtrtjumocu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtyhkmntxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtzmulmfno.html

Java: // 手写递归
来源：http://hz.xuanzx.com/gtodyzfujl.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtccvlsqqf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gttcrotups.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtqygmwesj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gtpbvhmtte.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtdulouaty.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtyphaddka.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtnpbaxxjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtflezisni.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtvyyfqgmm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gtobqierji.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gtratuovci.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtyingabsz.html

================================================================================
来源：http://hz.iojbl.cn/gtqlkqlnnp.html

O. 并发与异步
来源：http://hz.gzhubu.top/gtskdwnefm.html

================================================================================
来源：http://hz.jiagoushi.top/gtqbpleini.html

[O01] 启动一个线程
来源：http://hz.redwolf501.top/gtlzpjuwgx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xylfe.cn/gthigryqcn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtvvenovrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dashuyun.cn/gtfgpurqfo.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gttsesghar.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtigwgjndl.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtgktopfcv.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtokpikonk.html

C#:   Task.Run(() => F());
来源：http://hz.316326.xyz/gtadfjqyaz.html

[O02] 使用线程池
来源：http://hz.shangyingyoupin.top/gtckrignzd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fzhhl.top/gtisoyjgdc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtbvzkjivk.html

JS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtfhuhgelt.html

TS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtrnwvrgbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cqqwz.cn/gtiyfteumu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yangfankeji.com/gtphuvaydx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtefwpmiqh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yonumen.top/gtkwjrhlam.html

[O03] 加锁保护共享数据
来源：http://hz.pycfn.com/gtnnjssptj.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtirklkkro.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gtohvafcmv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtvjguabau.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtthqonqzf.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gtihsjiere.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gtjyqsjwat.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtwaqvbblf.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhiwuduotai.top/gtrfkwsyqm.html

[O04] 定义异步函数并等待
来源：http://hz.fzhhl.top/gtplxohceg.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gthmighwur.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtmyulycju.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtmcecwmob.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sxryk.cn/gtsmdyrywv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gttzkdjakh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydjk.org.cn/gtboffhpbx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtodhfcien.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtwgstsrdm.html

[O05] 并发执行并等待全部完成
来源：http://hz.fzhhl.top/gtqllgekot.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtmmriwcpx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dashuyun.cn/gtpsrstpdi.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtpjaeyumj.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtktitmiio.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhoulong.xyz/gtzbabmnlg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtemscbiph.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gthnklsdoe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhengqikj.top/gtssgdeqch.html

[O06] 使用进程池
来源：http://hz.jiagoushi.top/gtxetjsfzc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtvpdtbwvm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtmgjyfnge.html

JS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtivcwurcv.html

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtthaajhkl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtvtmjrbnl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtegvroyop.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtrfkdaxkd.html

C#:   Parallel.For
来源：http://hz.quarkkingdee.top/gteqswksyt.html

================================================================================
来源：http://hz.snrcjt.cn/gttqthtnab.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gttuntetav.html

================================================================================
来源：http://hz.sweek.top/gtogjihtcd.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtzzuinjjf.html

Py:   str(uuid.uuid4())
来源：http://hz.fzhhl.top/gtnoinjume.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gttsbrmpdr.html

JS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtsbvdwfvj.html

TS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gttsvkvmhg.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gtaoseuvgr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gtepvsefno.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtgfrpmsus.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtwdjqwzso.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtgcgdkpsq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtisxpeugx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.havefunace.top/gtqxtigsdn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hysaishi.cn/gtuoghpjkv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtrvhretxc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtkqgzboep.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj202588.top/gthzggwvgm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangkeji.top/gtlpviaqzf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtziceigjd.html

[P03] 生成短随机字符串
来源：http://hz.daxiang520.top/gtoyuqkygz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aizwys.cn/gthjvmcdmo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ybcxt.top/gtunpuokip.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtpomakajx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtoostoudt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtosfjejdh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuxming.cn/gtiyjgjjej.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gttsrrfbam.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aibaodan.cn/gtrttrnjvc.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtjxjcutyn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtafwkznrt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnxiangtu.top/gtazlsjsoy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtymoahhad.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gteeieozkh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydjk.org.cn/gtxypdfcyu.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtbwuupzht.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtgbwtbdrk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jyoumei.cn/gtvjgmetat.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gtgivjlbvy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtgkgmbiin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtjanrssnh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtkoopgcog.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtufppufpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgufenzy.top/gthyrqiizw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnqzz.top/gtlttpctbq.html

Ruby: a == b
来源：http://hz.yonumen.top/gtccfhtiic.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtmtxvirmc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtuvhqdcfj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.vqdsnc.cn/gtnxzpgafn.html

PHP:  if (empty($x)) {}
来源：http://hz.hammf.cn/gtqeogxqls.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gtivmchksz.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtmpnxoeum.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtqivjdrkl.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtlyeenehx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtvqlcfjrw.html

C#:   if (x is null) {}
来源：http://hz.nanxinkj.top/gtivwocdeo.html

[P07] 防抖与节流
来源：http://hz.zhijiandao.cn/gtidpvpzdo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tian-w.cn/gtxirzjlom.html

PHP:  // 手写时间戳比较
来源：http://hz.jiagoushi.top/gtwgwqblhq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtgsvsnxmb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtamdgxfau.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.316326.xyz/gtcoresjic.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.mhx1999.top/gtknkxispf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tian-w.cn/gtjekriuik.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sysykeji.top/gtvxzqetsd.html

[P08] 处理浮点精度问题
来源：http://hz.hnxiangtu.top/gtzocpancx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xinyue.icu/gtvzeaovru.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtzqksfqut.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gttvjasvfc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtkxmpaqrv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtvwmrlaor.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtrpituwvp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gttrzcdajo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtoxukipee.html

================================================================================
来源：http://hz.hammf.cn/gtszcfscrt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhiwuduotai.top/gtddsdyves.html

================================================================================
来源：http://hz.cucudq.cn/gtsrzmroxz.html

[Q01] 创建表
来源：http://hz.meibo888.top/gtctxtkddl.html

CREATE TABLE users (
来源：http://hz.tanke756.top/gtcfrffseq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtiamkozze.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dashuyun.cn/gtwwwbkqhu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gttudlprcr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtnvwtevfu.html

);
来源：http://hz.jinqigfzy.top/gtwhmuqror.html

[Q02] 创建带外键的表
来源：http://hz.daria6918.cn/gtuppnzoqc.html

CREATE TABLE orders (
来源：http://hz.shangyingyoupin.top/gtvfepsajs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gttfacpmrb.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtsqqzljzt.html

amount DECIMAL(10, 2),
来源：http://hz.fengsongda.top/gtfreyybly.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.meibo888.top/gtnxxkxysu.html

);
来源：http://hz.aizwys.cn/gtycrbgpwp.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gtxxlkuulr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtgctjrobq.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtrddenryh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gtatfszsqn.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtuwtloebq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.0kj1m.cn/gtryojjzuq.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtpuhmqjjv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fzhhl.top/gtgcaxqeix.html

[Q07] 删除表
来源：http://hz.jyoumei.cn/gtcmwfjeyl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtmajibxlx.html

[Q08] 创建普通索引
来源：http://hz.yongpay.top/gtewmprfog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gtihcaudxt.html

[Q09] 创建唯一索引
来源：http://hz.yonumen.top/gtboskqhoj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtjzhliaki.html

[Q10] 插入单行
来源：http://hz.birdmap.top/gtkvtthewd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtqdzjipyq.html

[Q11] 一次插入多行
来源：http://hz.birdmap.top/gtbsyahuic.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtkvarfyiq.html

[Q12] 插入后取自增 ID
来源：http://hz.feifeiyinyue.top/gtfcyaofzg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhengqikj.top/gtqbawicnx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yangfankeji.com/gtntxdnbiz.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtvxwrhytl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ivvv.top/gtupmognvn.html

[Q14] 存在则更新（upsert）
来源：http://hz.haohaochexian.top/gtuwfxpotk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.meibo888.top/gtckmispih.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shzxlz.cn/gtsclnbegy.html

[Q15] 查询全部
来源：http://hz.zhijiandao.cn/gtthdzmokr.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gthuzqoqic.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtcnnyiova.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtqtphxauk.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtodhdjhmo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.iojbl.cn/gtmgmnhqbw.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtbexllqfa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tian-w.cn/gtgtninjbk.html

[Q19] 范围查询
来源：http://hz.pycfn.com/gtolcduvwe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tianlin.xyz/gthnttjsbz.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gtkmrnkbey.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sweek.top/gtdlnbenda.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gtpxcmaeff.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtbjwktcbn.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtjbhvkcvi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtfngzbrov.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtjwfwvwdc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.feifeiyinyue.top/gtbgdfmejp.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtdkfrufuz.html

SELECT DISTINCT city FROM users;
来源：http://hz.cheryme.top/gtnzmvjhqc.html

[Q25] 只取前 N 条
来源：http://hz.zycfv.cn/gtsmtgizsg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtweweoqog.html

[Q26] 计数
来源：http://hz.yonumen.top/gtmfrbcyuv.html

SELECT COUNT(*) FROM users;
来源：http://hz.cqqwz.cn/gtssquutbi.html

[Q27] 条件计数
来源：http://hz.sweek.top/gttfgktwyy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.bjfxy.top/gtbjngesrf.html

[Q28] 求和与平均
来源：http://hz.yongpay.top/gtqqfmqrbb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yongpay.top/gthmzswqji.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtdnykulos.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtslkmagby.html

[Q30] 分组统计
来源：http://hz.hywenlv.cn/gtocgsxewr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtyptqsrcf.html

[Q31] 分组后过滤
来源：http://hz.daxiang520.top/gtbxcasuwj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gogol.net.cn/gteeftlzhn.html

[Q32] 分组拼接字符串
来源：http://hz.chenlongwang.top/gtrhzsbqoh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtymgofgsf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hfpthk.cn/gtgjemqdsr.html

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gttfxtlocb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gtzfvugizq.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtmqagbukh.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtacqeleae.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtsdijbdrn.html

) t WHERE rn = 1;
来源：http://hz.wangshuangyany.cn/gtmsckvfxq.html

[Q35] 内连接
来源：http://hz.feifeiyinyue.top/gtcwncpblt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtkrmdvsja.html

[Q36] 左连接
来源：http://hz.birdmap.top/gtilsppiyb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gtdglwrrxp.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtymfftpqh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtpawbfwcu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.316326.xyz/gtzkcwfqge.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gtqfylcbdd.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gtnxkjoaiy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtotmxnled.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtrdrpoyaw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sufxvd.cn/gtsuvjeugk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtejhfbmyl.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gtuzvowfva.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.andypj.xyz/gtuzhlaxcp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhaomingkeji.xyz/gtifvujfyw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtttezdwmc.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gthllnwoqw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtnbnalkyn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yangfankeji.com/gtkhytevqe.html

[Q43] 标量子查询
来源：http://hz.iojbl.cn/gtoaovwejk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yangfankeji.com/gtgsrgrnjg.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtekkdudte.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtppcpdsqv.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtjwvchimg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtgabghrzb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtzwxenttj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtswbphmkj.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gtzqjybext.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtbecpgxmm.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtscjsnkjk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtxvojtpli.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtkncxtrjf.html

[Q49] 更新单行
来源：http://hz.smart0.xyz/gtsnncctif.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtedycwiak.html

[Q50] 批量更新
来源：http://hz.hfpthk.cn/gtqkvussxx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtgjvaevnv.html

[Q51] 用子查询更新
来源：http://hz.ehwqpu.com/gtcmrribrt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xylfe.cn/gtktevqqcp.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtqnnzsobi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtwyvqurjp.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtlhpixccn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgufenzy.top/gtqolfwqmn.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtnxtpjwcm.html

TRUNCATE TABLE logs;
来源：http://hz.jyoumei.cn/gtbnjxgtjg.html

[Q55] 排名（并列占位）
来源：http://hz.mhx1999.top/gttqgbilbt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shzxlz.cn/gtihfmewal.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtzdmdgagx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtexiahpnq.html

[Q57] 行号
来源：http://hz.ivvv.top/gtwluzkeja.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtfokbrrwf.html

[Q58] 累计求和
来源：http://hz.shanyushiyangtech.top/gtcfqgjmlf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtbgrtsszr.html

[Q59] 分组内累计
来源：http://hz.xingfuxueyuan.xyz/gtujpetkje.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gtpugkyidr.html

[Q60] 取上一行 / 下一行
来源：http://hz.yvedp.cn/gtsjutsocx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gttgdqstju.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xylfe.cn/gtyoxvsrbc.html


<!-- 参考信息 -->