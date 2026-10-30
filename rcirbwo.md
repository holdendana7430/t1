代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gycmhqdmu.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gpfkowdxd.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gmyfwinrc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gldeqzrtm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gvvojkdep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gcnzekcje.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gylbyahxu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gchpixdyd.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gibsydiuo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gpofkohyy.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gzymtxsqt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/goyspfuhq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/glixcjtoj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gscfknoia.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gnjawqxtb.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gssifbzpd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/geqykkyrt.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gukkuuoor.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gjrwltllw.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gbrdsmzts.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/guxqoipkd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gtuqqwiak.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbrhpkttp.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gccwqtzls.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwjgsejek.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkqbracce.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gjfslpikj.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gfcpkaxlz.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gkinrczxv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gqjzadcam.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gbfhlrtpv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwnmoqout.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gzgnikigz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gezwnveyx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gmklmtlek.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gsymtyczh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/guzfpnxco.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gwdymtdea.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gniuiwmnb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gwimnflex.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gtfyqjfzg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gdpbpqdqy.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gzhjdfbyi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gcaoeguxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gsopdrstp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gphmjjgoh.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gxcrbtgsr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gjgoccbhn.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gaefzcmlj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ggibqzkmp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gicdrabas.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/guupfqdjn.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gsqzwpcdl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gbvzihzal.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtxjhaigk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/grgtobsrq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gcgigpatm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/genalenwg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gzgszhnti.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gebhlafxm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gpdybhiwp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/ghkpbykeg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gaovwwcsj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gehdtmfdr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gskthpuyt.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gvvktgwkr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnjvqvoqx.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gqhzbabpi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gccytmqgs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gwuhphljx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxspqytzx.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gdqqjtcja.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gbhnojmev.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/ggcckoopd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gmyyggkfa.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/guzuvherg.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gbobtgzfv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gyqddxarj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/goawbgaty.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gfbmryxbm.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gmreaajbf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gltapcmnm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gnfmicisz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gitvwyvmp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gecotgkdb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/ggxvjpznh.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gaxwhcwep.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gpdgstnou.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gzukdovad.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ghjlieohm.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/grukzoiiq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gdktfeaqv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gueddjzis.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gzaljpmtp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gcowgyscz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gmrwgwshx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gbogmqrsh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gpvqxbnyr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gnnhceuwg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gxkqoxoth.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gmhbvband.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gljpsfxqe.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/guodekyxh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gycgujuen.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsafouygb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gifwcfogr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gyrvxvzgp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/grojgliov.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzqnthxhg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gonenmigm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gvtwusjgo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gegpotgjh.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gotxoatfu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gjkodpxla.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/ghgcuoouo.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gdjczhkhp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gjemcdvig.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gnseubdmb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gpaoxjhuo.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gapgvyqon.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gjqrtpkim.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goycjqvww.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gllgbjkea.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guwkjamdr.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gaomzjkha.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gmfvweqpm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gzqjnwvkv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/guyunpxln.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwktwkscn.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gefsllnsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/grtnnwnoq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gblnaginq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/ggsxryzxh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gvefzlihd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/glwsbtomx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gmjzvjwbz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gzgehgrld.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gelqapkzo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gszfkeuby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gcjxzzbkj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gttzcmqvv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gpfutwvrx.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gcgbpdphn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gzuslwxmp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gzvkocelb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvcjveoia.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gwdgeixwa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gltpqwbzy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gfmflmpyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gictnzpbe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gpptrbggu.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gwgprabde.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gkyfijjvv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggwhjnhct.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gymtwseuc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ggxbyvwzl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gkurpxyhi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gfjpdionf.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/ggwfsqtot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/guqytqurz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gmiojbetg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gkwwhlrov.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/guqmzwrzc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gejdxenkz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gbadxkxqg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gedojclvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnvffmduq.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxzzplx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gcxcwlbli.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/goadnkxnq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gqngofpkl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gihkijfez.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gzkbhayvz.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gkkflocrm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gsljthodw.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gvfdcjkkr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gtcgmrgpy.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gdtcwlecm.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gsrdpfgny.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gpeydggyg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gahcvqric.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/glzklubgh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzpyekuit.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsdzjpral.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gljtmrerv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/guadkokdb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gkgholugv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gaaazmihm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gchwsymfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gisxpssss.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gjvxklyjt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gtzmvsgki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gwjefocgf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gmpdmebme.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gxqurpznq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gdafiaelx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwaqrcdnn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gjpctpusj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtbjuuviz.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gitvsirgg.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gtoxroetb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/grkpasrjn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gvcrjmbwe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gukhbvqix.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gqxpugsok.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gveysioqw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/govptqvqu.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gfptfuioi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gblmjrzkf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvacwre.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/ggqdqumut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/giavfswgy.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gkrimkapw.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gemfwfxac.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwzppklai.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gjzqtomaz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gqcetszxz.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/goxsnetjg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gdznmflqx.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/glogmjbyq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gxenrhsaf.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gunquhzup.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gormmfmdi.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gnyxlnqup.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gginwkmvc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gvlevrcda.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gupipomgb.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gmfzonxaj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvjwbayll.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/glsisdiaw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/guedxbgwv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gbnrwdybu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gzorsthyv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gkrtrrhez.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gisggjhpy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwdjnzvwp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gtfaqnawc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gakiwouyx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gnvcxwdqr.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gldgviltx.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/grvthuhwa.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gzstwvbga.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gkmukzyfw.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gdslrqtip.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gewqbvpvv.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmmumqyfx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gziucelwm.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gyfoublrt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gulhscduv.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gsoukamfh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gwkeolsnn.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gelqnlhkt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gjozzlffo.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gqmhaesft.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gooyhtanl.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/geeicdbxu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gwsgzdwmf.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gravciiqc.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqzusmmpk.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/guaimnuzf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gjajnhaem.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gczobfmnb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkqeclgsz.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gmjvtznnh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/guvtygfdc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/ggiowffik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdyicszjc.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gqisxzkyg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gybyuszqs.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gymeoytif.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gyufqfvtm.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gzmwnynsx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gfckqxlob.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ghjamhtds.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ggczfboql.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gnillrcnu.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/ghqcsodfd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/givfiedye.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gndzopbut.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gybcignhz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gnirhhdpo.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gtqclwafr.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/ggxfnduwd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/giyeylkpq.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gffntsxnq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gqeymauec.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gfxgvruzm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gscmsrvll.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gquejdlfl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gjlytqlor.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gvvevonok.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gmnyfwiop.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gjtdvgrbi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gmjtogghh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gidpegkuw.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gtukmqohk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/grdbmjbbb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gvtlpvcjb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gblrhmktr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gnordjlot.sHtML


<!-- 参考信息 -->