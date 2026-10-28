代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.mhx1999.top/gtraworrfk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtlnkuayno.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtbimylvan.html

Java: // 手写 HashMap
来源：http://hz.hywenlv.cn/gtqdoyaxhf.html

Go:   // 手写 map[int]int
来源：http://hz.jqgfzy.top/gtjkjfqwza.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtgcqxzozh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuanzx.com/gtyphahfxh.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtiuqzdoby.html

Py:   itertools.permutations(arr)
来源：http://hz.birdmap.top/gtwmmyeqia.html

PHP:  // 手写递归交换
来源：http://hz.sufxvd.cn/gtbnrwngph.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtogfaqhig.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtgidgakrr.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtsniritib.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtnsrrshka.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtkxgupybv.html

C#:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtlojoenfu.html

[N09] 栈与队列
来源：http://hz.zhengqikj.top/gtixdjaleb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258888.top/gtcpudotlw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtvqkafkbm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtedcrgose.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtruuidlab.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtipmyviox.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtremjhzrf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtpvniqpdg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gtonfedstw.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtscoppths.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtnndthtqf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtigflxjgv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gthyrsxiyi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtkpmbxvvl.html

Java: class Node { int v; Node next; }
来源：http://hz.xingfuxueyuan.xyz/gtzjwhchax.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gttlkaimzn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gthgmlbwpy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtkgcwhdeq.html

[N11] 二叉树中序遍历
来源：http://hz.quarkkingdee.top/gtyzwzgsjv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sufxvd.cn/gtpqlhchbz.html

PHP:  // 手写递归函数
来源：http://hz.yj202588.top/gtsbgstdnf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtizxphycp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtfotgtllu.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtplyfbsjc.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtuxuyobvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gteqevsrlc.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtxwhcggwe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.andypj.xyz/gtzldpvlyj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hywenlv.cn/gtxgjidbbo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtehdfgnqm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtwyrzecve.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gttdgmbhyh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtbvhcmeev.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.0kj1m.cn/gtswtgklja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guowangkeji.top/gtbeplaxzy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtqertllvw.html

================================================================================
来源：http://hz.c1oappe.top/gtxafbnaqz.html

O. 并发与异步
来源：http://hz.9152youxi.cn/gtnzskcxbl.html

================================================================================
来源：http://hz.aizwys.cn/gtwykqkxyk.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gtwmlchagn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.havefunace.top/gtaibyqvoc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtmykxutfc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangtech.top/gtogfgncpl.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtyapelagz.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gthgtmjmrr.html

Go:   go f()
来源：http://hz.cucudq.cn/gtcfqcaznt.html

Ruby: Thread.new { f }
来源：http://hz.aibaodan.cn/gtzsbcqbvf.html

C#:   Task.Run(() => F());
来源：http://hz.bjfxy.top/gteojdtnht.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtaaybcped.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xinyue.icu/gtakbktrdm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtjiplwxbv.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtijmobnxd.html

TS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtfcoigbth.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhaomingkeji.xyz/gtyoddxkye.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gtgkehyjey.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yvedp.cn/gtrhzenuwv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nwbrower.top/gthbhyuuoq.html

[O03] 加锁保护共享数据
来源：http://hz.nanxuanxn.top/gtgpmirhto.html

Py:   with lock: shared += 1
来源：http://hz.0kj1m.cn/gtkptxecvz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hongshengwenyu.top/gtyznvhzaj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.kuanghao11.cn/gtgumhykjq.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtmlyeqxup.html

Java: synchronized (this) { shared++; }
来源：http://hz.daxiang520.top/gtndtiwjlm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fzhhl.top/gtuenvygad.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtozyldjqt.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgufenzy.top/gtbpkhfnjj.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtnziuylrb.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gtzfizwfyk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gtqtqgpdnr.html

JS:   async function f() { await g(); }
来源：http://hz.jianghu66.top/gtzppqylvh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtgsljzpsk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.iojbl.cn/gtyrplvfdg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gtkkdxhrut.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtshiwcoza.html

C#:   async Task F() { await G(); }
来源：http://hz.pycfn.com/gtmituzxwq.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangshuangyany.cn/gtuzbyzzta.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtlnsuscpk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhongyouzk.top/gtwwimalbo.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtowejykya.html

TS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtxjwwbduq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gtdyxjioxt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydjk.org.cn/gthrbgvwam.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtbitctyrh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gtmffgvmnj.html

[O06] 使用进程池
来源：http://hz.redwolf501.top/gtnvnjinqu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gtgazygzam.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtxcbaccqk.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtdvcvsyan.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtsqbofwoo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtolhglzlo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtxbhdxqzq.html

Ruby: // fork 块
来源：http://hz.aibaodan.cn/gtawavjtov.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtxeimcmbg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvvulibfj.html

P. 常用工具函数
来源：http://hz.tanke756.top/gtahvanlxb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtjtrdjusu.html

[P01] 生成 UUID
来源：http://hz.jqgufenzy.top/gtizswxbwn.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtpjqspnqk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtndtpnjty.html

JS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtbtjyofhc.html

TS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtczraypgf.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtvmxedlhu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtslmzvknu.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtepfayozp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtkaostzed.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gtjwkivpjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gtglkundgp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yongpay.top/gtkgoedleq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtkpotjzxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gthatrwggu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtoldrxmlz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gthxwmtlzu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shuidangran.top/gtyxmwswsz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shzxlz.cn/gtuzqaakil.html

[P03] 生成短随机字符串
来源：http://hz.gotoacloud.top/gtdjwjbglq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtaljislmd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gtlsmwannb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtlnaisizl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gthdxbryoo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sweek.top/gtbrrnirtg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xingfuxueyuan.xyz/gtlkjkvlqd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtmuwitbrz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangtech.top/gtogggktlv.html

[P04] 求长度
来源：http://hz.0kj1m.cn/gtvbpomagt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ybcxt.top/gtxwpqhjmp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtuwrngliu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtquezzgmt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtnpvlpysg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtlfgzwqyc.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtjmqeptkw.html

Ruby: x.length;  x.size
来源：http://hz.cashguo.top/gtepdfcsyl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yueranfly.top/gtiapbtylf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.vqdsnc.cn/gtbwedhrmn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zdqjudy.top/gtoohnhyou.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.316326.xyz/gtsnpzcmkj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtekpajwns.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtwafcwrta.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtrerersfg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtclbbjmmh.html

Ruby: a == b
来源：http://hz.andypj.xyz/gtwifanfhj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtqmnswqtm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hywenlv.cn/gtzdoklggc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtcopznkld.html

PHP:  if (empty($x)) {}
来源：http://hz.zhiwuduotai.top/gtnldruchk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtgkpmgqas.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gtoxefmgue.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tian-w.cn/gtpmdazrnp.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtrhswojmd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zycfv.cn/gtxvqjkeyu.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtevfjwpkb.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtnngnmpho.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gtrsmnmljw.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtqflfvrzm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtuxmkvcnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtkfflomei.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.feifeiyinyue.top/gtsvcppnxm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtafakycmm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuxming.cn/gtotqzjhyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuxming.cn/gtowclxqqa.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtjarelius.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtqgtizfpv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtndsmzrlp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtpgrdoghg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtzwuqevpo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydjk.org.cn/gtyealjygt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtldlxixsy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ivvv.top/gtmpchgfsy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtxlbyzxsj.html

================================================================================
来源：http://hz.shuidangran.top/gtvpbifrfm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhoulong.xyz/gtkchviddz.html

================================================================================
来源：http://hz.yj20258888.top/gtlpznnffe.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtdbwpkcgv.html

CREATE TABLE users (
来源：http://hz.ppjwa.cn/gtejcladka.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtkzxokalm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.316326.xyz/gthbxsijay.html

email VARCHAR(100) UNIQUE,
来源：http://hz.vqdsnc.cn/gtlldybnbj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.guannengcc.top/gtjgiryfnz.html

);
来源：http://hz.gogol.net.cn/gtnnxncbfg.html

[Q02] 创建带外键的表
来源：http://hz.aizwys.cn/gtlmeltfuv.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtssrezjrs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtpyegnpnn.html

user_id INT NOT NULL,
来源：http://hz.cqqwz.cn/gtpvgfovdu.html

amount DECIMAL(10, 2),
来源：http://hz.kuanghao11.cn/gtraqjwyrv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xingfuxueyuan.xyz/gtefyomydq.html

);
来源：http://hz.daxiang520.top/gtrdnivtbp.html

[Q03] 增加列
来源：http://hz.guannengcc.top/gthxpsquzu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.redwolf501.top/gthhvtyyys.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtwwpgzyoy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtccalodao.html

[Q05] 重命名列
来源：http://hz.ybcxt.top/gtitysyznm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtbqsbjqzx.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtwkbfnmnc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gtznrasjvb.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtvajkepeh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhongyouzk.top/gtkbptveti.html

[Q08] 创建普通索引
来源：http://hz.yanxiufei.cn/gtvkggidtl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnqzz.top/gttqfrwfar.html

[Q09] 创建唯一索引
来源：http://hz.jiagoushi.top/gtfydabkzn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xylfe.cn/gtzbptompo.html

[Q10] 插入单行
来源：http://hz.hongshengwenyu.top/gtdocikuye.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gtsgyuidph.html

[Q11] 一次插入多行
来源：http://hz.0kj1m.cn/gtnkmaizjv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtsevrerie.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtcttmdzdw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtwgjjmqwl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gthkphcnkp.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gtmixpuchs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtbdrksgxo.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gtjmoadgwg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yongpay.top/gttlrcbnot.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgufenzy.top/gtdaleylwn.html

[Q15] 查询全部
来源：http://hz.316326.xyz/gtmjadhkxv.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtfpgbkzdc.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtscezgqrl.html

SELECT id, name FROM users;
来源：http://hz.jqgfzy.top/gtnzgcontc.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtvzsclhmr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ppjwa.cn/gttigctgbs.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtblmtvfrq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yanxiufei.cn/gtzjdlctid.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtxwiheabp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtuktorwdf.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtfxzcfmdd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtjdgmalli.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtcifhsfqu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtjcnpecix.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtyuvqlvdf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.havefunace.top/gttyubwhsv.html

[Q23] 分页
来源：http://hz.sxryk.cn/gtulwgbrvu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhaomingkeji.xyz/gthoxsenpy.html

[Q24] 去重
来源：http://hz.tanke756.top/gtpolkspgx.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtgvofeqwl.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtcxsrbwtc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtgihitgrr.html

[Q26] 计数
来源：http://hz.tian-w.cn/gtgoysfrgi.html

SELECT COUNT(*) FROM users;
来源：http://hz.gzhubu.top/gtzndmsitb.html

[Q27] 条件计数
来源：http://hz.ehwqpu.com/gtagradbhc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtjrxvjswh.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtrilcircx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.kuanghao11.cn/gtpxkmaqzk.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtyvtmecmj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenjidiqi.icu/gtysqjetpu.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtxmhjnzrg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtvgkpdjuq.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtyhjptlef.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.kuanghao11.cn/gtnpzxvnnw.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gtgobjoiop.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtvdfbzxfw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.guannengcc.top/gthzmwdfnr.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtytgzusbs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtkuwtgbnj.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtevzaehej.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gtibmneskz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtctuxavvd.html

) t WHERE rn = 1;
来源：http://hz.nwbrower.top/gtcloozujl.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtqraqhcgh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtpobchizv.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtwfpwkyzm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtctojrygn.html

[Q37] 右连接
来源：http://hz.haohaochexian.top/gtyuqfwfvf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtyystglkw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ehwqpu.com/gtgmgkswmn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.wangshuangyany.cn/gtvayodpdb.html

[Q39] 自连接（查上下级）
来源：http://hz.sxryk.cn/gttednelmx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtrrcresec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtzeazyqbv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtfbquewib.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgufenzy.top/gteeooskrg.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtxtbdnlyy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zdqjudy.top/gtlcxnkhad.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gtlxyjveqq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dianchejie.cn/gtbqtgamde.html

[Q42] 连接条件附加过滤
来源：http://hz.smart0.xyz/gtwacapwul.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtqrtfjmua.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daria6918.cn/gtadjyhzol.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtbhkwwlcs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtjccsyfya.html

[Q44] IN 子查询
来源：http://hz.aizwys.cn/gtxajvwozi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtfmsdrqjv.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gteblyiywr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtjmkoymyy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hongshengwenyu.top/gtarreoang.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtssdaymym.html

[Q47] 与平均值比较
来源：http://hz.ivvv.top/gtoanrpmth.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtbphvusxu.html


<!-- 参考信息 -->