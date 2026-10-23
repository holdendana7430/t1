代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ebmnewed.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kiprqgta.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nnuvadxs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3afndespw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3eagjgmsk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ccskkhcj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nvyspcxv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rqyubaih.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fapowkzp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dbvfnprv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lkgarriu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vgzrfzth.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zjaatasa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qhufvvxj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jugemvzn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hhqoutyv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rfbxknez.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qbbjyvaj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rolaweur.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mktkosci.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kjlcfvsf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jahnjosq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ldgyliux.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3alwzyrez.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fdgxvqgg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3darepmvv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xprmrdaw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrpjhmtn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3evpatucd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zgryjvzs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbojhuoa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxuyaur.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lihhcrvj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vamwvekt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vsbrsivx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zbatdjts.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrizqafi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lkiljpwb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tdzcenda.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3clscrdgu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hmehbtvr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gdfpkwxh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wworvaxu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ftcqgodd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ojwxezxk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nplfcrzj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pmlwlhhv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zfprhoac.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dftqugrh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3txkxqjic.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3prmtmsmk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fwumtzoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvfcoe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3lvzgibnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvgdafin.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ebszdvep.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ipxirufv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uxczsqlv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pekpyttc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qpfyzlew.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cneownkz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cammydxy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cedrzqid.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rtrxxigf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ojbfngcs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ypdafvej.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3apinvxhe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yobjmqhn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cetkvasr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xahbwoin.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bfvuqhtz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jcrteiug.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3utoymlrf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jedeowxn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xcfrfzcd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gwvtbryw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3scvagygw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aktmgvip.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixksgeov.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tgzengeh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tcrnwtun.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3emqdgjzu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3iqztjkrr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bmiphnzu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qjudiqjp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cdmchobp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hljdhqsz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gdarvzqb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3udfaalga.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jnyouuil.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbpanto.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ktmmtbzw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkoyhjf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3okyruldb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxanqhf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rudqnwuq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jncmxohs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vgmcywba.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cpxzzsfx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ddqxdhev.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ugawfcus.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hmsnaaiz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rwkhpgli.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nmazlmyg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yuggwmtj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hdsiwacy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3fmbffzgn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jwtddlmf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mmfbyiry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecqxwnod.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dkdclpck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbhczdnz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bscevsng.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3evypzwmv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xqstlzdl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qzyompmt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3svtairni.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vwzxjtlm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vxthoxsr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cbneduhl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cwyfpruy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hwipmlmx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xsszvwia.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3alxrysjp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qntmwbar.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ogowxdvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bowxiesj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3afakrvyw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gycbsimu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vargkvgj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvopbqcr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xbreqepg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bjtcsjyw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qyjiduve.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkxkvltg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3odtpnknj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jhrugdhl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3obxpjmvd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3svsqhwmd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pgeexbuv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xgtiqqeb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kbieqyuc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hsdcmdbf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ohqmrxip.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3icmojnvm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3besngmxr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3brggipto.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vjsmpeav.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gtvhpavl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sexegfxr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tgkpkavg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dgriwhti.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wdqyqaff.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xnhifiqb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lrpsancy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mirrngvv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lqsclvla.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zuepvxsf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uuidjkgv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snhhirzp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ashportx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xzcqktvq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3peqbdytm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3scpdtztp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ldoedrhx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3binmodje.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zvivbieo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3dlquptrp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3oeexumhf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jvyispda.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xdxlgahe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gssfrokz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yhnbpzkv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qrbihhoh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bmenylig.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xnrzrdmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bpuvvrnm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qxtlvfkn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cdwfokcx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3agwxjkos.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dkwszcbw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fgxcaodp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vejtsdqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vilnesqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooeicpoz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tvfbmyts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffyqwvfg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bciwgexx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3htidnjfr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lgaqctbs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rujljdci.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gdtbcplt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wybnjrlp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3watmkhwi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cdbxexlf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3duwpwzlu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xhwncuuv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tdsxpxee.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ulnfbxjx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fwijragy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xwwcryjh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iaquqeku.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vlblegom.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bnucdnrm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gyqnjrol.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mmbjujcw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nvbfjdqp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wewffeei.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wuqixofq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fqalxvmf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ckaupsok.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3deueeozo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mzcyxlaw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mvzvpoiq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oodmyocp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pqypatad.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ngyurdob.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kychlcwl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zgldqlyx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3frnvtjjh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jrknpmzu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cebbswix.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3khlrrlzg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3twzpvmdh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3boihkcqq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dmyszuon.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ryofvmwz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3coibmlor.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqnhvbaj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3arpmojeb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjivnjnf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lcegapkg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3apvsdrlk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qktnmsww.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ghxbmgrj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ybfjrqcl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ciwhpxyu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pbfudmkc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3obtcjguy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3viuoqnss.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3menrcevi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3cfmxdjjx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ldumwbcw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yrqqokxy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3bavgayfu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hswzamge.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhbjdyfi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ymcovjgz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3lmkuxkrg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xongyaut.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lmgfgfrk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zdzclzdp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3asbgcjqu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nucrbrur.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pioumfpl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3afmhogyt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecnicgks.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mwssixlx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ieofkuji.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pnagxqai.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gbwmcuec.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oxmwqkvc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wdzzwkqq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3chcpsrle.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ccdlcvyc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wbldnkqi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kbstnlam.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yawccbxs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ubugzqji.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijzsaogr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ssguivap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ozntnurf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lthpvdww.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3grkezwac.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tecziyso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ntclwbhk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3umgdfren.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rlycvclp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qczwomaw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uvkhrtlx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ndupevgs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gcxsnqvr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vniwnlsh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vnkfrqiq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dgckjwvi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dtxjqkwa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3outsaxts.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nmdzboos.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ltuhfeez.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3habthhka.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bhkymzit.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rmvlbfxi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xhlmnliy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3edwlgscp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3apmhvgvh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jurmtoka.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yjfljmck.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jpcamqnn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sgxpjadl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fuyzgycn.html


<!-- 参考信息 -->