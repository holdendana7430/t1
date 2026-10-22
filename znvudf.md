代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jarysdgk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ajyphhpk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwwnhl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vositbjm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iukmexdz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xbdfgbsy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mpzshtxg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gthvqlwn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enozkirt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qsvoomuq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bzdkyzkj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kxvorsvx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eowsqfzu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ybkmibzh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sibivpwv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oyffeekk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2puyjrokb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2axftkyom.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wgoklrny.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ngmagntx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vmswvbnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbzbqqzj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pubjhanx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmmyzahm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2buzswztb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2oyfhgknr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qtnsfwhr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wtybexjk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lsuropyk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hnsvmfnb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijgzmueq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rbidlbka.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gkfaybjw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yypznzaq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hxpnfisr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wvzjomej.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2fgvilxwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kgmzjute.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nlqnetwk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uccypxrz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rbvrvqhf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2unlmrwlt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2drgcvqpz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ksddyspa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2felkcyva.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2icpdthop.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aiiheatf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kyghkhuw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qrfmztyd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xogufifc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lxhpnlyk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ntcnuqdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpjofkal.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nxgwzqcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvxcuqos.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ggunepwg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wjggjwdk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tbkodqhq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2neiikqda.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mluxulfl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ojqtplsi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ahoromrg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2komhizvc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jmnmwegc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2orsurupg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ptuerlcq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hsrryani.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2weutynxt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2javbegfi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qgjqymso.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bhiprzbg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wwrovtux.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hyvfbtqc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fdhcajcv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eyncdzzv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2alxvtyhw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fofmzftx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mmliknxa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mndiscqi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2chulvirz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dcqgcktz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrryqan.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dpxvotlp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2oyddjurb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gnmcseng.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hpeauhkf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gkenvsrt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kshmvlpd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wblapcui.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qgvligsb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2uajicwys.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ptrdnkdw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wkabkbnl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ghshkntj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ftepirxm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ultuurkg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rwddubbh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wycvaxnw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gelqejge.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bdiplqzb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fmaxczal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hhhlteer.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2elsdrkdz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2praphspo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2orjahgyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zrloetjy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tujjpedt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xegczxak.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nfsgqwbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwrpoibz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tqchdtaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crayknlb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ptyehxwk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wzkldnyh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qtmkpbcf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bxvrlbph.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uhndbzsx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tjnqoruu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zwanlnrw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2refxwmxw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kghfnntm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wszrvype.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rhibfakm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hvpqgvez.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ewkjagoo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wcdfuauv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ctnbrfbr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zfycdeml.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rhcezkyy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bszlexoy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xqagzwzv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2iipxdvfc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hrgawdew.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vghhxvep.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ufdwrffu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2txmnmlmf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wglgqkhl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ljmfwemh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2basswerm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vrjazgpl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wywpksen.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ndkjevsa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uypvxxbm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jerangkl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eyfnbtam.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ismnvynf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ehwmyyun.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xxnoszxn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cgeqhoax.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dalnhibm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bkxggkuw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pjbyfgre.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gfkmvpek.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2iuecwfln.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mneraefe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zxxiooex.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2eokrhnwe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2oodtfxyc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cszbgruo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kefiqsuo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lldcdxji.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxdocnhg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpqfgimp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gucrotrq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2poradeki.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lstbivts.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pibxrjom.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xiaqomrs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2sdhqexrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uaeufbka.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bgrktmev.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2lpenvvsw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lgjxudwd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2geifejxl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2laoogcon.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bzwotbaj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2acgxnqpu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldngyncz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2djdezrpz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kerorlxb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2onkpqgeq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vtoephdd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ifuinppw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xxdiyoog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoxtxqhj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ohjyttqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuufumyo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uekaryce.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2uppusyir.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ztluympe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ipnkypgz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ocefrptr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yrqfzieq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xaoztaek.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ccqblvfr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vkjzkqwk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ptjmxlfi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yslwcvqj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vlwwtdgy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2eqadsliw.html

);
来源：http://www.52xcode.cn/Article/details/gt2lrkioluq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zbslzvqk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xqinrgtn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2crfnyijp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bbnfvocz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2irwhrddg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ttbimcaq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fmeipezz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nqzdthhv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mbxrbtpg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2blbnfngd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kixluebg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2buavpxxr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zmzlofzy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pgxjowfw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qjzmpkqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bqzoasew.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dhlunwoe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tnudfkaz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kqrolglg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dswqknzy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2shemvdsw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2sajcpncy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2efqfjgmb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qhwcvunj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qsrkpktt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tlakeohz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2okwsgojx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gyqqmgws.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hljvfhnl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fqvtgmdu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vangsnbs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srjsrttf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xxhqzvdl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hxkgnviw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2modtgrek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2apqpblfd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cmcvbnkm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mzeoxahp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sueppnlm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ddfhxkyq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2aycuwrid.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ekujpwey.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hdcuoenn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bugdihre.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fhoriyph.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2girgznuu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qpwmfsqr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pbhdmkzp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2exvsxpge.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oqzhrzss.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fjfsddtn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zdluardo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rjjnflrx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tvmxsntg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pfdivnas.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hdlcbcpw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qpkyqiwx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jdgygzls.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fvhrkoqc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ngatyedp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2towopjxa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tavvkuxw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uznqtale.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rpxlmsig.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2afvsckkh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qfqtjhjc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bnvyfjtx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vgukcfgs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qbizemys.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ekwqwgjo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2otgcvzpe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jukutvxx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hgiikrdj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2theyadof.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2baqveslh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vxowccyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ctciqqpu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xksmmrsm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ffkaukvr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iwmkyosx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2axgqjjdj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2sbudujrb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jepfcavp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ocafrjiy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pkzyormu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dsytnboz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rutmzweb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zellvkvp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qgjuduei.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2smltaebi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bactxfkt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pqwqznmr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ktpkpjxy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rbfeljhd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pyzuvyed.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mzubbkid.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kkbucaws.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ojigyart.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bpeekzig.html


<!-- 参考信息 -->