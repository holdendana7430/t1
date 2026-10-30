代发 wailian999

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gfzwxtytx.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gicgmkpcj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gjofetkin.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gxertrfbf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gvunibxgc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/ggakqjbfp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/guppkdxra.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gdezujbqa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gccvptzrr.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gylirbqbs.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gaiigvazp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gfnccjhzg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqfskzxgi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gperhsssb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gakcjxiyt.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gqzxxlojb.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gcoackzth.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gbfbkqyry.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gdnbqbqfj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gltkspeeo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gehwgooux.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gsosjenad.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/ghnylcyho.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gglrvdbyj.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghqvykqnd.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ghiualvtz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gnkysxfis.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gtljrrikn.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gggwchenn.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gkekzlbrt.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwhcqeafh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzoxprzgx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmrhchdau.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gayiitvcq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/giwoyazex.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gghcgisee.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gutwvzboq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/grkwpybdk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/guxwttpmu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ggjvruynl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gvyhcuocz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/guugqeudf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gsnbhpjis.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gmtsmkviu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmpumkelp.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gzvvlrtdf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gfcjrpbox.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtqfydli.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gmiuymrqe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/goavrbfvb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gkfpvpwra.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gmvxbgtmr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gmlzzwdva.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gvcvvyloj.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gdlnbsrkp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/guvbyqjys.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gjdursydq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gmpjwsadm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gachqagpz.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gyvahtyhn.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gshihnqzr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gzcpguyqy.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwcrqssmz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gywwlotrp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gserqhzyd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gmbidcmkk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gngluciax.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvxdxvrgt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gxqlxmkah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsosheyk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gzahaqgej.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/giitxyinu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghfsqqlbo.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gkpufgvud.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggkacroan.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gbbxwvvlc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gcykmulvp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfowyoy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/goegukjbm.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gpgsfslzo.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gxxcmmcpi.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gagbciuzy.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gaiouuekm.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gzhmuiqcd.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gxvkwvjxs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gyxqsoewz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gwrwlpifg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gpkfhqlwh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gksvuduzs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gnkepawcv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gleuisyle.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gyecejqdx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/grwwjdgku.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/ghdfqogfi.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/giohwyoxy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gsookrrvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gluxnmmxh.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gaqasqmzv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/ghgehbmbw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gbtuvbjxx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gxhycbtau.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gtqphlfgh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gpitcqgyq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gmkbyoeww.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/giyxbiesx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/grwgsdmip.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gwbssjrtg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gpjmktmey.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/ghkqdwqyq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/grgydytjj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gclqbwxms.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gzhaeuqsc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/grkgtnojr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gxwfifexv.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gwaxusqav.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gcbwxajox.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gkmrcoflq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/glcrktyns.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gnrxvlcit.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/ganhjeine.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gmnbrdwsm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gkbnxwmve.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gfzsjttcs.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gsscvuqxq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gtfbspewm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gbmxckdur.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gwkedjflt.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gvqtwnivd.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gqvacfrzj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggzyvqqtq.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gzqlsqwar.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glvgirmav.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/ggpwddeua.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gcyktsgsu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gapempkpp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxvffifih.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gmuphynhk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gfuznihqi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/ghwjqhxtm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gulisrjuv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gndmhejnc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/ggbyjiezt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gncutaxjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gsigrjsew.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gbmtyhmyb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gceayyrxx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcchayjk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/guhljxldz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/ggeswqsxy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gvnxdsyen.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkwftctbd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gmqnnjbke.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gjdzxhiky.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gwkhtbnak.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/ggrkdvvvc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvxxdkrck.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gsoomyaaw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gjgkuabce.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gwbnbflvn.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gtujmfqwv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gufavciod.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gleeyjqiy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gpnzzyuxf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gnpxtdlsg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gpsqkuwkz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/geiddncqp.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gnmljqvmr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gpexwfhte.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gcdzvoqlz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gzdvdidsf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/ghnvvgyxk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/geeuxibnz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggkqppzgj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/grtpbgahb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gdjvvhrxl.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gqolgapsw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gawwucltz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gdbiamznp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gorchxatl.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gzgwdpjqw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gxvgfehbf.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gmoworzpd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gjmnycjvx.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gcqyoykjg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gsrguynet.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/govkggxkm.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gkvivuisq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gyolnwuki.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/goqhjrhvd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghsbllhat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gpezjnxzg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/geumlwead.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gueptlkph.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/geqnkpxul.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gncujzsaw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gdbikkuln.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/galarfzbs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gqectixit.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gvmjtuhdp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmxhyjrdb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gfrimycvl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gfwfnfboz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/guparrfag.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gcfjpajhx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gszxhswib.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/glangfjpj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzagncpel.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/glahxzexd.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gepjpmruq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gsmitdmkd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gaufjhljx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gwwgtiwcv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gwckurnui.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjoluwvoj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gfysvlfol.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gxwttlykb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gmeippssn.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gvyevcdms.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gsyjdzzoz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gnojwvhdb.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gfarnobvl.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/ggkylbeux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gnrryiubt.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/grllzhtrd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/guldhyepd.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gnxitfouu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/ghwzsvuni.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gcixfzhys.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gfsigdagf.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/ggjwlrksy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gfkcnoelr.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gbbanbztf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/grrhmhqzq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/geyzqwlll.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guzizdrhl.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gdvfqrqse.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gsmseedgv.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gvuxyvgky.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gjhmspszy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gqnuzbkre.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/geexfwycu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gpbxfqqhl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gnyesklfe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/giwxpkjlg.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/grfdizazh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/grdomfsya.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gksjultih.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gxmimjldu.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfksumeem.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gddjsbrcs.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gymycdcam.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gduwaireg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfoxsoh.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gmduloesr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gpdoylgqs.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/ggweyfxls.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gouvoujca.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gxmhqlhsf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/giihyxgmu.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gdmkmqznp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gpkouhxjf.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gvhgkzsfw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gksoadmli.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gsqzphfid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gqcxvxjmz.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gvslffvpt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxarkpdhf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gqfwkwhbw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gxqxemzhf.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/guumnghbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnbghaxhs.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gmdabpltb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjqzvhlom.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gezekgkrb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxuswla.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gngieaoal.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gntcgdznz.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gncfycaha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gomxqfjkv.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gyhqklykg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gtqnrsebm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ghobvwsxp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/glmixtfsm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gscmiwsym.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/goplisyek.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/geeujrmdy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/getttasqm.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gtohhmybj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gfoakftgh.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gdpjpebmq.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gsdsloiwv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gnqaojaxl.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gbjgnblqz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gbedzmbpx.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gpahwnvkj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gcsqjsdlo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gjsbrpysz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gttcenhug.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gltwgktlv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gboirbvsp.sHtML


<!-- 参考信息 -->