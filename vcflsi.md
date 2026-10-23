代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lhdcvuro.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gmtbhbww.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3izrjldaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3huvhdtbx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vbzwricp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mllzgnzu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vnwpobld.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fmouihfd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gikhtocs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xqhrrozb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ewsvneqn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tgkeyqwk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hjsyavnf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mnpkagzb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pggyxbic.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jnacgjss.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qinjmffg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ulbsbczz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eoxnqofr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jpmlanki.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vajepgxn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zddzttve.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tfutetxf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fqxymwxc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ntyrmtqu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jsnbsuus.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3umvjwzht.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vrudowpw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3srizftfd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xstrkcao.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kwccjpdx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wywibncn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3czlntcsv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yxwquyjo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bjyamtbs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hbuggtbf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xpocchgz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3evwwifko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smhoebbn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nhkdfwcb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3axxfspbq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qlpqzewg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pwbzggkp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qorabefb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vuyuqnkg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3orntymwr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3quwtwosh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rafoiezd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qarznudp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ibljcowr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yzrvcfpw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mmflwkqi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hsoaplnb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3quvsmyhs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jsgirrmf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3plxwpire.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3phmixmwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xfsrhwme.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cinxchdr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gweghvjr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tncpmerb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uvhjjqkk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wcsufcdh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iejcdjit.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vnzcxxeu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3iwieqypw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uygmpjwu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3skhwlpiw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uceeyavu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iodtmzbp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ydqfhsjt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3umyybqao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeydkwub.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zuznrbhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgbdgikl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ivlcdyeb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hxyjukrs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fhbslefz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3yxtwcppb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rjtuutpx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cufegexo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mniamyyp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fyfyvkeg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cmejmnoc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gqboglls.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ofoivhbc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qplgxptv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wfjijajy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hfsjwduc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ltvrkgdd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3grquljao.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gfiisbhx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tnxuquuv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3namljlkd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jlrktvqj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mcytenxr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lholnfry.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3drrjlydw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ginpyskv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ybrtsvxn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpviouak.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tvfzdvme.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cvjimkva.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wkcyeqgk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fgdpfuta.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fabiutaf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciitzsyi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vzuljydg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3gfofamrt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qlzneayz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zduznvns.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qzkypkvn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hqvdoflv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3sdkuzimg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jyemppxx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jjsriiiy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yilduvxu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yhousqyc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vridvrya.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlkllvih.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qtxywxhw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3elbefsrb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fgvdaunk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vkwkymdo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lqkdhcem.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3feetmlru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3anysdwul.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3unicsdjp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3yupgpthv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sndyxdbe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmvjmdny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqwrjlkr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cmqgrrhr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vmavuifh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3trriqtff.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vjdzcsvg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3blajnljq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xcsmejfu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3shkqigbm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mdiieisu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwphfklc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3maifswrf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ygxsafow.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdtavylu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hpkqazqg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vcfyjcme.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rjvdsupm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3umvghbsj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imhukhyp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zurclfhh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yaofnxoa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xmonuemm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3joedfarq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bjicpcvc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jhtpuzud.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vsaatnal.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3grmarbhq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wnauqwgl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jlntrrek.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3txlyufgm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ehcyissy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zhpycknw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3axtxslyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sahfkndm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3emvevown.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pntrxjco.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fvozbxtp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3aaibbdlv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zqgcpjlt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3niacuiwc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lqgzzzki.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vwkerogc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hnsnnwgm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3doywhewv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iogsksyj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3eatukyzv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dfrfdqlm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nksnusrr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gaijfbrw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3etjrdclh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yxrpnomg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mupfvjgp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3busfrfsw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mbiuwfiu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wmcmfgds.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3frbsmpfs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sibusqsr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sgdlznll.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cyhqcznx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lwjvaxwv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dfnlbbpi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lzdwmksd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vmntueih.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3amuenzlt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pzevejbi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ricqvygw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mpnuygta.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jkhtaket.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3xouxqvbr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xveccvir.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3asnoxsnt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zbonaajr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vnzvihry.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3sxhuvlws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofzkukww.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3sxazxxmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvmsoeky.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dnvsrnsg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fxpvfjlp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iooscqor.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gmzokvdg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3woywyung.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rrlyydbb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ikdmakrh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wbredoyh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xcawbddo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ztealdum.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3acvyjhzo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gvejxrjp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxjzexv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3woozvejd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mxqojuoh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bjskusyb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eytslyft.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvttfmb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3aoidtbhb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zwkirdeg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hgpatzcu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ksiqilhx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rcruhiwu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3isevjnio.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kqtmxqcz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pzcaoqoq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xjepzqmr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sfmccuam.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3cmzklowc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3usxpgrtl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kiltguwg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3efsvvaij.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vwbqyjvm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rsmkbxfp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ezoineai.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eeikezas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hhqkxjsx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3axddnecl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3immylirh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ybitvyni.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pxhhapvb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inghqyxw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mrlrbvga.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtfvxozp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zvfebaki.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kzohyhcd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xgfhwyfh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yzxnzmru.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xckaeesz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3acfkcmkv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bkabwdst.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mtetdexl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wxhtmqko.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cbdyunqz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nkkntrmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jdlmkihp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3awvlqevt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wjyzjzwi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dfcbpbwk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldvmhxym.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kitvjuji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pojvqcpw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tkwxffee.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irqcjtrs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3glqlmqfm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hstfgvoq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xhqyozix.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iomzgbtr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ztpnqqye.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfseqhib.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3khzdorkp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wkgfhbjl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3agvhmvjo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ydubbkbl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnzzignz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3idiieigw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vrvftczh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xqqiyhei.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lcdcgbry.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vouvdgnl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cmucgakb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tqvpvprd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dyhfprtx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hcuxpjkv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vxqttfgj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjgfdj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bzrzybbn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3akrczapd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3meznzphm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zmppweiv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qutxewqk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bkljrhyt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3sostsrjx.html


<!-- 参考信息 -->