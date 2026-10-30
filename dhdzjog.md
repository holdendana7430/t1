代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphsutbat.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlhgrska.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gyafegqyj.sHtML

Ruby: a.gcd(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcdbdhaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjssgmvdm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcffatkz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gentlzaem.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gqstrfecf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gqyulbnkr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gwyyzmooa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaqqdawx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjcacpmx.sHtML

Ruby: s == s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnrzyshv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpxzruay.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvltxjwfu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fanxiaobao.xyz/Article/details/gmudkqpzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fanxiaobao.xyz/Article/details/ghyadnmti.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/glmljwilt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsyqkqhg.sHtML

Java: // 手写 HashMap
来源：http://mobile.fanxiaobao.xyz/Article/details/geqkpkyiq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvnvmqyz.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/guzqcwhmw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gzkbcmuxn.sHtML

[N08] 生成全排列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmqnkcgf.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrbxcova.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gqphllaex.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkozxbgj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkpumprb.sHtML

Java: // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gijcrexyn.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gsiyblplt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsxioeeg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwzjhsji.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/givxnoxyn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gsajejhqt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/geghxeixn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhhjdgzb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gjuinifop.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/grefxcomc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gyhtejvyw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzljokzt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxqipbv.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gvfobvyyl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrxgdutv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqaeyqoy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gseeydglt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeavyoxa.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grmlxzucf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwteevfy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gbfxrtjnc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfrzquws.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gynwxlzsl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpbkxjw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmfjgodbv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gmvsodoiw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzqybcwt.sHtML

Java: // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gprqjkgdj.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gwjoiaxdr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gmyfndhgx.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/ghslbipmy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfajehqok.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fanxiaobao.xyz/Article/details/goowegpcp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gqfhpdoxp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gqlkqdlgw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gzefwiaaz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpxbbbj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtefotume.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxqjzbdb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwcvowwo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaaudadex.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gbssjdjru.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxqatsp.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyxfsjmc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gmudwkcyd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/ggqxmukuu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gppchtzsg.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxmsxwq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gnsjhtkkp.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbwyvdfe.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnnbpdeh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gotlayfgk.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbagziag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/goyduezrd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gedyjuwuw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gkcjbpuqt.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkutntq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgzfraj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geydehjln.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fanxiaobao.xyz/Article/details/ghewsikou.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/gzualohok.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/guvbesvjw.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gboimfbfp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gvshuwdvx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/ggzduftzq.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gthuulata.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/guvsujyqc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfilwgum.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcochrjiz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbhkvukd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gmznryrwd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiqzglmg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjtgrpxf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnrevjuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graedqzqg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnttnxgez.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gunxjoxoj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqglazmq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsabhtac.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fanxiaobao.xyz/Article/details/gerhorjks.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvswvlrti.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/ghmmmntxd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gepstkfie.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/girnfhtyy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gfebbqjjt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gwotncaaf.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuqgkgjh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwjbokvh.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gzlzydijt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdugdztyr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfquvjaq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gexgsasrt.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gdqbmukbf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gbqysovba.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/getlyeran.sHtML

Ruby: // fork 块
来源：http://blog.fanxiaobao.xyz/Article/details/gadvuchuc.sHtML

C#:   Parallel.For
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmashlws.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdgiowrzw.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guoxsanqj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbcgzbio.sHtML

[P01] 生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gkdstdojj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblcghuxn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoedbocc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gejleehzr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbnzmid.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgehxkxt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqkyddz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpkqxnqu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gwcwzlvqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gyntoqvad.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glutyfhof.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbniivdrh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gswmpvvyc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbtiwijt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/ghndwtqrl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gnycoszfl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpcxjvmn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpnagxbm.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjczbgfcm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/galjzmqke.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuwwjdxf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmlqipsi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmuzrzb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiyrbfps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpsnefkm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadrggfgc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnirjsrxu.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghdzpbfdr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjedegbn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzsbatdi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdntztnoj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gliphlbbo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glefvzrjv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxzhcspv.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gbtbkwugo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscxqjqlt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gygkjkzdb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfrynjtk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/glxtlduhm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/gaekyemrd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhjbhhih.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjafkqazo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gcvmrhiky.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gvyaurrtx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbprhof.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fanxiaobao.xyz/Article/details/goliorppd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwzquxo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaplzgowy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmoegqc.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvqudivbk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkcuqmzb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgydzpfb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxwigbdf.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gabxuipnl.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqexglbn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/gxyckqbal.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtgdvnpws.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwhehqty.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gttnnblwn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fanxiaobao.xyz/Article/details/glxnbgtwy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/grrvlreof.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/glsvjlpyn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggklzetng.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/gosuxakgz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqkbsafy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnljoxpsa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gogmqhggg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbsobouc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/geybsoxtp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtwggpus.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjlunqel.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvzigrpa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gniukrchv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzazcqmaf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gclkvcjbs.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gstzbatke.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gxlgkcsju.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumzgviqt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gbejbkdcm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gynnwliyv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcnhnrrp.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebpszzj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/grgudqxji.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxtoahl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxsjsdpc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywockapc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfwckpkx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/grefwqsgq.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxhyziex.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejjjozhb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gwnawldla.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/givctqxmq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwraaoed.sHtML

[Q05] 重命名列
来源：http://wap.fanxiaobao.xyz/Article/details/gumotdogb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gtosjjejp.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjwcbnze.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdobztqxw.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunykufqf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuputvhn.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gobuyxyvy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gskmlpylv.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gggtqyafc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnzlpwbd.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgqoghoe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbshelqvz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrwgmoka.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gorkxuygu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gldekhhlp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gghteipdr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpvkkeaq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gzitggkil.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gnfprlevr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gdipwoatj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmbpmeqa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtijivaao.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkxkwvge.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvndwucs.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gdnmjcjhu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmgiryht.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gmtjsbnum.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmyzsaip.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gadzdcdgj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gygekaima.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gsfijegzq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmuhhkwu.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpssrvayy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdkynbup.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gwajqxffl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdlateah.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpmvczjr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasxfqddo.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gfzvvpbxn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcjownjg.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/geyoyfxtk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfletypst.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvvbbsnp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqagmddp.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjutzwayd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhqbybhr.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtossorbw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvrorusi.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgtskkvy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwjctvxp.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghemztipz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjnesmfhu.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gxqojafjd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcfzjqjd.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ggqcnheac.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gzkmfkguf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/giritcrpc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqzzhhv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcauaqpd.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqescfe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhaglzuy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkggqpyu.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gietawbdn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdameqgc.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggshfulqr.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbkgxnbq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfylqgnpz.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbhudzel.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxejgosmf.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gkdeuygod.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gfnustxvm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/grvxxujmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwstnycjt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/goaqaxhfo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/grngccmlx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/goixjthaj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmxpjdvm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzszjsqqc.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gsmobubom.sHtML


<!-- 参考信息 -->