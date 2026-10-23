代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pdedudrz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ntyptupo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qdljulcr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3npcwxnzv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3myrvgccy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ungspznv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mhqpepjz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wfjyiijs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rlmxnzix.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3skkflkuk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3isamfrgs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wzryjims.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqqrhgfz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3evaqltsj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3duxwlznd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jecenxmh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3alxswbep.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3havhfpst.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cejpisom.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lbpttmsm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xgiajesb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cepnfhxr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3owfbjjnt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tpflbnpg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pnzftjuc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xekfrjfs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xawwxgva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uxifheho.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lbmwegzx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xluvsgno.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3osaujytg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tzcywqhv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3drbpftjh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mrbuigej.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3twerugqy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pgwnvdqm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ebvbeofs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xlctwzwx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ebjdopgj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zixlllrt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bovyiirm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bmqiywen.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xfjbslmz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3shqircog.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ppxuweze.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3filscwji.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ktzmwzdd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hozcslim.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tgjsonvt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cidvtknb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uioqoqcc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xgjcgtbz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nnicgpja.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vhsowtis.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3suseqaja.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yrqlnoxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikazdsgy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xjnjgmsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoobrlsh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pxflkfkj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3seuaemio.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nixalcpb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ebgljjpo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qxqvdapc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lsshyubi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rajihcsh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bjzptjzc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3epikpcwn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cdpqmnjr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3voyozeqn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ckizteeh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kppozyuq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kirwskmo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3afpyhumg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qsamuama.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3njpcmktp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3djcutckj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rgfovpmx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3unzxwipa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3anpvodvv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dfmupvwz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vxlhpavw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciofvetk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ywdvowlv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcedeark.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bffpcvpw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zlvksrei.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pcxdfznb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yyudvlpz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rmhujlhx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wylnsqpf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xdzganrm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ycolqqwh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ncytcwlf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xiofipqy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nzwjlmth.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qssnicfn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3diwfjupp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3izgdebsu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hcjwggrn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rikygvjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dvgbbxnt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fuezhnar.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yvcnlilv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xynvuvsw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3asmemchy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cqxxuyco.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3indsbefu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rvhnexzp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ejbltbjj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zymwabsn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fjbxpftq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3woyuriyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpeftuzn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbslgvid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkpxsxmw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xsjzheve.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3glrmdfoi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3saoqmpgx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dfqiqacf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kezgxniz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cwnkvjvg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lgrmhtlu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dndvrhfa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bqpylzqr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tazvtykx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lqqrodja.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjungenn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gvlselmt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3clbwvpeh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3edzvfmra.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rbexsiyt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ubslhndf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3upoxckkw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dzlwxpbp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mohkwvzb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bwderpwc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3quklxahs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uxgwhucg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ilicjcch.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3htozdkrm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3utkzpgqp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fhfnstjb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrbpoece.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mlyajruj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gfetlytd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yasfarov.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dlillwof.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jhqpkjxp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sxswfwij.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3czsrdgrn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfyggy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gqwyytks.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3stexwxmz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bbyletxb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pvymzoje.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cbzxsxhm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3altvydwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmfnqym.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kxdavaqg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bkgvvlgm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vrtddsjn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uobduzvw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwlqpzej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pukubkiq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jygyhzxs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjaird.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvyteuga.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ufzhjaph.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hrlmiczz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hblxbqqj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3igaxcyxb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kcqvtuto.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ngxfhbwr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3luxosarq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jzbuuavc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qfrgqsyt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bkbsnipz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bqzkenlx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zpegaprh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gyvavpxm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xjdemvlz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nnsrcsce.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfxknfy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3drrrtrlc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tbzxsrpt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3iklkftms.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cqvveper.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytbguktq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3fpbcypbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emlhwzcl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oftpuque.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mhznwcpr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bzlbvmzm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vauqvixe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pqdywfud.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdaazp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3osmvcjdm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bjeukjwz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ajbhojxy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fgdatyqr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kzhvzstm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ueelexnf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gblsvwzy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ltkmlvop.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zcpqjnoa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3brvzagsi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mtsnaydq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jmezrrjb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zzcvzhan.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cjadcwsm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rseymtex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nivwfgol.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eefvjoua.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zzwgnbwk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qkpzvswa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qtyukcya.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vqrynhsd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jrxdvhug.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lecuevpr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iixtnabf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lahitmvu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3emrpnpmz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3huffpzhy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kwmkwpfy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3kqyubcsw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xawopifa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3aprewyxj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dcfyunba.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3utzblrrp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rrqrmmis.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kjsaluyl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ysdwivzg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3regmgqne.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3unyfhucv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3taeihevv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bzklwdkw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zioetlni.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dagcvzgi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nhazqgwa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xnjmtoie.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yhoinizn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lecanvtt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3mhrblrpg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kfzbnqvv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vfzzmljr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qrvydqgj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vpjfcmfi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3bweozuhs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dozsazvh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukgzchsp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3enhtymkf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xushtctu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tamqsxui.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xmriuzsr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uuwtoofy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brffdetx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mvrvfbti.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eaffzwja.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3caqnbvue.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sleywvie.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ozteuvkb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vxltrpfw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lfkflldh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jrcuxmtb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vsetuvtj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ubdhfuzm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3phsiupzl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vuirbaek.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zkbjhnef.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bbbdkypd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3udkthbmk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kpqlrhkl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gsptsrkn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qvhfzjrx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rwnbvvsi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zodbttxi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vyuyoeci.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mtclbhic.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lsvnqpht.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dxjjgzrp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3crrxpodq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wahyrnyu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xqncimqa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rvsdxmcm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nnmvylrf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xnfhbwag.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3uwjvfody.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vljbkqdr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bdqjsmuu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3awjxzeev.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3biwyyzil.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lbvovzaz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ppzytaaf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wmibsyxe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bhdgakun.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3toqwfmix.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nfnpkwne.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tjtsnpwp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3psnqriip.html


<!-- 参考信息 -->