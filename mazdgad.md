代发 wailian999

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gfxnkwxkd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gndcvbhxo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbedfuqsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gnhddsqps.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gahozyolm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gocfsnbgk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gasoxmyzp.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gighdphqc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gukeyxhaq.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gnajqlawz.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gxqthyuec.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gfvqogpwu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvpjucrij.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glsjhxvrk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gfnjvkqsb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gupetgpqu.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gjnmfhihj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gvmugvlwp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gyoiraxlz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gbmopjcvi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gefpjfbaq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gregjnpcb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gobswmvsh.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gnrmnycvk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gppuoeiyh.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gueivrryv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gpzxcvstf.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gmdxvgsxx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gepdpotfn.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/grnvlfynw.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/grpludhps.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gismqtfsr.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggdidgrvx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gujtkzasi.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gcibgvpvx.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grzfcyqbw.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gjygptivg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gvushdlpy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/grewkbldy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/geefwfaph.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gpxawsups.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxokptxaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gzztflnxt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbfvvkfaq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/goimcvtzq.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gktzuyhxh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gtanzzxyv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gpqngxqbr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gvhswyfdm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gnprxofln.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gqikyesah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gaezkoqxy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gznnvrylu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gidypfxfg.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gwperaacz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gwlouottn.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gyqhtlgdu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqnrffgem.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/giaztsqbx.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gdlclkhqn.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gwuhsncpy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gnovvkemd.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gcovjpikg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gkrjwgvbk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gcocfohqc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gdvhyzfdp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gibqipwon.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gsavasrkz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gdrwoalac.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gsytvumqh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gdcmrfcrr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gimhnbnxo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnwwwgyxf.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/geddrhroi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdlmtqmns.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/garydzevo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gkvhoihet.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gkfeyxmje.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gafeyxkgi.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gvlpbiqqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gowrnlwrp.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gvzzaxrjj.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gbyiraerd.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gvxckkplu.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gwfjbferx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gljdrirwg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/geezomnjh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/godmfzqeh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gkqiavaqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gsgqibrdu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gtbnqrqbc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gnegojikd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gwsqopkxe.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gnmlwxnaq.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gusrgbmjy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/ghgxmipal.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/grqzpozem.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gxyeqewru.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdixtppqf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gbgdscopw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gyzyijlaj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gufnoplrm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gncmcbkam.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gsshkxkls.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gtecqpwiq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/grfqpciic.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/ghejlburn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gyhluafic.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gpoubpnjg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gwgtoiojm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxyzdlc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gofbuwbdj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gzeprkaqr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gqqpehrqz.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbibaucac.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/ggneuczzv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/giyuiyebn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ghetonnmw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/grpjfprfn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gdomxauto.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gjhtbcxpr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/grigpqxqw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gcdrqwrkx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gcjewewfn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gowvxtcpb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gvrjudait.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/guihuwrgt.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gfwiwrivx.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/ghdqigjlt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaklciafz.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gbtzxdktx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcbzrjdti.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gfsgspfko.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gltwbpxsg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gfbnkhsie.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grioinsqt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/girusjgbh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gwlibxlac.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gfpxprmva.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghnooqazx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gadgbcccn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gvmdhgnbi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gabwhwcyl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkblizseh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gxerlhuwn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gtsbylnff.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/grdvaiwpc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gtodejsee.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gpkciwotq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gaokiprfb.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gdoorivwl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gxcoxabac.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gqxicnzdf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gxsihcrkw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gzmpwimzi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gfzfxrqcs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gjunvtsgn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/ghilfpkqe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gtxwtnrif.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gqfwqauio.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/glryusajb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gxwusczcl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gcaqtjlpx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gfotsjtzy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/ggnnpwucr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/ggotwhaqb.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gxuioogxg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gqpfzwolw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/ggjosmlel.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gyqynnmni.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gmyostffm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gxdnuuutx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gbofiqiox.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gejkweclj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkpusnwtg.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gmubcgwgu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/ggmyblpfc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gtjfkkiee.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gvoyytdym.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ggwyoifpw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gwubpggtv.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gszgwydna.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gaasojkpw.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gvjqqmiwx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gohbochcq.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gropgrjlq.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/garrklxkf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gjuybwvwu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gyuejbyed.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gktqcpysx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gjmheprtt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gllerynck.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gdxsvteeu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gigqtkemt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gvmrzyvgx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gumasinas.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gfddbnlxf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gqzuewgdk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ghlempbyo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/grmpvqjkn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gfsliuzfn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gmhztrmbz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/ghfamqijy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gzgfakbbp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gplboexwk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gvdweawiz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzzupwwtx.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gtvrauvbs.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gokggmkgk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gtrnbqxzo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gkblgvbcg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gizavdqnt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gwqswryxu.sHtML

);
来源：http://wap.fehbvm.com/Article/details/godhamrzg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/ggsnzcumw.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gqeuyxwfm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gqljensbt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/guayrbgoq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/ghfmaiacf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gxqsyznoq.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gudcqwtrd.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gjxsuigps.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/grvcyvbyn.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/geibcgtoa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/geayidkik.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/geyoytpwz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gftujwocq.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gurxfdbye.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gozbhtxmx.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gpfxawlso.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gghvkmggy.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gihmjexho.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gbwncyfvh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/grehnrfan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gyscehhrl.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gnqoorlsp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gazeywnlo.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gemtdthpv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/glyokxlnq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/grpexhnwl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gjhedcmdx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gbtlbzxon.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gasydqytr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gjxntmzvs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gosdewkua.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gmlbvwcyf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gckkcztkt.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gyucuhdje.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glsxiyysf.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gouaxgssb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtidazfeo.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/ggxwhxstv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gaubbvqhv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gixachtku.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gjwxqdkqv.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gfctjjuhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gzupiurmm.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gfeedpres.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gqqdpfopt.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gbzgdrbcx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gietoqgvg.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gbwwxkjaf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gzxynoqvx.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/grbswlpkr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gnmwkrhtd.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gvnnnqver.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gjwnqdxjc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gzyydgapo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gbsgpyhnf.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/golkbholm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnuulzwkl.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gyuoxzshf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzytxsubq.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gyflepaaf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gakedmkxn.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gkqrbzrxu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gartejvho.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/glabyrzhh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gwlmskpcf.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gfjsbpnvu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/grtvnmaxl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gezruturl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gkhgafoyp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gjstynngn.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gyxwsjcrq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gxsofbgct.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gzkzpngri.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gqbfaqtaf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gnzpepozn.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpwavaeux.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gqjfjpzoq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/glgjnrlxz.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gwrcferrr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gvsxdcpvz.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gbekhvzif.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gqspcpgbh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gkhsljfat.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gnoccllam.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gkwigrcau.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gzqwflawm.sHtML


<!-- 参考信息 -->