代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qrvynjjl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rbnfabjg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eihhplit.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eburcbhz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fgadekar.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ucyanwuq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gjuhnwls.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3glknujiu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmbmzmbc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xnxavqek.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mzircwqx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shdaasti.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3amchorae.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lgfzlzdf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mzwefrxw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gdlccqne.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xpgeokju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bsaxuuaj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wffqqikc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3enhgtkbq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yacuvgwl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kjamkrja.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ojpebdav.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hlzryjto.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pogokqmm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ksuwydjs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kwewidvt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bojiwdxi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwsrfaha.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jltdltex.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kiuosdff.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zlpotcit.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dbvwqlqj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3igkkjkdc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ywtsyxye.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrmcsgjj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lpotavev.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcyhurmd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ltzwxfpl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hmptoald.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kghivcrq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uhngwlkd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fhbyngap.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ibdcrhtj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3owttybbv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fkotzxbw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3irctehpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mayoxhnt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvdtukib.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3iribzgfb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ngenhvaq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tgcistsd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qjiydhqv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lhzzzxkr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ldipwwer.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dekhvecs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jhzisxvn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hvzdslhy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iwygmjzj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jmlpixzp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3orcbppoi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qxnutcfw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wadzepps.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uipvjyld.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ntobhvpm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ktvgxegx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pwstavno.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3flhvxntn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mfbbsjnb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qgtantjg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pqwnqrcl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xswuyuqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwwibmpm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3powhdugx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbtbnzfa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3aievszxf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jwbndfld.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kouehmww.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jqkvhjcn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hxbstoaw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yagzqejl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yucgelcl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3otkrfdiw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kdpvoohx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jkyhnjuj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fdonwgmd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lghlftjl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3svgaqwlo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mjjhqjyi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bnkpbrsi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3atsusyog.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yrthjthd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wonosinf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nlckykgz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tekcldgj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3czdkcedc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nqyxiyos.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mmebzlnr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqkahfut.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3izerbjym.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3scfdcneu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ayjnaatj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zaabuzpj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3svrsliou.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wnewcujj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nlpungcp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jrisnqjr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mvjtgcox.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dvqvrqjn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xkuqkwvf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3onlwjybu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pvjrrrsw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgszxim.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gcgfjdze.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dwnmcuzx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fmnetxnb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rwzmjixx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dkbjjzgr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3apwtlxek.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzlbhel.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nxffldsf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3sekrbkos.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ilghgert.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oarvpcom.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yhwknhef.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nawlfvvl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ivkebbek.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3esncjvep.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3mvuyqsvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsnrwxhn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoykajrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clzkrcco.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cfrdmpac.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qknfhfxs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gzrcqqkh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3byyvdozp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ghtzgqdb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rszttnaz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ufyzfemk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cepmqixr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3etouvxcl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3iyjpqbde.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3thygmcez.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3clznlvve.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rokmsotk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wscozzxs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kctrxnsq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sgnvqpga.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnthnryi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3swybywzw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylgbdgod.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3doysycvb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dykwhkwl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3shepngjj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ezfngasx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jjntvtqv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3iccspvye.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3umvdsdla.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uxvudtkn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3odewdhhp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qgsxkiqf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rhelwuwt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jxbenqpe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rchrgulz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tfxqkhhy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ezapdrxj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3muhxbvwz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gpafvrni.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mplstzpi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3reydvsxo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mqcyeyid.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dhsikxfi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjlytor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ksmbnzob.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tktnavdu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3eoqnafvy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vvpdtfgh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ewqnupvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dnbqqdyk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ejulvngn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gqehcfcz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zcfykmnf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciijtkkj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdxivwaj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xebljcaj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcwalguj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yegxjjga.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ccbnfozg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nxosmigu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pncubdko.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3amxdtoob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3soipykjx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3iinlsneb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhmdfeyh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zvzzmgym.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3cfrsqudd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kfwkqqot.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hknmuess.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3farimdsb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdftauw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rjvthttx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ggibgdqu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mlhahamp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ygocxnbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuxuvken.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3opvgqjcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyswlivw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zcbtsobl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jrhpgczm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zndwoveq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mneitmpp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3aeiwulbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3njdvguzm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kxizwsxa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bylopfwf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cvbyjpmx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dfdwpque.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hprwlshs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fffznsse.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbdhral.html

);
来源：http://www.52xcode.cn/Article/details/gt3uuidrknq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uteyjzrj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yjnzpovz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmgvyuof.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gcuxenau.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3oplpgtmu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3blbebktz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3cffbkpdd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3yybelojp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hfbptltc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oixcorvm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mbhvjvzc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xeiirbua.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3tpblsodx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dxovwgsm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qmpoxcxa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mjopjhew.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wuminyxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ghmdsolf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hiegoxrn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3acccqppo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dovkxoog.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mzfngiik.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lxhqevas.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3cripugid.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bgvtyuvk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zotjtuyv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nloquibk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aoyrisgm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3drsdjtew.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3alyddfpp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wvgsgloy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mitjrtml.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lmitsrck.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zlubjeuf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3unyovstr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ugklvejk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hqhubjuk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdwfsvag.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3riwxkjql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3psqrbpfe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3syuhnord.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xrbaaoab.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ctkljnlg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3txaelmle.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3okkqzefh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3teiaxfov.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bwtvnwwh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3omvsafsx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jdrvjrym.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yesgtwbv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3sdgeyfjy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yelpbhvy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dmfyqncd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hckjhpbz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3buaknpyu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkpwgipw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vbfpssrn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hsporvrq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3iqvvwrjw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bjsmzolu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uyzsgcfh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dsbyosdl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ufxaamms.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sbpleapj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iqzrmgex.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3uqfbizan.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3krkrbssb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ifonteby.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mklwuijw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ahcgkrhz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3frkwdgwy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ftcspwcd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ruoxwqtp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tfupeino.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wobupeqh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nziycfev.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kstsfdsl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3futlbksd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3smjleqdm.html


<!-- 参考信息 -->