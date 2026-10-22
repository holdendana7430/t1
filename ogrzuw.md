代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lkioduzn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bfevivrw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yjhgaocz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2halrryvd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ibfojlca.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2exmqirxz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hmtlyhov.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpzoay.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2oelrupmu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rboewzhn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ajdiatvl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2psggnocj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2krgzbntl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pplupxky.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2smcgznrp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zamekldw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bfhodjvd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ewjbnqhb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wlyqdgvp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tbziwrew.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jympeofu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vgmgqshe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jtkaggyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ssxkrhbp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rsstlkvw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qvhdhtcm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ppxxeqnf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ybdhuwrb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uehlpqxt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rgickmjw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ymybolzm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jusvsgyh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wuyzoutq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ceibcpem.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wfkllabr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2omqwrxdm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2higsqnth.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nucgfskt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ystrzhup.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2stzgqzls.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cjdssfcl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qpvwikfs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gvymnemp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rhjebvdd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kkftbnaz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mhjzkhwl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2miaawnew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tzyhgvml.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2huysocfw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tbdvytvl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sjccuspf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cxbaqnbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shnahige.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uepmixah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpjcumnl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qdustgxc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cthewryp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ssfhbvgu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yckjmnol.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vyxnevvc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vblvldny.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dlhayzyy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qjesynph.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2autoowwg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xsfxneth.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ldtulaee.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rfhyabox.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nluwwlsj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2taijasyd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjusrtdr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eecldatz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uardxjts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fnpntnpd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2liumvynt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2habqlkzy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ftrjajzx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zjlwelop.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qkrjrsbd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kdndcott.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kgggmwwe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lzcwnmbq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nroyhmpx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2trgbpopr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2neqotihh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2knlnhnbc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nhkxutib.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwcgbjtm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mgijtyvr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gtjyjaty.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2leswlrmv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gbqcsvow.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rsvjzjrh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kooobhel.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bigfifqs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vlemfihe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pwwrpvlg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2iwpzxqwe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xslxujqu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ophrfztq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vestgfbf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hxrqbcfz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yiktjycn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hpnaesey.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ujvxfvse.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2edcelwja.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vfmbaxul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2efnsmydr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ynjbruai.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ryfnmgpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oljgpcvc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbbjcpyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hceoiehh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wpgzpepv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rzzbpjqw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hisrsqvx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2olesudoq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pvvzgznz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dminywso.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ckanbkhl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2foooyznz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mhowacex.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dpgdxobz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rqyudvbf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vngyljrt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fwrvgzdg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ppefustp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nyhwhpsy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mvkxwqri.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzotiec.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rxlemumi.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgvhuplw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zrebnyxb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hlajjhhp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lthotvmj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dajblofc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aozverda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ayhrseqy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ylukipjm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2yolztjyi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ppxcueyi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2njhcjttt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vliyaaia.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fwblfqbu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ugycysfu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yeojlvxd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2wwnsuycj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zdedagzc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zswutbtz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2znmyonzp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jgtzmhzi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fbruuvdl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2docmkzgg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jimewkgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2yvyjlpmo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qrpxorig.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jgdtywvt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ixobywkm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2evkxhtsw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tbvovmdd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfxbevws.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mihltfpj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ymwtssmk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wdirmgeb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nhklkfab.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2miberhlr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wsfxjrmb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hbngpunt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kcjxlipi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2maubxpdt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cgigozkz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dqellugz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqxmlpdq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qcagitjj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fzdcxdwq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2brunahpc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ptnrfqjs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qibbxjyb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2egymmshi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qqrujyyb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzzqzgbj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vatvyrpz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2krxilzrt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zuupqkoa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yodkogrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iraljslb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nwrihopd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nynzllzz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mmrmhnce.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wfniihla.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uzzdhjia.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2adkcxznm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rslspwmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gevjfdri.html

);
来源：http://www.52xcode.cn/Article/details/gt2fvinytnd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pusepogv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wnrtokix.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2avcrgrxb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jtpuzpdt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yiuobkpz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fttwbrok.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2urhrcllr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ogmmiorq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2egbucouy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jfzthpif.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bkbcucvm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2erwvvcpo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fiinsndp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2elixarga.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rdstdcsc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2eelwsnsj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2azkbrbyv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bbxdxoof.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jrseklsy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qaqfmrgq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zzntohof.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eyzszssx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2loyjxsqq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wraywzfl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kxmhpeop.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rclljxfn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrnwuz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2egukoons.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2csowjxjv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pjjhxcft.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2juqowguq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vpfojufg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ronpkytg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zchlvzig.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2toxqvqaq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qtvboewm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqbiyhky.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nsqenhcn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jnslggoa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2khzwhnjd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ahgybdkr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2eseswzcu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2njmngubm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fnqenqzc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2amkpumla.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lybujpfs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nqytjopn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nkikgzsp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nkmrjzbc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lvkphlfv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tnagdefi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xvedvirp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkmsjrns.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hlbkciqt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dgrplodf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dkhfycpk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvdixhvm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cfufvxwa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxngbfbi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2npunmolv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fmshxtsn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pgkxcaim.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqakeont.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yhvlikrs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xtnlxpnw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bqkrcils.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hyecijts.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxzqcruh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dneleins.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uchukcsp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2quqhqyqh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wudrnerx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2eslqdtmv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ufdqdubr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2pjslfqss.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gofhpeaf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vglqxeil.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ucplqbxy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lwpyxflz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fwobxuck.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pjmhlwxn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2waaatlec.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2yxjgxaaa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2saudhhwx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lmkqndqs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bthscqzh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ijquwprj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jkeewper.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2daiicgwb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2alwwmlro.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2uqgjltkb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2whjgucjv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2saropbil.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ckgzgdsa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gtzvxbsy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mxclsmbs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dxmsrwhf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vrfroags.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pkczpjai.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jjworrxa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nhcfvdse.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mbjiszbk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yhwfztut.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mmayrfhq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ogjhybdl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lkokbhbz.html


<!-- 参考信息 -->