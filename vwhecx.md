代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dtqyfsrl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dzbrfpyw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tgipodlx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3igwdytdb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wrgpowtx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nmnjyrxy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lkcqkkbz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lwhrtjhp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bwzqnchw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ufyspbmf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tvuxpcfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzzooasg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vjdqylku.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uuevepwc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xpsorfge.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cjixlnix.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3pualmwhv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hphusaqt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prsstnso.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rqqgxmwr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fedrsjbd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3haqoaenq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fsrfiwgm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nvhdxfln.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3angfhuov.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lhidoihf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iccbaioa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hrdbsnxy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hzgtmjin.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3udjltduv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tetgehpo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uyxvfdmt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pakoohzr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lfvdtcuw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bavmgqsg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cyfwkafq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roqsmocf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ewachbni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wiuxnwyb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mqaabeuj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bcxnaijj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gbefrpnp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fmevbidn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rzeesvxt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dxmatdlu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hpwbocix.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gkxxobuh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zaccfnkx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fuyvjlfj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vbojmmlr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3wckiefht.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kvkihkfp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3biflfguz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3znjvjvhk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ocfaodfj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3sozhlmik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cijbfbgj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lcsjxcel.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3itzcanux.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qwcdwnxt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xtsusnvr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zargjdoc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpntvszn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3osflnzav.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rhqngdmw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cmehcilj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mqzhyrnv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vamqhdpz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bamjmytn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3swctcvru.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzacexsf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gaekuofr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3morkyufz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fzwsmeyi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ptdkberz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rqitrgrr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3foqrbhvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vccyezkp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3amuuqubo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mqnvqzjo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ppdxorjd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qhotezds.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zoykuebj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjrmvsn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bshgmlhd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vxtbmrug.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3eksecfqb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3saoaobqq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ohjvddup.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cjdibdzo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lcfkrydt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qvdkesxh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qbbbtcxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdsgjntn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ewxhuomy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsxdqool.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tltpwucq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3idhkytum.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3orzcgqzk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pnymddus.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wslzqzeh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rclztumv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lyjkajao.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hdoooxgo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fpysjbif.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qfgjhllf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xdltjixs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxxepwus.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3idhwknss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cvibinqt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3swcifyvx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ozfbinwn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pqhqiqwe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jnvzizxy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3grjxxaon.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pcadadut.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nnwfdrjo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3erfpzinq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3slhzccup.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ctjpgsnd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hnbozrwk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zhlbgcsk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3stkzyrdu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xkyvoyum.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3eccjxkgx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fxfdmwxi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ygnrdrwe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tkdjyrip.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ixqmenwd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvxfjlu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3adocpdnz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ewrvqitt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gpgdqayc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oqfcmfrm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ejemuycd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vqefyzao.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sahaepml.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3djereyhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bfmcplhk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qclvoxmm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3eudvxwip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nbgflxjd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mrodsccz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mgvxvlor.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pbyrrpnr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krfypsdj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejcdjhqk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3webeshyx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yttfefrg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edexmuks.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ktpldzom.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zwspyjfv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kohtlqfh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yxbnhstm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eoqqsqli.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jcbvcekz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3nvjyrmvf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uiuufwqj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3natldwgy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3azyeyqbo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdgokdd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gkzdnuxy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hymhxrnj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kpaijgkp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3fzzuvyio.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nxrywhum.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fgrqiqfl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3omdbskdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtxtdxxn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hjrxspda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwrvwatk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3khwufzxm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rykabbmr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qbvvkrro.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nhoaxgau.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3axfaskou.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3guwrntsu.html

);
来源：http://www.52xcode.cn/Article/details/gt3oiwqplrs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ekxcsiyp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rxscbzex.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gwahuksk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3swqegoen.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wvehwalm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cuyxplag.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sxiifdww.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gpcboxbl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dorugloz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xxialfoj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3auiwtvev.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gvwizpfo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gdzaakqq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3thmsprum.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yhkyzzzl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3thfwtsaj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lhhlikbo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ghglkgej.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gfafbrvb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vnwaoukt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3piuwyxwz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3iysvnuxf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3duqyqjln.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tccttyhw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gmmjmxuq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kopflczh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fmrkgbst.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pjalgjgx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xuqatsik.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3apqvmihy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zpkwfjxn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3idhyqkxy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mlxarogc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3owyxbpjx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aslmatzb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qevelqmp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plhutrnv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kgqrebtk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lhdceyie.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3asjavnby.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hfelfblk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dctagyvk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mpmsxdqs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bcqlmyrg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dhdjdync.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gwkqkfur.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rizuqafl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3obpduhod.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3uygvcdeq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3onczsidy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ezxvpvmz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3owkpokzm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3itcmkano.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3momkkylc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3gdubbufa.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xzkuyivt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kpfdocgr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tivfcaoq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rsjqlehd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3iccfmplu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ufefmzvg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ecczwwfb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxkcbboq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rpftvdvd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qewrtqjv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aucortjd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3safkjvop.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hclgxkec.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oaxjfjel.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fxzvwwqp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jbtjojjf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tqxtcfuv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eqndmwnx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qgqgexfq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qtyilkhr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qbxiophf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wynuplss.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wseppqux.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3igkjxosu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dhgxxqwg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wegsjauc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gjuwegte.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uwvavost.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ahdlnctj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wffykzdm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rzsxmxia.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ziarribk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ucwzbity.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bxkomsfs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mmcngeey.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jirlrkhh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ifwqkmpo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3smqlplea.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xkcbxpmx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mrdgwply.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dnfwgsgl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qcobfhxo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3svmqvphi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mxqkyfzm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3sjlvfkwb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pjwqjcuy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ytlffdkw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3eqvpvliz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xdfhlnsy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3unvdafoq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jegkmihb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jgtdwcmr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uqeoidua.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3plevvdzo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kuundijz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3djaybqeo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zrlbhpit.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3phfspbjc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pewpyehy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cnhuoqux.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tcjbefcf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xmwrpbso.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uorxzbsg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bvwqasjc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vchnuqry.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3imuoakgs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fifspolg.html


<!-- 参考信息 -->