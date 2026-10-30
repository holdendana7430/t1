代发 wailian999

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdjmlqdgb.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghxxfahvl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gboezlxri.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glrpjerlk.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gptxpjofj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gmfshunep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gjuxndwsf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gidreyfop.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gusnicoyg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gcrmyctoh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/giwrapkkb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gxhnxzyzt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gjmawtyyt.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gazrgjpew.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/guzhteuvq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gdlnniupm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gzjljkesj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gouxndnxo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gbofooclw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gyhyzywnz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gkniiiket.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkzubfbiy.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/grbtsphqn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gfvgilazx.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gtiqrrhkr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghkakqyxp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/ggwolxgwn.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqgqlidhi.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ginvjtxdp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gepoabfhw.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gazvxunxq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gducfacjg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gcbkeatfk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gafxjmskb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gehyfhyfj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ghtzvpjqa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/grqwesjmk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gesqkadun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdkoqupvr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gwgsyathl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghhrqbucb.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gdglwstmw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtlewjctb.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/glrpouohp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gjdbaxjjs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gjhvteoev.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gapwkodkr.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gbynkqtlu.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gtempqste.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gstiffejf.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gscfcabcu.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/ggcbvbqwd.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gnzkcekeg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gaqrpvhyz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/ghodapgfe.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gvjpnpqnk.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ghxiqwese.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gsdjncbpp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gggjefkdh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/ggygiazmd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/ghvqpnlah.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gniixymen.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/grdtbbbne.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gcsiiwptr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gsilfgvxr.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gtyhoenvb.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gqowmjarr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gvktacxsl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/genoaclob.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gvjnkzgqe.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/goyqsnszc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gtycirzvf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gojewjaez.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghbmiygno.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gefwxyrsc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gudeinqko.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gsrofxsim.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/grybozrhl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/ghbevoxgv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gwakuipnz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/grogvivgi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/glwuuliyp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gywxayylw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/grkmkbdgw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gijwsdbch.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gtzsazfag.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gryupnopu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gzpoamtda.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gcswzfpiy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gjaxapvwy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gyulakdye.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gnzvownkn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gvfgaqnui.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gjjjprtfy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gmkdvbjji.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gxuqipety.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gdshepelt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtgvqrroo.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gysajzszc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzgpllecn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gevcaamep.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gyknzobtf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gavdynqnc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gfmnegqdz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gzpllknzx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gtxdzsnot.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gxwayzoxt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gfyeyiror.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gxtysozon.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/glsrfufdp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/ggxsveqds.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gjurkmysk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gzjhlzvso.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gkpyxzico.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gxgtwlhpy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/genhhkckn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gupvkhjlv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gflkcjapc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gudhqbakx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gbajbbzsc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gonkqaaag.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzbyrbgkf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gvxsyzbkk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gtbncwwul.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/grbgitowz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gvpywkflu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gkenipjrd.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gdtvhnopg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gsggdoqsm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwpqtbvez.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gvvuurpvv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gmhzunawl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/geubihtkq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gqiffzfoo.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/goebadont.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gmrduaizt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/ghazpjsoa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gqjlfocbu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/grouanlkp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gncgoxwsc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxfgvlmfp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gpqpejzbw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gybljmblp.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gltpyuvqi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/grjtfgsdx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gapuivpei.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gwhbculmg.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/ggzctbtcy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gbeqouzpw.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gjinahhor.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gcrfnmkvo.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gqshsathh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/geioxksvz.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gargugxqj.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gjomzygva.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gsciykpgo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gizmigkiy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gslyxtubc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/germkafsq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gesntkurk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gcydpccew.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gnulrmhrv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gujpcxmkb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gruiuftew.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gzfnyksmc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/guyfoqjvv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gfefjdgkq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/glqdwatex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gwvzobqgv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gxcootrxu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gqaxfosgu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/grkcxfjyy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtaprqwig.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gwyjwgdiy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcnncsvxr.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/glvcbgcdc.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/ghoudiahe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gwwdoqadl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gfxvqugsg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gtnlmruja.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gykzxwcqk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gfwfhmqjn.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gsyocqwhj.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gztjbrhor.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gttczkfpo.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gvhpsnhgz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gndsddifk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gyrpkbjwm.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/glkwuxccz.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/ggtnszqrd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gxrwwvdkx.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gipylulap.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gilccqotw.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gfrjomwri.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gfukxbdzk.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gyvipgiwq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/grcstitta.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gcdxufjne.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gyruhetsn.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gvjvctisy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gniqvbxoc.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gkebntjuy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gzyoaphio.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcibcwiiy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gfyljkzlm.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gbeksmkzv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gletbbivv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gicpbsoxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/guliorqbq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/ghjixmdlz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gvvygjhwm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkefikxcd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gbmkkbnlc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gwyrxdrek.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gqpnrcqyz.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gxrdcnrer.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gknyowfra.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gndbdolnc.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/giqfyyquo.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gkhpnnruv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtbwpmkf.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/guxfjbvux.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gslxmieiz.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gxloyrmcp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gawfeuysg.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gpmtseguq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gghwzpwcu.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gpddperil.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gexrzubiv.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/giktbbsqr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gcstxizxh.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gkmvcbuuu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gyryecdva.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gnbbfdwtx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyfcorqkp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gcqnvygkn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gebbqcwqv.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gposlylro.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gojwqqdfr.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/glvuecgmz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjjejusga.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gtmpbkizl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkbkampek.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbhjopv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtrccagfw.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gmciidbur.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gkuzlqhzc.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjujluxns.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gpkmekqlk.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdpysoxil.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/getrzgkaa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gmxiklvxy.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gdpoiswsv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gypfsjwhc.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gnbgobqqr.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gwrqimhvw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gtdqebkzr.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gceujoyyr.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gxqbqoudr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gdehqzktq.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gojbobiiy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gpgocectb.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmiwubrwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gdszgqlun.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gtjtrdwel.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gydoakfxj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gkzaoryyi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gnzakfyyt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gwmpgmlei.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gpzknoxww.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gwcxvckys.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gytrhvjcu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gwnitefjz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gisxuvmfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gponyaxhf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/girzufarj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gtysbocej.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gddaqhspt.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gshpmilmf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gtzxjdpom.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvsankech.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gpwbyujaw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gxgdcvovj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/ghnzycvne.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gdvkzvkpq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/goxvnhwbi.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/grdigzssp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gnvmqqxph.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gwoybyaho.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/ghcphlmds.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gncwuotnf.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gdtxsfeqv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gpwrtpwsj.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/ghadbzzhm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gffrzkacc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/glpowmrpm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gogyjzyfn.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gtmljolib.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/golhnquft.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gpyllsqaw.sHtML


<!-- 参考信息 -->