代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3glxnoxfn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nrirabaf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3sddsuqed.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3aztgtycw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qqinfrdy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gmntacpf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cgoptjas.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3odzlkrgu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3grjmazaj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mokzdqfg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3svcvlffh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bcsekoji.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3tkdssbkd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wamqrfus.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3yitkkzzm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3acyelmua.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjsecopt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ahjjyojk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sacyeqdt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wypucmcb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jjajjuba.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hkfpqtcf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nihucsqa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3szgdsfbq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vmmbprca.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkfvczne.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3awvryzyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dfujqydc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uemqqsvn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lgmxhqvz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eicslfjq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozqinsek.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uqxhrakt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zfzwkrng.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lhtxabmq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yxpxbvar.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xnrtewxl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3szhkhcte.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dzcanbss.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kvfvuthn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3enzllftu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rpkqdequ.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xezpcspw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jtvpspeo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3liueuful.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vkyqsilf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wcmwopqn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zbcgjxoi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lypwernx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3drkrshpt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zsfatvmn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xyfzfqze.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zvrapzwe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zdaeabtd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jvfbwxbn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3trmcmaqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jedhlpzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uckbywwr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3szhlomgw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3svlsvgjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtxleous.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ouggmfyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rirrbgmv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3obgxvqci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uhyecyuf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ocdxbpvk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3exzrudpu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bxedcrhv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3njrngikv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vrqyanio.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3sixppljv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ltfkuvyv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uqvbqzco.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xeeprmeg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3evniuolb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3plusoqxg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yutkptvv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pcchuudp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3biqugktc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3egpdwkey.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3okjxsihq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lqqadmqc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifhvhpuc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rtbvdrjh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zribjryr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bpkxseef.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzmjmxwr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3haksoyqd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzcavak.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3izwmrour.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mwfrolsa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3aqujzfvq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3opoprqxn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gdhybotg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3srnrtvag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yttlmlgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rmelvqof.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dutkrrgr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wynphyfb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bkggmtxr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3frsbsbwc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ycigwzzn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aayjqvhk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ftpjunpl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ijcshxoh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rmzehxku.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bbyudgvr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbzzpcl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xjhutjgl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bhfuyxyy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xfbdgeff.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nlthgojx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3czzjuhgg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3matwboka.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nyueicnp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wtmnbmng.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3livfvmbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lemiphaw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dxqhbruv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjpswqvv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yluozhey.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mwgtaftx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cmxudfnf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bwpshxqv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zlhmdsju.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ecvdooft.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hmeyihhb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gemlfpym.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jyfkrqxp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3neqzxznw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xypgbxhn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbcnxuvu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bkkedpqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3luhrdjyx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nlseaqba.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xsnmttxx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rotytxnq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nhoeddfb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wvbqhebw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mtvpqwsq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nrubwshb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ydzkamnz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xczrnmmt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wzqaxbhd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bqwvvdvf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nguwzddx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3osaejsie.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gcndvzkn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qfaewczh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ipqsuqik.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rslizqxh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qhkzeyui.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3snorjvbh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xwsijnxk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kurfavcg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wnomudhu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3epurvzvt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3netvqekg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3frjxbfzi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oftkdyzh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbxjzns.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mikrbnmo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3allhbnye.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3uzyjxzal.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qqjbsonq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wwwlmdtj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3eehsyjlj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hnywpwgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xiaoldli.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxxwnxcr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qerftwhk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hthqxyhq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gjomafsf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzdhgscl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qdzrxvyp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bdqseuey.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jnboklfx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uvhfrdgp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rdaovngz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3llwfwquo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fnevbaqd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jmcuwfpo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lopjprus.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3oprzzcew.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tfzcvzcr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nbajhfrs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jagqulzf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rjhetiqa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3sxuikvyi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3yupqsysg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wyqktylr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fhaxqcmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orubiruh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cgowsjcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwnufogr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sdamxjdn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jdjevcav.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vujqlhub.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nhmyadzl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ajqaenhn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nlafbnvr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tfhnyiiu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ghrriwoj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mzcwfcqj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mizppcfq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3urwabzml.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ispqixhp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3duemlepg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xfbrzqfu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fsoupzqk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cqxusull.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kfztpucu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tijkokbk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rlbcptxb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mqxtsqdy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3uywfsjwz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rghsfhtf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yydxerwf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ypxqlwzy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3madaqwkx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zwvfhbyy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yulcoboe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xjmpdstn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vgrhgdck.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gvydhxtx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3sfhstxxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dnguoeyc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bjccjmpr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lwibpbqe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nqovkxlt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hzunxime.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cxvtnaut.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bcbcmvtf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wyslaikt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xdysnvgr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3snhmyxes.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssbakoqm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bekvdmkg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3enejhzha.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3algqimzd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tkyfzjjp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vapgqyzt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mjxubasr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zuyamedz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3eyjjrybk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bwzgtlff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gsxgzfft.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wtsptuud.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3daenjcfz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yzdyyrap.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hdqxoovv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3npevruko.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qtlbcsyt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fnwrpffn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnctkicu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bgzoerlv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ssndvzjz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3asjbcacu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3udxriamo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kmzfpljt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dccntxrm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bpnzcqng.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zybjdjyy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fsmugzbv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hecobnbc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vzvjuvae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dqnkigoo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3apeknftk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3umpvxnta.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3itpbujvf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eabfkfnp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3assbjosl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dnzzpctb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iakudunz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3isbkywwa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ufxxfkse.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3shhlehuz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ulxvdxgv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pschbdhm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3saeebygs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ytrmvqbz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rnssaqgv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hgezbehl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3swaebixg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wsolvncd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpoxnlce.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aibcikne.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xlwkcmhe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gstgztdg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fgnyqojt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3biygzeng.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tafnztji.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jgmkaeqg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3usrqptis.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3niyauywc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3piglemgy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3aypakaff.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3thhfuzdr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nsclrlia.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tfpzftym.html


<!-- 参考信息 -->