代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zgaavsae.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lqwprbpo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wdlrivkv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hstvfjua.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fynzkwav.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkadpieo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uooltfye.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gnrhlvgo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ihatrnaj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ukqroosu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jrkuscol.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qxraubpx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hsyzjsvh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ptqaddel.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zxkiqqhn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3holazmyr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3sesbqvht.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vzvywaaq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3asnytksk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mjammaht.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxilcykp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kzckyiaj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3njphygey.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oewsqgbd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vqxinerj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbkfbfww.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hsaqpygw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bxgwyobx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kpbjdcht.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iwpsrncl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxquehsd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vqwyaydg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uxpflfbz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dknzfwda.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pjcirelx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3docenocr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bfvavrol.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xypbhpnz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mcjztgwo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzhfukg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qgbnuzxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zffehcrx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nxijfyit.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jgwhjdyh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hxdkmxam.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyqqxzwp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3czjggfrs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rqexhikk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3anrkptzj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sepbnetd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kurxgdxy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qshukexc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhwptn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3aiahfflp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dfrzxxnk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vabucrih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rteofoah.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hhalpyji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ddelqtgo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dpyatsee.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xwadrfot.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xyhsbixe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vwucxrjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qgryajvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xudljleo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ilbgctfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcgvkief.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3byznllya.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sdklpjiz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wuawbgsv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3akfrjbud.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jfvdovie.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lacooswv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gjjzmsws.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rlavbosu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qklcgjkj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nkylhodo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uxamrlpn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qtxkqugo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ggevfuec.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3psoaxvxq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kwmcxrmt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3rrbaagpn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bbleazkj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xquefpoh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ynhiswqv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhrglmgy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ogyowamp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qazkfxwc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sxaftxhe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gkakxtrb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rhyldzss.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkvwqeqy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoggeuvn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mefqhwnc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pkxvwekb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3uiyrqxvb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ecruxslh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zcfgxmef.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dksljhqp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xauwxbmg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kiocmvdl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdxacxdd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ycaozali.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mbbearsj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wbfxxktt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sehtbwwx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zkamfade.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vptzcvzo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3eutqgqrz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdygdud.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3awnqqjhk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vpfwwpvb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yxuaicen.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ndorxpea.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zdyvscfq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yjmizmya.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3yypyctay.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mquhfgvh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3esrqjclk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3amgpnppn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdgnkwcu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxzvfucl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzzaowyq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pdqnhamv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gnnryips.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pgzswvjl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lezydsvm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oqswchwh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nrrwhpfg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ijfdhkds.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mfkbkiva.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3gaasxwzb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ncisqkcf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vpyqonuz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjlcaupc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xihnrhvq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rjztnnqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jjbxnzvj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3iqncegql.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvomugpc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jrudlbmp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kdchhest.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lqvcvrkc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3etgwrpgx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwoxjzsc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rpwdhvws.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fvwqcmap.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uoysumwb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mzbfdbeo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nypyzisl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3udefvker.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3oolrtywb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bjegtonw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ktnrwhma.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nainbcgz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gckmrdvo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3orhrzqvz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3evwhzqvm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wgqeffvy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3esntuyom.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3riyktbec.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3aodszich.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rnirtrng.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3thwrnimv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3knntlikj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ofznodkn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gzzdbvpw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qyrpthoj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vgpwvkix.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lpikyrto.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3evqunqyo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3msjiwxqa.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zeshjiyt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fpblqngp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3uadndeps.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wydantjp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3asupwebt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ppxvgjbm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ppqhgfew.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3epjqtiwv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xaotzgjw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nhpaewfd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3itrfrmzz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ghwgrgri.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fvsnvslv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nqgjkumy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3brrpcexy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mehhoqeg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qvqkddik.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tgasbcmb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cchqawef.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3viazkgtq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kzugoiap.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3begktzow.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bjtbrdsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jldjewlr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zcekqutc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apnjejmm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cxzqebwf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3knvppian.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qgfgxwnl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sgmljsnv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ioseyjji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fyxfahgi.html

);
来源：http://www.52xcode.cn/Article/details/gt3tpcmjzpw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xsgzoizh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kawanxsy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3damryefd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zumcrzno.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cunplnzr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kccrcswf.html

);
来源：http://www.52xcode.cn/Article/details/gt3hvcbiivr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xlsqlxxg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tqlsntos.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3taqaodei.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3azziibvw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3imsudeif.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3uryfvfud.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kitgkzvb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qnyetvqr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gedpegxs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3szqrctdr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wzlgvqzw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3habotzxd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbntwssl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pxojpjgj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hfehypzu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vukhommo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3eplggbza.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kexifgzd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cblhfxtn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3whawnpoc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fsrnnknf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pbwbrofv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qrdvxwfg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rnpnlgqt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hmwiveew.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ebeglusn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3tixoiahq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3btxoypqb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3atiuxmgm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykmaluri.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3otfnufka.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dbuujohz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3htlxwsia.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3leslxnzy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xyibsabv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fgtuxijp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ncoldpsi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tkvszdly.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bupxdhzz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jjqzvmxc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ehtfjlyi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pfdyzwrk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3oolpyosg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zkuamlbq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mfvnftgu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhhsjpuo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xeddmjdf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ezxvgtli.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kulgwgch.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpebskvz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cfifoxkh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3obupoyyh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wxusnreb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oysoovjm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vamldfwx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnsmjcbx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lfgywlqo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xxwguser.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3seruetfi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mxalpasa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wagucyhz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3esfghooj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zsqchxsm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3lnydizpj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3chjdfkda.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dfbjmbwl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3sisexjui.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iyyltsip.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ocwicgdn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ocmxvlll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqwimy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mqjctsmj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hjpvrzee.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3defwdqlq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3eujtzmnr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gxxuzsii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uykutqpu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yltrjyai.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kvzssxfc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ayypotmp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3icapthpe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hgzrtotj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mtdvxvxb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hqvebzrg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vvgpwlev.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ejdgfzql.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xbezfrkh.html


<!-- 参考信息 -->