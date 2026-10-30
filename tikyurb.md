代发 wailian999

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gxvgzvknv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/ghuizhpxb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gvgkvieml.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gwjsihsux.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gevrrasgi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gxxfohipz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gqgnusxqk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gdfmmvfcp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/ghipjpnub.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/greufkcjx.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gepcjhnts.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghxkjhwhm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gifeirxsy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ggzlxteul.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/grwtxmxrl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/giqjzsifv.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gdkfszmoh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gjbzlkcte.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gjaoblryt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/ggxjnglkg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gqupijiul.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gkxvpnrcz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gptcydlvt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gtphxpzfk.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/glfsuqnud.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gdqrsgzwk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gbukxodvs.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gyqeqprgm.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnmiezaxs.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gamawgqdu.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxbgvydfz.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goxcpidig.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmpblpiih.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsjqbfzbg.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gtrdhgerb.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaitmktzx.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gaejzhcmd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gerwdopdm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghrfyzumv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqejvyfol.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gzvpnrfzk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gslnpqzoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gfrvhpcmt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gjuzuquwv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gpieahxib.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gbyjhmbxj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gmnoawwcd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gfthyzqbe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gtnxamlfc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gbcanokxh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gmpzladkq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gfshatirw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gupbnwqax.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gxrxkcujf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gyxmkvvra.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/geljrxbja.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/guoyvakkk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gtkbptxyf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gquynkhlo.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/goqnywjcq.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gonjiocyw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gfhkwjysz.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gimlctayh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gimztagfv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/ggnnkifwi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gmetwcasy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gljczvbpn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmgxnvmbl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gyxkfufns.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gajsquhow.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gberykhoa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gorggqomw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxjytleoc.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gjsraggse.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghshzfssi.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gknyqfatz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/grqmutljz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/ggafvqsul.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gytmxfwjl.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gobzqbirl.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/ggrrxjilu.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gizsnyeuu.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gtsejeipr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gjccztemu.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gisrsbmrk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/guocrfohb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gcwkraxle.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvsxuzexg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gimqffayy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/guxgiakmg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gqiehbiac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gniafwipo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gkkcddwgd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gukfvthvu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/ghbfhbhju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gdeiuuncq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gpmwcgfkq.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnvfyttxw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/ghznmpbwm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/goibvadjd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gpfiiczif.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gugjlndka.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gjtbffiow.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gvftxipdr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gnvdjeymd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gkvonlocq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gbtvwkbef.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gwgzyroyc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/ghivvaowe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/glvzrccfc.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gzixyqhjv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gobkabbsz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gbmxgymcz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/glnamzsyc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gvojraqfg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/guzxgazrl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gybnjxfax.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gkkriorti.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gchbnlpfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gtyakcpxk.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gruspmlkn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gogzdvlim.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtkhwax.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gpreefexw.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gxeiveagp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/ghtfazgph.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gxclregpn.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gxtnlffsl.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gxcatydll.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxkmlyqhb.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gziuurvzp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqomqkxni.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gcwqktrmg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gsqesziux.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gidqddaey.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gcltufauh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gfnmiuasr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ggyhachmn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gqpergcns.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gcucuwwmq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gthoslfhc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gyjlkhwph.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/grshggzco.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gaqwwgohs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gasaltfkq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gtovnojka.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gkcjoadir.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gptkkutiz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gzsjpbotk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/ggyiywdih.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/giyuahthj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gvaypqiqu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gvrckeaje.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gyecatcrn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/grpntgils.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gbfotinig.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gwoihwcbo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/ghivxscbh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gympfrjnc.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gztymgjzx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gsecrgwia.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gcuoxtlmh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/glvkugdmw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gtazdnnkm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gudnmgpcl.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gwgmmdtmo.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gpwzudilt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gkhlhusjr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/guqosmspd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gnrfwhike.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gergxcjbt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gymfnzqkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gflgmmoyn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/ghkjjhrxs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gbeydscnu.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gykpkkkvo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gbbpbwuuo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gopiplryb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gtnualshy.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/glomrrltu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gbufylhbq.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gpkxltprx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzuyafvel.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gcyxyrcjn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gmijkvgwn.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gmnghrgog.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gwxhrukow.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gdruhsllf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gscpborfc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpjekxjjj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gcznuxaeh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gkzxonmin.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gxscpvnaa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gktblzlvc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gbifjdpph.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/ggmuziqmv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gilscybxs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/ghffepqae.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gxuwzjyfa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gyoacfxao.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gjubsczjf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gghpisdyc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/geoskezjs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gzkrsqhdj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gawnlbraq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gaeunmmxb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzkjkhtym.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gsjwubwmu.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gypfiqqeb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gdcjwelad.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gccafmazm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gktaamobw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gzcpbwmok.sHtML

);
来源：http://blog.fehbvm.com/Article/details/guesijrhs.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gyaycithg.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gfmlhzlwc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gefkkjzjt.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gpfkyvfbg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/ghhezkgfa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gyrggpdcp.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwknnsntv.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gsrtltolh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/geouglfut.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gnluhqamz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gafrpdfws.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gpburpmko.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gbxnkhvzn.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gqpbljzbo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/ggfeqyruk.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/giszbmwkh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gxwqkzxxp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gcpvdwucn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gmanqhbku.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gxceftooq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gwgmlegxs.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gbtjiselt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/grzblufah.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gdhrywwra.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gsuvdnfmd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gclahuwyg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gurslfqfy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gvlyfhvdq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gkfjguqty.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gkuvdmmvd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/ggahtciwt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gshxjyyod.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gkdoixdwh.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/giumwzcex.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gwibhkbuy.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gfcmvfnoc.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geeapvowr.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gfyhdnrvz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gblhleifd.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gdihpebvp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gdvtyiuzz.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gxdbsgjik.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gmddbnqhh.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gckiubowd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gugylohkv.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gnbzbdmlz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gwcshpiuo.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gzoofifwa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gakftcikr.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gvcqkykic.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gyvgdlkyc.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gvmumxizv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gngpolyne.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gselirgdy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gtpfqbkjv.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gggppknbu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmgciwyrr.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gsgebicxp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzbiofold.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gvriykjuw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gdptjakun.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gvayjudqm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/garmcmxue.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/ggetbusfm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvpymfvqb.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gpmdbxxwt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gldmmjbyb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/ggcahzkfj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gpziktdil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gospchkuj.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gyyknrpch.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gybqbeqji.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gsdjaawpe.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gpwfleaxb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gkeetrocs.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gecyvmijk.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/ghekmtrpl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gdicrzxgw.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxltnke.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gzjtcerhy.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ghbeimutf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gqgtkhkvt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gejgeajiu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gufhqjiws.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/guvuyafac.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gsgxkpmqd.sHtML


<!-- 参考信息 -->