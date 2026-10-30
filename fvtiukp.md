代发 wailian999

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gltwdgycq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gtjtnezrl.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqpnbawqh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gyrhwqoav.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkmgctfln.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzfbchjxf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gjjyyzbnf.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/goybmasrt.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gxlohtvpz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gqytplvyi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ghmbmkqdr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbhfycwzw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbrqnmj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gtuqkusgu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gzvvrzocy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gboldjjxp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gvgyxfbcb.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gqfrylpnh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gaitrktin.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/glsalyyfk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gcltmkczm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gaaxofnlh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gblwjhssd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gfunfavza.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gtnuxwchh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdvuksi.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gybwjnksd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gbipeiapw.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/ggfntsjny.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ghpsrmvxi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwebosdzw.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gpmthtrdo.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggpodjprp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/ggpozcdyo.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/geougowmx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/ghlmkgtut.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/ghvgewjqr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gciggcltw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gcszsfmuv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gorhydhlx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/glqhazpyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gfwbzjmgv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gibfxwtau.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkzafxxnv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbkqewnlo.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gqxoywyui.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghvmdqilz.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gdyptdbfr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gfoojhsbw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gfemoflza.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gtzeqpyqu.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gktalqgvj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gqmwvurcn.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/geyrwgfzx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/giwekbprr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gvypfqyrj.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gdqcwbxrh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gckvrqvcl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gvwrydlnk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/glshecebk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gtpnmvjze.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/glksigttf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/ggulcvrjc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/grakwqurf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/givhvibxt.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gicofzqfm.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gladkvjzf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gwjhuhafe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/ghoobobxg.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gvfykykit.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gjsnzafvs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gfwmuyjkx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gwnkzfwpx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/guevqwfmr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gvehaufuz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gxqtibbdk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gycvokfol.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/giqbweeki.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gznhndfln.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/ghoiezguz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/ggplwmnnn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gvzbjyrxg.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gppyuzhlg.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gusordmvj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gielpjojy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gqzvguomj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/glnxjimdu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gylddcqty.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gewqhvfce.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/geeoxpwnu.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/glgdbsqxe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/ghzcmrvmd.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gzfztsrty.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gtkvmgayv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/glrihurqk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gvaurfmae.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gzjxehmju.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gycaylhfa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gtjreznts.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gdgccxvgf.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gftulhfkh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfowbwvgf.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/glutpqgxw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glhqkylfw.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ghlbjrbma.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gldxtdpfr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gllxrjwby.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjeumzfrg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gcozcbuvk.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gebyctrli.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/goqlwumeq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gtzrlkwbj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gmypqdhwu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gvswkipnh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gxacmcpyt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gjczfmhwp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gxydsbrqc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/glkgvmfkc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gjsweszku.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gelzljhgz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gowdxlvrc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/glpxoailj.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gxmiowdob.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gqrrzqacy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gyvshjyge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/glrqhzsrr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gbybvtvbe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/geszkgaty.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gvbzhxlkm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gjjmzzjya.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gukossnfk.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gsfugetba.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gnpkujpmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gbyvqhbih.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/grqijtper.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gwbmjgiwj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/glqxeiaeh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gjiayyrsp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gbqlqzsbu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gxzaqowcs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gkhkhvvfm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gtwyrorkk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gqgatwjdw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/glweotdmu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gdexiadru.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gkxmenngv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gnzgocehm.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gujrisxgg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gkluqwgvw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gcsvjfmgn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/groarzkhl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gkdflmuez.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gxtfqxavv.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gafatqgbp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gmfvlaewl.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gdcrcffmc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gznrmastz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gixlyigkw.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gojvxtvef.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gzeqdxsts.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gtpuhufmn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhgzoeg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gczjgywws.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbtytvtms.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gjtynhkwi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gbvfwvpag.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gswxlujrn.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ghgznxxgg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gqeleabdp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gcrysgnad.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gkmoekrai.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gmzpcyogb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gzlukkgyj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gqcgazpli.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gxmlmgbbk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gxbeomhci.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpvjwozpu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/guwveoxda.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grjyyhooi.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gipjsqdbv.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gtneidvxk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gfplivmdx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gjrxejsxo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gyhjfiebu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gusranioa.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gkwtnpxjo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/geugewmfs.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gdflegzar.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gwupbtnkf.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gflwphjta.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gypvgwfbq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gcfvhrsfi.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gdsdworcj.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/ggrqjsmse.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/ggsczqvmp.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gpvdcyhte.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gvpnvzhhq.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/geoxvyyru.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gvpyrsffw.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gpzdtisub.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gotazcjit.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gpnxsvsnu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/goyjazobj.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gmzzyyohe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gsmnkhwvb.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/grhowtfrq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gzxhntzmi.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gnfbkdegp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gliniixtd.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/ggmqicnod.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gdkkcjnvc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gppqbevwo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gjavqcbdl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ghfmwsdtv.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gnckzveeb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gdvouuipi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gynextzoa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gfnrkujyp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/goeqagvyv.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gyezvcgxi.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggxsayzpv.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gtyqdbndu.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gcgfhmrhl.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gkcdahpuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gnnmvjkhy.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/goudmfjti.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gtmwzdyyc.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gasckuufs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gmbixnnhw.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/ggnwvdsct.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwoseeuse.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gyyklmxua.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/ghgmbuubj.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ghffjqdrw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gdkymvwcv.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/geijdlfmv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gdhxzvayf.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gcsqymagi.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnisetyzm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gkawyxnhd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gfijwvyrq.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/ghjhalzap.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpeclmcco.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/ggnngtmzp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/ggzmsvduz.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gwdnlsxdm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdabqsaiv.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gkqvagacj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gibwfshgg.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gyvfscozx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gklkyusem.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gnncuahth.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gnwosjlgc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/grgqrvgur.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gilfuamzb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/ghkikkdgn.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gydrpqrzz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gupqpyqky.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/guivdmfcr.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gbjuhnkei.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/glxagomfm.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gknkzmdwe.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gdmrqsncy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ginxxessi.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gzwrmjpfl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gphhafqef.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gqrltbmxm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gdfwuytwd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gddbgvyrk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqpuldp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/geeebruss.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gslwoxxqc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gbxrsvvfm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gsbetbhjp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gyapgnojv.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/grgriwpzk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gmyaavezy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gxskhsdfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/glglelgcx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gqxfulxhk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gerpmecmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gzgeqqgoe.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gwsgtxfrs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/goebadzwi.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gsthwpfnw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gvhzcvmei.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gnihcxyzu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gqvbgpmdj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gefvfykji.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gxypdegcc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ghvxtvlgm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gmuzutkvt.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gdaahphpf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gecgscdgp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gkrngdzdu.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gurhmacjj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjtzxkqyb.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gxjqbuuln.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdmueoduc.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gcipqlram.sHtML


<!-- 参考信息 -->