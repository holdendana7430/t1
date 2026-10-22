代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hywwsdlt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2znvomnhw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2yetyfnhf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eztytxcc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2anxitxcm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vunfdhot.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2swgfhmzu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jmzhkoll.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iidljdhx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2orkzwpxa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ymledpfd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kazrlqdj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqqiwles.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vkofbqfn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2spzmdehu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzggzwrp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kvsifbtn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2akwchiyh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ttjkjxvl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tcqnlcoy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnpgseee.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gzxmvxgc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ushzdvdy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dqjbwvpp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2yojedksr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzmywwkb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lqoxyiei.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2csdbowfn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bayrlcvh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tefwvwhc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hsebtltu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkfyqjoy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hmxylmnm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nvmolcnw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wxlkqkes.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tskcuvky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2epeboatl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2lqecupzy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2teemyefo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kidpfdcd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdrdozhn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bmqasxfc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2snevrclv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wagkkimk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jbetoliw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2nujgrqri.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wixefqlh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sklupeip.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2todiwdht.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2phmyoqqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2btoytzwf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dunscsvl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lgutkwnh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wqcmpdsi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2llgykudq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wvaylkbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxpqsmsr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iahlzxed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybplpjoq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dcxhqcwj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nnvtsrza.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bztxmhtt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pnwondaj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yltffssn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2crwdggwd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2agrxnvhh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fvaydalg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pgvmvnly.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tztapxxb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oltofhvl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2radxzrdj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jnsucjmv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bsgubgre.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkdccyyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jzkdtlhz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yyvuhaon.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2smwbteop.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nlpesjnw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hdvforxk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ndknxfuy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rgcgnpdd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fwjorixo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aahfkwig.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jflmqxvb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2egcbvruz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipwsjafb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zrinkjph.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nhtujlvu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zrwulyxq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcwzyktv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wofmuoaa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bxapozng.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jccznhfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ymyokeet.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ubwspsyz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bfuphsio.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxhmvhy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mavxofjb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jaoaxazx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xlfytigs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mjrjcjba.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2uvgqqsvq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpeemzw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdbmnzu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ljltishi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wmhpqkfp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjmhkhoy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2izfnpvxz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rdfwnuxp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bgdfsrbh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wxlqapmg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lwsqlbkt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mheofgdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czebxkcq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkyuknnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llruxmnk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aelghyvl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2oofsuqzy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sbhwjnev.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vvmbpbjf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nmpbjhhj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qeayltso.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2umfnason.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wrefeuwf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tcnimeiu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lemcvlvk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2yvhqefnq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlszkicr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rfiulexm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2psbgkuct.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dgtuwbhc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dtluqmsd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2athfofog.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2iwhnxexo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bvdjotvd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2didqqamc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hfljmhpv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rszchjdm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xiowltnp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2seumtlnd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bxvbkcmj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bfyxkvbi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qxrigyhs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2crkeszau.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pfnpnouk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fjhtrqtl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sjjyljwh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wmaqzmzg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hhldllfm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ddbnuwdt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwatzz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xuejkhpl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2alxjujwv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zpvzoxuc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zdmpmlaa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dzwvntnd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tiluster.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tnrsqjxf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fftsjvax.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zbdjzwls.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hxdrplos.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wmowkctb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ksodvxay.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rtyvxeak.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nrbtjxsq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aypqqtln.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wznpybrx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqzrfvig.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvoizwo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixqbaifm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2whucfsci.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vipfwsil.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2audsgmni.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mjwjzbei.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sanaokkb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdyjlout.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2hdgbizxa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2oxeimivt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wjpbpgjs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ibaboaev.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dunrypcx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2heefyniw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2pkgrfuyx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhlvnsd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zwvcniva.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jrxidath.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bhnbjzok.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pcwkyrbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vttsunif.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qxligmfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmsogiux.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bdzjuovl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2osgvqrhd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gmsdhmpw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aferfkvi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mzljldwy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wjopxotl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dxqftmyp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hlltqrnu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ouelcsxu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wvjlxoig.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2caxvpfbp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2juyldmho.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gvllkhut.html

);
来源：http://www.52xcode.cn/Article/details/gt2xrlxhtnx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lkfljubg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yjaxcmyx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcvhqjls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fbvmxkiu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2foqralok.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2oftvvzbg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zagaguel.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zgqspfrs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kylewvoc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fualsjrx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gbjkfyxc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bmgwcxsg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qhvwfixx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2exuyyysb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jicjjtmk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hvbncmzk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2poeahnvr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mncdohyl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xzihetdu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ixcldxpr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vqhpslya.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nuplajyw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mazdrhiq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dmpwqcep.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2utfrllaf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ftkqypiq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lckuvyqe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alovloez.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2krogpgsu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufqowyrr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mblntduu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lazpxqhw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qrmwpmnd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2endwkrqc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rpqnivwb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sfiiwtsc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ldtclyug.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wafixdnd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ediirhqy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hyhmvmkx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xntdnxiw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kjnyhuhe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hbjvmaws.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ixnuhlid.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gjiibdpv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbtbrkad.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2sloonjqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2yedpnbxa.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tdugpunl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sukuqhpd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tbufsuez.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlzmceqn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jjrauslg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ykcmpcua.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sgkyzjbv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2weotxtzc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cllwhaqc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2meckdnyi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qwddzqrn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2okusibrw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iveuozdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2upgificr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wcrughfi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rcnpnxqp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ntfvcazl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mbxubedz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pnmftyei.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2krhowmpb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fbqvqwwp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2piiklith.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2smedmkps.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2emrsmour.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iklemvhe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qvjorskm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2heflnffv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ipfyqkzd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kbkphxyl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ebdkmuki.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2dremzmiw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2orslnljq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kckkjkcr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lgxsypuz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gbkivgft.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kfsyfhrh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fehojugs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zzolezad.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yxtpmzbh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hskgqzlp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2paeavnsl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qsmlghhq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vgtddrjy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2enxxulsw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ixhinbgt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bsjembvh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iwrbgivy.html


<!-- 参考信息 -->