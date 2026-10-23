代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lblngfeu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kjadrztg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gzeglgbw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zbruvgak.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3upckyppa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3unncvmvf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3siozhdbe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zgxhscxo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fzwkeypo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xjmizfne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rilmcpod.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xzpzprul.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hurvwiag.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uuhgpgtl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yjgtwcnp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mhjigoma.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mtbxyiel.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jwxwtkcl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vozeckui.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xehsjsbw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xunzwlqa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3prvfdovk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3owoywmkv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dtttuede.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vcalobrw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hayamndx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhrnyidz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3icmkjmkm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zixzmicv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ciskhlfj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rqstflzc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ingjmptk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tympcqqu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3avokjsze.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bbsjyfkq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlzqzkrf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jyjggjql.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vmpqlmqj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kakttrty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qtlevbuf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rnnclvou.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3giwezxcz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fbsbwnzc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uglwjltq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kmbdarms.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3toblmhby.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cnxxaxev.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3monhxxyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwrefwf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkaykjnd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mechptaw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3biofccya.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mpxnshgg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jxihxntj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bhfgrxmt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztavzwbg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xcadtesc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3esqrpoqn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ibqpfvey.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aqxdbihy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3djjxpagl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3unjmassf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3biknwfbq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gnncpcou.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tczbitpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uuenkugu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3abvmlhhz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ndziitxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baledeft.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zbpouxpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyrudlkk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kchveaij.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jdydnlew.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3scmwddyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jrooqamw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qmbbigtz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xvpluecv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ieynzpev.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wgpedhmk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lpdsevsc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xwmymwjh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dkwjlqqj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ckgqmaea.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oazfoptn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3omlxridq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dsgbchsj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vmvhbwqt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3byslbpxn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3eobhleip.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tvdgwhtn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjmwvsse.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qpbkqxwv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ribpfeus.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wjodcfkk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gluzlcnc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gcailujj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3katouhlv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsdufxjl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ztadjljp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jobkpjwj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3buygqlgi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3enfxiwaz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lxkkypmq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ebevqrzw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kvbzkiop.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3sakiutej.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3otkcxqgf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zsdrwzix.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3imurvfnz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nnayecpd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3srzdcrxl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3doezqzri.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ipakpnfi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3crsjnygv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcizkdk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvltemmx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gcwujtnj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nprfejgj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qwcyihby.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3aotfehrn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vgbtcpfj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ehfzqiew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3uoxqoxnh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rjrxnbge.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3iyfulmbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uybxmguz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbiqbgxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xibvakmv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cxbwnbaq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3yukwmuje.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rsaxlkeb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yqkfpfxk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3othgxxfu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3naxngegk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3obidjjkx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jtmyejkf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jsvxuecg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3txwowuvq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lfhweoop.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3utnwrtjh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ubqabpav.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bwisytyp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3evaapykn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ebtqwcet.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xirvmalg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dvvproeh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3khjyeuts.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rdztnzzj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3furyzecf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ygnnkdgb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3javhojjl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcsrfyd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3slvomhal.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3drsnnjmh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3skceafna.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nldqyxep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3whpxhbiq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eddxzxea.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nfbnuypl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yspiabbo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kiebrpiz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgivixl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ydgbmeqx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jrivgbnk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3healnlwk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3alzedlzz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ljqpyjct.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ypucmyxq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cxitulii.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qzfsgzpx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3berysnhd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3doissqtz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rqqimdrj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nifskrju.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3buiuygfl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lucuyoeu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rlrqrkts.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnwzuikx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsinwqql.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jspkuuxh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xivsvula.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyvcqkom.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nhrijfmv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3pjmsadul.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3npnrxyeq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aiuyblac.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oqxilgbv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psgcomqh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bekjopxm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hddqmcmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lqevbkoy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tuwgutkq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xsbjynwi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kcrwgrox.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dhiqdwyu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjplisth.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qygaihea.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cyvbgyuu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3eqydluoe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ijijjlff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvyfllid.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3olbueeqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzbhwlgy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lyruttdl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dplxeekg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iwgwnlzs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jufopmdw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3uecoddkq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tumgbfhx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3llodiixq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tjgexpbd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xpkqccqq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3eumeaygw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pbjprrsm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fhcqaepl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3opuwfrya.html

);
来源：http://www.52xcode.cn/Article/details/gt3jxupgcig.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tpgdmljk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rqinnkcx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhobilnf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wgkbnyye.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eisiwcdl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3uhzscxqd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dchskvyo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3edgobmjf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jbwfjsda.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3glkfibdp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kjkrdvry.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wrkmsebk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3hnhnltzu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oihahtqd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lmcltwkx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ioiekwoq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fxggssvz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgmwhyow.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jjaofeew.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dhdwwbuu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gtbdmwkk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lrawgdwa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3poscpqrw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ejhltynj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pymunegn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tdhhebyc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zrxxjbvm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pytekmyg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lxkppiji.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bikqabik.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3agvozarf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kuhoiqxg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fxnehvqx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wugkhpky.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3blaaoves.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hzwedzfi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dqwhkigo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kiimraqb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3awtyitoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gzwulcyh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hktuzbga.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cerkivqw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bxmnkvbk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qwruaqrx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tgyxhpgy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uhvqjprc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3gbmemeax.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xtxuzbvp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3oktnlkyz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctszbkrf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bzwabntm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yxdybzbx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qgbrmaov.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rfmvftnh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hdnholht.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxuenqjp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yiziudol.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tptpynno.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lcbviaxa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3awgnlktw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydwlpxwl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3axcagquv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ejeapwbk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zpmsbfcz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fmevjazi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ljojkced.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3pskvfbhy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3rvlikzon.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxnrlrif.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lxklolgz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ktfyxqoe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xltwcbgc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ljralxof.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3qepchvmu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cunkfcnn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lngxfuos.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fefvsyjq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dglhpygi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qpwgxvcb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oxbsxwgg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ifmcnloe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qnjoarfk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qnqcpcoc.html


<!-- 参考信息 -->