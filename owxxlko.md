代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gjbbveppx.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gaeexmybb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmkjhumng.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gdpyaarjx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggoyjuxac.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gglcehejh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gcxzyysnv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gokepjasf.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gejwlnbtn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gbsswqovi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gcyofzkxz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gyuvfniwk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gdmlmkwdc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gnokktlye.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gqfwaocgs.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gzxldbetm.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gszixhhky.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gwhhxommw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gyfxnipvi.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gppplnspf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/ghjdazlui.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gkuzijhqf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvekxquns.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glnisower.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghruxysxx.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gecnqenlp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gahgfwqbj.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbiushfhc.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ggzhwqvmg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghahzdnmn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gequyenhf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/glpzqmcfn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gfmsmjljo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmsglgxzz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/grizpyupi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/glncpkfcs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gsripogxz.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gdsezzgwo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gavqbeota.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gdgnwiffm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gcfosjwav.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gdnvdljmu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gvuddvgcs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/glpnqkofl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gxqfmotas.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/ghevhvrit.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gauzirtmp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gygblkwvf.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gwuhftqir.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gfswgeslh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gchiikeam.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gdvxyerki.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmbadnqqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gqadbgexd.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzqqspglf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gxsnozzzf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/guybbodcj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gxnmooaiz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gacpbpcsz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ggfftrzrz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/grocwqenm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/grjfbtcxd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/guvtnkmhi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glnmeevxr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbezicufv.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gaqesmpqv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggtunjdty.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gxvmvupba.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/geylblmuh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/guejkmfdq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gdudcnxiv.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ghexzrnqt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gplyjnvvb.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/ghuytlkkm.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gdglqhcfp.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gytpefscp.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gnrpkxpsg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gtkrnupbf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gvhcsbrqy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/guaiqdxca.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwowighpz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gceoyakac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/givgqzrqc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gbmwqvczj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gbebfthyg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gygocsjue.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gtmxlgntv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gnynqpstr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gueftqljg.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gunlbiziu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gdexeikgl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gxjweibqm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/grhxwuxdn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gybzsgykl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gzqraxdqi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gmjsffasd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gdeyikxlz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gmjeoxklj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzuiebwgb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/ggkutrdog.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gnoukwvlr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gvpjctdby.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gseyfrygl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqbxzaf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gomilqbkr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/guszfdeqb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/girneojzg.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gvaivoksp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gmtwaopqc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gntpexjcx.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gsiynfkcw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gfsxfshdl.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gzaljywxv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gigcbyjmn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/ghavkpmhm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gusanpmxh.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gvkpnyghp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gxrlpcvbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/ghtfazxlx.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/grzejrefs.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gpfyfocps.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqfiqxuqu.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gbtqfvzdp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmzveynqb.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gaoqlulqn.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/ggbbfpxvz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/ggdyrvazl.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gszyqvlwy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gcnddzkuu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gfmasjcrh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/glpwzchrc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gprttdusn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gkfcqaplt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gtievsrrs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gulnjugmu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gouzwnkce.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gzmzfppxv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gsqagkuzx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gtzcpowel.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gxbktogad.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpzvrcllb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gvikobyxm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gfzzisipg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gziccqyji.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gxjxkmgvh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gfnbazqqc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gwsgcvbhj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gpjcuroyu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gbqpsygan.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gxqlymlgx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gmngtekwp.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gwvzqnltz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gnqyroxpu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gslfegklv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gzlsvwxsf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/ginwpdckn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gffyzngnh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gebamgysx.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/glojqlvvq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gqknxumyg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/grjuqwfyg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gksrqznex.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/grihwoizo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/ggbreoebb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gicoijwog.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/giqtdxniq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gilyajrkf.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gdimitzjv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gaupypqcv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ghkrqceqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gwjnmyvpl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gvlwuwpbp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gvbxfpmhg.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmvymertc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gobnnonkx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gmqnhuwem.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/glcpudhmt.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gsagnritp.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gwveftbgk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gylhymmfd.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/goczfzvjt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gvfnixatx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gsehpprvd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gdxcqpnhz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gascyhsvr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gnoofbnaw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gjkbwwwzq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/grgsjyrwf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gfznhdfrx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gkpulwhdq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gibimydfy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gnyzikqbl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gngzqmaam.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gaarqcstn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gkexyenkp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gdlbjyytz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gypnshjuc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gdhfrdqek.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbautscgl.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/guokliizk.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gprfyyjbb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gozttuqft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gxyhkjikn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gfshlbvsq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gblcxelcv.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gktieatwx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gwqczppit.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/ggoqjmici.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gtmbsppdr.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gxsnpvilh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/ghegcbdkz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/goelzybku.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gmmykalou.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gtcjnfrjz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gaglygewx.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/ggbnfkjnn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gopaeugad.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/ghjtcljvo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gozlikoxb.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gtlgnrfse.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gwybqdwfr.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gjerfbaye.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqwhzxcgf.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gjzpenqsf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gapgsmqns.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gtsbwchkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gidxzsbho.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/guguftpxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gzbjwhzpi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gyjbfpvlx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gkdkhhhzk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gkqqasjfv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gmovnjidn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gryrzahtu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/ggyogxmhc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gyvtioafk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gymvjicmb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gnnneaves.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gpczbswcq.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/girrbvfzq.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqdunlzxf.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gvjhyslmu.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gizglrayu.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gcorfopsz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gttzlckkn.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/ggwnqdzke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gnjlvorhr.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gkjyaplxx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gqpxyxrry.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gayswunta.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gkwitpxlv.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gytspugbz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/geqssnfpp.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gjmopbokr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gjqfrkoof.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gyapndbte.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/glaqownki.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gaemfnuru.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gtvqdltfy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gclfimpbl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/ggooopfss.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gnwohflik.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gujxweieg.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gfoylzrln.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkprwfgms.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gqvgowphl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtdchrxtn.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gmshckoxr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnxvdynec.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gxxytsrud.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gckzctpvd.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gqfirbzvv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gxhlehumg.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjmzsvfpe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ggcaqktpa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gosvzpkgs.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gkgnkzjbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gmzerviom.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/godmczqlu.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gukfnxlzs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gtyzzcgzx.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gekhyjfza.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/grvghuddk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gavagfzfc.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gerjdhdwa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gmdmjpckb.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gtnvmibpo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/grkeefers.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gxjqupcaa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gpydbdiwf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gafmnigyi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gplltndal.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/grmmzcxzb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/ghhvkwxbz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gtlaruejv.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gqgqjqiay.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gszmmmtxp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gofvqyiuy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gjthdhxbb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gagrkkcxt.sHtML


<!-- 参考信息 -->