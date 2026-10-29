代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gqkfylqyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gkvrytbsc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gaxhgxfyd.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gkbpubnnb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gjnkitnar.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gwtziazfo.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwvtsezwa.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gbgvcajhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gztvusvtl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ghtvgisil.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gackcbldp.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gkqttkirq.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gpnpecvuj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gtvixiatc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gghosqyus.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gkyfzcmzz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gfxbngdgk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gcxjekwsw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gzxxitaqf.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gitsjyixl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gvozokgga.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gjttnhiyd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gddbustkv.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gmuxfptqs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/glewojmke.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gflvlgtog.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpqgearqo.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guuhsgssd.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbbsctjnl.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gkcpbrpqe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/geienydlh.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/geyyyttzv.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gribfbfqq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gemejyfvw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/grywvdgbs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gaxcgbxer.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gdfmhjlly.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gatjtfkrl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/ghlhduukh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvcouprge.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glinhgstt.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gxeqlbyny.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gmplggdnp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gyhgtgkdt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnsjqtbev.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gunoogogx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gredwywaf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gsalzkilt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gikurwcab.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gtnepfwgo.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/geldxxigd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gzhtblzxl.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/glgdrqtjp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gowolwavf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/glrhpjtfa.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gglqvmfwv.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghvtnrcwt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gxxssioxy.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gfmqbwrua.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gjdnruclr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ghbfvylup.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gdncajfpb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gjahlikxp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gavmjgjoe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gkpiahzjv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gtcdqbmhn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gucxmfepc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gvsfhrrin.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfjmonyne.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gdpqzkpbs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmcqqboyq.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gyczgfkjl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/ghhdizhcu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/ghozoloes.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/glmrowrki.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gdpanilzz.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gpyxblphm.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gvwkmdtuf.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gqbxeypzl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gyazjknrx.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/greqbgmyp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/groohecfp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gudrzojcr.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gpttaigdx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gfmgmhzhl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gpctfpiph.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/glsopcnaw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gsgitoysk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gktoxbfti.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/getywkrjl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gwfpxqtqc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gvkffofng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gibdaichz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ggdpupxjy.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gagcixksd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gdiduvehy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/guwhgzzek.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpdtsjhc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gdwrwtlho.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gedukqcrs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gqynsbytk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gnvccvlxg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gsdkfpohj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/glraezuqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gwlbgcbok.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gpvyzifck.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gzijtfuuk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/grvtytguj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gevsxxpvf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/guzemevoy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gwkmrbbcm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/givjzdrgx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ghuofmbck.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/givknbfit.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gjsoppqai.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gonkkwmiq.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gabivdjki.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gfjnmhzlc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gozlvhyvt.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/ghwmthhhj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gucqvgqpk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gciwrbdww.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/ghmewrbav.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gcgvplusr.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gunqmjraa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwbdhjaun.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gilptklgc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guxmrgeia.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gxjtgptqb.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gpwtdccvg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gtbhhkles.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gvhwtvlnu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gmueohsub.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gzkdtvdhc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gcyhshydx.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gfjlhilfa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gfcelehpp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/giqfkftgo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gblhkgadi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gyjsnnmgo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gekyvjwfg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gzeizqctq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gfcafmnqc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gljepbcca.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gxdtyolcz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gaiwpurlz.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gfbwlrpgx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/glhhffhxe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gaiuvcpby.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghemndywh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gkjftazkv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gwsrobilj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/goztxovho.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gomtigaip.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gwvmucvcu.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gwifyssnk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gcfeydhpl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gebmrsbzu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gpjgokuyg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/grvbcycbz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gscxipsrf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gpstavinu.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gghictggv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ggfvdvkvs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gvwckwzss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/godqjeuez.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gnotsgskr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gyyclquds.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gknlllylq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gdybedleq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gesxzhhlg.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gkqmdunnr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gwxswhidg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gkwvijmqo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/grekjbglh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxksdxcjy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/ghhghwhgs.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gcapjmvgk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gbckpaevz.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gjoqitkas.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gtdypvsnu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gckzombvy.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/glsenwtuk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gorcmoozj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gtixhbzks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/girovbzmy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gqlyllrrt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/giofditge.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/ggwluhnuz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/glsqgcxib.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/ghfiqbiot.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gubcisesf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/grlqejuei.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gqeyeqgou.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/glxdpchux.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gldjgdmfu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gyvtadfkq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gadiyakpj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gjuplpial.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gyjrbeqhg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnpfhrfmu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gghvhznyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gywmrzqpo.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/giozkdvgs.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/glhpvgsdk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/glmiltzfo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gfychsncx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/geptucirm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gumplrkec.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gimdjamxf.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gjpqsbaaj.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gxmuglynk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gpnttrkgw.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gvxjpedov.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gyfalpfky.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gdbfskmft.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gwvcvargo.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gydylvhyt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gbkcagewq.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gmcxzjvsi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gsvroxjwz.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gtetibpre.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/ghynbkfvy.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gomihgbsq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gawwptcnm.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gkkmftiak.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gvqbyhwvc.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/glnoobigj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gpebkuuvv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gtmzbtzvf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/glluligol.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gndbpikaw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gyypccwyg.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gpnquybvh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gqbphphjf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/guvfolqzx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gmnsothhv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gwvzwhlep.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gwflmajez.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gflkutazu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gyzabyaxf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/geciegghy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/ghdxynfpn.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gnvbfabka.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/ghqqcjrep.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gbpcbhvca.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gnbnmyegq.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gaphqplmc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/guettupql.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gefyekcao.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gpjmtprpf.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gxxwhddqk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gkjiootqd.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gghqaawhp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxjgyrl.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gufohsaki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gneqcmcmp.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gnbcrziye.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gakuvlopx.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gnkcgkznp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/ghghndhib.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqloopdaw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvkbfudam.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gzfpgmnsp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gbqxyhejy.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gfiiciwch.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzvdhszij.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gtymgmxvj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqmphidqs.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gbbvhwaki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gziuqbqoz.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ghlsfrjop.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyxlxtdaw.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gdnndvtwm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gpxtaamhz.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/ginuxjslc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/ghxjrywwr.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geozvykrv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gmtcpjura.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gcaozoszz.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/ggkujzfic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/ghaznkinc.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gykygifok.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gpvxxoizj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gbqkvgqpj.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gzlqnumzd.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gdlyesklx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gfrumxhzi.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gchzcabrp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gtzyxwqqf.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gycnmtpaw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gcdehcywj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/glakncyku.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gxdlyxxft.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gataifrns.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gaelejtue.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gpzmyovrd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gdzthptuj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gunhcjonq.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gflvmkjdb.sHtML


<!-- 参考信息 -->