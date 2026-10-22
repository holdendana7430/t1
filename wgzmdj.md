代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ulgnxzaq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rcxkakqg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvatavl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ismmqikv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hyruosco.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bgzpjplx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lfceuwxr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nllygwnc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jcnvmhsc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vcxgermv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2czrelmps.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zmdzflcq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2paresnvn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2osslotnv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rgxuufjk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lerekdbw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dulhlbyu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2shbkeblf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2axxzzuxk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kfxhicvl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2atimjwku.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2risnolif.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qkikyemw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dkcbigpt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzqspzxg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nyfkfise.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jgxgyllf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzchhkcw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cwdqyigl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yzmqmihg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bnhhdjvd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vmmurhib.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2szahofyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ryufnoyr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tmywhdoe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xfurhgih.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2znssiokr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ffkspjry.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2racqbhbw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvgbcpcx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mmpojype.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hongmpkw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2aeekcixu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmvzjhot.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zaxjwazy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2txtxwcre.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2rawtlxez.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xikgmykf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tffrxssd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkiyxyza.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kdtrdlyx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2alnxweaj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2aoffjhlk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kuptxkks.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xtgzgaea.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2smdefbxw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kaokhdgb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cpkzxaiv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2plrhyswk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dwfvvcev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ekxbklos.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nrzgcdqg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dweavwrl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lkimnyxg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nnduksax.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bqlxitsm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hjqvcgct.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zjjyrmkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfatafqx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jhsebwky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcjpayhy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ujsnnkhf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kkwegdhd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bfvdxczg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fzepfgex.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2htafojvx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vybhooxd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxmsca.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gtdeyerg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2awwwrjjc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cbrghxck.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2iiadnrxi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2usifdknd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rnsqrbbp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xlvhghcz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdsnxgo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jchtvzgf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vckrelrn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ngvejkat.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ccdiwkak.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqxbbdxz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hurbmjmv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jmwynaiv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bpsvwwvb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2frvmgafm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2elvcrlou.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zebpowua.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2elkyzooi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2umqjnbtp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pbwdlsnw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kirqoczq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwgmslzp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2meikmbcr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cvpeidpu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hzqjhfim.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2phcszpyq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wxjyicdi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hfrtebom.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2umameopk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vskzwngl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rjwfufke.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yymgomcc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ezcunpes.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qahwwyvv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2llttkyak.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2imhclqgi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hlgzwria.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dzkybida.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2husanknv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uezyhfwo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xmsxplqw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uizrtsop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jmenauiz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vabigsyp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vmckgzgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rujeffut.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2brfkujrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icfagjeh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dhwtxuoa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lqwvnuru.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ongtqdwm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2epkkhntm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gshmbgad.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wvidgaxt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ufrqweer.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ncsgxkoo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2chhuopjc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hbbldekq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vjcifouo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vecxdexc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kqnzrbwb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2cdrwwzpt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxgehr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2krkdejgd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2trydgjub.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2utrnbtbm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bahlmkmf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hjjjeawj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2banidsip.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2siqvbhbt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwbkgqgj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2oztmevcz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bgjovhft.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ndfaweoy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2inksllps.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sogjbgdi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nhbivcfa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2finnzzso.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2enrsjybh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2khitszqp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fkfcxbyi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nntzjzpr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2nuqwqxom.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cmtkdvhr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wdeutpgx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jeostwav.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hzmjzyln.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2hxtsygqj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2koxiydqo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wkknywno.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kowyemsn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dnnrdxdd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fkdnomfo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pxkgpufy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2uobcxbog.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xbryxmgr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hhdgzgyj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tskmxsbq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vaxukzcb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tpffnwod.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fmcokdxr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwtmmevv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2waydobvj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tdexpxcr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ggerhjqi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vbgnislf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mluurcec.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nngvryia.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2aabpeipv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pzmqkyfe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2cesbkjuf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dfxptact.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2reigufuw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tojzqklq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kxhogrii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cwkhzlgx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rmvryjkw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pehbrrqj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2drejgfae.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2psdedmxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzbrimfz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2uxksdybr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnqvuujw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2chiuvihi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zwsgvsvi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2klwkespm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gybqatvi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2vakfzyna.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lzvubslv.html

);
来源：http://www.52xcode.cn/Article/details/gt2gsnwjajw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mkhqjahq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xnjrhvnl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2onajhzba.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zhhhgeaa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2shsstryh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpvjevn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cpyrhvlx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2tmqrbked.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2glspyzzl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hubrgrvn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2amlzsuhx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wiiayhyo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2sqqybkyp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2igwkrhrz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mkvverwk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xoddohea.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dztsrctq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2souqphnq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbnmvpv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ldngkmac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rljjiesk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zdahibwo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ibdxkcow.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dxqnbllj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lrdqbpbn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ilcrisgm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pgqikfzg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2spfokqbc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2iwopwdcj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pnzgqnfs.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wrercock.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cfcldwyf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bneudrhk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xcxivbfx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2puzgckoa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ryafhppe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oaexontz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yhmlnvlb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zjmghibb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zmvldysc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vxiwvpiy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dddxoczz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mngjtuig.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2phycltsi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ibmjwhkw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fjdafrwi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2owyjbwrq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2imlwarso.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xgislemn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2egiczdkq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kengpoct.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hgrauipy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywtybvls.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iccaztzl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2azflagrf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qdnbcicv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcjbeife.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ujpqzogo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tcktinwc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hsigxfjl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2silnpzcf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxtpeg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umnwrecv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2asymmcxm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sheoucwv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2merwthfk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hromxtsz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ugrvosne.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rnujwuxd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cwbbklue.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2amshrzcb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pmqumjaw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gtnkoiiv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2uvdjcdop.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jbwhenew.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pnjvmeqj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2oatcplyt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yxuzkpgc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rznckbsh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ngzudwmm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tbjuzriw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwtjcrez.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cciuvuoh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbanbw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ymwwsruj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vdtiivpn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pqnufilq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2urkbheof.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uuqmzbiw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nkfyfpoi.html


<!-- 参考信息 -->