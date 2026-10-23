代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3iwiuyerw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kwuzgsso.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lxgqbawk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ymawtsqo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3siiiqgjf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jvhkucuo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3onmapnyw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uxstbacw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvgbtasf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xmrlzaxx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lxylpqdu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aksikqgf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3djfxxhqu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eehonfrb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xpfimjfm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdnymkqk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hlxcwbzy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qkmvvvxa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wjptyvza.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3niqazbsj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cjiycqnh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sexcbjxb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kxhqwasz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vrczirmt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kkodacli.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zopwyevz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3klofczyd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3grkkpvrn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsdezrj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rrvbljta.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bglmgmnu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pqagfqmq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xknnfklg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zampcazi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fgupplnt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ooyafsba.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kssddgzg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3trsrcldw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lwoxnuoi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bmsgibtv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rzvmyenp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rtcjzyhr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bqqjjosq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tnxaqifh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mfrtytdb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vwqvqvet.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3idbzqaqs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntqmnugp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dwztlhsn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pibvnqnt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3euybuuwb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gmspsosh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ghuueprd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmumjbwo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3orxopdix.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3edhlwwtl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ynkblehv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wtfovvtf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3esbxjkrd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3btobbgsi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ydgpzoal.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dunaxpun.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3egqdpukh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3behcborx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rxxazoom.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rbebfepk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3auhdhcqh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fgysbzfu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bmchmrvg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mewnsbie.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uylxlfbk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mzapctgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arkrpebs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tkwhtguu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fklhqfrq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mqbpjrbs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xqqdvvgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hhjamjin.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wkctsspm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gyjqimuc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3eeemojub.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vjesvceq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ernkljyb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kievlnwb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cemccsfd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqopesy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xvkynvbj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3apduzcjz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fgfyfnba.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqybsrqq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mnowfzfk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zfxkdyii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jqvppsib.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xdwopvte.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xgavpsml.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qonnzlck.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xvfrenoi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aamojsck.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zzbcxrsm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wshwutyw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gendhann.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bhesylfg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cgwcbxxs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hzhnkuob.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3uijggnbp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ihxvqabi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypwazpxt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yljpcbpp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hfvjtxal.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qyyrfskx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3uhbeybit.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rabzfbcr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxdtvsz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tkoizcrv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xcqodekd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vskizuxu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gyowwkiw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xhfwjlbv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rxbcudxl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkieihfs.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gspkirfk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jpjewboh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3trkzzchc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3shuepczx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nopbeege.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lhyymixc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ddnpeikl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hosmmigx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bprjxxpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qksokjeo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfgyrmta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsrvvvfv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rlzaknwe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3errmwerf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qhkhsuqd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xhhobbgk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gnnrefda.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iebnzahu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ctlobjxb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dgzcpkex.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tncamcbb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rlyulsky.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3chnvvigz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqxmpx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3sjhfwitl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3biitmtyh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3smtcsvix.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kntojlad.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skvuyhdm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oyhwmrlt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kdipqhzk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3sqaapryk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rsjmkxwe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eaujdapi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qebgaukg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3sjybwcht.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3snegnxgf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cgrzmdww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dsxtjigv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rmjzomfd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qzlcwmtj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iworprec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xxpsbgfa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3iaxelwer.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3panjdiik.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iarbsrgz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kctgbjry.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mewrlnty.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kihschca.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wawuwfhv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3llaupgdj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jtlvwpeh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqaokfrz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jpoplbnv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ouecwpup.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jmusnmaa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dnyonggx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zdkwzdle.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lmtbutkn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hokeomkx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eywkzbjj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3npnqednv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjudegtf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezibtkej.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oegbmaqu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lntcyoog.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vdgeydld.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ntbbupzc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xoixlcjx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ulcewdko.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3assermju.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqpifxz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3efklqwvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qmcxjrfo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jsyaidcw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mjyigcki.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3smkttrqc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bibuhfjm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3pxgwquex.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3goxbdbxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nntgafyp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3skhhuyhy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rarhbfak.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3urzxvico.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsksnkxp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3asqoosvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjyufxtg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3uwcvlfaf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3btxcitxu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fzkyipid.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gxmxbljr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3erxqnsin.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3emuxhnwf.html

);
来源：http://www.52xcode.cn/Article/details/gt3owknmtwz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3cvvupvrc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dqqxznsc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3twfxujjs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3skzzbhqv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3doaezdao.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vwnqoewo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kwsfdqyo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ymhesaar.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bdpxzxid.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwaypgcw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qetaxfny.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hzgikwkb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cknchlkx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lnkrjzvo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3otcwoiar.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ytqbqmxe.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mezhscfv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fmajrvat.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ozcxrllk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cwfpebdd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zkhfpqho.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zbkmsovh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hxxokrqe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ipkjgqtz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mkhjsyrl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uywofrwp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vyklmfok.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wmkiyblh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eqeonwzr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mvyoesyz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wtfwtqcr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3scgcdgol.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cpdauvgg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mikwpguu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slaynbig.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fwvtlrzr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iybinxkk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xbcbxngy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yjcjihfp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wuphmvyx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3geyjifcq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdeinkbm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3afoweexb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iuzhdfaz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znifhwut.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ghckslqq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lalmyfir.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fthorilc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bjflctth.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fzkgckso.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kxcdqljb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gstjwtwi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxmrckqn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xkwqmnhm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3psmvcnrj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3czhsopax.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykcffpma.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3uuilzugw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hceprenx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wjnbgbdg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qxtxvxhr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yyflzjgt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kjzhgqcr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fqpzghye.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gjefwosz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zduppjoc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rjuobscs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptmjwocv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iuczcdke.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3coqjwody.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pygmyhxt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mpbvhocx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ynpkrvxa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rtvkxxwc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mkdhoskj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pzoknuyx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ruwtjyjj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vhwjxvzt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rgivelsn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lvetsdef.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ekplstbb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cvgctoln.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jubygjik.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tpavzhok.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cqrhswmb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vegishtj.html


<!-- 参考信息 -->