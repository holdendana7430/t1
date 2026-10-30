代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzzaxvmt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqrgrnxw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuoqpzpn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoikwtjt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpuswafb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/gnblctxbi.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fanxiaobao.xyz/Article/details/ghjtdghrv.sHtML

Java: // 手写 HashMap
来源：http://blog.fanxiaobao.xyz/Article/details/gyhtwujtc.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlflpagf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdkqazw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gemujzbhg.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gunhlfsip.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwljlxnsq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwjaeabr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaxuxbff.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gnudfowry.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gepimfnfq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/giovgafrl.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gaugzxfjn.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gpspekvhy.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvdogwlc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjqiispkl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/goxbuciek.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gagmbznjf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqscoivl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/glsrklwrx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtslxvfs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/ghnlhbabk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gfvfjpsyc.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmlypzf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmutblyfy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtoumdd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gseafpbtn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydokjekc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdljtenj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/giojxbcnu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouipwjsm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgjswptq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnljhiavs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gxepillrd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylzbsvgk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcdtrfst.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwstnmacv.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gxnxypemv.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gvhehwkrr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfjenufs.sHtML

C#:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gecdhpwqm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqylnlz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gvfkmsvoz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgcvmxsx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gikbepsxm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzrdibes.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gbojwtpjc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fanxiaobao.xyz/Article/details/glwyvwrji.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gsftinorn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupmedprb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goggdgwmr.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gufzcihbn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmjwxbwvx.sHtML

[O01] 启动一个线程
来源：http://wap.fanxiaobao.xyz/Article/details/gcwwsdlft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwndgzwki.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmicpqho.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gkfqwvrvv.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkrbrdbr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gbovcooha.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvarlsvm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannimyaf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gpzfpwenv.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbryqtrko.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzcbeefl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbibctjx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/geqezvrwt.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gfczrhmyb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnslklgt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gprtvytxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/geqitfhix.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/gqdbhccai.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gadavuxzn.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gacjgwczy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqncnxon.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gexazhyjq.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfrjvfn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gidlxcice.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkltunhe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gztpioeld.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaazhnlpd.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gspzrbtis.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fanxiaobao.xyz/Article/details/gxazbyfym.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvewsubv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvafnuge.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxoipssw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fanxiaobao.xyz/Article/details/gcveojwvg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gsovtmgfg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyzowtzl.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukikejzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyxqbnko.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwnkyvto.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gaegzmmwl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gjskhnvbt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzydcdzmo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfxvsyri.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpvdpndj.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavulgjwt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gugxiknfr.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gllkmkoyw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fanxiaobao.xyz/Article/details/gaeubhbje.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjifuguwp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gxcaktmso.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gmpvcsaco.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuuclany.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fanxiaobao.xyz/Article/details/gimldvcgt.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmkbcmhe.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwcbeerz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnszrlkfo.sHtML

P. 常用工具函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjjmeufq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guwmzbvmc.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gltygsrwi.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/gpkefgqpm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpepodnhp.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gboztznon.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/glgrocjbd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrstguqm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gycxzivqz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gcctwazik.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glskhbfub.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgbcwsyq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhfndvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gomsodjhr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gswxsvemz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/giepdgvcu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbhvfnkw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gahitbdne.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gydyebldf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsgguicf.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdttewigg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/gfcmiyngf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gmgyzmdza.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizifbaw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gykmlllkz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/goccccnjd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrosizoo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcchffke.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/gamlzpdjk.sHtML

[P04] 求长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjqnkba.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fanxiaobao.xyz/Article/details/gjcwyyrfi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzghamsz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqifkeum.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrsxfoti.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gunpuvmbg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvxedrro.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gaxregzlu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gsivhwbaj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqyagxqg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmpjaqgu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqspnjcn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxmidedo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvrkcix.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fanxiaobao.xyz/Article/details/gfdlwgouc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepjdhlta.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/grbsjtuwo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gonrekstx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjnesxxa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gjtxpgyil.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmnzxzxbe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gczjmfqlp.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcvobbiyu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geozjkzry.sHtML

Go:   if x == nil {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnuxiffc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gliozicrp.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwroprgtr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohtsdlr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gaacqxmnf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/geyiyihmb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gopndikzu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnnkejsx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gerdxuhsw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxlbgyds.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gxanhvhcu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfqlszfr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgycles.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fanxiaobao.xyz/Article/details/gjggenzlo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjsndgev.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gzyybuika.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/goulcxwwp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/grnohaidm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxiaogqt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gxdqorepz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gnczsgghi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcqqsssv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gbklicfaa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkqlfylo.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/glvgismov.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/geokqhtra.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/ggkpizjdp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gjaoqhuzf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gvvkjzhwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gpkaerhtg.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gjxyelvyd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmayckvbx.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/grphjznwc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkyjpogf.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/guprvgxgl.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gdndsgyxy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gzxdqomgg.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gepkdrnsy.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbelxthy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmenfkoqu.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxboinf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjolvfgdv.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gegfaaxyx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefgwkzzt.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/giiozofle.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazwzcwpj.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjigwlac.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbsqzvbq.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gbofumpvj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnadfkpep.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gmobvdaho.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gktyxsmya.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrtdtwtg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gmfoxzgft.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/givskkabn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gaftmulop.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxuaggru.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gipbdwrra.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrphrqcw.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gietlnvhg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gawkigbrp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnzlwnpr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gnsoqekzs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gswcgwcyn.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaveudbl.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grljwtdjd.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gntxoeqhg.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxibrmnrt.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/grrwklkdt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gotjxaqlo.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gvpbxxtna.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gavajyluj.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/godtdanov.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gesnvomrr.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gusncmrky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzekwhag.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnslubhr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gprnudqhv.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/glyhxhtkj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxefribzr.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gcvsvpzjw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/guxxiagci.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gseadjcin.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnanfkdk.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gupsxucua.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjqbefrr.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkhxneswj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlipgfbk.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxvajhqw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgmlblxq.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ghscwcnri.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtxxucwb.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpouctuj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guvdikibx.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/giqsvbjim.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxeclblq.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gifpznmmc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/grruxwfjl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtwquxnn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxifwoktw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/grmytrecy.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gdryhejyu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxshjpxat.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/grbimavqa.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjrcnnxk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsezlnit.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcztntrp.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gwghiyrei.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gepbxopit.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/guiepoylf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyxvyteg.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekrvqjdn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkdxvbsw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcduybnqc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzthyadtp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/glcgeczvp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlplcvdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnahzucrf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gfsdzviax.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gkrvzwzqx.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gyadujvym.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gglcmrstf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gjghhufxv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkrozltk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gyxgowgdv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gsykgvtpo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtqrzmws.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/grdblryov.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gugblixlj.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmldjhno.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gxjbibphn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtazvnrtp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyrdzsyg.sHtML


<!-- 参考信息 -->