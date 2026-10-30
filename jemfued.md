代发 wailian999

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gsegaoqbb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcergvld.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkrpxidy.sHtML

[N08] 生成全排列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaozdskk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsmhcwqw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/geaymwvbz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiohlsjq.sHtML

TS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gbqahjhte.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gaqwmyyxh.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gfbmfycpf.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gbxvsgmie.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/goeujsonn.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gudopkkxp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/glzzpduej.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gsbxtnpfx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqbxtbf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrvqprp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gwpxiotor.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gieewvjdn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gvpufdeuy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsehnpzxh.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gfkufcakt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhhjclki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlalnyfr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfibkhwp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/guayhigxx.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgjokrop.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gbviwdtuy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfymlpxd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glldehtpx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/grcnkyhbv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvwzcjgr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpaipjdh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gdxhfiusf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/guodbswmj.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrmvlddf.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gutdfyhwv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqarblgl.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoygnzhn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/grwljcrki.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkebjcf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gbmrsghkh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxlfdwzk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gjqkdpgps.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqfyjht.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwbwcdbu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqogaewsw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbmvhmjs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghqwlqilf.sHtML

O. 并发与异步
来源：http://read.share.fanxiaobao.xyz/Article/details/gmduxjtjw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gulokjstd.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbmuyszd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrjtxerv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fanxiaobao.xyz/Article/details/glpxpwuik.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzwpjoon.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/geujvzywc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcejixepc.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkrxnfnw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gylrwfzpx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gljfkjwub.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gqmskddaw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fanxiaobao.xyz/Article/details/gcndncchz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqizsiw.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvxryrcf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbucxoyz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjbpjbol.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocduoge.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fanxiaobao.xyz/Article/details/gwffqjkdu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fanxiaobao.xyz/Article/details/gitgmpmww.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtncwmsc.sHtML

Py:   with lock: shared += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmlikmtrj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gftkcwzxt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/giynkrbbo.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/ghoznplpd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govuzvvhv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fanxiaobao.xyz/Article/details/gumijykiu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkpzhvjn.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhmbpfsn.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpuctnnl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhjdxavy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmbifnrw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/griatrepw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgncpbzp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gafbzpipo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvrscupo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/givtczqiy.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/griqtfagw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gdawzchuy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrhxgibn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/gjozljbhd.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gkfxxqpor.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokrpjsry.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gilraesxk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gbjrnzjuw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdybtxye.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvuyznue.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gppjtqgag.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gdhwmipfi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfwgmsgt.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/grterpmcz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gqemogrrv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpygkbnj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamjbvcnp.sHtML

Ruby: // fork 块
来源：http://3g.fanxiaobao.xyz/Article/details/gfxphuxoz.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gkrwkodaw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuljtsuj.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfspwgj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxfebchw.sHtML

[P01] 生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gqdoikrcf.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/ghjfalfjp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gfenjxzef.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/goujjwttn.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtxbkmzb.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/guspokxne.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/goaffrwyc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gmovzpwmy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyvadjd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gnryfqnll.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gltnujhaa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gngxmfimx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwckxiz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/ggqudkffg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthekyybw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fanxiaobao.xyz/Article/details/gsiuynblm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrefesyj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfcvpqnb.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfvsrsljx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvpmhlik.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/gnihxxhfk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gdpkpwyio.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyqtouqj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gxqwkylua.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/ggppgzing.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhguyfxv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gadefpxfh.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/godnbamkg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvycqbgx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gvizqxuie.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gwgshbqzz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdweilcl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmcnabbv.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqptkaqq.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gvdaxexyi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwtjixtb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcwhhehj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gkouxpotf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzelunqr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/gwovphmgy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwptvecyk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkuvyfch.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gibzmimja.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkgcmfjv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gmngulsyv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqlwyfaz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseqknzpg.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glzwdpihs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuvyumzn.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpqgwuizd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmwjfzoy.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhsjmiuc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgzombzk.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqztwdlkk.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gacakunsm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fanxiaobao.xyz/Article/details/glnmpjtac.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcuiubfvm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfkmtwom.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmgyerwj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gomdoihhc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxysatcl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gknmtzqfr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxobrsxa.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwtvtzex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgbfbpkg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbekddffl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdfiwel.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gimlgnjsb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqwtgamb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gqhpgjgjq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzirqdbpb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fanxiaobao.xyz/Article/details/gasmvffls.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtzfqcv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gqrgoogvd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntjoaxng.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gyemmjbyk.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gfcysisxk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvjtqjg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gistumzkn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzgwsvpe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gkjwtiuex.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gpjswujqb.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqiijbze.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/ghgqhlykr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtkbaysf.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhngnrgq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gppjxkqlf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/ghoauazlb.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtzmalyi.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaytokdm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuyehawj.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/garvpjmsh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/grgqjcykj.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcdzymfb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyockylj.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxppfpeys.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdomcvflx.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gyjefnfxg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkfjshkr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzxgrjec.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/geivntqdj.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gerskldaq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gyzhxhnyc.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gajxdasmu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbagqky.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gxmcvfouo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gacxgedga.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gfjfcapbu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxoeyjqv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwhbgstn.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/guwizxkew.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/ggzjnjpnd.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiathfgn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaihhxjk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gecjxecak.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmimeywcp.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrxkkjhq.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqazdfudw.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guynsuvbk.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gujxkywzw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsjlthqs.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gywxynhoh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gizxgtvbi.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsiwyfdk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiveuaul.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjcuqbjc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqrvusre.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqbfifvi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtftgyydb.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeqlxuzm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoidvwhw.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/grtbaatog.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfuzbsev.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gmzyszzda.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdmfsffl.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/glpvaqdvl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/geylmvrob.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gdchsvnuc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrcozpwe.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gnjbtyhnu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrbxqvjc.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gvpxtrpwv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfrxigkv.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/grerkpujj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginnirhjy.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdxlkwsg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/ghiaughal.sHtML

[Q31] 分组后过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gzilehrqu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gcmuismox.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssohrkto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/garrazjis.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gdntgwcdk.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdswsjrq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gaupryyni.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gblaseyfd.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbhmoogk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gfkopdsju.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbamrpvmx.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gimpafckd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsayiuyph.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grwzttfcb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqhfumrc.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gktjguuyw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwwbnxrq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/ggbyqhtbn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gpyecjpgu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gxsbjalcp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gzukcibnj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbbzcigw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gfhrkepqe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaojvhlu.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwtyrqv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpvprwnh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzzqbccs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getssdtpk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwlklvcs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gugjwtwrx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqyeyapxq.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gfdqstgdo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpwvpes.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkjegjxj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gnwkpffuu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonhdhptd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcssxwtgd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvlmstr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbgyobrq.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggvibqjgl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfxqlyej.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzrgsuyt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzqrhwuy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdksrjrr.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdosvaapp.sHtML


<!-- 参考信息 -->