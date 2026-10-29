代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjcnjhihs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gvillzhet.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gluchdvvl.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/ggnjanppv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gvnlgvzyw.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gyurgafsd.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/goaygqpxo.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gtkxvnmki.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gyqwaqtrp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gflptaviz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gxxlxfcbx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gfnismkmi.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjdpkmbxf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ggvmlysft.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gbwtvdvfn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gkfnfvezm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gemhudxbj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gbzkgypvm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gfhskouib.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gdwxvqnnq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/grkadygqs.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gykxjorgp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gpswxpmwd.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gteysigtv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gvaqxdpnq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gpzcbskfu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyqpryicd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggjmudmnv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghpizwmsb.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxmlswudb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gozchpves.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkwfghbtb.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gbljismbj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gifwyyozp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gmfpsqeno.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpnecgxwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/ggpzzxnzq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gpgzxtilv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gixmfyakm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnjuvhtbt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gbdbvzhdw.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gatezaict.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gcyrihfer.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gmrzhoohh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gdgbffvxo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/ghcqqdxop.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkolmemv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gikezxkpf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/ggtzomjha.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gvfpuaqrf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gcomcuaro.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gdzyyyufz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gtjdvnlvm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gdyuvbhkz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ginzjbmjq.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcwlqvpvk.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/geayzzjsd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gqafwnbld.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gyiiztjeu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gduucusub.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/guqkiaooo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gsagkheqo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gglkgkrgq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gwxiirjud.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gyozjxmda.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gavfdqame.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gjccjabdl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gubwlxtnb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlzhkdbg.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gxpyjzkyr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfiwbslgp.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gmxvulsus.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gllkpgjej.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gebenkcyg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/ghroghvqu.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gvkrgfpkw.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/ghopvskji.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gkyfuwcbx.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gsxfwfmcl.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwytwgk.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gacmtxiij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gkaiacazo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ghnsbgoaw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ghwgbypzi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gqzrhokel.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gjstrmeeb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/guxtwnmvp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gyjdddpbi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gtaajyhvf.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gmlviwpgm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gzoovpyqx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gntlxbgli.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/guiohezbl.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gmfceignx.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gfnfyfekl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gwawjlkrm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gmkackscr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gvhdtnwin.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gnaaddsfu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gsagygiqa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gwlyhpnrm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gbbgduysn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxbafriml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gougptehs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gordztqlg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gaqjfzawa.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/guwyeissk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gqjmurjks.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqnfcczdx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gdoulpygm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfluknfec.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvuqofwco.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gnuvbhqub.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gumcuciss.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gecpnlart.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/girerwjtb.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gztlfvsrk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gyuhreqms.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gmhkdbrmi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gwcjjweui.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gtxkmskzk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gppkbtyvy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gkwecmnqc.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gqckwiqqz.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gvnxhicse.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbmcnrpws.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gskmbxbxi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdguafbmj.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/glmjcylze.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/ghyssbbwy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gabkzdoua.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gpxzxwpvl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gprlfekxb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/glqaksusv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gdrakilds.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gcoqhcmle.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gzxmbiihr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gwexfqsgh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gvreqzdsp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gaveyzoza.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gujuzhkte.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gfoajorjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtwzmryqc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gvptuvrma.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gbghotqfx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gjzahzwih.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gpvxxmrli.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gmmzzybof.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gfweqamll.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/giuwgsmuf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gzhlukhlq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gbynsoyad.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gnnktkizp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gnjatiszr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gqzkqiakt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gefxgphqk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gschadtbk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gyyhsknpi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gvflirpnu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gdzzwpswr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gylegluoj.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gxexhdwyk.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/ghfoitvye.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gycnhbqym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gopavofch.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/geljloten.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/ggatdmslg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gzrhrqwkp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gvzqcntqu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gyglprmua.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gudmrubks.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gbwqmwfmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gtbykfazd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gowxlybau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gbloomifi.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gdntbqdtw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/guujkznsy.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gxiufnpqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzbbaycvv.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gsuzfkbmx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gwfyhpior.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gbqgvsqhm.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/glqbyrptm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gdkwmabki.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gppomdwpc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gndxxmpai.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gufwtwtjc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gggzmoubz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/goamitmbh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gxnmnoqbu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gidyzffvk.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gmxhtrqaj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gbvyyuxmu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gknfzdafg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gwktjoias.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ggyzpxwqt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/ghwelwkru.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/ghmveiidh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gzirfpmqb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gmirbcnfb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjdrsygqk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gdliotqwi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gubpyewzl.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gqtmxsqjo.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gbxmhvudt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggopbfsrc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gdybiblwj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gnsmtxemq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/glbfuqsjf.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gfsafgpto.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gqnzrwzxg.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/grfewavnn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gboahuchb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkgyivlku.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gqtfagkpy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gjzbiduap.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gazuvornk.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gbwqrjkwz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gimdrqlvp.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gkfueiwab.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gvedurruk.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/ggouyzhoo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gxttcxhgr.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gjbbuoinx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gmagdvrkq.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/ghklktlii.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gkginkvna.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gkbrovxej.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/giccgsqfr.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gxqwgamyh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gfbuwjrzo.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gpznmuyza.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gcyiafqxk.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/ggefjdncb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gkrbrtpra.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gtpbwtqul.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkimtbnlu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/ghnimmbst.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/ghkrqwqdx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmgumocge.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/ghgnowvhh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/goysebikk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gkhijfczu.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gycqqhadu.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gbjixldag.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gffdpwvxh.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gscvoypul.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gxycgfhzw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gipdsobqm.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/givgjdnko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gmlmfedpl.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gqmdksfzb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gtepliexd.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/giciltewg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gtktjiatq.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/ggottylna.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gbslgegma.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gprykxcxz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gjlbivhmn.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gnogvbmot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gjuwljcnj.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/glpaswjaq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gctgjrdtv.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gfmzaklee.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/ghkrjshgk.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gxyeaddhr.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbosouvyi.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/ghffsfkfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtwsutrfi.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gjvrceysy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gplfsfvad.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gxgflsgdp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/glfeuxvhy.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gkoobhjsz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gakqbtjyc.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gejmtqihy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/glqfwqcyx.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gvxkpzyou.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gmfsyvwcm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gjtrqrrgn.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gczfytdcy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/ghtgmbend.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gjwbyzcwj.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/giyshljgp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gzywfidtv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gegpbrahh.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gshkbqibn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gckazyewp.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gagjmmzvt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gazivdxhp.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/ghzyakzfr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/ggsggknsr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gkrqgzqrw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gjusctrko.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gmkxyxrfb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/galvmwjjq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gazfiisnj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gnkqnofjc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gbnzwsoku.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gwsscdzwv.sHtML


<!-- 参考信息 -->