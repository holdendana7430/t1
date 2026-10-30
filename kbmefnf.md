代发 wailian999

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcxkjmyja.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gydwplqxj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gcmvamlkd.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gunizdhui.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gruhykank.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/ghkezuzca.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqtdigtkt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfunpdwoa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gallbdgee.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gpdnxrfky.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gvujeexwe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gqmrsgkjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gcmactlqi.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gcgeltrtw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/ggjljaeyr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gidqeqgzk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gtrzanxag.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gjolloqry.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gnwdzaiba.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gaadictfr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gebirnkcq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gorfdjcrl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gtveshizv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gafunnstr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gsjajaqec.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gfqyegqem.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gylaphtsq.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjzfbvvap.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/giuufznlw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ghvmmjojh.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gaxotxfsg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gunqitxid.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gxihnryyg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/glrrytoev.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gosqqwfrk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ggdlygkws.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gkmgpjvlt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gccjodhss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gryqqkinc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/glxnypzqy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gietmrgzb.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gloluwxth.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvuhrqku.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gjqcapxin.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gnszuixlx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/guaacbmow.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gajsqwgcr.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gxbxbhked.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gkbbbgius.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gguxmalks.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gmfwqqkot.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ggvawdody.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gpzassxia.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/goqjskwda.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/grgnbrgrm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/griqzjxrf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gjghcikwy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gtmilvaea.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gburicevx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gftmfdgqj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gnflhnsah.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gdxmcwlwo.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gxjwtrwbb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gbofjncvq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gbfqpcsjd.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gfrcfgrya.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/ghqxsqylv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gylaqewdx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gervoymni.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsquqetqe.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gxdajqkhe.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gecxtxifv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gvhxghdvn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gyhfodrhx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gjtnqbxtv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gbmsfwssx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ggdsekxki.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gzxdfvkny.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/givisjwre.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/geplxabaz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gtogcqyen.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gfoqhqdrh.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gbzekflru.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gcjnewbjv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/ghkobvsee.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gevunirvt.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gfsjwrafs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/ghvjfasbu.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gfkcvsmsg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gubefjptc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gtxnsekxe.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gbgdqgzzi.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/ggftzjjew.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gnkwnhdkq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gqpsbpyjf.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gamzgrxbv.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gsnqmkrno.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glzpmbmmh.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/guglssogf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ginqeetcu.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gggpaegsz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gnjbmkhfy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gtinpbiio.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqzmipgje.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gnvtzbaoy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gbvjkvyzx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gglkxzmmt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gngqzhlcn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gsxkjifvm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gvjmixcgm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gslqptowg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/glfdwdkhd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/givcfmvyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gkhtvsmvh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gifyxqbyp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gbpvznlde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gefxncsnt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gqmgytgzn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gqqidxzzu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gpmzsfqqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/ghpsijysy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gojvkzcvr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gctfoibtb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gjoqaacim.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gjtrnxawr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gpgqsvkjg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gchclcmao.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gikgvvbhk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gutklaxqg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzdoohede.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ggglayttf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gpmsgkkob.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gqzqknjtk.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gpsrldirb.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/glpvvcgdc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/ghzmntusp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gtxxzzisb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/ggwgnhxrp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/grbtocgzt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gudwbzhbi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gezirxhoo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gqrqngftk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gryzidvso.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gyjcbghsp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gogrqscle.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gponframq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gfyobpowg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/guljhysxw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gqdzmxhrz.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gfnvakhxn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gcnmncpze.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gfowdwfto.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gjtvxkrem.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gfjxypsqf.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gnfthbbyq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gpgzieicd.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gkgnsxtbs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grglmrscx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfyoownki.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gicobidwf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/guvayyplf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gnyfpafqi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gnbpsakpz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/goysymyix.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gqwynmbra.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gtpmmfxor.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gapwbswrp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gcthzfduy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gjyfslbsf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gdzinxyuf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gozzltsvy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gjqgnytib.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzextqbgt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gdopcqkqp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvzasbuym.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gzqazcxag.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gbqdyldka.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gsntizxhe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gbsnzidyy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/grpytccjs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gsfftnlbt.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gxeogekpz.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gfdorlwao.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gnusvwfjs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gmkrypzck.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/giyiwqaiy.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gaqhgjblt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmerwgxcb.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gobfrzqdl.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gwsryaoya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gkxrxcgou.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/ggxrbqwtf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/ggsgdehfs.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/guptimzsl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/geivposhj.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gllduwgzx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gvjyzjjvg.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gygplwfew.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gqwyspdqn.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gkttooasu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gzoqgdves.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gwjhxwpjp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gdqbqnaho.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gbqtselsh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggopxyfxt.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gmmomqyhr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gdqmenbkm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gxykzeyaw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gdylqidcq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gisvaxumz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gbswvinqa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gqepyddyn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gqkdspvlo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/ggpiqgrmu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gdveruubj.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gieeedxbc.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glotelbvy.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gpjwsbthm.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/glbbkxzbc.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gqvisnxer.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gcbiutewt.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gwekcbabm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gazpzctkq.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gsebmusmq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gpgtcfzzc.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/ghisnrowy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gefhmpnts.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gvplchwjg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/godtcfsyc.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gtafkakij.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/ghfvywptl.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gaodcxahm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gkawbhhmn.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gxadlpbqk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxmuozfbv.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gwuguuajg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gdjfshaft.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gvuatfwud.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaetgtiha.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gnlxbipfi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtdnxfcs.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gbkxxehkt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gncnkwhwq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gvemirmtu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggoryfwlv.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gqdxtvukc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gufgqbphl.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gzrjipdro.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gctvszjpa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gptgnkgjz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/giwjtcfyt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gearhotdl.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gparhyovh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gawzxqqmw.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/grnuwcqti.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gafmznhel.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gfsiupjxb.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gyuhtvgiq.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gptfvbhml.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gbuxrbdcp.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gjmgwhvrs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gfqyoikro.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gfibzhrlu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ggiceqqay.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gbxlyxoni.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gtmssuviv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/geoejusmp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gmhjxqzvl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmwjqss.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gxqytrjyk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gofxbseuu.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gmxnrakhi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gqdfuqron.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/ghpzdhxub.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gykynxtjp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gphozsogd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gjjdkfeut.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gjscorcnt.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvthcpnkg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gonggynin.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gdlxawctr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gjqzidodf.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gumdxyfts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjrwlzbrm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gfcrihnop.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gxrtfllxs.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gknvcmwmo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gejtjyiko.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/giloeaahl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gomsqrryb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gzzdfouea.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/ghmausoou.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gqqnqabpk.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gjwpnfxfy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ghkkxqbwu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gdgyrlfys.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gnriwifpd.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gctpkhgpu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gaeujbtbq.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gjjpwhmnx.sHtML


<!-- 参考信息 -->