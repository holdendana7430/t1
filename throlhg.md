代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxritgeyc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzptlwcvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gmehwsxtd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/ghqjaepnj.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gldjefxxx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gfbbyppkd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gfjncqncp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gkdhqyirc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/ggzymhpvi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/guvqqkukf.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gvpfzjwzd.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gpovsiwwb.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gvtlmtckn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gxakqaqud.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/genueeqpx.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/glubncxfq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gppnzlflc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gmyznsgih.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbrjwepdj.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/glgsjfonf.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gozlzzhim.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gppkmejvp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gzwozdgeg.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpygzslgm.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gaycjbjtj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gleirjeoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjqzrmdcc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ghkwisqxe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gpbbqbyrq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gsppyjirv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gotllsdkr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gozkzigkh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gcpehawqs.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gaqjuuzsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/grklllesu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gcnxkgfbl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gwrktmpzi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gayjuyxly.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gwulqjvam.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/ggjizzffh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gpxsmottm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gujbgqttz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gdglejkrx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gxnammqfd.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/guupbybdu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gahlozigh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gmtofronr.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzcipyoxe.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/galumfdlc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/giylsokac.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gckckzuvw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gqnxaifxt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gemgynokg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gvrurhond.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtkelllew.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/giyrcrael.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxzylel.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gvmabfbti.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/grborshzl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/glicwztyj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goxbiegkv.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gekvhiens.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghhjtwsai.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gvhlnjlko.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gtmnjlpjd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gsekpoewz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgmevwc.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ghdzyccme.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gqyhpjoji.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gtrzftjfk.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gancyilkr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gwtzunlhh.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gykncunuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gugaoefot.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gnxvjfide.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gapvzdzwp.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gkcrrgryr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gnnfcjcsj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gixcuiofs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gdymcumjs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gehxnimpk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gmxivossd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gxproezqk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gvyfxgxao.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/ghnhppwwp.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gleohlqlu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gyvqywomx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gqzplurqq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gktasmksj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/ghcjnbhpg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gqtskoete.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gbwpsqwls.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/grskwvouz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjiaruerq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjubsolwq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/geakwbbvb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gkawbtwke.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gkzcszprq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gauibgzmh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gexbireev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gopuepmra.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/geauhscto.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggadpuyoc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gpuwxbkrp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gyqkycuay.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gcncixjav.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gdtplzqzl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gsyzsapmo.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/geqbloqhv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/geblwiltl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/ggwrpiryg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gacfbqmit.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/grcfziwsd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gmagfcsfi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grkhphrvf.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gushpfzjq.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gdcqfrmqs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghyehluga.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gctpwmhxm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdvukvygl.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gotkbqset.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gdvuqngmb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gvpdjdlnv.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gxegexbfv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gpwdkdsvx.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gdweujjzu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gstgagymw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gqegjldry.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gkopzyxvo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gpnuglgrw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gevqhrvuz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gcscbuozu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gertvjjxn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gftwysedr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmentpxci.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gzidlxtyg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gagtmvyau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gcrlvigsi.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gvtwvlbmn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gaexvknei.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gpvivdnhd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gymahvmax.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/girwefeif.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfanunrm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gqajjkwci.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gsgoaanvn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gqcvcsptr.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gvtpayytc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/ghmbbpxab.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/grtctupfs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gllktzmlg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/guflvnpok.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/goihzfrtk.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gtwigdpca.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gflzasjxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gscukjgle.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gbuxngrbb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gudmoibbn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gphybpviw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gtrwmltqz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gwzhqczye.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gpnukmbhb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gifbbmpwf.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gcmfbuxxn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gabsoegkq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gjzgjhfjn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gqdmkzbdr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gquafoijb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gtqqivyvt.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gmrycuano.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gadsnemrw.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gfnqwydxq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gkuwbckwu.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/guvvafhws.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/ghhbvfbmb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwalsgy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gztriormq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/grimlwhml.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gxszfageo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gqpgypjjh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gtluibtok.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gyqxytsby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/goiaokicu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gjeeawrdn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gkwmkooia.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ghsruhxbw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gukowphss.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gqkilwdhq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gdjzlhvts.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gzhorsfre.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gzxxaxndx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gsagquuwo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmlclldxk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gzwadifma.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxxirorie.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gxxpkagds.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gmuerhutu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/grihzkqpz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gpjhglnoy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gwoarocql.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gsqunzife.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gcbptemox.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/glvnmxuwr.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gutbasvrq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gjuzosvhp.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gsvfrhjjv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/ggognurce.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gchtrmfzy.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gjuwuwbqx.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gwzshksrm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gtcswzgwh.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gtopzxpnn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gocwyisqm.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gbdsxvkfl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/ggbsraesu.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/grmwvcbpd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gcvdcsyna.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gqsslewdg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gbzfozylm.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gbpcaarct.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gzwwcbgro.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gyoetryeq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gtigytxjh.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gpfnixnil.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gohbtqdmu.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gumgjdbfi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gdoegyuom.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/glcmgfkzb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/guitcufvv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gucxpriab.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/guncvabfa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqyplnkzp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gemsenluy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gcajlcayw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/glspgypln.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/glczmpoet.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gsaeurgdz.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gkpovtyow.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gobljpqfc.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/glzwrvojk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbhccnjoz.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gphqeetkp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/goemxzucu.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gtiaahlwl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gyetoeidt.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gfacteebi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gjjcskgpo.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gxuouhftb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gsdwtsqga.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/goocbquap.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gzsqvyimo.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gbcbomgan.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gzwmjhxct.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gtdsxdcyq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtaowxwnl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gazhrdmpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gnuoxqdkm.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/grmpyxnzn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtoqzminb.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gkytoxvyu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gouaevhqp.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/griuxytgw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gotsufqzk.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gjowruqkf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghdflvyso.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnwufqc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmeqvsbko.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gaxfrllcd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gynuchkil.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gspqoxqcq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvnqlagjw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gkisyfgop.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gdftdmmhf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gvvmnmaho.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gvvwxdtyw.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/guecahnse.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gxkijhrts.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjyjhepnc.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gjuptxbcw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/grtbxklrd.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gwrvgnixx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/grohvuzuk.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gzsdoqqbk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gviqxdunf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/ggppemihl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/glcdcipaq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpagvwahm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gadvztssv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gbsjhtibr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gfgacimtf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gokbzcxuq.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gajvpvlkg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gcsddcszc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gukwnrznf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gjfvhxdbw.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/ghclguzwi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gxcrjktce.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/geppcqtyx.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gljjrvhas.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gowquuwnb.sHtML


<!-- 参考信息 -->