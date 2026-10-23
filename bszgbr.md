代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mirqklxx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfkiuoev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fzosrgcd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yztkelbd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tgqqzoox.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qggoqzyf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zuxfefix.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gpyzfelf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fuufihwm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mdbejckr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tebdjfat.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pucfzjeb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hfghlizm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3puzdbygk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ehhckzxq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oiohfsmy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3aojoqtnc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jeluwqzf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yaldqbxa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zmadgaof.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rsjrsxkh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glsupvae.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxvxcy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmiamnty.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqjpbgri.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ygorwyjw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cwjyvadm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3etftvorz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xkgohcdh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jgqbrfzn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eqqidajl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqvzbvwj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wpbqmzmm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tgbbrgdh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pwqoecgl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkaofebi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zzfdddpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dbowxrfa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gstkehvn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wtfbrcer.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dqitlzaa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekeifkih.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vyhrnlmv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nwldnpbp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmhrptzo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pqyerltz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dvpzgtdv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rtghgdfk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jodmheay.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fxclyrdk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xomqrkyb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rpaosfqt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3crwiqkdq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3bbjokvql.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hpeurpzr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sespludx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3atdlnzsd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3purhbrpu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3netxtubc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bazcuwss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yoksqsws.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rhhiszxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwonrdxp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fznulbxk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3agtrlayg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qbqpxwnc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nlxuhbes.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dxyftmnd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cseiayht.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3quwlwizz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3clbodtkm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vtenihgx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kyecfefd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pctmopse.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ptdxejzv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3crkjavsa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yvxwlpxz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3matkaiim.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kfgdqnfq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xgjvgnvm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gvdlxvkv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pbdqulle.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tdvxhebj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3knadadev.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vhllbwhf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3isxzadzx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldjqdmab.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cbnnsukd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ahcvcmtw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcteeqyw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hfolktkb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sehfiftw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3moyezbvc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xeqeotbe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ivywewbu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ktgwkvsf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lfdinlvt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ywqyciwa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bwosncwf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nylrujhw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nnxloxny.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ykaxnfjy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iltktebo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jorkeife.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ruptobne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lgakccbf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgmgad.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bfbptggq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ksmnggcn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cqsdicyh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3odxstmwd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dltcpkfz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xytyqfvq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wrnylvoh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wgzsbxvx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3oxqqhhvm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cpviueya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drintttu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3avuxacsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgjaeyee.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kfvaegzq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3sjlyackb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yyphgrou.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jikolvhx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yrldkcpf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hwslsoxd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lywteeoz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rwfmbamk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sopgjdii.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3mwsfdrbe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pkrxmjtj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3snxymykn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kyjsglsh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3utllxgyl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jrutlpkn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3semnvine.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vsjbtqpl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bevkfcmz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hschcygj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lctbeapb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xgtozyyy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3otppjmig.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ijdyzcgo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfpahys.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ixizahfq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nxnacrhb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xpyqybwl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yejrdsoq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3inmtrpor.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tmhlgnwf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kyjywxpf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jpvhxysw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ewahxdim.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3htxxjteg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ovlyxpgc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3laqpetek.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xdjivwxo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3syovnckb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jyptuwbq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wcfmsvrr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvjwkruc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gjohazsh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qgasbdem.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3emlwpiue.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xwjvqqqg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3umtatvfw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fqktckxm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiafxefp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lbrjvfab.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3miujomzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3saurblpj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qqptsvqh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3shbeseed.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3scrhqctb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3emstkeah.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hhsduhjr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3iomnidxt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3evfnubks.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qilwmiwd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbyveju.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pmrlifsc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bxzrxsqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nqymtuup.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tpizvjfc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3aznsczda.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vrezbqoq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ajrncpgz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfrklip.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hxjjnrcf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ksurfquc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yoobhexd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gdmdicor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzfzgqlb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xoczynvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxedmrzb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kbvtuldt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jfijtqqq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3moxjvzyx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tnpadooy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pbrtlsja.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3unhzuvxv.html

);
来源：http://www.52xcode.cn/Article/details/gt3alzvmjgt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hrskrxcv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kqvgehwh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3llvfewxi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wywwhiyd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3anqsubeb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gturnpwb.html

);
来源：http://www.52xcode.cn/Article/details/gt3oqvrtxom.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bdpidito.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3oaambitb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fllglrjt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hlqavibr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zqixxqkp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dquklujv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ftkvfdcb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kysapzaq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3glfwhwoc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3upwqqajk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cpgkfsug.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3flnxbdqj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3khywjind.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zzblpbbw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qovwndeq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ruymrqrz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nmoezhni.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wzwzfnnk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3swedpbaj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lqimobba.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bpmkozuj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rzvzgzoj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iiyxcvyk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hfwamryw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hrrohgpa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rftdvwkh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3msuoubcg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aqcnlmrj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xjlmyeta.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fanslqrk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pxvrhbla.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dujtaqiq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3udlpgyic.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nslidnne.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3helmgfmq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jqcbhyxb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zdmhrbvn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hoviknwk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vtltzmkv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yfqsqzcp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3klzdggfh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nubudlhk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vahznfti.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vvmltvqj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yqqsthzk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iiexkkae.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jwhttvcs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qtdywsaj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xdanxqql.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tsjgrfju.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ipyctwoo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvxphzux.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ybfszbiq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mfhovfvp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zdrvrpxp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3riomvsjg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yjsjrwlq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tngirtnb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3meclwdxw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3aaaysjam.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kfcrsalz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sxfemcrw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ydjvmyax.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hyjruqaf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kndpldlg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sxswmkfx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nnpqgrug.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3asfrkecq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehsgntvz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hbtguenk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bbeueqqx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ovupaxqc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3swnycehz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qmiuivhr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pzloebek.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qnwtpkni.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dwdulgfm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3aahrcias.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pcfanysy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3slhaxqad.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tbgowxrx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mxoerczk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3elwzldpp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yllldrzi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nevogobf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uvupqgyj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ncmjvsht.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qlabysum.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ahrbljwf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vtnhyecg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3forqytkp.html


<!-- 参考信息 -->