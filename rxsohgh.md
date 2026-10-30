代发 wailian999

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/givmkquqn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmtofip.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gibwglttl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gegjhxamv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gryrthoca.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/ggwvwycjv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gwsktpeec.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/glrxsarkg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/giunmpvfz.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gslwqidqd.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/glivfaspb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gcprkqnpj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvblkjpec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gyzimlksd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gkmirbfis.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gcwlxoiau.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gcsedwirt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gegjhvcnm.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gxylptqns.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gunaznptr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/grgnedeur.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gznjgisie.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gdfiupknx.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/grngyubrd.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gfvnmddnn.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gqbgbcmof.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gbteaziqz.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gvanzdwva.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gxhwecned.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gqegtlevn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmtfxgdde.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvmemolkk.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpfjhgbjm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxktdphis.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gxdikssrf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gfjsdgywk.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnbvbxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gnomezvfc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkeribmpb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glskhwssr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/girxibvui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/ghclawppv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gshuuesvq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gjeadylal.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gmjhyrfcb.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gdyqcgimf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gtkjeyewa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gquxlcgoc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gbaxjufgg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gtgfgkspe.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gmlbqyzfi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gosqtyuqp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gzdegnuru.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/goczpaozs.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gulmsekts.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gynnxxbqu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gwrkahorl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gurmeooec.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gepdmicox.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gmeuyaeqo.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmnprygjo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/goyyhbbmx.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/giabuijem.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gvwjhjuia.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gmlmuvztx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gxihyoivf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkmmhxryc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ghaabqtns.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghikxbiuz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gonnwdwbp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gneerzpnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtliwgskb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdgxhrxvf.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gdvhlubfv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnzcjedyi.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/geefssfkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/ghslyelha.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gldapecui.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gadzgidxt.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gddnmpmcd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gtsrasbog.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gtogfkyfy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gicrltbyf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gkrsmodjw.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/grdajlwow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/glbyjsznk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gdnqoyvsa.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gibcefqaz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gbnfqzqty.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gywwflftt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gbbnczgtl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gbmjftnqv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gcalciufi.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gmlvfuoqn.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gabrrxzgl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gunfthzqm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gikosleko.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkahvwuxo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsbqnydrb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gsqgbdpfy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/grdgcizso.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ggxgprrkq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/glyvkmetf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/godndedmy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/geuclskgr.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ggpswkiay.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/ghwvvtumu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gpmlozvpi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gsvzsoyyp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gseinmnqe.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gokoejjga.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gznfqzqio.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gkxybjspw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gnnennncs.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gmdevnqbf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gmxeimltx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gqscsjrhn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gxlapppbr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gzscyokce.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gxpenvaxc.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gqtdilbqi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gtrevznxh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gwmthovod.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/ggtfsfxxf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gfpyvfucn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gztdczvgj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gvptoatsy.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gysltjoxe.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gupdlvvbz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzwtoltoj.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gkopbqkea.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpahjjgpq.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/ggpobrvtc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ghuhdhvvu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/ggnmhltkm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gtbcnoiux.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/glxmamuoh.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gkaffbnnm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gaycdytnx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gbwzuvyzx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvktearxo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gluaftxva.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gxaadkrrg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gdjtwbiwj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/ghifdycri.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gmlgspdwn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwznztffi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gjdxcrzjb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/grbwohzis.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gwxvkqrmu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsbmdbkjd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gnziirtqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gfalejctu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gjogynoui.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gegppaflh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/ggxkihmpz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gojvcoihk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gdqvjixji.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/geetajskz.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gxmacotsk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/guwhowmlp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvkzlqmjh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gqgxrnlje.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gukknhpxy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwnhybrvz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gvavssusy.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gbdgapmat.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/ghvvfwdoh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gxohnhmqe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gwumssrvw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gzzjpcfiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gwilcclqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gaxbydtlr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gcgmcafdt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gbklwdmme.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gzhfzqnss.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/ggkqmoiwr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gizsebdsh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gkewuegen.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gviyprofe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gqzclcvff.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/glbahaoyp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gqlmynizp.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gzexcvwmh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gvlwmiwli.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gkihipked.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/grrcgxxcg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gbidpogpt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gzpaxemrm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjsjxuyct.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gltqgoqfu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gelbzitos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gufmxoqdx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gprgqmwkd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gnewaaanj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/goncaikxj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gimtgafgq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqpbfwmiv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gdoyuvyzx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gjmlaoedt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gzdekcxjm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gmfgoggor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gtgaslprw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gyvpzhwzd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggeohmzch.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gkafdkxnc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxgimoyuw.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/grchbjzck.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gslakibha.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gidfhzzxa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gjcdqonvi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gtaqkuatc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gayomswmt.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gcvjrnlri.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/ghgxqgefn.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gbikdgrwg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gcejgwhvv.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gymrlkqjt.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/guulxoyjx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmzyeyqhp.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdlhhhqnj.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gxyyooudr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gasfownle.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gzxetxtkv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/glozonurp.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/glhqzeijf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdoptkdm.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gixqfhvpi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gihxluagw.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gxbuczfmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gzpwwmzis.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gmeceoqop.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gaunshwcf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gxsyqqxzb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gxtbeomfj.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gpdrlxvvf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gzkckxvvm.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gxdrurqnd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gtknfllxm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gcinayeen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gzuezrgxx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gwxvglumm.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gglinzoux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gipsizhyx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gnhcorhlj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gvvuszrto.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gcpcltpgj.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gnyjjnefv.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpicwrmwo.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gechngjow.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gqrgaevie.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gpqpmhzkj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/ghutuvjuu.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gczddtxqn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gpecocjtb.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gqxyckbjy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/geyoezmcv.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gbpvcibbp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gmfhlggjx.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/ghlvoalny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gufdwujwi.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gixlwrzrq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/glueqzcjg.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gaiewptbs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gaeacddiz.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gszodjfab.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjdjrnmok.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/ggdhpazqy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gryqucbfg.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gywoiteyk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghacskoay.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/ggvremews.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghrtrhyfw.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gbzwqfisc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjedjabnl.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/galafhmut.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbfdwizkd.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/glltmooaw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gdlcbjvqb.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/ghxpxnbia.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gpjxsikpv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gsubtxlaf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gosqcalot.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gapaingxz.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gyjaafemm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gltpimgia.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gnkdavnmc.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/guzeqsfvg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gcxlywujx.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gegukwvyo.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gxrpmmeqb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gozrqpejw.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gkhxutuen.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gunfabqcl.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gnpjrgdkj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ghtyyrlww.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/ghiaoiqoo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmszuhodw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gnsrnszqx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gzdpikaqw.sHtML


<!-- 参考信息 -->