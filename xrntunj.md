代发 wailian999

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwdldmjnh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gbgxdkpxb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gjzefexxa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gahylxwzg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gclfypabj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gukskqbjv.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/ggfsscsxb.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gftlesquz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gvffpicya.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gabeitdur.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gidcwoeml.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/grjjpvptt.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gbbxwnina.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gervzewff.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxhowwsvh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxkluqgyc.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmyxrwdea.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/giyyygprp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gafgbafcj.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gilpbswov.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gwxkuflii.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gtbmokyxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkridma.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/goprvmaib.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/geojwlbjs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/glsjemexo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gpqzdavro.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbwwoirnp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gihmpmbgg.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gszpgmixf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gcnzmmnsf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/ggaqgwxen.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gutsqirtx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/glpybmfvd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gnpsdyenj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gecwdrcmk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gnjkjgilg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gnddqngvc.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gsjotxzhn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gnigyskra.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gvraivlzu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gxifrlpag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/ghbqnzaas.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkoocknfu.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghxurqwrv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gqyrucuke.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gtkxbgyng.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gtiingpyq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gwjvzptku.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gmsfjocrj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gibtwzumq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkqeikwts.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ghinflbcb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gemhqdkbz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gdqzcujih.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gvibpjazp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glxljrfbr.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/glafmjuwo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gboapuykt.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/ghjrcxefb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gdcsygdhh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gizipxzku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gbfmyzptc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gigynumgc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gvjxihujc.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gjzxyrofl.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gpoczbydb.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gxlbplklq.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/ghkcjhwll.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gndvxrgkj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gkpvmnsee.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gsuejbhua.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbgkhhojc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gnczujlse.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gjkmenput.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/guqstyhlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/glsunwkaq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gduvdbiua.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gwmwbzgvo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gsmjnlwxs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gklwiaxdd.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gdnefuozu.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gilyzoibo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gpajsryly.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gtltilfox.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/giytwpsat.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gywnnqkms.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gthvkdxol.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gcrggrbfa.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gyjgwhzjg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gsgqxrssg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gctafouwb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gfkygikgj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gmxbrwaxm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gumbhozrn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gdcxjrmex.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gzkfpvpoc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gsbkzkxqp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmicotgcj.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gnyfdyics.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/goezvwnic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gakvvepve.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/ghhdgcvsm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/genymfnan.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/ghaulrlsz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gfuocfijl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gbshezdnr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfusaoawp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gedswqakk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gyogyvfpl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gidtdtoah.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gcrkwlpaf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ghxuapkgp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnpvlrzuh.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/geirqcntu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghyvmkjpa.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gwwxbiqqe.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/glhqwxdgu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gwbjwxwwq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkcxxvbrn.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/guoikztzt.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gnytqzpws.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gudxtgekq.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gndhrqkhs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gccsiiegn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gkwuggavs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gyzmxhqkw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gfmjwwonr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gdzepflrr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/grfnucswv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gvcpthunc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/grirgqppm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/ggtfqjgqy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ghlnsbcml.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gmanjccnh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gnjdafrxh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gjxvaqjgz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gxozqqrif.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gbjyaqand.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gvlcvxofn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/ghuduymer.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gkoqujowv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gffzfgdlb.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gsizxbhjm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gnmawbsjw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwnhjqchk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/goankuyqm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gyoivdigu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gklflhyrh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/guvdebdqr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/ggwvndpgt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gujlmqdri.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gtwexxnhv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gxdlfelyd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gxjxyussd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gjxfjbvzy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gxytkpmsw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/geiapfcxd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcuucggiz.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/ghjucaeze.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gshijrbke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gapxowsfn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gdewokbkg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyevmcttg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gwnznrxgk.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gikkiioly.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gxkhjcamk.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gpniuxotx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gouduckdt.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gsozifzmq.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gihmfcess.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/glxzyosek.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gvtsgzfks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gdcoyysqj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gptqfismj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gywlzgfte.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gknvqlphv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gvxferwxh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gkmbcmjno.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gvaasfdru.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/grxqkbjgq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/ghyawityj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gtxtlyajj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gmfxduawd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gfromkock.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gneyrpijk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/guefrecqd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gdbdcdevu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gijqrbbxt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/ghlnflzwx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfxyfqisc.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/ghzhienrt.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/glhwbcmxe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gqswiwkvr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ghqhxaoqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gejjvihas.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gsjfmkaob.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gzokyabne.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/guwsewaxg.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gslmclban.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gbilcsnog.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gqiaymuju.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gzmhqzmbr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gezzvvzyg.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/grfadxiho.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gykyvjost.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/geqzdbvie.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gnaqstlpk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/guzmhrwfd.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gbtvawfjn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gludvtcie.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gkihsvkcw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gluijtoiz.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/grqqxznbz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gnwlvzpec.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ggqtutspl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gvuctxedi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/giizjlnul.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gsernlatj.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gfwzwgzcw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gcuomokmd.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gjrprymuv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gjcphdjgx.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/ghuschvbp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gkdvdziny.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gqichwqvi.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gctfpcypo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gjpiofgbb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ghtqkgxdh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gywwcxxpa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gpfjnxuad.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gapqwnwxg.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcytqbamh.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gnxzpkbfh.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gsxtwanzf.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gomtupucm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gqlfaslkp.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gjoroydra.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gsrrhwrqt.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gcrphewlb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/ggzzwqesd.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gxdbvwpqe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gcnvgzsla.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gtxjtaccc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gudfrzuhu.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gcbniwjxo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/ghpbkgmlc.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gslpinsyw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gnkfmznkw.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/glbuvmjsc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxxoynnej.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gqrmkgmtn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gbcknzqrq.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gdzqjwqwy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guaiticlz.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gmamkpnpz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxhtssizq.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gfkrzzpqs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzbhofpci.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gmhdgywov.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkjzsaswc.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gtcwqkleq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkpjkxlrv.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gjcvaxixc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gclkfzlyg.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqjzvujiu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gfcnyssxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gjdyzfigg.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gwojpkjzi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gxafelssl.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gxhcbjgwy.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gohezbcgz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gljxwamxt.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/giygmianf.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gfgodfcqa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gprgsmhbo.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gencgnhas.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gihimkwjj.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/glkdfupps.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gzecygogx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gnyiwsctz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/guzlfgzlj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gkrwsudyz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gjkspeiis.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gqkassmlk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gynevsihp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/guesxmwfi.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gvnownotk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gtavcagpg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gwwgvgjdy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gjtmluccs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gzxmcqvoe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gkoampeex.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gjxhrwwzo.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/giskmsilm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvaozvsfc.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gvbkjrtut.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gobxehbwb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gvzesofvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqvfttndm.sHtML


<!-- 参考信息 -->