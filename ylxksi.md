代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yonumen.top/gtnnmslqbm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gtiujfsakn.html

TS:   // 手写 Map<string, number>
来源：http://hz.hywenlv.cn/gtqiknyqdw.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtyqkudhlk.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtfftajppv.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtrhgufyrv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtphzalvjs.html

[N08] 生成全排列
来源：http://hz.yuanzhike.top/gtxfumsmsi.html

Py:   itertools.permutations(arr)
来源：http://hz.316326.xyz/gtanbfarnx.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtcawninam.html

JS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtjnvnzgii.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtcfunfwxk.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtrsuynuwb.html

Go:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gthswcrdiy.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtouyrpmaz.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtjhtlfvki.html

[N09] 栈与队列
来源：http://hz.zhoulong.xyz/gtcjhxssxr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtarcqziox.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gtaqobamqj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xinyue.icu/gtasrxhhkt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuanzx.com/gtzqjkkvck.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigfzy.top/gtriimvfyf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daria6918.cn/gtthtjudky.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jyoumei.cn/gtesvooebo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tianlin.xyz/gtwbejsxwu.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtwiteeqgv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxuanxn.top/gtqcginytw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtieeexzhz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gthprvwjxb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtansuwqsq.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtfzzofonn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtuxawtjxa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ybcxt.top/gtoesdcjrh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtgvwuhdzg.html

[N11] 二叉树中序遍历
来源：http://hz.smart0.xyz/gttprvbhsc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtlcqutkka.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtwxwwswvz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gttwenxlrx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtjbksvfcp.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtigvxklrb.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtujbosfou.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.fzhhl.top/gtxmtxccag.html

C#:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtskutntuf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtatwkfhsz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.bjfxy.top/gtjwvodipr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ybcxt.top/gtxnpjbftx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtortspkxz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtsubevdkn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtqcpikxmw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gtkbohceoz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gtjvrskyrq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gttmboxihs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlhxlvorb.html

O. 并发与异步
来源：http://hz.hammf.cn/gtjniinqqs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvrpjvkcw.html

[O01] 启动一个线程
来源：http://hz.haohaochexian.top/gtpoqxutyi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtejzoeykv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtfjxogifd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtrfxcqcvl.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gthsdyxbzn.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gturxkfmhc.html

Go:   go f()
来源：http://hz.shanyushiyangtech.top/gtwlycqkqy.html

Ruby: Thread.new { f }
来源：http://hz.52xcode.cn/gttxemsgfr.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtmqkpjrxx.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gttumavgpp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtevjmxpvw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gthjuuimwt.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtqjssqnka.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtggkgvgyr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ybcxt.top/gtudlnqyrk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gtwmbarmgs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.0kj1m.cn/gtzdmzmphv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtgpkbosjn.html

[O03] 加锁保护共享数据
来源：http://hz.mhx1999.top/gtwlfqmweg.html

Py:   with lock: shared += 1
来源：http://hz.0kj1m.cn/gtjeugbtrr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtooeyexqy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ppjwa.cn/gtrxuqzhru.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtmaudbuqw.html

Java: synchronized (this) { shared++; }
来源：http://hz.shangyingyoupin.top/gtshnrlsau.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sxryk.cn/gtoasakhls.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gttrzfpmid.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtbratrinx.html

[O04] 定义异步函数并等待
来源：http://hz.wangdashe.top/gtihopiyrk.html

Py:   async def f():⏎    await g()
来源：http://hz.chenzaomai.com/gtbgpyxais.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtvjhajiwh.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtudjoclfw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtxgtgpboz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinyuanbaomall.cn/gtairjrctq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gtitakmeds.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtfolshezc.html

C#:   async Task F() { await G(); }
来源：http://hz.316326.xyz/gtbotnazdb.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtzavjelys.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtyxaeszrl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj202588.top/gtqvesuqmk.html

JS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gthttzbmzt.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtuvvmnbjv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtvmqsesca.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jlsjyb.cn/gtvnsbqtxf.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtnebxtrjf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gtiwvdpfvd.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtacmootyh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xinyue.icu/gtxesmuviu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtwibxrxln.html

JS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtgnemqenm.html

TS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtedcfgvrp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gttuohlqha.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gogol.net.cn/gtqdgdrejf.html

Ruby: // fork 块
来源：http://hz.yuanzhike.top/gtmcmuuiqx.html

C#:   Parallel.For
来源：http://hz.hywenlv.cn/gtumfrzigr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtusellzta.html

P. 常用工具函数
来源：http://hz.shuidangran.top/gtuwotjpul.html

================================================================================
来源：http://hz.zhoulong.xyz/gtibdwsmco.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtdlvolsfg.html

Py:   str(uuid.uuid4())
来源：http://hz.yangfankeji.com/gtupwichtc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gtpsxvbiqa.html

JS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtitsouuqc.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtxygkcopf.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtcrvndpdx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtpshukatl.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtstjruted.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shzxlz.cn/gteqcjyqcq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtpmzkmrch.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigufen.top/gtqahmkukx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj202588.top/gtlzlfnxkb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtcljnmpfj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtmlxfuhba.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhongyouzk.top/gtnxdecafn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cucudq.cn/gtuuvthlcy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yueranfly.top/gtjessupel.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gturzzngxw.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gteqoodbpz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zdqjudy.top/gtanhtxyiw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.pengpengdd.cyou/gthrgtcqpg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gtqyjklghj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtibvaptng.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtahauvioc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtcgnmcprb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xziqi.cn/gtjgybycww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhijiandao.cn/gtukdqjdtz.html

[P04] 求长度
来源：http://hz.smart0.xyz/gttbtwicxc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtomfrobnc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtcxcoudgu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtfgscildm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtdaxttvxh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jlsjyb.cn/gtshvkhihz.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtkiaarkem.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtfqfctrfy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtjjzvfszb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtstvhcgvx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gtmwmdumko.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtivdvygse.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shuidangran.top/gtuimgaelo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtfrmnzirf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gthrgidnou.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.mhx1999.top/gtgkvlepui.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtkccrqcmv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yueranfly.top/gtsxhxoprw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtkcwhwcyp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtiysvbuyd.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gttezwzruc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtxrbnchbi.html

TS:   if (x == null) {}
来源：http://hz.zhixingplan.top/gtfrrpvvyi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtvrdabhnx.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gttlklrmoc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gotoacloud.top/gtvhrkbxfp.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtullhuqax.html

[P07] 防抖与节流
来源：http://hz.xinyue.icu/gtqqihvcft.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.birdmap.top/gtskodcrup.html

PHP:  // 手写时间戳比较
来源：http://hz.zhoulong.xyz/gtxlrropkb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtaioyhdze.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtusvcrwtf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangshuangyany.cn/gtxsakxhxg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gtuiybcpxe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydjk.org.cn/gtjrrfnnam.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.smart0.xyz/gtpnaabtbg.html

[P08] 处理浮点精度问题
来源：http://hz.jlsjyb.cn/gtjuprusuz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuetiantiany.cn/gtyfhwiveg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jiagoushi.top/gthrkumrnm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtzwxldqlt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shangyingyoupin.top/gthfsrgodn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtldlwdjgd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.0kj1m.cn/gttfounemm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhiwuduotai.top/gtbfgeozcc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj202588.top/gttcivnsrm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlodjhdrg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gtnxaomsbp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtauxhgixk.html

[Q01] 创建表
来源：http://hz.birdmap.top/gtwzjnxsis.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtyayfscrb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtghhaebmn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gtkjaredds.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtxvxfdujr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gtawcljtyj.html

);
来源：http://hz.tian-w.cn/gtnkhqisod.html

[Q02] 创建带外键的表
来源：http://hz.mhx1999.top/gtmyeooxpi.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gtxzofqxjn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtwwnfftgf.html

user_id INT NOT NULL,
来源：http://hz.yuanzhike.top/gtpikjwbku.html

amount DECIMAL(10, 2),
来源：http://hz.sxryk.cn/gtbkzdimvp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtxqohakle.html

);
来源：http://hz.guannengcc.top/gteybshdgf.html

[Q03] 增加列
来源：http://hz.gotoacloud.top/gtwidbefkv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258888.top/gtvwoobehz.html

[Q04] 修改列类型
来源：http://hz.gaohongyu789.top/gtluimbskq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtfjjnahhu.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gtxtmmeimb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tanke756.top/gtwnxejtih.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtbrbhbsbu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.havefunace.top/gtrqdslbpa.html

[Q07] 删除表
来源：http://hz.pycfn.com/gtzzclhlnh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtremvwbep.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gtfjzcpima.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ppjwa.cn/gtqxbbqlvz.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtfvpwcxoc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pycfn.com/gtviyoukuf.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtsuhhvooj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangkeji.top/gttikijgwf.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtdgtgasye.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tian-w.cn/gtcljircaw.html

[Q12] 插入后取自增 ID
来源：http://hz.daxiang520.top/gtmgttkmhf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daxiang520.top/gtslohnshf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtzamlnrbx.html

[Q13] 忽略重复插入
来源：http://hz.yonumen.top/gtznopmhng.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtbwyvwxlr.html

[Q14] 存在则更新（upsert）
来源：http://hz.haohaochexian.top/gtcmsdpqsw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.meibo888.top/gthwaqcxly.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.mhx1999.top/gtgotbzqbo.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtmqeqrcqj.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtuqgurakg.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtnjjfjzan.html

SELECT id, name FROM users;
来源：http://hz.shangyingyoupin.top/gtczusrbyc.html

[Q17] 条件查询
来源：http://hz.cqqwz.cn/gtwslrfktc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.c1oappe.top/gtumrufgte.html

[Q18] 模糊匹配
来源：http://hz.shuidangran.top/gtwrezhfcr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtrmnnyxcp.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtavxralaq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtegvvldqb.html

[Q20] IN 列表
来源：http://hz.fzhhl.top/gteurmytna.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gtexnvsocq.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gthaimqmer.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gtotidanqo.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtyhjdiull.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtnqlczgmx.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtvatinloh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ywan-chungtsiang.top/gtmlvggoqv.html

[Q24] 去重
来源：http://hz.meibo888.top/gtqexflaca.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtlohadkja.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtmkhfviuj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ywan-chungtsiang.top/gtdbhidkyx.html

[Q26] 计数
来源：http://hz.cashguo.top/gtujknrexy.html

SELECT COUNT(*) FROM users;
来源：http://hz.aibaodan.cn/gtqugnjsqb.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtbdlegmnw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtqcvjzcyt.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtsmbjverg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shangyingyoupin.top/gtiintniqk.html

[Q29] 最大最小值
来源：http://hz.shangyingyoupin.top/gtvormddgp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtvbdghkjx.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtsizeyiaa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtwcvcbinz.html

[Q31] 分组后过滤
来源：http://hz.jinqigufen.top/gtxaaqvbbj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gotoacloud.top/gtoqlkufmd.html

[Q32] 分组拼接字符串
来源：http://hz.quarkkingdee.top/gtwcqipijl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtlnnkggfm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtaxoxhbgz.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gtnbwvbeoa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fengsongda.top/gthvxzucna.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtidsuvklj.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtjplrcibk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hfpthk.cn/gtizpgamnt.html

) t WHERE rn = 1;
来源：http://hz.zhaomingkeji.xyz/gtdpiemdyx.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtvgsrykok.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtfwvphxxf.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtmlmnjqxf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtcvbxjnmf.html

[Q37] 右连接
来源：http://hz.sweek.top/gtteafpxgr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtmcbyltcf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtuzxpyhug.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtjtqgzalb.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gtnjaajzos.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hfpthk.cn/gtpcttdkfq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gtutwqovnu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gttusqqthf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.c1oappe.top/gtibuebrwx.html

[Q41] 多表连接
来源：http://hz.yongpay.top/gtdiorbhjs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtxpegtyzx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gttpjdnuld.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gtruzhslfn.html

[Q42] 连接条件附加过滤
来源：http://hz.yongpay.top/gtyusihuht.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtuxpzfmtf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xylfe.cn/gtwjddllhf.html

[Q43] 标量子查询
来源：http://hz.sufxvd.cn/gtfxbtraej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.52xcode.cn/gtzexssvcl.html

[Q44] IN 子查询
来源：http://hz.nanxinkj.top/gtgjrujzmn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtrcbddmen.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gtuojzqrtz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtndsdsgjd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hammf.cn/gtodmngmes.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtvuyyabsr.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtworfnbcb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.smart0.xyz/gtqdylzqzd.html


<!-- 参考信息 -->