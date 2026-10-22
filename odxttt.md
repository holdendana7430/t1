代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2aydxnqin.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgbscllq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dwyhgksc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bdftemcr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2szbkdxoc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2stzwvjkf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2apzelyvy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhpcnkbc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yldojdlt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vmrykazs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qjzftppb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gugdhgdk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2svjzmsts.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wxoonfrj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cbjrwfxo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2stfyxiyx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ylrucjyx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wibnqmxa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2edbvyqci.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jdrfhvjz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fwjkyfzj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2alurjjsy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fdqyjhuf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lvxdhvqh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmdmgfco.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ehvogrim.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lfrzkkyi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oamyymvg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecinuwsl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vsqqjadc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hfsybccu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oyleafnw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ptpduqhj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2atcjmbmy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hftkjegx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2khyfaqpc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qvxkijow.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tdjoeanc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gmnxjdiv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjfkylnd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kmhqpwar.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrzpvvk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufsqtwkn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fzlwypjp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2aeoxvcmw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jghoixqe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ybvmosbx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jndalkct.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2homtvuxt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rabcbikn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qqwiaozi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzwxrlmp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbrjsxou.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hixaotbt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pzslkhvg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ugwxfbry.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iuwrobvg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xwccagjb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2emedcgxj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qimvtman.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2teraixdn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xmthyyxj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2epeezajh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ymrobgvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzrrfvqz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zjchhcba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hysmecgu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2duhmhyqu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sxqhotag.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vzxwoete.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cxerhhpe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kiymydfi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zyryadyx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wxpyvczz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2pmsnrahy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uvajgrku.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2odvfrfgt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2brmuanvz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2oxedibdk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2esgtynif.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jalifuvc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2osnaniba.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bcnwbcmg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yqlayebb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2okyizvil.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2actraqae.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2adevncac.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bexorpiz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fstswsjy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oeoephub.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2teextmxr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lublfsya.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2txhlxgdg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2irbqcyuj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2reahnofi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2epmixxrb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yaubpyid.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mifpdwxa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfzcbaxw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wrfpwmkk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2gxerrrgs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lcnmboyn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mlgsgrfz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xfrtzram.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2eatbpdir.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qfifgmou.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cnyhpbna.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pnbskqdb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mobtggqf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rupsitgd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2myxhnqzo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2svmlnaim.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ixzcfmrq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cpztwghc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yiiwnwhs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yydytpem.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2unfvkaot.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rlmzlemb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gmazhbop.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tntpcntm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2griiqkkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pulardeu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbpsfbpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuooymle.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bfblpzaa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gvpfffev.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vrsdchda.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2utanfeam.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pmmyplln.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2yypefekz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cnkqewdq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jtahjmnj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vowqyubq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fgakywvr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jrvrgmdy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2yfpmcnlx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xlzeaees.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2omdogiuh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fvvzuotf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oaybqkny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cndnopkr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2djgqpysz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2btcgfbbr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lufrpzmz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kawzjoio.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nausarbi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vqeyemhn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iuhdamnq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2sdzehizr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fpfesabc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bzihednu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftdrqlvd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qtmvvgxu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yjfkwtqq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ozcpyrhm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zgvjttne.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hppqrhmy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2huixknkj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ytwecncu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rydzetbf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fhitacix.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2enzemozz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gwxfpfbd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mcjarikd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yiiuamnk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2bklsrbhw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wbwdcyow.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wshyugfa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pxbtuzus.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bnfypiwy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pnkjxwet.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eegbtjve.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wlutqcog.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojwjdtjm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gitlaine.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwirrzty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2vayiamgx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hluzhamd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cmobzwgw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2alcdyzpi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ququeadg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bmsuljmc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wzwflaba.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2fotcyyui.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bgxprthd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2oipazbmi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hjytbxmd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wzvslohc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ypbayktb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qceglqqx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lrghiolr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcvygoec.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ibtynrkn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2osfjtqwr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2osgfnzvf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tkmdrmlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fupsdoyp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2digheeic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrlrsrky.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hvqgycrb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ugsfsyse.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vgtvvozr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zznbcrej.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2frjjsnbr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2knzydtrf.html

);
来源：http://www.52xcode.cn/Article/details/gt2majplpdm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dxhwavey.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yjprvjql.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mhvonfpx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ulabkhqr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vtvxtfyj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vcnxyusn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uyybtpnc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hdxetrwp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jxnzcguh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2luqpatgj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2utogwugo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kqlmveoc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ctqekeuj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2madpsugf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2oggxnrrv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2eriavrch.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jdmcetgg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2grqfbocp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gqyzwxpu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2erpchwkr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qadhmqjf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vwybajkc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nwptmblb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gsflljka.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sgajtezx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hczotvfo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2khondsgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2fubgozvo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2idgigfbf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fbyaezbo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2eurhcaxh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kmratrin.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eviphhsg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tvcvzxkd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tsdnrtct.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yjloyjnj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hrhcoork.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2aetxthwi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dwiuqrsg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oeroxozc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vkpftlom.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ehmqkwel.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2powvrwut.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tmpovlnw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zvkdadde.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2cmgmeqnb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qrlihtlo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2awgqchmx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jzenvbjy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2beymhdys.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gplfdgmt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ajwecurv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lxgmhcnq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dpzbbvxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2iachfyik.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wqtejkgy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2koryvcbn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ztsuwogi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwwgwztj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vpzanors.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yfiqwera.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pdhnuwwj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvsqalei.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2oocaxxga.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lnipdnxf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xnkkyptz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ejlcbfrf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xlgmljxg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pyylgrhy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2icbocnhj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2disjjusv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ppabbmcb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2toisjbex.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2yotvrwch.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pzrpzkvb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eorqzydb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lnpwcuen.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zonphmgi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2lmxdmmrn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ifvgfxhi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xlyekdxn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xjcqwrxb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2clcbdgnq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2oxedbqwi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2olujcvrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bmhzcrwg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vhyzkenl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2glvilpqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sejzjooi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bdrhmrmp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vcajrect.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2euujebsy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bgnupekg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sladmqym.html


<!-- 参考信息 -->