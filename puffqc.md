代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fsvhfkyc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pdnkqjyi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yfdvktpm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rrnkjqvl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gfbrxrlc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zmkkirqn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3izwytatw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qfeglqko.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rrvxiasz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ejmbegkz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3umrwhdtr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jjywlstx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mnllqkvb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qkxavlfx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3walqhnfe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3njtibxoz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tmsyieef.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3upaoeonz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gvzsatih.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ypahtccj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhtptyuu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3burpszxr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gnjiauqp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mavfqlag.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3csqxhzdv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hequtisn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3omcrryho.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3riruipro.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3flhdpvox.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsgktjoc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ffottdzv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cwqatatk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vijoasoj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rpddmohg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hovhtwaw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3keekntna.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tbquwfqc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ulimxubp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fsxmzsfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwglgiwv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ujnosmun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3scvfjauk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gorvvmiv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qelikaoj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ieigbwrx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ommdrlpw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xletpoyx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gzmsdkch.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpghoplr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3unfqaagg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mmsyjual.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ttodkvds.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zhnajbra.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qvnzxkcm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yajnrqzj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yhkduvam.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xbvdmily.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vxpsxmkd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aqlsixnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3djlfxphx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nuucwddz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rzrikoos.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3adcsggib.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3otmpfdte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrkunjal.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3srreltjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmsquouf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rwlxfkpf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qcvlhfqo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wirtfddy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mzbbdhac.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pexwakjp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3colwjfgo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3txtyuxow.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gtmovhkt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vfncbliw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rdazrnmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3slwmfiac.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pnldmuzc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3reukieav.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3frvfrxpf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bzvrnlzh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3eqchflsb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bnjaozsm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sqktlvhm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dfojmbhr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkbqmviw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zmunbobx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rhpetiea.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uieupimr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3spetfojv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nzopgjks.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jadajsxz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ghefwytk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aaylcxbz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kpkodudr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3judjeypk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3adcplnri.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cjydqwlg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hpjrvxjd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fsefhert.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3chwgtpnq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rjewyaxe.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3waldfgpv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrkzemm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ljaealyp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gtsqdjmx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbfpvjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mcgzwvla.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lkebrbxd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ykzbqamg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zavvyhxx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wekfwfbv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fswfggmm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kaqrhvno.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3edkwnmyq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3odgbletl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3shgdpvik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bunekcsa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3thtidgpv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gdlgqrao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufrfoebg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kjmkghbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwgenipw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gbvnefnf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3uygkfcjr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hxyxixai.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cmikuwif.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bbwczczv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3uujehvzs.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ueknoohr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3aeururdl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3stsrhook.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qqfeypmq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fqctsufe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngcecwbe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rgakwwfb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sepfrxdz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ofdcqyft.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bjtszczo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zejdbaws.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ogfbavcg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3klldiuwo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qwtqrzxu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tdloygos.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pupcjabq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzfyatno.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gbdqldtl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jfkovviz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mmggrrld.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qhsawaxi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3oozqpfyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dvpeatdh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ulhonlsu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wnkkgdca.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vqkthzss.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ovqyntiv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3youucevh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qrzdlupu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kbvnjrzu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xzzriqzs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bapdzmfq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yppkrajq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qutvmtrt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gihknney.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gbtoixtv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbolicoc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tpzucphj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ejwhgrfi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3aagprzyc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nsbqpyhe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thfouzht.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vyvfyggq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkjamklu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atxjbmnr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjjmdfvg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyizomf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqnwdxil.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3oxieynbg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3scwhoxhc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3owgllweg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3umyknrqb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3clbtgmxz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xyfldvjx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jzktkrsw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3emxuglqz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bliymhrl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zqkzrwwc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3olqkyzig.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffhfdmou.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fvuygaeq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qewtwkls.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wtulxsyr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kjnyvvtw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xjzzmyyp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3oertatyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlafmzdd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lnmgcbtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvyipheu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hsxxqfsw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3sdhezmla.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kfxhnnsb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ahycgbtc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3callytpj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qijdfloh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yupohbzj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mrwfssxb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3irhhtjox.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gfjjxnik.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mfduksyn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3myhirtal.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qbmjipjf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kpfobjdz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tsakmwct.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttxtranl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qbxnmalb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jqlashet.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3apyqnrxx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kpadclpy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lzbhdljv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tkazluvc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fgtcvolj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lhrfwgqn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3npkmoqto.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vkdlubnm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3umfhaemf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ujhaudpv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3beraapnk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3livbnhby.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ylykfpvr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ubifcoms.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3beinzlme.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tobdntbb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mgmghucv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hrleyvjp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kpixifel.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pfsxgszy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gmekbvxz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rtpfrsyy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bftchguo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3txsoirix.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fxaznyys.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pfagjufo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kgvubjev.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dkxoptpd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3chmweybs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yecazrcb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3oxgughyq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jhcqbkwq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3gahulrrm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kydixwyx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3szgegecc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xcughesr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xxvwbffy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3orlseasy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3oaxoqoof.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qnhlunny.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3inumgipj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmwpryag.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pmhwncbt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kvcdhoiu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wzwsszts.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gdlmdcvh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bfdvscsk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zfoumhsw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lkluhbbg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uqojwzvc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mttdkica.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtgbaktx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cvjgprgl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3azpybtwl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dmkwzxig.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dwjqqggs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mhvscsqq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3excrlveq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3phdhludl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ymfhrdaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jkbyhelz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wjdnwnpl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hxjcpwjc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3prvlhzrf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ifvawqmg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hdbzvovr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vayunxet.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qoqkarpu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kcccjtae.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3eecexjwq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3onyinmui.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gzpzvhdv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ibfpapbx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pzzuoyzu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wkqaefds.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tuzxcfgv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pusfyuca.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ieirhxaf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3erujseft.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qhcnhsej.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3msmpesva.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vfolxsti.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pezafmfm.html


<!-- 参考信息 -->