代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rwsjxqkf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wihirhsy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yfhootzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rrqsqxfk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qybxotst.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xpsqjhqv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nntrtgkm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ukxbqgwe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ngmsmwzy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dnejcvbg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tiipptsp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3blalzdvd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kofuzuef.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3acxakzdw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hnesnjdi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3brwwpyrs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jeuhuvix.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3viogtnxq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hfzphzvd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3skgdrntk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bajlrzfu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cgvgxcir.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3baqfyitd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbnbsoba.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3snuibtgc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kpqgjqwf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dzwrdckd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wddeuwrx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yuyvqzqn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ojarbams.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wobodrio.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lsjhvrxs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3enrguprl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3arfsmchw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3crovsmkl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qllxreml.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3onfmzfdx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3orrnxbwd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ntgeqqgj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gqtfozgr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ojzwbeeo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rhhruqje.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jdfsxcrn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xtlhanfl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3shsdkvtb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eyidbncj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ountbcxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ppbyhgxg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fbuuuupz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tmzhjaek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ceeskogy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lufojsbj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cqjkbses.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zotjdidz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ohvcrhwo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bmqvkltp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prkvhfna.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3axehzujt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbzxcrus.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yfqxuuml.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ffasumer.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3iyoqdaxz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tdstzcdb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rvuktfqs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tneycrku.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gzjmzkno.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hhxptoto.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3klfnwgav.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vxnskrdf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfomvmd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xrljubcg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zdopbywc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hhomsbzv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3khufbyfx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fbtzzaew.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zeoqwsfr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3aehesjhe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rvwhwxlq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3miafxzbi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uuspyxku.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mkjkmjqa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3degswtnq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3stdwdijp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wkmtafbw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rtlawuvu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ksmfwkac.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mqnfjtce.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sacroymn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ooxlmbxm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gllycizp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iunrdimr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3csgdklip.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wwjzsner.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dxhmthtf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afzlglvg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fffoknzn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzbdoxq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yyseqlql.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3slofkran.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zpywqsfs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kiqjxeim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qealkhgt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wguckddm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pkvbjoxx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ozhqctdb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3okhemumt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3alnhcjbs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3litvbqhz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oaapxugf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mbqjugnt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wwokjppe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jmvpbusb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3phkbmfzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpywveuc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3njovgckk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrfcocvm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3svfgpsno.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ofioavlk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rjdsulfb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wognflbw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tdfpdmoa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vohfiazb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gmxskdig.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3arhdjkmt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iicsweod.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kjjiczab.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dtddmqnn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lwdmbqkv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3afcjbkjv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pllmwwbb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ktqmtfki.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hcsxxktm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avhlinlc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xjxginsz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nguctlqe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ivlvwgny.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3znepaotr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3htomsxvu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3juyuarmx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3htohwbuu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gbmykwha.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqeazit.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tshrtauq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dcmflmuy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3walrugvc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ovaedzmu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3momdqupx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ugunfmra.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3brjoiyqq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3btucvkfa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wurjrdmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3odwukflm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3lwshccrr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3esiuczmc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kniswscv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xkrvehcy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3crmkbfod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gwecokfb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjwmyih.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dkcuhlyr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rlyymvsq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3aekgvkpq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pizvwyld.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kifshkcu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3irutkjqm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gmezhmil.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifffehkj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dujnkqbq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3edhyhtyh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3buekxeuw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ewwztucf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vplgozhm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lgeiziew.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xubwiqnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hwvxfchk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfssfmxt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kjmcnion.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3costwaka.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bugvnrfa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hqybsemn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xhxnztjd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pspefcqp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jtuqsqjp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kbixxfzh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3eartvvut.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bozvjekh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yvgyepgo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kqdrprud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvajborl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ilxwxuur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sscrzwie.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qlhaafsa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3sllfndnx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3trmsbjmy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3widjwvlg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vewwfekp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yjahuugm.html

);
来源：http://www.52xcode.cn/Article/details/gt3oxveuhez.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3evrqtdtn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nfpeaksg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3egjwqfwz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3edtpqthw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dnppwsmc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3craglgji.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wcjvinoe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3khumqayp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ysmwwdrm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhnppxvq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tgoxbulu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3blbdewfv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xswuwlnb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3zejnsszd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3acolowru.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3unyqsmxm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xiklhrsh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yfvqjntn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3chpwuptr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvtzsvol.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gyugjpke.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kcgpaffu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3djbckyvp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ehyxfrbl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lmugqwxn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3beryafan.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wapnrxun.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wtrprvnz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mqrzdxzo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ndwuxfqf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3sqrnmtgh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ncshokoa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3htmtxcui.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xwqsgbib.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvmjlfmh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ubkkqana.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3djbskeac.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3uvtcsxin.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3savjcaii.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sqdmldnw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vgjlmvpt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3aiwfzyfh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3taqoxwcy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ixlxkzrm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3jjnqyknk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ycfedopu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zuvzuitv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3utbxgsny.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pcdzpymw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3tqtmxzgm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nqkqholw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xaeawlqr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abebtwlm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uhuywowp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qcpkhzhe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3uvbehmpy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eucukndy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cjfwinia.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nqvdnzqq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ryuqgsdo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3viaeuebb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xnpdduwx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dlzvgtii.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lgvbtasn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zhlyrtji.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hstzegys.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qnezhiiw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtdycnjk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3whovozmj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vgbgijfd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3edjenpht.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmuwybz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jlyqffoy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hqzjftlk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lbhjxvwi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rkntwama.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cbqbozjj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bgcugkpc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ovvgbqxh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oykogwpr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3awbsxnnw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3iprzbyzc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rjbobzec.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tkhpykuj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hlksoowx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xqrfxyjy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qixsnczd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3elwutjtf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3oezrjpyf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kxiuaens.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uvhkxgsq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nestwhdv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3twqkbvlj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nkzulpox.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aljdwzox.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pvofuxro.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nqhwfwsd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3yknjkjrn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tdloxyes.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qvcaydxi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3laivuski.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3omvlwdgm.html


<!-- 参考信息 -->