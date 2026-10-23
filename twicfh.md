代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3juuccdnz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gunblqsw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jvlvmkmc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jurxvhoy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdburob.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oirtzybf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gwktorit.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gvuiywxa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbsmidru.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rsxmulig.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xvvdtczf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iuikxrwv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bmbsuxuv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yxfipqzr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oimutarj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3itrxtvkn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3knymimxn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mskdmehw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pdhcxjoh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3betnapmt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bzyikggp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gcxvtjop.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hqvhqxqz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3viccbyso.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rffhoint.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3aecuhxev.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fshmrwpz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rxeahmiy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rcqarklr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lmocqlud.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zsocoals.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qmsdaemd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3flbdsljc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ryxxlvjn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ugcznrxh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrgubgtj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3onybljsu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wiboyitt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zexiwlwk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wkqxvvdp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jptjiokg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnavapof.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ysniswcq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aeecljpr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wjxuhkrt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tzobdsww.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3marfdvjm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3feokewvp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lvrsonjb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xsuntgsj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmmuqwb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xyshwvey.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3usirjdlm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnzvfffy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3khgvmtna.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3chfaryna.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zkjbvnhf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fyiilgdz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wxmkwkns.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uskvryln.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qiaimytw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3moozwlye.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vzcktsfb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iirzueqg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3grjkmdrr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3djhcwvdj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wclzrmnr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3epsyttnw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3szubxqwm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kkbbydyx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ooqlagol.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3epgafkuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcunauss.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nfvnfcko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrpjgnkt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cdqigeyv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qwhmlwrb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3pipdwexx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pcuesrnt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vyiszmab.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3etdueoeb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nrwexrff.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3iwmzmjzz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3miiwmyjf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eivcmkdm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzbgvxh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jjcenwqb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wqislrhb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rebxbkdt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cihmtcco.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hibyfuhc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3snnniwdj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bbydwaln.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kvrdicml.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3epokxfxp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zerazrgn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dvbedhwf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ktntrank.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tnvtalgu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3yqehcodr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bplpsjea.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rybfzaab.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vdqtfory.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ifmrbmve.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ocuuiaqf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxgsmzhp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iotufdsj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gagnqgbt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bmyxkeib.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lwqvilsc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohsijyls.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3witlsbqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3viaeqsjf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3unnrzvsx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxvoyhd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3luuxcxzb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lbrsrowi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xjhsecbz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbmymzm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhscfui.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vqkxcmls.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tbgaimiw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3etknmpel.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3maarmziw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fgzvqcoj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3exbcbfwu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aevctawi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3labooigh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wwldxmbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojrnkqvd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhoeokap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xttrlhon.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3httbgral.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ihnwjqfi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ttxwmigk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zonengqj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3edjfuoiw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bfbwahmp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rwhgjuvy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bsmqmnss.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3axitrefr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fomyaycz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yhxsyiql.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mliqkkhh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vdixccop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ynelmxfi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gcerberr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xtwkxgyh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wicmxxpz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ozqjvnrh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3njwqgbco.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ewjbggze.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mmezgkth.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rupvdbpd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pcmfxgxk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yyxstpxx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lpawqqsr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqzsnqu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3feorteao.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ftsrmqoo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3quscesxa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3carrxfgp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ljgexgyj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ozzjmknq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cgolkdkd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3konmznrw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xfatxkgy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qljyxmgo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3flgatksd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3abbktrxu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kiikinqa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ctolwklv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tkrfbsvj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bnewhlmm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fiqpnjdd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mkelvlxg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fmirbngt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3btttfqps.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tiyufuah.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzrxdrxz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wwqsmbda.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osqyomlk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehhbxhfr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wexdbfmu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fvtyqiah.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fitgysrv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xjemriue.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nzgpieue.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nltbupnt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hjzdkblk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rneclmna.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qpdpgdza.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xwjyqdfu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3eucwwqbk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zdibkfyi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qlwrzzii.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wsdiirqc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oczlxlcx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ccuisduk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wxivuctk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qtixitrl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jiyczuef.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dxcrnsld.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3exaeenle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ottgrkbs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ylkrrahb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqsmxvwx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3osxmvyzn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kmtqlqnk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tmjvxyrk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3orphvnlv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3opttseuq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mctstoof.html

);
来源：http://www.52xcode.cn/Article/details/gt3jrjxqvqz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rdxbdqld.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ujtodemz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tansulzy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ayqsamam.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3croowzmo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wajnodqv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kgymolyw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ttnjnewc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yhvyxzrf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mhgxlrkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3thqcfafv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zrqceice.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cpfpsmuh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lsvivmvh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3lghkuaxn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wewmfmpa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tmiqgjli.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xhoiahfv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zlbauprm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3sokbioiu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bnnjbulx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bqznttme.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tmgjamqq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fblhibio.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tqkjcgis.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dbaumxbf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3woagikwn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dtmuybdh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zllplvlr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rjbskfij.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qrzbywqe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ejycrrnu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3unhfrdld.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3adbdzenn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvamphjv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wrocmqzs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xurjysiv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3obmrfwpc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spbynulh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3roexezbz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zojyvwml.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kswlaqgv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3svapuynj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3owgyvgnj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xktzcdim.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3efguubqd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ufggdlgq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dhgjulsr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ywwsxjtw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lphsatfl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3iuitohvk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rtejkwcr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlkfodaz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hnpnmced.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nzwhabjj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ocjsbcev.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqtcuker.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ehqdznzp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjzrhauq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jtrlebri.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3npdobeex.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jamougjn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fuakzoaf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lgxtknjc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dygllvfv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gunqsjvm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nuvagtwx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tuburwln.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qjjkmhpb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3mtiszgjo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xjqddqmr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3tftacdbl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vxeaafhb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3sogucagy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wzfaaenw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yftbqghk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nfgplvyw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vfdfwwkm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3iptmivla.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ertuztav.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ngdpfzpp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ucsbhkmg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3eqnwphcd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vrakxekl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vplytfmn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hclcthok.html


<!-- 参考信息 -->