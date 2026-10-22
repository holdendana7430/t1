代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2stzdobyo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vqmttwss.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2agxkseie.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ebwgoivd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wtbwbqgp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzchnj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wknlilxr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2iajjveii.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snwknvya.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2snpmpscw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rgigsfaa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jghenxng.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmgihbkd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gyodmsut.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vackhtlw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2asuswcbw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2blxrjkmh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bcrueabp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ovnfkekl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2inhibezb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xajbpxwo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tiwaunzk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hogbjnxv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqnfymsg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vyjkvlft.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2djgqeeuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dgjdsccb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbvyossy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2sureiwwo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgvuhqr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jyxfulyb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wagkiuqw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdlvxbc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwuqvwsb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sczryqam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2itvhtxic.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tefbsrmv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pynfqqjb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fkighqgj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eoebupwb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nmkjhdrr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jzopkkfw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dipwjljt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dzdngwug.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gqxdkrnx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vfqkggvn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2chdoxqzz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2omofhfop.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ytqczklw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2pvhpzhtx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qhlwimhm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tofjyqan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfqcngnc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xazqpmcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlesjcyv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2sgrecnsh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qgggufin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lmmctuex.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rppaiwiy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2igvkthae.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xluwgrjs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2aopozlwj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2snrgzqgh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xsyaahgf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ilontthd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hqedfelc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jrxhiibv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hhlvdrij.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cuitqmrz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzlajk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2aggwnfkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tpxydhyn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2umnsddog.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ehuiiocq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2forngxqj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zmtoayvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ijjpqcnb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zhrhdfzj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ervfskog.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjdsuk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgclvcq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eukkfvru.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2swkhapyl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mguxwuro.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rlrswkku.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2omocvrux.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iciybuzw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hngrrujs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2smqbjcsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ssuewqlf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2svstlbew.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zswexism.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ezqvkpas.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pceqkosl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmfocid.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2skmdesek.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pggkdpdm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uegvpkmb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cljpruie.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2obsbvbqt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2eqticcwo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hpgzigjf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yoxpkbbp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jtvapjlq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2senocsel.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tvtdgxxt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xwghxmkp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gkynvxem.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2okgievyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isljqnya.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qyxubagj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofjkvxvm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kuhkhgir.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fwcmyfqu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cakfdbwv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tqdlxtfv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cpkeuqoh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wtsjrdgw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2apbzoavl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xsgmfujg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hvivdbgn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cjpgetbn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2shalppdh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijhxuwts.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fbyzkfkr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2juvpskqh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rkelnehw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zmxbtmux.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vbjjjwsd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dnrggpok.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pxbusqmn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fuumadgj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bxzfemra.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rxrsdwbv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fzouyeox.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2avvpnavy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2chxsijfh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uhegzvhg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dvwjrxrt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vcyqetvh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gkgzshsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qlchvnrm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kpijngpy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ecytqxlg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dgwnsgvw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mgfhzdck.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2nrknslqn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2byzueytp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ccklgbmk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oedbrcxe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vecxsrqh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2oxapcbiu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqaqnhkb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2semrrrgg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lmoeaypj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hcocxozu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ceintbdg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ipdwargr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eytmmqay.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjgpsgwj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2iexgjwqb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mnnvtknn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rytyfgvo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxzfzrpm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cxlpcgcs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nuqscxgd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uzafquby.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ayljglcx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2oubqbegn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uuiczzfb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zkvuhrlo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hwwlkmwy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wyqrtoay.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tpttkipc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yhnfacwm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2afoqepoe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrlrkje.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jxpqidvo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2flrutqvn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jxhjnxrr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pczzlbvg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lfqkkvnu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ccovpnlc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mbpsrjrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vusozvly.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qgksjbbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybicaske.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zikzrgvn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2eqedokbf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vxmlwbwr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hkxhwwix.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yjublkmn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qazukphm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qhrmxoya.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mkkflbio.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vkjrwbbh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wdyijmiz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2glyqgfdv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ipxiycgj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wornfvha.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tbpeqpjy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2neqfvlyt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oztkzwnl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tcqughwy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fwwueico.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2iflzlgus.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ljdvrbcg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lhdjgbyf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2nblmlcfp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2djanlpph.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jpmrmdve.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dxtenwmq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ydvnpxja.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2stvjixbc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ybfqtmsh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zzymtduv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ktseinef.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2onytusld.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wnnypuuk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mtuvwrmx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xkwuibxb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ravmflxd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fmhmddrc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ivifikdn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2caxbrhjg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2sgskdyvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2puklchtl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pspzfpwk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2agikoepy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ljnpazxr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2imlvbsos.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qfudlnii.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2frlocbgk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2amngjrgu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mnyncrcx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fyfgzbvt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jucqevne.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2atedyquu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2phhhfxxi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xszvvnhm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dtnlexkd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2aicjhowd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ihjghmio.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dhqvgpjm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2lantpdqq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2uzuvdqwm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ooozxhno.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2oifroqjo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bozqqsiy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wnmfqdvx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpsonqlk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cvqesror.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrfusyri.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2igxsjpqw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yboekfkk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2psexalbs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yktixrem.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vtcogshg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uraftqhn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ruazgokg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rtqrabdw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gopkrxop.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mihsjytk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xtxioizf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lalvhttn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hcuibcfs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hjealhez.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zjjtmocm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wtyyzeml.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ayfunljh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ehlbscvg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nniiyhip.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nsipaxde.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2awivprcu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qqrelryq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lkzsoucw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ildycebk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ojpmxgju.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tzdmrgyp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wucsgska.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bujarrtw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qpxnigqr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vrwpsylq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bacsareq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2uupbbmlv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2adlwncag.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nlanjcod.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pwoliqsl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2stwwduwg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jzlhanpm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rocvbwfq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rdiuvffr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2sqmpkefa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qlhvgfzy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tfzbkkun.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yitmyzjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2otogfbyl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zpoqmxvz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgdjxxyc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vdjnrusy.html


<!-- 参考信息 -->