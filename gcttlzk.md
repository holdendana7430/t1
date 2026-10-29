代发 wailian999

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gjsxzghzx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gpvjshdlc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gpnxyrcqo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmxmstvap.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ghopgrnsc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/ggotvttvv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gfoywhafs.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gsafpxbfh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqbisju.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gvpjcwhyz.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gvzidvyil.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/geajvjtye.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvndiykcw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gugnzgzba.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gmjfgehub.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gfjmyhauu.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gndsqykuv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gcmivqvus.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gbqgmyuum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gghhibtfy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gcpzguqqn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gokybizrz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gbkbsetlu.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gbibpfpnj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gtmlrosjt.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/ggiqzlshw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gphshooks.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gmqmwpqee.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmeoyewgj.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gfnqijzkz.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghgsradhw.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glhcoctcw.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzljyhzvb.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghlkjvqyg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gcovngidq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxkhmgdkl.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/guklspymr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/geaujmuvz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/glqtppgdl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gkbzoyjxc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/ggfebfzhs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gokmbciay.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gccgjulbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghmanhadx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gjivjvtoa.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gpweornbg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gexbakjdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gnqtgwlyf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/grczslvgv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gfuqxrthj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gaceyhbkk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/ggslfvnbr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gemmnsusk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gsnjwvxqv.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gdgfzxncs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gxdgbzhgh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gbmxniwyx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gpupvflbk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gpkxseiyh.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gfeptwzef.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ghiqyryrl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gxcfwmmeu.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gugivjqeg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gmpwbdmzv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gpuicfvrg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gqcastdtk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gklsksczr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gtvzqhiso.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gsgxojkcb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gpcnzodfa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gfvxzyqcb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gptpjzoeh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmwllawkj.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gotlegamt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsuegmncs.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gevccyxeq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gkyzmtlgk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gouqbkpzw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gdlwyddar.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/glbagwgwr.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gtecomecj.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gutmoxcmf.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gdrwlpymh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/giijnxebg.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/ghjotukxk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gvoebvwis.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gsukbpxmk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/ggrzvwohf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gfdkkmtql.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gierbfpur.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gexyujmsh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/giwmowghc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gadqqzody.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/ggpsfwlpu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gmwcoavjd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/guyovaosx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gdczunzlt.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gsmpbbrzt.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gppmayjwl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gekchkggc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gkliviuho.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkujtjrun.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gbktvapaj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gvxdvrwlv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gwgzgqzoa.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gvizgirts.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gmxisfwtc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gemzmfedr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gaersmqox.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gdmmdgjzu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/ggcxwyxgr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gazrfbezn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/ghfnwvpjx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/glhnelhec.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gsgsnaevb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gynaqlobz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gvfkcsjmd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/glpijuauf.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gspngljqb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gxtnthwmx.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvzwvqf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gwvyoshgh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/ghbhvqxsb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/ggjncybsv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/guekmxaey.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gjsrakuwq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gujkqyezp.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gqljmtxsu.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gxwifkngp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnrrzlxwl.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gjmsncfde.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsqfahkwe.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gcwvwbuui.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gdpnxnfyz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/grpbmwhai.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/grrjfjuxn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gxapxrvyq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gzcsovdwi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gmjqwjowa.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gzwjycoos.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/glllfmqvx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/grrinbgdj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gdbbedeke.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gvtsvjaew.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gzbqernfe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gaweztlwq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gwtgfnpoq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/glizgxsjq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/grecmrumn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gxuihbxeq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gvvuijzdl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gqqimfcod.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gqfjsxiqj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gdxfztcfg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ghqibyewf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/giibnmopp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gtezbvrbi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gmajpvuel.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gvkdttiwp.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/giexnxsaj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gqbzsscqk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/grsqzdise.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gwwolrmzn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gtjhjullw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ganxhhble.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gcbatsjly.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gbzzdtkuk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkiahkaia.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gnvlwlxrr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gfczwyckv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/ginlibvff.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/glucuzmpi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gskfgjllk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/geymsqhrk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwktddrju.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gyyenhaxf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gvulxqgef.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gwtyixvof.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/glgdrdkoz.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/glnjgauth.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gifqsfvtg.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gawcgaolg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gpwzogcpu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gqwedyzoi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gzhyoavgj.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gciuwxwts.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gvjrjlhvx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gtvdinwug.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/goiprkvhe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gfcrexapn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gumvjzqem.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gmmprivln.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gyipjwxvd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/glbxlavui.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/ggdtwplmf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gsvhrqdos.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gkpywvhcv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gsjzwnwdv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gjzqolwgh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gljlbmumj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gncgvjgbj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gfjdvxter.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gluvhlkvm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/ggzqmzfac.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsfxbwuss.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gwctasxmq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grdutfbea.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gbioctvgu.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gyvrpaixv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gtpzfhupc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gvrbgjybv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gufwwgqqw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gofvrcgfz.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gnkrkubns.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gsalvbxyw.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gzgermoih.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gjvlfhczc.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gjujwykxv.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gxzggspdb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/ggvdjbgze.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gbkgbcbzs.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gwdlouhrw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gtgabzost.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gzplezlob.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gdcuxsdnc.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gexybpaiw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gqlsaqjsa.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gozcthqlx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gonvftdsp.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gocudgooe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gaicdwwza.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gbuzooqfm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkckdyol.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gycsdqhit.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gagzwteou.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/grbolsskn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gbbsnatik.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gafnkskxu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmkhhtlrz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gjilagnje.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gjvanzhou.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gkgimnkdu.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gjsdxfgsw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gazvresui.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gckdgdzlk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/ggmpxdgdy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/glqkmnrgn.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gsupvgydl.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/glazhisrm.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gooupmypv.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkfaboirv.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gxpgfprkc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/ghteckhux.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/ggnwoeozg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/ggssjwxve.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/graxpbqbo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gvgeianbt.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gwhhvzzba.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gmtmxsjvj.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gvrarebdo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gjorloofo.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gqrfhrihk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gwvtsocpj.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gfvrqqiso.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gjqwpjubl.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gofjvapyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/getzuljmu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gdfbuxuei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gdkjlskmk.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gstqfbcxv.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxigtcfhx.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gwkuzrbzo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkgftrsdc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfkkxxy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gipqqkaud.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gtpelafeq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggvkdgnjw.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gtzagmbyj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/grgnvdavl.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gkhqpomot.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gngdodslq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gkqwkglsi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glxyzmigp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gbqmggpyw.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gmouvdepk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gkdazpzdw.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gcqixdiyu.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gfztkztza.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gqvuzoaaw.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gtvebcfno.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gitgzzbsc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpwfhvfei.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gvcekvjcu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gjtdpzypv.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gzkruigkx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gpslmzhan.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gyjkuifzg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gzwidhwlb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gjdkaqpok.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/giekunrum.sHtML


<!-- 参考信息 -->