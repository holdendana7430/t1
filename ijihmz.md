代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yfmhdfus.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ocoepjoq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ghcgzuvq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3suhvrmtx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nijpqxys.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3diquxdrg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fkwniaeg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pxeebrch.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nphfjefg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbitqrud.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3upayhdrk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tmmyejyj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3icziygtt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ricrvfrs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mojmrvmw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fmxfrozs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3afanjikr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3epnykvbo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lzsmgraq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ymfpmywv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zdpotaul.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3toanvizu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3lpnopgto.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3edatylik.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dugjwile.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3arviqopd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cntcfvre.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sspginap.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zpwkakch.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3totplmfa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bfgrhltj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qxgnxbjn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hobbhlzt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wmmvjqsb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbtiexis.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iatxqurb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hbyhufnw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qghrfmds.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3skvmxlwk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ehhekaxy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vophcceu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mrvpwmzx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yrnpkhgi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrfnuzej.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nflnhsdj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dboiqhuz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymentedc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pfkcjyjc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3anmlhxrq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfyrfkk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3shmuwfgi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ejxxhtek.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlqmfyvb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vjlbiqls.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jqfoybmc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3trmvrscv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zbooggrh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3udrtlect.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gyatcjwr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uqokqbjv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lpwfbutv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3owaglukn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oizdjbii.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3omkaqxbp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qadhhcuz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zkmqthec.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uvizwqrl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cjaqmmwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pluolbat.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3uejrrccs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhwolrmx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hukvzpgn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3thzudmmj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vtlegnhm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hgbyxopa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rlwmgrbd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sgghipyg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3kbdzaxpr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fjmqtccw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kwlfjajx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3amebexsm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmmpivf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qdiletax.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ysagozkh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wntputsi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpewgdgo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fwycuztw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3npkpggjt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3iwforgxr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ocazgbly.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qbaradef.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nfzpcdcy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zjteukex.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uelifaiw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3domjaugt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qvrnugbv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3isuebqlo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zaqtfzrr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uksywsrk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jqyidgmc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lzxyuqrj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtriqamc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tqszincj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vrsxxvfy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fuanahlq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ujmoektk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zwaiuiab.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3epytnatf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vitycmmp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cgsbukxo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlsesth.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zsukjdvt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3mqmeutxn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3idstwgsv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gfceotkf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rygmkfeb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pssnjctc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3maebhlco.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bqletzuy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lqxnfcjs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rpsvbaoo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3aopmxpay.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jnfwhmoo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nfpxdzvi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ezovqbeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qahspghu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwomdwcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbmghxht.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hhwuewax.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ujxkmakn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dolgfihy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3obuczaii.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sughylos.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ridxovaa.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3afactpzm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3acwpsatu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zizgxxek.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mbnqkfno.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3axrmbjul.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fschhdta.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cgjyomqb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3znyjtyug.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dffgsijr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fxemjcoj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnquzzhz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3abpibcer.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eihbifdb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jxyzhllz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3imiazxxc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qjydgshk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3otmjlmwk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vzxcabtc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qqfkesnt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3utaubwqn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mwnoyxlw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pydkcmty.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gkcwyizn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fifgkedp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mjedexxs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oqtpukqn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wrgnvghe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pldwovez.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qyndrxml.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fjdellhi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tuysvyzp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yferkeqo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sjnzylkp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oxbiwkba.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iftuvyyg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vglwlstt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3buqfjqen.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nrzogara.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yxnbhcvx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ymlnbgfl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ozkttydh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvhszsot.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gvhzqwdy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojkrervj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znmokjlb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nalvpxru.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wijqgkyh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vcpfothy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3eqkfrbmt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3evmznbgv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kiyjwyld.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mjxoidei.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eokdciay.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdaqptsb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bgghklxx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zpwuimby.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vjvsdhtr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nzndlrvy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ehnmyshx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kchwfucu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3eolnyrwv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3whlunwlm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nooigxdz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gbrtjzvg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hartiadg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jysghgsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrkmxrgn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3efnuaxhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohgtdotg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yremfxdu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3aygnyvof.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3srayomqy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lpmetmmc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wrcwllec.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3isanfppp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3epakpfhy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zlpybcxt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jgbytxin.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xxpilujn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pabfozua.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fvvdvffj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pvjldfzb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hhmbhwns.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ibrncfjl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kyksurjd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtojkmay.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kciemvdb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fmuqphek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ilvjajaj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vfrysacc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kqjalxdx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ilzvyvop.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yapdzyrt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3twaoashb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nemebyrm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yhvzmtfc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bmwdenbc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cadrsuil.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hngeorrh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ruokhkks.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vmcwrgmw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ydkfdsoy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pcvjksib.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tqbtadtk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wykkbtyf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cptntkpj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3azxckrif.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3prfahywm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ataopjvp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rjyrkdku.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvthoubn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zqaoqnve.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shrcieej.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lxcwtnwd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kgabltba.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3naerclhi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jtzpwnxx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jlfdvcpc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jpbfkkpz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hypatwya.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3krlbclrl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bavqpgsq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cspzclhm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3htihkldg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lmlcodqg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3augqbipz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jyrwlhze.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hevszuul.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jymtypjm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3highkyas.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjvhxv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ebbexdko.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ravdvztg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3epzgjfbz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ziqznwys.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3psfmhfhj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fsciojkh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qtmbzrwj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3udktvyou.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dubfudmo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uaswqfkg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ryhrnngw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ntkktvnc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptroegwr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vclvkles.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pyyaniep.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fnaohbyi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qgddgvlq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3fswfdvhg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wraaxzhx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3luooeono.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3khrfvjgs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ggpaactc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3touodbsv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tfqxjxmj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zemqwpck.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zccwseqy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kaqitbkl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qbrebiak.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lnxqhuom.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dxihxdwn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vptbxqxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rfqedunh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lkpemfdi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tobtzepp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jxsvjuce.html


<!-- 参考信息 -->