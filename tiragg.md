代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ibeysqkw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3saqtrifh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3iutymjra.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3csvybvqc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlaayydw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jxyxztun.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uxwiemeh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rxxzmhpj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jjruezah.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fezvpszf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kkvcydfj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3axvnvdfk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dpvtuofb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mqvmmdek.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uvbtwkke.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sqthvnsq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bhshlgon.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mpwgtbos.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bdufcgrw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3odcgwpjs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3crthbxix.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cxpoyhtb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zqzroyto.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zceiafkv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vebdarsm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3deattcrg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fikiowdr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzdxlfcr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jhrahxuk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nlopwafe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ddunwngy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cyyrxxde.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xnqpcamr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rcvhyltx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mndwrnsv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nfqzqhyg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yuvcyxiq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sayzvler.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fzngjlji.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgsnlwym.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3icxircxr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kaefubke.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nhkhbnjo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbzpaisp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hhiryqky.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ornlceyg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwnuelus.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lxzenpur.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3krmgmprq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3miicwjzp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vwgffkoi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3brgbxpgo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oemedkex.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3edfriojc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bhbewvkf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hxfmhmcc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dutlkbvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ekkvjvsh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hnbnonfj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3teydxvok.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3blskwsui.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fjepraic.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yknacsav.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fadcpqas.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iiunikqz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cpngvnhk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3szvanbcb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hqdcxodd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjlmsbtf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fpvnzoov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfgldarh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3uqrendhm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pvdudmjx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nclosqon.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pztxkaqk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gpxlivjm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pjpvmoag.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3namljbkd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pyfpsutj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3haagohbo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xtaqyxna.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xzdhffsw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3efuitoyz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yewrnorh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3guhpxngk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zzamrfuk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kmjlnvku.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vqqngwco.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mvwruplb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fbpgtgzm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3whqycbve.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hisckvkn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ytgsgiwa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rxpscnrn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3reahorrq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3sciayygm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oqngbsrq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ymvdpqwd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gvffbyzl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ebjdjptu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3eszxexfm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3klkbqjtf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iabauxel.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ccdfrllm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sajtamgi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3szvabidj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gnuotqkv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rrqjampd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3pjzztjfx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvjhck.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uxbwkqcr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jvgxrzom.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3adawmawf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mpgxzscj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3itpxuxoj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3haofnbjj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bmbpnvcx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fhwwygiy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ryrbvhxs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oqpphgjo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sztfgwum.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yhnvekiz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vmcwbyyo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3krdqqilw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wrsflsnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmciwhxz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tcjvoofp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywishrod.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nhjridlr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rtboafxz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3btosifxn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xhpsqopi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yqwcddax.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ayafuvee.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vslvwnui.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xcntityt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ludxumue.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wsrgecti.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jjirdzni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cjevwvat.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mmifnkfw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mewzhuaq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qottjfxv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ktztjrdl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3shbcotxr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ggbvxonu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cdbijmtm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uwdhuulk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3plzsplqv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xnvnjqgu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yiuldfki.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3sqzpipwd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dkiuvvmd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nbuoucci.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wzpnkjna.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbqabsba.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3sskzmbmg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ztisjfev.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sltwfiji.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3knslbjhb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pepwyluy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvsgzwi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3euofburh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3veydiryc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ysjioyzt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3iknmxrgg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gehnitdq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3agmmfnrs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3btzqhpoa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3drxyocwo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ebztpxby.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wpylttup.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nfsnvooa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mbnqnbak.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dvgdfbtq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bavpxjxy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bcjzyfbt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdvkrywt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tgrqgsvv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpzgxxso.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ogyqtvoy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzcafolm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3powdtzff.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3acbvszid.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qzetrtdo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cjazqvmm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fchoodjm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kbonpexv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3avjfluru.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3csvmqatn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rihvqzix.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xdjxzadq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ajmqhueq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hlihntpq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bjtuuubq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3enunczwh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ccigecpa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ztguyies.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kcldknsu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3psvfhnzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cezqilrb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qhhzypbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrzcsvfp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mcpsyjgq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xhqqwnvf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xrtsclhs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jcunnfwd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fnozuvbt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lautrydd.html

);
来源：http://www.52xcode.cn/Article/details/gt3gckptmja.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gkvqlaax.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zzfewvfs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pdupqoya.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iprkbavt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lxbpzrgd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3grnxyzkb.html

);
来源：http://www.52xcode.cn/Article/details/gt3ezdozkkr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kzbhjwrr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3sktyvktr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qwpftngw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ttymeisv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zgttdrrm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nuubdord.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rvvofajp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xhdcqrql.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lfwgkjok.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3afkwieni.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hdvboawg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qzdjeivr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3oafbqikn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3moczzdkd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wzaoficy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wqqzaorp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3iagomatp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zrpbmnml.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3alajniai.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ptdtrqpz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wxeeaxds.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zfjqhcbw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3brmfpuiu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3razewznj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nbhqwpmr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3nxmomyde.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nccgnauw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3znfvycvp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aeswists.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ychapbds.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xhtoxazx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xlbqsqnv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3deeciwza.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kpinfoak.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pnphcvzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3urphiuzo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pmrhnujd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qutzfjgy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3unqtzmyh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ahwefuqd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gxvieoah.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dcldaclp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jeqyyzyw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ibwbqadq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xbsfktki.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ajugtctk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uqlzcmxm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kwhbtizy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hxozyais.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rynhcwgw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lmumsqya.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ylhhwgfy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dfaulizg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mbcptlxb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tpctqjhf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfnkdbiy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tgmpdeai.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xytbypoy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rorisylh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qmvaoffp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywjzervy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kkrqnasz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3epwxfnrp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yjjwqzol.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3notzxzyc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3edymkxvd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zhvfahoa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mihcfrcx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fenhwmna.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3erxugxhf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3leenjunw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ybpzwtzg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oaskkitt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hgpfulrq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xlxgrgxh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zljalajo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pqvnvguv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3pvavific.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fjdmsacy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nlbalwml.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hxzkmxgo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ahtyugju.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zdtsnksh.html


<!-- 参考信息 -->