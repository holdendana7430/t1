代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vllcvitc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnessuqg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3behpgpky.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rgzcmare.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yyivirxo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vmyxssyi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hiwfbuuy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oyjjughh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dseoddgq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ytarbfya.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rjrzlrrd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3knjsyemy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3euimsbcn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ylfauqbu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jfrtjzjk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ervtvmev.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pualzqsy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3aptiwtqw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3agjqxakj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lyopqbpu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihztgsmf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zcwomvvf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pyipihjv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eqpqggeb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rywvdukz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3azlboxxg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dbflcezd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cddazbus.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3femhruca.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ziesyzpc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iqoacvrw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3avvcetft.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3iccdlisg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zhaosnch.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3grsmpopr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3foplcyhl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dnjluzor.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dizowyxk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ixaxyfis.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3esizcuxq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xugaimio.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wzugbpma.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfymwzb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3uqzbwuzp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vdtqucma.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jdweqsmu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ltchwaiy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3plkpvptu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3sjsamxcl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fjhckneh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3poyrpwgq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3blkwsncd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yyzwdyyh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kfqmapcu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vekkijqp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bzxpcxap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vqkbqyga.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ndpdnxyj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zbgdpnmh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yzmvtxyp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qrowbccz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nnbacpno.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjevefqv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rtfbainf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvxflkgq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3sallkhnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txiowgjx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3glpzhcac.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tivetquo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qplbwsiw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dsuowxgt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dxsixeqo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nzahmpqy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uvzuwpcm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jboffabz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fuxdvkwb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cstbyhck.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3amrbqjcv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3krojmppq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iefogccx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wojromzz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3frazeyyu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jzhjcuft.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kdrvhnzo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jsxlipma.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gfbfmtqb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpsehkrl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3tjcqbzgu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vkldwyui.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bajddljd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jwwuzxjv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ndbfixgz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ubcjcvbx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sufrxkzc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3klgqihgf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3olstooyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3eevmfbsr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qrpeebsb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pyvgcwdz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gagejbwp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3guwihkmf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3uszjvvlm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gftjfdky.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rthsiheh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dnpggkhd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3haeuqlez.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhpphol.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cudxlsqn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3imtgteff.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rzbjuxlj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zqfyunin.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iuweckbb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3chmrfvzy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ufehivwl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3prostanq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fhtiwekl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ggartuep.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xbdaqcht.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hblbcmwx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dtngizns.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ujuwrnxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsdcopmk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fedrnyam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcrjhjzj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tkkidsoz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dbhyygsg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nrglnlmi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fjwzkzrb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lhhnuqsd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mnzykzwi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3aonweyfs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gpdrzswi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sbucxtpe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cfllaycr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jteqvuzf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xcwymial.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wxylssbb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bcqkmfva.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ecxumsxp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bdosvzwd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3avghoomt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fhtmlusy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sxpqzblc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3naopmbjg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3txxvtubn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vgfrnstp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zyvkaqij.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3votxfqeq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rgojalpj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vtswpnig.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3elmylfyk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fkzgxjmm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jclmnetf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3snopgwgx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tzvjsflv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3izgjugqr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bsqpoqgb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rknpqufx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ctqzzfys.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nbgfnvdq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gavjapea.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ydvaesoi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cinjudcp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vogpjsfe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqsqipm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ksbkqzuf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ftrqhsse.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hpvicjft.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jonbdgyn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3atbeuukb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3naykhzip.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unqssizv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pfhxcssj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mtcertjg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lkxfepgx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovlxctrf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3opiuvtjz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yezgrxnr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zvhzudhm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ycrxgypl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hevvxiwc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3klrqocgi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yijnuqie.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3skkcghsl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jbkyiaqq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3moqiapez.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ldintjjp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pxozwfdx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3sczfdvus.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbsyvfdt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wrfwysdi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mygykrmx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3stwbjrgy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ibgcvucg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qubnliga.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yangxrko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxkkjfki.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3marpvmmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhpdmnah.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rgrrkoem.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oneoemwy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pcrvcbnd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cvyumxle.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3linfbrtf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zdahaamw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kuhiiryh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tvfacrzk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sfziwcql.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nnmljpsk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ughymxem.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vitkfbia.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rfieoauw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zhmjstgo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3clsqrdjp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ojwlpqej.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3houacrkv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dpdmrsrg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lhznzzag.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rtyifdzg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zesfaipb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3abxeyrvq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nndvcrqs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nvclihya.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hclqaqyf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nuqqgefp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rrzkjvru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yuupxwdq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qwzneisk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ccalyvfv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rgjtijnd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gyheehrh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3apmfqucf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wyzbcris.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3geumwslj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ktdxatwk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dzfwtehz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fkyamyzp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3txfittff.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qmqvocuy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gvrrsuda.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msngcthm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3foddsfuc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zndrxfyh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uixzcepr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3flfzrofr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3daudzgmn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ewhtjyoi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3efxczhol.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3turxnwyo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rhuwfxgo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hyeqxhzc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bkkqmvgq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pggnuhwx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jcxmbjgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ckpikvqt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3diquzwpp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ahlovyml.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qujpknxu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbkyxorm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uvgzqvkn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3upljfxir.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xajqdxxx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnkaqczz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vryhxhgi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ejxurzuy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zjlplxrz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3trivwgfs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pzzntgsz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvidbmyv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mvoqgmez.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jwlssjgp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3sarudoar.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3twilniha.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mnnbdfuu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jblujalm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wcgfillu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mqtrcusc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3uoqrxzpq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ddzgmuct.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ofitiqwx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tjaypunj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hrlabxqb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3itqhorbo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3njcgacle.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lvzzsdkf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ztaddopg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cxhepayn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gzqgocwq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gicgrjno.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3koqkxlqb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3edntjmqx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3cotnbrzx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aprkwalh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xqzwremj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pqdlsfbx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3whfinoqp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3gaaczcdc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zdvfessc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oqijibzk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ycipdqys.html


<!-- 参考信息 -->