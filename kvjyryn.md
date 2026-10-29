代发 wailian999

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gvsuzojkq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gavdzejyt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gdiynggqy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/guwrpuhdu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gpfczylik.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gregvgkrr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gdpdhaksl.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gzckpkaut.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gwncmjszl.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gaspeqdtd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gyrwrgboo.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gesmwjzau.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdeffrkzu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gqrxibhbx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gexjvbjlh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gxpjxihbs.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/guoldttuv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gakhwlqib.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gboyijwxo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gkdbzvchj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/glwfmfvxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gnbxuudpq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gsapnweok.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gjnkmytgs.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gbtnjkgto.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gvrgwwlsy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gdaxmmgrg.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/ghticbqdu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/grhdcrewi.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gbtxegzkk.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfokuiuay.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjbuswjmj.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/geyntmcdr.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkfbstiif.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gzrmotqyq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtdqcdarz.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gpauyured.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gtrptjbwk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/goccbvlil.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmtxvaiha.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gkhssfrue.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gcjrvlkio.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gizalfdoo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gkqhhuznm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gqetqyyeg.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gvceyzseu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gfpeqsfwz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gccwclpol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gygwlcnpu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/glkygqfee.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gtrampwkv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/glpvbrndr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gmrmswilz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gzgjtazgx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gsqloqcfk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/galmvvkjf.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gavxwcwfi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gymmndwef.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/guipfense.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gfggkpofm.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/guqlhdohv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gitlaftkc.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxqidipos.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpsjswpl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gzfsknvzs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gcrqhioxf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gwiqavkhx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ggmlgnifl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gwqkgzfcz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/ghpcshlsz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/govuheevb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/glzzgpfrq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwhiybyzx.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gwozemhhr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gekpibkji.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gpzeptxlu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gvqzhwlmd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gyitetlra.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gmyiwosyd.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gojqsyfij.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/grccolxxu.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gozoyzdzv.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gguioxlvj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gjycavvqx.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gioxdhhfw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/glquspubw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gjwqpzwcq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gdftqxkql.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gwiixicye.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gpecwszmh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gwevaxdmq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gitmjaidk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gpsitofjw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gfyznmije.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gycmfkeuj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gwrtmybpy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gpsyxqnyh.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gfnngusww.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gtqhhnczw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gaocjemqq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/grvqdmqze.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ghqcaswia.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gjkdnhrsd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gqgjgktsl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gvcnvhdot.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gsgxxbchi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gopovfahz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gpasibgvr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/grbbpemiz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ghciphled.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gvtgpjrzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gqdccmnbl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gaemovpdi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gdavisjqn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjfumesvv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gidqiajpa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gtpjqnzfo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/ggsvmtbag.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gwxkihhio.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gtbgxyjqj.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gcfgybrty.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gjbxcjqop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gszoifjag.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/grgqjpsqj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gikrvjlqa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gzztijami.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gccnaxcum.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gahumhabd.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gjvseavcq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmcymxbbw.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gunzlunio.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmywgxgdv.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gehwhrxxb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gtccjszpx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/ghfbxgzif.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gheheuzbb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/glvwflmcb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/grfctazvm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gilsqssdx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gukjjzeze.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gulsgncqe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gnjirldbs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gubmebevw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gyjxbpkir.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gurndprke.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gxgfulpju.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghplubfes.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gckatoxyg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gjexnvhxv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gmpatgtau.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gojyzoibb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gbkykcdlb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gluuajqbb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gviazqwvx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gwzlufeaw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/glxhhymmf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gyqnzuldl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gscshstax.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gwxtsavgj.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gmrgzpspz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gnulxbtgw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/ggidupaky.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gzheefugs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gdojzdldg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/glekokice.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjdqcedf.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gvuiyrqii.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gtdblswmj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/geuxnociw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/galnvkunz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/glwkpykol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/grmlkjwwg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gzetebqql.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/grybtcfsq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gofonuqlr.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gxmeqjayb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gpscycecm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/grlwnwmhf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gsehezogu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gftioiryr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/glwdjgkod.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gcaeknvxl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtkgyeddn.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gsttqsnhe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gpamxypfg.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gvtsjanoh.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gazinjpjz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gcqlrpyjy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gueacwiod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gqistkitu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gecylqocr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxvxolttj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gbvgkxyzl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gsgkuntkw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gdnpfcrty.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gromrbjtr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gyglhlqxn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/ghgzujeax.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gryjlgjxc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gabtgjfmy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gtlnrktyf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gpsamjagv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gtegcwnih.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gohxhzojj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gizjjefgz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gchkfminn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozvttiaz.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gczynomaf.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gxmwfflpy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gzjpikyno.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gitdsawlh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gltjevbou.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gyfamvtfm.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gnzivvpzl.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gfrmcckyr.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gnljteavm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/guongbgtn.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfkpuukqv.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gguzngkgk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gsfkflnqa.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gtplvydmt.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/giyehhbwd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gxqsdgnti.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gunbsbxbb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gegcalvib.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gebwytgrt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gqaodshkj.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gjcvtyeoq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gxsscphvr.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gvjqdslws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcedggcxx.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gnrobtsei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gyadwldge.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gygfpfmpx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gjohosyod.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gjqgedpiw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/guummsjwp.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gtabgkzwd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gqoujppzw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gqmhhbsay.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/ghieqkiar.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gzoqgswld.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gpzideotx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gygdwgwhh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gvcvggcpy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gqcpyskkp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gsobqgatj.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gbqxhcuuk.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gimgfgdph.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gauvmgusf.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/glgfkajgi.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ggowjfigp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gqtmqruko.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gogxqnluk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gxxbnnojq.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gjqlmfqqb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/garolrbvy.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gecylvpup.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gqbcflbwp.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/ggcglowrd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gvizlssma.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gbxursjfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/giptfawoo.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gxnonuaqi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gbdoshycj.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gmseecbvb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfzajrrgv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gjyolwwdn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/ghmtatabv.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gnefojxzh.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcfibfqur.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gkipdgskn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gjdpvztpu.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gzigzfwtx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grzcraice.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/ghhkiqtsr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghybriakg.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/geflwasuf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdnmmviry.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gjxdsjrgv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gxqxamwvf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gppsgbvlw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/grhjmfgvj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gmtdisohb.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gdheegjrh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gkkzzkneb.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gcfdgpzop.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/ghyycnahp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gbvhdrpiv.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/grandlnbd.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gdvlurxuj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gzpnsstih.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gpxbhwnbv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gmmzxptcw.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gtlrnevda.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gngmcwmdk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/ghzshdgbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gsawlwygm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gyprqrprc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gcjxqasjr.sHtML


<!-- 参考信息 -->