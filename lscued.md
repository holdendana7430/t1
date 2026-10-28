代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jiagoushi.top/gtohtiaizo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gthalqfvkn.html

Java: class Node { int v; Node next; }
来源：http://hz.andypj.xyz/gtxmmmikch.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtvkkhfpgy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtananwhzs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pengpengdd.cyou/gtzqzhmwfe.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gtrjcqpjkv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gaohongyu789.top/gtfxezpylk.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtdsnkmqxc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtfwvrpkhf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtkmcuicqs.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtirfanhky.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gtmxbaabrt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtgyjfburi.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtcvgefdbf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtpjhkwjig.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gtzowlvoap.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgfzy.top/gtigrvqhwt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gthngjbnpv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtkvznudna.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtaqgdpuxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtveksjvja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtuobgdtut.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtgxaofmat.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtusuujmbo.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtcwriipct.html

================================================================================
来源：http://hz.zycfv.cn/gtfawmfvaw.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtjbhjbgvh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tianlin.xyz/gttxhjgtep.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gtipxujzab.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aibaodan.cn/gtzptqvufk.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtfoykksul.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtywdrhqno.html

Go:   go f()
来源：http://hz.tanke756.top/gtzdpbwdmu.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gtjqqxuwax.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtwucqayrx.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtwtmwkugv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtchhwhptf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yongpay.top/gtedhfqlix.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtlratrsbe.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtfvtcvrak.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ybcxt.top/gtwtuivfau.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtqhvblftz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fzhhl.top/gthijfflco.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gtycqtnwze.html

[O03] 加锁保护共享数据
来源：http://hz.yuxming.cn/gtrujatjdo.html

Py:   with lock: shared += 1
来源：http://hz.zhaomingkeji.xyz/gtempuluoy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtnrtdoupj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhixingplan.top/gtsdmzxiil.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtrusryyfs.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigfzy.top/gtymkxyhvm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtczgttwlx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtezlouwdd.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtrmtoofzi.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtriptuvxt.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gttnuuulze.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sufxvd.cn/gtnjgakimf.html

JS:   async function f() { await g(); }
来源：http://hz.jlsjyb.cn/gtkcwlxbsc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtqjrtuzxj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgufenzy.top/gtiwjnvehy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtkawleajm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zdqjudy.top/gtqhleufmy.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtpoexbowl.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtuzspwacq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydzc1.top/gtzoceeqjg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.kuanghao11.cn/gtitlgjsth.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtnncoogye.html

TS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtjmnohnuz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtimcbxrjr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258888.top/gthkxabsqu.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtknabjrer.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtjabvlctg.html

[O06] 使用进程池
来源：http://hz.chenjidiqi.icu/gtqwntdaxw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tian-w.cn/gtswpltofv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtkepjbsuw.html

JS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtjwfkwred.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gttlqkfxjs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pengpengdd.cyou/gtxrjxdphm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yvedp.cn/gtikqmlldw.html

Ruby: // fork 块
来源：http://hz.0kj1m.cn/gtbplimtvr.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtnldqlbtw.html

================================================================================
来源：http://hz.fengsongda.top/gtwgqzydzs.html

P. 常用工具函数
来源：http://hz.sweek.top/gtoilqknhb.html

================================================================================
来源：http://hz.nanxinkj.top/gtbjfubpag.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtnouxoiuq.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gttuhvetuv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.meibo888.top/gtitkswnqw.html

JS:   crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gtbmvnjmyi.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtltgtperu.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtemyqtepy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.haohaochexian.top/gthincmilu.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gtfaqpymoz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtfgnvqdqd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhoulong.xyz/gtnqolgajo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.redwolf501.top/gtvxovuygo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gtjqrwpdso.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.c1oappe.top/gtbeumqpcw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinyuanbaomall.cn/gtkkmiixqu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tian-w.cn/gtadydrabn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jianghu66.top/gtyopzhhop.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.52xcode.cn/gtqttialxz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtlihzmumv.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtxicpbpjq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzhubu.top/gtwjtwgdar.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sweek.top/gtwjbsytfr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtkleiahuc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtuaswzsmc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtwnojneoo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gtpqlgqpio.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xingfuxueyuan.xyz/gtzqjjwkvl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtyxyeapax.html

[P04] 求长度
来源：http://hz.chenjidiqi.icu/gtinovagcx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhoulong.xyz/gtjmqwsyin.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtrekcgltj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtzgnhncdd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtawkrmbsw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gthblzurzp.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtaarpnfww.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtafrygmgr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtvhjlnrev.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuxming.cn/gtiuipskfh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xinyue.icu/gtwavhgmaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnxiangtu.top/gtfunpvrtp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.feifeiyinyue.top/gtvsncszkn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gtjnsxofjj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtyqbyiqxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtsznnriho.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtxujhejht.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtxcnjrsrm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtrzkzxrjs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gttyumsdil.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtbbhtyyxo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtnwpmjeny.html

TS:   if (x == null) {}
来源：http://hz.sweek.top/gthfbuuben.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtecdhauft.html

Go:   if x == nil {}
来源：http://hz.hysaishi.cn/gtstpojxwf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jianghu66.top/gtroshpqdt.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtmkxvvcke.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtwjqlpjqe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gtipsjcrwu.html

PHP:  // 手写时间戳比较
来源：http://hz.c1oappe.top/gtxddofetk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtybwcjgie.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtihnkspig.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gtqfhvercy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gtspfwxmra.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtubsmovfe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenzaomai.com/gtabjxhohh.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtlsrrgjft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhongyouzk.top/gtzumkgjxx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cashguo.top/gtkwgcbtsu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hfpthk.cn/gtjaolgwiz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtbzfshyss.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtlenlensx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhengqikj.top/gtytqdoghi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtbygxypeu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pycfn.com/gtwyujptqn.html

================================================================================
来源：http://hz.yvedp.cn/gtrcgixvoq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sufxvd.cn/gtuknskolf.html

================================================================================
来源：http://hz.9152youxi.cn/gtxnhhscxz.html

[Q01] 创建表
来源：http://hz.9152youxi.cn/gtbnkhwhyp.html

CREATE TABLE users (
来源：http://hz.quarkkingdee.top/gtluwkbzpd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtoqzrfuob.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtbcruxgos.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtrekfqmrx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtypbhfbyg.html

);
来源：http://hz.andypj.xyz/gtfmniqqvb.html

[Q02] 创建带外键的表
来源：http://hz.zhoulong.xyz/gtrgjspbxl.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtchqohrqh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtzgenbbcn.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtpnmeonpe.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtaachnbmh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tian-w.cn/gthzkwtenr.html

);
来源：http://hz.hysaishi.cn/gtlvtagypb.html

[Q03] 增加列
来源：http://hz.gotoacloud.top/gtdtvvabam.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtjhunnfwf.html

[Q04] 修改列类型
来源：http://hz.gaohongyu789.top/gttaxvfwrd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtlyhivyzn.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gtwivbuoyz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtfaookgrt.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtirsdxztz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtnqmawglt.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtbjewldzd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinyuanbaomall.cn/gtnerxtypk.html

[Q08] 创建普通索引
来源：http://hz.chenlongwang.top/gtqvabstxw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tanke756.top/gtahuqcyai.html

[Q09] 创建唯一索引
来源：http://hz.tian-w.cn/gtojynzchr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtbgeqjbnq.html

[Q10] 插入单行
来源：http://hz.52xcode.cn/gtrngxsvjk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gtarhcmguk.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtkrdnhmxh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtmcsssvxf.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtzsuiimsg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhoulong.xyz/gteignsjmx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtkqckzmfb.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtcztmwyyh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtegqkrctb.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtjicrujsc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yongpay.top/gthcapvmcr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtxifilfgn.html

[Q15] 查询全部
来源：http://hz.gzhubu.top/gtnbaiepew.html

SELECT * FROM users;
来源：http://hz.c1oappe.top/gtefytciig.html

[Q16] 查询指定列
来源：http://hz.yj20258.top/gtlhtkpsgu.html

SELECT id, name FROM users;
来源：http://hz.yuxming.cn/gtwuuhcmdz.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gtbfnesbjd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtncibmgck.html

[Q18] 模糊匹配
来源：http://hz.sxryk.cn/gtsnmieatv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtzhjaqxla.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtelvusshb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nwbrower.top/gtftwdaszc.html

[Q20] IN 列表
来源：http://hz.daria6918.cn/gtxrxjscgp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sysykeji.top/gtiyklxekd.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtbzdqajht.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtoplrycuj.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtetavxjjc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtnffqkhiy.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gtxatwwfvx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sweek.top/gtgrjkvogu.html

[Q24] 去重
来源：http://hz.chenjidiqi.icu/gtehwwwjoe.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtqkmwlzhw.html

[Q25] 只取前 N 条
来源：http://hz.ydzc1.top/gtpubsfxln.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guowangkeji.top/gtavjvjeka.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtvbjusosw.html

SELECT COUNT(*) FROM users;
来源：http://hz.gzhubu.top/gtgdvgduhu.html

[Q27] 条件计数
来源：http://hz.ywan-chungtsiang.top/gthsssfxij.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gtwpihahhe.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtvmfxzprm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtbtfbcdzf.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gtityukgot.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gthuzxwprj.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtgcfbmtjj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtqidqnhtr.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtqsgbfbfm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtztldhwqb.html

[Q32] 分组拼接字符串
来源：http://hz.ydzc1.top/gtzacqlntn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtnllduura.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gtxnwsxkhu.html

[Q33] 多列分组
来源：http://hz.pengpengdd.cyou/gtuozjltaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtlvtxbkev.html

[Q34] 每组取第一条
来源：http://hz.havefunace.top/gtytamkrxz.html

SELECT * FROM (
来源：http://hz.shuidangran.top/gtfzfainrc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtdhawvisa.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtuejskeaq.html

[Q35] 内连接
来源：http://hz.sufxvd.cn/gthrzjrlze.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtkuxgmrov.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gteyvwdpkf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtcwsataqu.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gthqjmxudh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtbosazufo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.0kj1m.cn/gtzewsofjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj202588.top/gtfovxrldn.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtbikpefsn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtwvnzapuv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtkjszeqef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtvusteiqf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jlsjyb.cn/gtnbaisfwt.html

[Q41] 多表连接
来源：http://hz.xziqi.cn/gtemqoxowz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtlfmaeutf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gtbvrcwsim.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtnhhaxlgp.html

[Q42] 连接条件附加过滤
来源：http://hz.52xcode.cn/gtfrxfhmfq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxuanxn.top/gtpjtnruxl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pycfn.com/gtjgujftds.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtzdjlkmsb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.haohaochexian.top/gtldljjjzb.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtlaqydgfl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.feifeiyinyue.top/gtfpqmvsdk.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtmxyfikut.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtgqbrheau.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shzxlz.cn/gtoemtpcfb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gthschaxub.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gttagopfzz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtrbcssgnh.html

[Q48] CTE 公用表表达式
来源：http://hz.yongpay.top/gtcxsbqwii.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtvfgspdgk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jqgufenzy.top/gtmbywtdkw.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gteqzfodkh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtbktpeicm.html

[Q50] 批量更新
来源：http://hz.hywenlv.cn/gtiwaiylaw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daxiang520.top/gtlsdgkpbs.html

[Q51] 用子查询更新
来源：http://hz.birdmap.top/gtihbdlkxw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ybcxt.top/gtvexgnadh.html

[Q52] 删除指定行
来源：http://hz.tianlin.xyz/gtvyduasnt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtwzazfndf.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtgfipifdb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.snrcjt.cn/gtkoleliod.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtbrgeqiuk.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtqxzjguhp.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gthyyhhngc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gotoacloud.top/gtqhwfezuc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shangyingyoupin.top/gtizxjarzb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtyausyacg.html

[Q57] 行号
来源：http://hz.guannengcc.top/gtflpwaixs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtidwevqzr.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gtcphohkcd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hfpthk.cn/gthlblqjkd.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtgoyysqdy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xziqi.cn/gtsboptngt.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtfmltkrxg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhaomingkeji.xyz/gtfkdcsowb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtkowtjszk.html


<!-- 参考信息 -->