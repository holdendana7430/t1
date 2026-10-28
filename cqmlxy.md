代发 wailian999

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtvdakuihh.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtrxcihvzc.html

Ruby: arr.permutation.to_a
来源：http://hz.zhengqikj.top/gtummletyo.html

C#:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtjwmfxzps.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtuoltjvvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhengqikj.top/gtqcolmkeg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigufen.top/gtajclacfh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtfzrpezii.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gttbwkljxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gtiswtutbf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jyoumei.cn/gteygfcthn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cheryme.top/gtirjjfcrq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtnuudjtmj.html

[N10] 链表节点定义
来源：http://hz.guowangkeji.top/gtvtfkepbm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sweek.top/gtohsiriiy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtkkctqxan.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shuidangran.top/gtarwuguxa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtpbtincbw.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtigurcqpa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hywenlv.cn/gtqtrjrixx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtetfnkyww.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtyqedvdnk.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gtaqdniflx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.iojbl.cn/gtottxiwfj.html

PHP:  // 手写递归函数
来源：http://hz.xuetiantiany.cn/gtzebjalpf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtfnkjlmdj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtdflpcept.html

Java: // 手写递归
来源：http://hz.sweek.top/gtkbmauisr.html

Go:   // 手写递归
来源：http://hz.zhongyouzk.top/gttqkhyrzm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gtsekruwoe.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gthrpdkxgo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gtifcvdeci.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtfhazwyec.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ybcxt.top/gtiifrqupl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtvusdufnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtpvwmtfkx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtsukeoasg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yvedp.cn/gtyfvxqyxh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.vqdsnc.cn/gtjlokfrkk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtwcvpnivf.html

================================================================================
来源：http://hz.cashguo.top/gtluhgjahx.html

O. 并发与异步
来源：http://hz.shzxlz.cn/gtluwmcfhd.html

================================================================================
来源：http://hz.fengsongda.top/gtxujegcwt.html

[O01] 启动一个线程
来源：http://hz.zhengqikj.top/gtdvxccyiu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gtgfipzikr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtmxubhhgs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxuanxn.top/gtntvvvygz.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtkztksrzq.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtgmhvoxpp.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtmpfjmpbi.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gtzpcugzed.html

C#:   Task.Run(() => F());
来源：http://hz.sufxvd.cn/gtdvhtbrrw.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtmaghmoov.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtxehaxldu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gtgkhjsdvy.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtpcscskur.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtsaucudhz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtmwfhwqvo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtdjjbtemi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtdstbafnc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtlrkqdptq.html

[O03] 加锁保护共享数据
来源：http://hz.jyoumei.cn/gtqzalpqwy.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gtdlkniouc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtxeohxnfb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtjmnvytwz.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtgvlrwxht.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtcpjwfkyy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gtawgbjrja.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gotoacloud.top/gtbdbqqhfr.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhengqikj.top/gtkvakxfmc.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtowfkryzd.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtjwpoitid.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtralortkp.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gtftfczccj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.0kj1m.cn/gtdgqhjawy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtvgjucliy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ybcxt.top/gtexamhcnf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtgichgjoj.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtocemiwfw.html

[O05] 并发执行并等待全部完成
来源：http://hz.redwolf501.top/gtgprkgtul.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtfleohcgk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtbylupjty.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtwarcdpeu.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtdyrgspoh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gthmohkmto.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtekckarkw.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtchdvbbjk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gtxxvbefci.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtisbnwhyf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtneabuxci.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtmccwzwzb.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtjtpxrhzw.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtssemxdpe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gtkdcmbiuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtxlisepcl.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtpxivxysh.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtcmovcacr.html

================================================================================
来源：http://hz.jiagoushi.top/gtmbiieiwc.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtefmosjif.html

================================================================================
来源：http://hz.nanxinkj.top/gtepqgajoj.html

[P01] 生成 UUID
来源：http://hz.yuanzhike.top/gtjdqduiun.html

Py:   str(uuid.uuid4())
来源：http://hz.yvedp.cn/gthzrynxfo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zycfv.cn/gtorxyvqzu.html

JS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtfrcorwnh.html

TS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtvscbrzgm.html

Java: UUID.randomUUID().toString()
来源：http://hz.pycfn.com/gttlfgyrya.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtvcotmtjq.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtjgsinper.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gtjeuywwbn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.dianchejie.cn/gtzcmangry.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtjxdhjyev.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yangfankeji.com/gtedxomrgj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.vqdsnc.cn/gtrfxpkjdm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gtyeqrgyok.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtnpyfzjof.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtjgjtkhsi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.vqdsnc.cn/gtzwecupih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtbrlqhpnn.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gtcpzshzfr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.52xcode.cn/gtafawwqkf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gtlzcgzxez.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtvrbwkeqo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtcnfevisl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtublrovub.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtsjpusuwg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daria6918.cn/gtdxitzgir.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gtsbgayvhp.html

[P04] 求长度
来源：http://hz.ppjwa.cn/gtxwvuspwp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtjrdjwpjf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtcytdkump.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gttkwkgaxd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtehxwlyje.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtccllozqn.html

Go:   len(arr);  len(m)
来源：http://hz.vqdsnc.cn/gtelvikglg.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtmnjmufvs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtljaszmfw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtlcyewovr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtpczjtycr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnxiangtu.top/gtidzbwojt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtqqpkfreg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtbyzyvwis.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cucudq.cn/gtakfnqovk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtiuffzmns.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtsulgmxqh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258888.top/gtoenpijgt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtfecupffd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cheryme.top/gtdugngwla.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gtfjvlfcne.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtepvgbbsd.html

TS:   if (x == null) {}
来源：http://hz.zdqjudy.top/gtxuiqvmsk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.smart0.xyz/gtveydenap.html

Go:   if x == nil {}
来源：http://hz.tanke756.top/gtvncibvue.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtawwaklzn.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtpjzwdsir.html

[P07] 防抖与节流
来源：http://hz.bjfxy.top/gtnklbaspu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gtdfttzqko.html

PHP:  // 手写时间戳比较
来源：http://hz.cashguo.top/gttsvyyzsw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gteoctopgg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gthhivunzb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtomgdzsrk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtamipkpym.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gtofjabfwa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtykcecrlx.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258888.top/gtjlxvgrzw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtkcytlqya.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yanxiufei.cn/gtoiyybcep.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenlongwang.top/gttcrfnitb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtbrbplkre.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuanzhike.top/gtrcbvmpuc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.meibo888.top/gtlttqkpma.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtcchdhrpw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.9152youxi.cn/gtugcgltpv.html

================================================================================
来源：http://hz.zhixingplan.top/gtndbtvvbt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtpifmatel.html

================================================================================
来源：http://hz.yuxming.cn/gtgxqmcqio.html

[Q01] 创建表
来源：http://hz.jinghuilouyu.cn/gtrdhqdtce.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtzsuzutqb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.quarkkingdee.top/gthrdurfef.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jlsjyb.cn/gtrwjetovi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtipolppgn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gtbuinznro.html

);
来源：http://hz.nwbrower.top/gteryfmxbq.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtpmppcbyv.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtcgwiycnf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtlweotgis.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtewrtzwpt.html

amount DECIMAL(10, 2),
来源：http://hz.hnqzz.top/gtrfkbbruy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nwbrower.top/gtzpxksypd.html

);
来源：http://hz.yuanzhike.top/gtpdruygav.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gthizyttjv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtcnrduzlb.html

[Q04] 修改列类型
来源：http://hz.sufxvd.cn/gtvfbevbvp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhiwuduotai.top/gthgxwavzq.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtybyhizml.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhoulong.xyz/gtignjilti.html

[Q06] 删除列
来源：http://hz.yonumen.top/gttnsthyjd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gteoknnclu.html

[Q07] 删除表
来源：http://hz.hongshengwenyu.top/gtwzgxqahv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258.top/gtxaradmsa.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangtech.top/gtxfpfzxfk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtkeijzmak.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtwdkwjhez.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ppjwa.cn/gtbgtqacxr.html

[Q10] 插入单行
来源：http://hz.hfpthk.cn/gtiflpxyrp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gtlretjznn.html

[Q11] 一次插入多行
来源：http://hz.quarkkingdee.top/gtxenewlfc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gttjacjefl.html

[Q12] 插入后取自增 ID
来源：http://hz.vqdsnc.cn/gtuaizvzgi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gogol.net.cn/gthiwbewtc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shangyingyoupin.top/gtsncstoic.html

[Q13] 忽略重复插入
来源：http://hz.aibaodan.cn/gtntigisvf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.quarkkingdee.top/gtacjrdvli.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gttfsikzew.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtodzzqeak.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gtrdufwklt.html

[Q15] 查询全部
来源：http://hz.gzhubu.top/gtfdwtsnid.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtosdzdxrf.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gteqolnvef.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtylcdslvj.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtlqjxhoep.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtmlhxifix.html

[Q18] 模糊匹配
来源：http://hz.yuxming.cn/gtqmbbutwl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnxiangtu.top/gttdvpukws.html

[Q19] 范围查询
来源：http://hz.pengpengdd.cyou/gtgvfmovcv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhijiandao.cn/gttnugjhrk.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtalpcyuwv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtbwmjffrz.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtpebqhecw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhengqikj.top/gtqkkctleb.html

[Q22] 排序
来源：http://hz.fengsongda.top/gtyvgjoouh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhiwuduotai.top/gtpvdvxmjy.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtjringgnj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhengqikj.top/gtseegtlip.html

[Q24] 去重
来源：http://hz.jinqigfzy.top/gtrmiairuo.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtsmpyfwbx.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtducpotys.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtfmhqbnex.html

[Q26] 计数
来源：http://hz.iojbl.cn/gttinhtonx.html

SELECT COUNT(*) FROM users;
来源：http://hz.cashguo.top/gtijkrdkdw.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtmsgekmxl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuetiantiany.cn/gthgyluide.html

[Q28] 求和与平均
来源：http://hz.zhoulong.xyz/gtiqdeotcn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtdwqdihlx.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gtfxjptymi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aizwys.cn/gtbuahpurz.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtdhizttgm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtpfwmpfpk.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtgxeclczr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhoulong.xyz/gtvhrnsltn.html

[Q32] 分组拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtkintcdkr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtyngodary.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtbprxqlgc.html

[Q33] 多列分组
来源：http://hz.jqgfzy.top/gtxfybjdfv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtvclnoeya.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtoalylzzb.html

SELECT * FROM (
来源：http://hz.jlsjyb.cn/gtbcsiojqe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtbpzrnhmz.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtzduudvhu.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtwjjogfbk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtnucpafhn.html

[Q36] 左连接
来源：http://hz.andypj.xyz/gtyfdxxwts.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtslzopusv.html

[Q37] 右连接
来源：http://hz.zycfv.cn/gtpqmdrsha.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtvchdvfnw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtottswrbv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.52xcode.cn/gtzgubxmus.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtvzvgsdnq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtnmgdqdjz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yanxiufei.cn/gtawmuaewq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtptncwnnx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtztspcija.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gthzaygabo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtxaceotip.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fzhhl.top/gtqlmtvxli.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258888.top/gtzkvzgvpe.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gttxlfieec.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtrhuhpncu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xylfe.cn/gtymsfhtim.html

[Q43] 标量子查询
来源：http://hz.c1oappe.top/gtyxzhtrkx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtwuebrxws.html

[Q44] IN 子查询
来源：http://hz.xuetiantiany.cn/gtihuqmypv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gtvfymhsxp.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtwgpkladr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtcvngjvsz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ppjwa.cn/gtinnnjpgs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtzuxfbzla.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtvvaaktyd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigfzy.top/gtndldepbe.html

[Q48] CTE 公用表表达式
来源：http://hz.daria6918.cn/gtutdlpitw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtnopdfuih.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigufen.top/gtinnozmjm.html

[Q49] 更新单行
来源：http://hz.sufxvd.cn/gtyvwlczbc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtymvboklt.html

[Q50] 批量更新
来源：http://hz.zhengqikj.top/gtyhvxikuw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gttolcodzg.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtsxgrtwuu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sweek.top/gtxoonvzwx.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gtnigpdvdk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtpqtqvckw.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtxqgmotgj.html


<!-- 参考信息 -->