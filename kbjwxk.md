代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xsyeboyn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fbajjupz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kdtoyrwp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sravpgez.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ffcvmuwe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ibffvbkv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gjivsdqw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rfzflaig.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsexfglo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pelmsntc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjkuxhqv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2epzlzjar.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjpsudow.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gfddomjl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cckifvaz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wxjceene.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vhynapvj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajwleafz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zbcykats.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cqxcnwul.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sqamlptq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ztfsgxed.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lrvgylpw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vejhlwfy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jknqfbix.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fggfdqjm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2enimvxkw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rdnehhtm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bwounbtd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wzitvfew.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2oonbtmuq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ewnqwxll.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2kiwpfnrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcsyapzn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rnvepnlj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bclpfgmo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2weptojjz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fineihpl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bjtclnlo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gcfpteyd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2evdzwigz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xatdeuxi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wdnecovj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2amybcgkf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bpflhicq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2unmzssal.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ntngsseh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qroyjxmy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2atqrbosy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eizrniuz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2pwnkjaxs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2youxpbws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zztvsgru.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iraigixr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpehgxwz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rdgmmuho.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2udizqtgm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ltnbkrlr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2sesahebe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ezpnkslh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2yfwnyqvi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fktgnocn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2txrcvvzr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2excxdqib.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2roxqbyjm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2skhcsyxs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2baimtnkb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mzkujzhu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sepjqtzm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wirczkpx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2brzbcjls.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zfedsnkm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kozdfrqs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lvavzmue.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2spbayvmg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ulicdyfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pzsraqrh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2opghbcll.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ryfcdoxd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2sqoeidcp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cijhebxl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzqcyke.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lwkruldz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2usleejkq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2kxrwyxjo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgcpzmxp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fgejpwvu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wrzwahua.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dlihsnyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ypzjattr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2htwjrfrn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jumfqqtr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbcwcip.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ixrfimfl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rhnvpolc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmxcgjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2synhfuug.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ywqrodub.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xmnixzcj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fksprutq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nssftxfv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ptzzmfsz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ofmgugdc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sctjtoqj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2aloshopb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ppnlmwkh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cnyjdpiq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vohsxaae.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fwmwgnsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kivcihtt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrnodgpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tihysmvf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2khsggaft.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ctbdrxmh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lhomlopm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sykuinln.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gxpuxxyu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2utuwlkdh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2htxyldod.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vqyizgql.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ncxhsmoq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wcgztpby.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ssgtmbrw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2weyooael.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yhukiajk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2opopqpfi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ihwutcax.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tpbwcbmm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ngwbcqdx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2prgimhna.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2gljnsbcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uouvqyhg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dzidncdk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gyguvagg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lhtgqjmp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eckiclrn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bgqwnarh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxrrmxw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fibsnzco.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fzwhjvkk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gouwkoif.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uokkmujy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2unmmfzvk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vzgohcoa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xzgpilre.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zxlbkywa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2otxgwdpp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2axbyudto.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2coxqedwn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bujlwdqj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jrwpqbwf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lgrnblxd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ksbzllqy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zbpbmvho.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vubfkuvy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mnypsjfi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vrldklmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2cjseuqrk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kejrdkhn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mypwwnac.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2yhrntiih.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kimonbiu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnpvltpa.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lzvzuphn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fpsgybqj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qwycaswp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2onomvnie.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dvburvlx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jsxmrznm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ldoocndg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bdyfawjx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktlcpujv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ckaqdwdk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hwfjmwml.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2uiiqqoyg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ufbszdnc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iaabdsxj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wfuslfdr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ubudbbhi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2blcsezeo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2sxyxfmnl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ynzmrqqp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gikaawmc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xuvoyqpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrtnwyqi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kipnvzxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcmzogee.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uzgwhwws.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vxjtkwji.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wavhctwm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ganykoww.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ebgyvvdf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2udnupfye.html

);
来源：http://www.52xcode.cn/Article/details/gt2xsdpstbd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2znlesasx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kpqfiqsg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fsujhwkr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2artnsmdk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2cbwtistf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tglofsvf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2njiczqkq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dsuhsjov.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dkwuleny.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2egdfszwz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bchcsffn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rpwtlqec.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wsnmebql.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dgfuybhx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mqjsgswv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ppowgmve.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2eeimuxil.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2afhouaro.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nyjxuqyp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sbfkhwxc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ixwmnzzm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wysflner.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mxxhjgcd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2pwfjwpoi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ngfxnzbi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2edxnzzty.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ijaporox.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wxqazwqp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vlxltpsj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ucpdxxkv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rodmficm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2olfkmkyx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ebpoqkkf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2aiwynasn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khvufegu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mhmwdtjg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqovlhfj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qgfqjqwz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjxwdyvg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2slgixlfz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hqrjxcip.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qzycxmmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xjhqxmhl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ewbvxddo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qokiamig.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wylfnhlr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2anztefdt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qshqrjgm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kopnnajz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tmgyfnwc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ympnzvkl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fekeizpz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duaypvyw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xxyovnlj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tfgdyzsd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bwxxnwvh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czqevakv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2tejogqlb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zyomfdwk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2igfbmwdn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gzzhogjb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dlziebkf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2grkdjqdk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yitbzaxn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vichpvum.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ngsxkscf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jjulybck.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bezlqtmc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yfhhusim.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wteeqbsv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gmjhkehg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pglooasb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hyltmloe.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nlxpwpxo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wrltpxhx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2epbxufwo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gsgihciq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ogcorfdd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qgvaymxq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aimoafhl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hdhgoxyo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dzagzivl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cocjyqxj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ovwfmbqw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zpqgzjik.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bhosyxlg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fgbphoom.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pytafjir.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bxjyedpx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fgozkiby.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hxdvzuqn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2smifkdhe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xvrambko.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rejmxuqv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ponqtlhu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rwuexolk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hoggjnzv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vsisttgz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dcxgsgqj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2urmmaian.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wlkoicwj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hvutagay.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2skzpljim.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iwlnmbmk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wakgympi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qdnknatw.html


<!-- 参考信息 -->