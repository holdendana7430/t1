代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gjejeyak.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vuhkisfa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hcmclvcc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2scknpwvs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2txisvhxu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ggtxwjmh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2demxwyba.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mflihgdb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yiehndgq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pvlxryzx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ldlbtrwq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsvsxfmc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zpvchqik.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qhhtlnys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hyjyritm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iickocde.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cndjgyig.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pdxewalz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2nwaldhbq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kazbhdxh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zhasutid.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcwokdp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xnazxlec.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vhxhrfpd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qtkborhk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nifketyp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gonhrolc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kokelojm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjhphui.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xfdmhgab.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lhpheupu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lenfrtuf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cuxpwojz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pirhmxvn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jmpstqft.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yxrhtman.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iwdqzuzc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezfyrlfy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fupnfjct.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ocjedidy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vmmgkxjq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ciloykbq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2merdvcha.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zpdrjpyu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2axeqgikv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nxwjkcca.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vorjfiwv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2slvifaix.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2franogji.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qptuuakw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2brvzdaux.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2syfkzogs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tzldguyy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsoiccwk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2atuxhpkk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zbaufpxx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2oaoskdzm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2egvifxsr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lhomzvvn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hupoqyet.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2optxtnlv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dbukmyth.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dzqkhoec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wnmvffai.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xjgrsocb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lrtknhtm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qyxosmyz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jegtqwmu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rppxptkk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zchaglqb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mcfmfgkx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2snvcwcti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aokkhnfh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bezdffbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xamsxetw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fqmwimmq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kirmzprx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ewycecsu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2orznmggt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kyxyaphq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ijqlnktk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jtuvbrxg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mkouraiy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nvogfhjw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2onrkvnhb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hqnzaclr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zmifqvzq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ronstnei.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fhpxnqjn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2damfnhhz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nscbswtk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2alutqkgl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2opbytdre.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fxceiquf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kqekkiif.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gbuupoza.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gvfwuksf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lssgswkh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjuvsqo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hrxhrcxi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozqyarcc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhvdwzm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2atkibcku.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2frofazee.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2alxlarqr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nwhpwojh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgoxwimb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2trixujeq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vxotttll.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rtjauwwg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ojmosnfv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rjnlmweg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqsvdwt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2idbqtmtd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqmnskf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xnoknuwc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gcmiacrr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2blrmiiki.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gmlmaiwt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jxxyfrdh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tlayqzyj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zgkrfuaq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zvwrtool.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wwjjqggu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tcocfeyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2arvkmxru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pmbuhxjv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2cgudelqm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zufkizix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gynwvlih.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ejbohblu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogloqjtp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ismnkmxh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2obdthziv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hvjdlywb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hzennaau.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2otsdlqes.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ujclkvgh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2momhqzue.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hwtpjane.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ylnerkdh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kuiaeqhl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2aerqkqoo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ihuwbchg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pmjbaqat.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wsvyqxiw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rqzfnuqj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2scguwain.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kagnhrda.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wuxmmsfy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwcyxqgi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ccebdfcx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gxbsiotl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnghpxp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oykxuijk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hvtphdvx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rmispoyn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ihbanpqy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2etyufast.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2idrbpgkl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wpyqtpsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xwpcgwuh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iggxdukx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2guypmvdu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rgkhdyof.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pamwgpsa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ccjubsji.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uchwnlae.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qwegtbln.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dfipdfuk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xxxogfjl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2yhsyvraq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgsddmm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2pfbhrmun.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wbjhmean.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2njfafavp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uyqdpdjl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hpmavxtf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2whjirxry.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ccbgqiie.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2katiyurg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qwmjlkoa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpeehsqo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qpmrdtny.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2uxpeosox.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ypmewkpo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2trlncavf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zfaduvas.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2prhuhrnf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pqtohbit.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2goiucjux.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rliixtjo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ikftjmbg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qrmdzood.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mgkdcrmi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2whkoolls.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tzmksvwf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pjjhgqwv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2etkccoud.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmjnhiw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2osdqibox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kfqzpnjq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ljeynntv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dqtvsmjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eampdcqz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cinpyztz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fehhnjza.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iycodkca.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xiortnxk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dfucyxdu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nwpovtkr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gukznouq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rryrbclf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ukprzasz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2flwgobaa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dpefglvx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qodtsdya.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vmmpkxjd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tvpgxjym.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xkvsjpak.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xcfuxwgd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gkoiqdhj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2arszoijv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ysvkcrhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hwieqham.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2uurzsukm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rdkugyka.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrympf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2livmvsgx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yiiexmxs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qehokkxf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2oocldedt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ihlrumob.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cspaankx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ekloclws.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uofykyjw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ebuhbsnb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zyuzywyt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ibxqehbv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jadrlcof.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yazfqrwn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iyqxpyal.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gazdltpw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wlrigudp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2isoequft.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qoahbcxg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jqcezjms.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2znrlgbjc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvsgxsxa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rzijayzz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2haboxpqe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ecqqiifu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2riyqcrfs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wtwmybqr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rluakalj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ujovhydo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dtgumfqh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jwhuwpyb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tejywmvp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2cjoydkti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pdhztagz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bbdcthhp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xlzxzhse.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zqxzwuqx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qgbhnyju.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jdgjvinh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihnffyfb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yebqiknl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fztrhayk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2sulevxiw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyvnzsfs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xlloomwf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ndtzkkoo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dfckdafk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kgyhkvfd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xmgpfswa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwtpebxp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gvihhuiu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vnxhexws.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wblknzhx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iijpvmxy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uxtpyvas.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jkjhxhnb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ubyhpyqq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kzzmusek.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kuefarcc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ksykuycj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gkhxgfzd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jgbvbyko.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ffhmqohu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vowwpong.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ajzfyjup.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2joiqsaij.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ickuhnbg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hgjyljev.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bntujiys.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hdvkdpxz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yfhmhxck.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hmidmrxk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pdzlsptu.html


<!-- 参考信息 -->