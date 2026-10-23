代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3njbdfyzo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qgefzdyt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3objtmgyc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bblknqcz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gjmvexjz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dnmfnedr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sxcdwqql.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xcquamks.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rugeolqv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3topomhpc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kxehnphj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tulhostt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mwqelmld.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3opcxusbj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bryjsijk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cbnbmppc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dnrwnlru.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdwltlh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hlncqmns.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uyqayszg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bkuyqgxe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3avnbxsrp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qeweldfj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3hlvpbbju.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lubljtrn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3morcoelo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmkoydbr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eelbwbxh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kxgrfyfc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sxehkxse.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mgauhwgr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hszmzsrq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bxzgqyja.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kixofjmu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ygvzuuwd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rdeiojuv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mliadnow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ssedvopp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mhxhyeck.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fwxwsvii.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ncikbytv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lgfucdlg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3limmuntk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3eexdmedq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3igraxfpm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tazqligv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jgrifotq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mvinvfxu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rcuymmmb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hydnfwio.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3atuckrev.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wejmbgzc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3uipnbpwh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uojnlroy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jxyovcwm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jnaipsmz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhkjbiad.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cibexbve.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fgxovixq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tcifoghu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3idsftrmw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vinwlapa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vmaawogj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fesptwbl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3czodxjzm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3znbjessw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3svvigihw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cfhazuhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owlbxuyf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3iitknzqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbyfqcfh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jaosgbcj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lnmyearp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nwpjcwlm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uyaznwqp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kixztcfz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qbjjnvco.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vbwfctct.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zelsnbgs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3obfjjsia.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aluiwfec.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmctuuh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3klssxorc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3giduihim.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sfdpmqmh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3heltycsm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gdbhgdaa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3duxlmqon.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yievoazd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ixarufht.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oqzjnlhq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qselmqbr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3cbirydjm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3knzoswgb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jxqxnzgp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3adkjkyrq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nywfontc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjcxgtun.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vesfikmw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nmqcwelm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rmvahcjz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzuhznnk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ooahibjb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3avqtoywi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ekmtbeai.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ejmadyuk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnyjbgbv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3cmxxqojt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hzgnxteo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uecnuetf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vybedruc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zeoiqsoe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kymjekor.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hwobocfw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oahrhijz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xppforhc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3udfyfqle.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yifcxzto.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kijnfacj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nytqshiu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qnyajmmg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3odsvyjwn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lhszewlj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3lbosuzkl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxfqgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqmndvhc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vkcxncbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mciixmud.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dekngzmb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nmyventv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wukcuqhk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3btuzhhpa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uzbbbbku.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvcfpwsl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wogmuqws.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gsdbvdkh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bdjusvpc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ejpokkxh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ffcffwnv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ajufqhsp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kygqkwob.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sgmiwjyx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dnpmcsub.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sclgrihn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qokphktv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ujigxbum.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3legiawih.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kgcaoagy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xznzwcwt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fzjtlxlm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3stslsyuo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zixovtnv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pqphvhhs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mgmhjxwt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fmrcojti.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gsbgwrdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ztctbtoo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hreiescv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mxijmkcc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lliqmrxd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3coxfriwz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hahtiodz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3msrxpykk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3huuqxswy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3amlrnnit.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zswjadss.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kmnujiwn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qfplaacx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bolcxmeg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tilmnkqm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzivnln.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sppmkcnd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3entmpecc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dccprgld.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uvyuzjoo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bqtkbpwa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3nauenyrd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hctbhjhh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xebmtthf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qhrkqoxe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3adwblzwf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3inrcccpr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wzdddudv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wrounajm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3shaijjlz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hjpiocuf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3khrgqqrw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3codtxixa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uqszrmav.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3habckikh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bczbsrul.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wbaqizbi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tddxiwwt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3equcsvvq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eoceyops.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wnnsmrey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xpescdso.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3amatfomz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gxwjmdje.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mnioazwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3donslvvy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xssqhtij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mytsqofc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wnfhrhev.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uqcezfdj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3utdqenlq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vvxyrabx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3axnlygln.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3prodxdyb.html

);
来源：http://www.52xcode.cn/Article/details/gt3zyyvqfdg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3legqdcyb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mbndvuuj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wsrthhbg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pypputzl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ozehnnqn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zegubtpz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qdhrvdwb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3podhfado.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jwdpcajw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hnwwdexe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tydfftco.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nobtcled.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3tzwcysnj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xnczfaer.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vitnqtgs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rfqicwhu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3giwnttmx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bthodttb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rkemclgk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ccjzuuvt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tsjuyssf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zweynxhw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yaeooljo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nffgyjdj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nxszmzgr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xhbioyid.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mtquwrfc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qmsdwmmu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jjnqbvcd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kvedbher.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jljsshye.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3evsbcbww.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3unfqlayk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ghrtzwnt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qzohurps.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ygujpqqe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrjtzpwc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pthiosii.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3soqmvbfx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rjtulqek.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3puvrhroc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3aokhbxny.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wrlwleoi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hkgqzhfc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhjixanq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ttgdbyaj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3viiarmbz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ztllnfnf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3duecuqqk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3amupmgzi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wuoofxdc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fftemsul.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvydkmcv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3brunbhor.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3azdjtisu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3pjkkqsdk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hechykbp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3iydevims.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnskxqlg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gypwqvvo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffmiickd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hairatzq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqudqspl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3uucfucem.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gquhyjij.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ooisbchj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3idmfnqtk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utyukgwy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qipolcig.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fntjqqjy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3aknlsdid.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fsipbqmc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lbyixtsn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wzrmchmw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zhsutlkh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lnfsjipa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tppaagqe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yfwdjvqx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yfxiieik.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cdjbdgvb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3warqutwd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oaciqleo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kfmjjaae.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dozlfqfp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nmfdpnvj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jyuypvus.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jtglnkpn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rykknzdd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3sqtdqzba.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gptcjlmr.html


<!-- 参考信息 -->