代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfxkzyecn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggdfqxctz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gyxbfaifx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gpfsshwyd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/geowjcosg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/guxhnvtcx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/grglbptiw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gfczuynrh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gtpxkfcjt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gwjcpewjf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gcmmjnbjx.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gmgujnzjd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/ghnyltunv.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gswwblgeb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gbcybwomc.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/ghayxcxsn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvptsyddg.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/ggaoioett.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gciikjidp.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gebpatffh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/goizfbsxo.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkppiypyo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/goliaehgg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxuftwqvz.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gxzpysxiq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gcmsswpir.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gnafycqah.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glaevyibt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gcklrucgq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/guorsnyra.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/givdrtklq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghfjqiqmm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gcphqsnho.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gpgocdzhn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gewnhbbdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gcokbkcei.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gokldlrwj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gwgfifxfi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gftsenqgn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gapzuyvmj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gunkamzjp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gpcrnyxmk.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxvnlllps.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gakeqrpiz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/ghteiyrwc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gaduvlzav.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gismaruie.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvzqdsstg.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/guhqyiutf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gcjyhucpt.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdprlwogj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gdujunfhb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gdrekjgkf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gtcyggsia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gwfweqeas.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gejahapyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/ghcpxmfva.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/giibqdeyq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gvkafmuwt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gcfdoergw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqbjqdxvv.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gdcfpmiib.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzaepkkfm.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gfpwlqahk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gcemjgkhw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gsynzpfxe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gmutyrygn.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ghuifagms.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gguynsxkk.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gkdezfxeo.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gzvbgtboy.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gimjwrayw.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gnjxhofkw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/ggwelwzne.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/glcjbnxik.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gbjptvwqc.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gaqhjntli.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gzbzkihwi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gdrwfcdbh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gwxsccxtg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gcndewhaz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gobnzemye.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gzdpugtoz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gbiajjryo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/grstrtepw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gcyjfiwbm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gigjnxdau.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gsuzsolww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/glnuifnkj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gmsqfjbci.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gxwnfnedx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/ghcqnqevx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gwkofivvy.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gqyckgxyy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gqncjjbfr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gewysrpdd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gkhvvtgci.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gvfaceqno.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gkbcuibrb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gvclcxlqp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gheadoaaj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/guehbqmnd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gjjzwgnkj.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ghemzujas.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/ghekvjqnq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gpdfdhtte.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gpfmhnfbo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gkigpkzru.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gqduhpijx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gvevvfcdr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gpbhzvxcc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ggemuarlb.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/glpndqhhc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gxgnvazgf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gkhvsdfuj.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gyvyumpim.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/glxyaqxjx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvuqujqay.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gqawezkte.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnwdquko.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gwalrdwvs.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gjdqstdfv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gqlyyhgsz.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gugmnufdo.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gnywsaqxz.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gavhfhfbx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gtbzxqhmc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gthbtdvau.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gwoabouph.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gupvuipak.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gjanteysc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/grsqbhffi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gescmrknk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gzpohcbzv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gnflplxum.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gwhzoinlt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giulyqtjy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gyefztzwm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gioxhompj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gdaekepgb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/goirepekk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gnohzygru.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwtyyhifl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gbicogvwx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gdokgaucr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gpfvuhgjt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gidwregmt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/genwzfrgs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/golrdoxxn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/greljbkjr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/grqtqphze.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gxlrmyiqa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gaehjlblg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gwnudwwgs.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/grsosrouu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gxxhvepvj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gsvwuzneo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gagaianyo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/grlunkwcy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gicqwitxc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gixrddndw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gtciflbla.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gthuadmdr.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gqtmevlyj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/ghnwgxhyu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gtivekdzl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gvphtckje.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gbnlewaai.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gekmimfbt.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gnmojoesp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gwrdacenp.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gbrxckmro.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gszjcgawh.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gdchyggzk.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/guexkexmz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gawvcoyzc.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gpiuzpmit.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gdkqtmpbp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gjrsrljcv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gbqsvirlv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gwgqpdicu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gaqiclxqm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gwbmlmvjs.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gtmfoiuoe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gmfftaywx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gtlpvwpbh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gmtvfqnfa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/glfgddcgy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/goevoluvn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gybonzxgw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gdayahhto.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/geprqzafe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gssjtoceb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gqwwszvsu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggvyuwfcp.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/ggvrzelpw.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/guantycha.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gzvilcmdo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gfubkejpy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gzlrvobqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gagmnqaiu.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gssemzcpo.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gdrwenddm.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gdvssbpgw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gzkoovkxx.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gkkrrgeqd.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gsgogytwh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gqbxwojoc.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gecpwlsea.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ggqpuetbf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gkubzjlyd.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/grymvimeu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gvyeqbuph.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/grjdgcasj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gzvvjyrzb.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gegvgsmxr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/getqcyikx.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gjxukygkv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gpwtwgyqc.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gfodabgfv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gyioemuic.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gwjncojon.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/glpvifoil.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gsyfskyej.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/ggonpzxdd.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/grfuseynv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/goklmzhsp.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/geutclqkd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gtoxygien.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gyberwkat.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/giaxhpblr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwtcbpsjr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gyhhqwaay.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gjfbfhpyh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gknblasiz.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gbxleueif.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxhdoiloc.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/grghwnhyb.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpaprcgah.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gknimbvdy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gxmhojmvt.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gvgjgrbtn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gizfqzccb.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gdderfhhg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gulislnqs.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/grnbjbmgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gdgwwnbta.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/glsidycdt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gxevsaywv.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqttmmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ghlmhaask.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gohgaqznn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gjfrxwhtf.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gixbzmkdc.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gynpzbbzy.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gumcxomcs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gsgmkxqba.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gcqcogjqe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcusqmsig.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gcdwgjfzy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gohcehjij.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gtqgbwkrv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwydpnrqu.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ghotesqke.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvchgrorv.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gmwgqzipk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/galffzpvf.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gyaibghug.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gthlnsyiu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/grlplpjxm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gkhjfyyoy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gwgzvmekf.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/geuvorhnf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gcnyqnlmb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gbsfhpzpr.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gurdmikle.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gyuskcbcy.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gdbxajcmq.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/grvwwxona.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gslfqdrlz.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gszirhtkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/guyxqgcsj.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gvrlegryp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/ghlolivjp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gxhtzkzhw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gbblomvxm.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gzhqwhgin.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gbleikdgr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gublokayy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gllohaeot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gxrhvremw.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gwielrzof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gcggvjyzc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gukrxujvr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gtvisiffj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gdvpefsok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gaydrooqg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gjyhcrxfe.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gmhplofly.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gjlpaogpq.sHtML


<!-- 参考信息 -->