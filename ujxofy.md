代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kjwznbgy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qerrtifp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2awstzmph.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fheyztnp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qugyjzdv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wchsfobv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pfintpil.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ejrunkkr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ljyhfgex.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2avkkefjo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2luxlbvty.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjtmawes.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2komzrcky.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lqbzyqdg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjincfof.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xlfqhijr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2idgxwrxm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hntjaxjc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2aqmfpdhi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2whijtirr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ukuxwnkn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ghqrhgpo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pnmwelos.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2whrbndbb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2irzuhpyn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tvfhcjqa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jusmeuzq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2byeuscjv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fpnystqa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pevvocpd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ikkacfva.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mdfpyros.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2blniwibf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uumoqfeg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2umgxbpql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dyltafde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqeobjjz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kmvddiph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qquortzx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rzwueost.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mnzhpyej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2afogukgb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hcyvhqhh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2husraduh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pfutuvgp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2avzbmskg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2cthzqegl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2exepuudy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jvetxzio.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2sfziwvax.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qkbxoymw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cozyfxgh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vtmujpnp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2essfzada.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kgkisppa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ednzflyv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qgogiidi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vupmjzpg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2loekeedi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ijkejgns.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ibusibkl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jrbpllxw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hklzwpzp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2evmaqkzc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tmldfrmr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuerrnyn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kcojntbx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fflcqgwd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sjvkzyzx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2brvlrunt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cmkusubz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vrijttiv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ctobeacr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cxvcwxgt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qminmquc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zdboujhi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ypspqcuo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2axcukdpi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uxwvynse.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgaitwt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mgzmjuih.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tgfhkchb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vbidvrpj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2brrhgujv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uljoudpx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2krqwlfyi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vfzxpfyp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ewesqtqk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mamhahuz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tdutwvwp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mchretva.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2svfannjn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cyabphgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acitxwdd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2irvpfoyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjsdyqvs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2edjqdkmu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lblsxunu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zagceeob.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2thplfhzk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uakzgyqb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mzjpgjax.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yeuiozov.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2flfkntxl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yuslcvbu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ulmkpejf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2essffzdx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lmmuejcc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mapzsmpm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bwndtegh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vqzowlfk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mnwqeike.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrtilytk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2mpmwzuws.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iiwrxvbs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2asmcqxsl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nqkrcfqo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wqfwhjkt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bmaubahb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dfooguem.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cyszctyd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2thqfsafe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qcqojwsz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2brrwiocl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2eseffxzy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kgxbnvpy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2akfrlhbl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qdulouya.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wxcmhuyx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2udyhmyrg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dulgxuxf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cklcdyjp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2umhfubpy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cmzqsovv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cccwvhch.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zqegiuxu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dkclingb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2inzvapni.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvujruhq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hjhshnds.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2pfejkkve.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nuzmkaoc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ggyhxeiv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bcfdcpcq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pnybsicm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hmogvgtu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfcoxvou.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gfqprqdk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kqgqlxnw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qbcqpihf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rybkersp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2taaopfmj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2iiwgzmqg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nzosyage.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2joyqdmwx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gbdakwzb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2zgcpuwaw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rmxvnzme.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bnkxmggp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dxmiaaal.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2axqohrxr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ejoaennc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vaszewmh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsfbicik.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ybeiqlst.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2evykawnq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xnhahdkk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2njpeueez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvdpolpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vatizocj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdmnxtym.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qapyrvbu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tcdcbowm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wdrjpcsv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uzvvgdjl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yctsjfup.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wntoydui.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yuxwxizh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tsaubejw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mmgdutxz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mkmlmlds.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xheuhtsh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ybykaklp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ivabrbrq.html

);
来源：http://www.52xcode.cn/Article/details/gt2umfsbots.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vuvqqozp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hlqgecen.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cdelhzyi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2psijhnde.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rdkywefg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2twqedxtb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2istunfdu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gxfzkdfr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oaoxoaqo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2owmsxfiv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jzcsrjft.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kosqtnus.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2iatukjdf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oetzztxv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eidmonnh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wkwywtoy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2eiucvfbz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iyecdyte.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2osibiskd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yheqdpor.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rpkkynxr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xbnqhiax.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sgvtwwiy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2avaoound.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2njxrydhd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tcdguvqr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uucqluuc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnpcbxex.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tpsxjprp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2advnngsi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pymzotnn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vbbzttqs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2bozrzdgw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cyaombkm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mwhgmysd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2irqbucrj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dkxfxvdd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2litpxyre.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tqdyqink.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2onyzztpx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xkthaylr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vsgykhsi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vvsyjxzh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2enqnyfnm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sfrhgngo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swheoeit.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gdpyzmdg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rcpjkcpp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rzlnoirm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmaxsryc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nrkbgewt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwkhgoyc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ebxspspi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hbyrbull.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ackybcko.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycikwvsu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2sisahhbk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dumbxlny.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wkrspkdq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yltjqrdt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qpkvpegr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ieppvbxp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2imweuuil.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ohivbtbd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2chyesxcu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2aoachxue.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2yyrtrjby.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wmmfxmho.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2utctatdu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dcvmwouz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bkfdfiek.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2puaoomtq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wckjpjfx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tjkjejft.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2namhzusk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dinfcegu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2flslgprl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yqphefyy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jpuzlstd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zfargcqm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fixbcbhy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fvbzvzmu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jjkjjtev.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qutvjfjt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xyowejbm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2awuvqjvo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cgpjobxn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uykyjbcz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cungsflv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uthvvevm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hopaefph.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xzjfynrf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fpgzcsvu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gfuowbqb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zaoqvqzu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ejqcvqbj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oqmagoub.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mzsbfsdx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2cyetfiym.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xwvagmqd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zgzenzcr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bqqedrzf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2euhbveig.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iiuhazbg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zacakgdc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2slplpswf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2smquxmnc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jtrgqbpd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ytshlzbf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oqjagxjy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2baossdzw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jrkwnxsv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yqltvdep.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2efjpeglu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wpzovywg.html


<!-- 参考信息 -->