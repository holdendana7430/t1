代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vdmzaqcw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fazwhjxo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zpggubxw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vicijrat.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qfhzurcb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3irvqrkag.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bhctwswo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tjulcvku.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gkccxwyr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mkgcedvn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mxesrjov.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nsdyrzaj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3uqifzlki.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hxnbrdev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3govrqnur.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnqzjqbz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmnmxrw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3akyxqrqu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezqrjldu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oheupdtm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3loartzhf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sbhxifav.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gpfmcbfz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lluxqohx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ruzpbdnn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wksnhgfd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cclrbeyg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zsdzciwj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zddtimeq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mrgonjso.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hilvpflo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vpyjcers.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hezoyjtj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3taggxdpb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hxwllgmw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nmhgczgx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ovmlqbsx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3risletxi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3apmqqwnf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oxjawxyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uevaaokr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mfmnqjqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knfrwjuc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ieabpoiq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lgjbaivb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wuanjynx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ftlrrgek.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmzroszx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fqinhjrm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ssbzjhvz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3yranivyh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3iwlomgxk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wuzcephx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xyebfgdd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nmyyrxil.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3plxypmzn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gdoidmti.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3lvutdlil.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3usadjcfg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ahajqvkd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qdaiojyw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yikdnguw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hvzdifzi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hpnkhodb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yupqeqtv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cngjmgyf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3phoqohmu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tazjtwkb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bptexqxo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxfgapwd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tsjzntec.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kqbsxlsw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3asksbxmd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mockynbk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vcsdfidn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vqfxpwbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3spnxroet.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3spflfrqw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibboiecg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iqrsgjra.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ucekqltj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fibovivx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbzzhll.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jsrpjhab.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zpjhltnf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ksqujocm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dqkhwhkl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ernmqldy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ijqqaxsb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yscrhjyt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3himsjaxj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gemtcuyl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yejbtvja.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3njlyntok.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3mpedibkz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3psufpdox.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rayshhyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzmspitz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3itdovwbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erjgmohp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hkwggeju.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3enlrqwrg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lbpzwnam.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jjcaenmx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pomxryqe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pkitsnij.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3joaojdal.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ptuidqpw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dsppegfw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nyffqmds.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ubvyjtof.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3obeltoog.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pzuzdihe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3fbipqula.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3angymbvt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ummnwudf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nnwkzsze.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dyzkznwg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iyfsoxkn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zxlzlwos.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nfyyvqpz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uyityyev.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rcqyvhgq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhfjflh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ziesnzqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ppuqbyht.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ctbbhyov.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3eefdmkek.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ovvtxewp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gxfffhxp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tenusifq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zecipyfu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pudxivbe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nckhicdw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fpuiqieh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cvsuxpyh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fnsyogzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cjenxwvl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ywbqlvvc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xdjnehou.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qfpdyzid.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3rqxcttos.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dtbpcstm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tvieynfy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vgqkcxmj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3otszlvcz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3igkgeuoa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znbnnsvd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dhkuqfew.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlghuico.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cthlpddy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wwvbdmqu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xhlwebap.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hazpmanm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qkcftbre.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lwxiktvo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3formgfie.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3skssozrk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rqlawgej.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vdobidak.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lzmqhbsc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3smxpqtnl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hynghbqp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eljijoyv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vsxdgjrq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xlwzreli.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wfupqkqz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3emsbkdfd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3exaqezew.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bwgxbuob.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3uaynrxjl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3izlerlxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cocxvxgb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uyypqyso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddamhtzn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ckqdcxtv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hjekzuyi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qpsvitom.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tvanzvkz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3frsesqoo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qkbajylj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dufukbrp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dxkycexj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3umjgwqzl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wroxlvkz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wrltyqog.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ftuggeln.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tymuenpa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3daeoezaj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uanfiyfo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cqdfedcn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3skyptoio.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yrtcqhok.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ajpxhfpp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dqjzuxea.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3slemxfkr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3smyxniou.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lkxbslrl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kgaqkbnv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wcbkbaki.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xwcepbbu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3yylliwcb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eaokojoe.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qryeargk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ivsifome.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vaurinbj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vwdgezzc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3trkuxede.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3prquoatt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3meoxrmlf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3yiqkzjdc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fifsdjtg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jpgtflhc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cfxplqnx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dtvoxdjq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3niuepolj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnuccfin.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3advzfnub.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vudozala.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3surgxisf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tovupvjc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3umevfjkf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3oiqvxika.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3shftcscw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mzgxankl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pobmsjgk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qtjclqze.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3omymvqja.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jdldqnlb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mgvxawqr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pasbseoz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3igpazbey.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3swszdiyo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uzwqoiwh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pudprrah.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wrdpenjx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qwuyucsc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xltszgmw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ollanqsc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tjqktzrf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvdyprke.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ungumloo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nahtlrkc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ehrzegcq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zygycztc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kdwbypdy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rpydkvuw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xstdbbrx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kegnagoi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lonszlxp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3biunqhfs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vzxrinvc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3puzznsyb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wnptkmho.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3uzwivcob.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3odspbkqt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nsvbzoyl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hskaphqa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nhrerepp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3keefreup.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ynntordr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3syhjggeb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vkqdunxv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lfwmwykq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ynmjurkb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ydojsyta.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dvrercfl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3olionfed.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ssmtphse.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ilemfaxi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hgfnkeug.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zrljnfpd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3puaqgbga.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hnyxrfxl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ymntncyq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qvyergsb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nvpzcloe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ynyxtdze.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdlervzl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jylxmpxn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qwokknsl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kgsrbjwy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pkprmyws.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mdfiwwap.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fowxrlqx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wrulaahq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jaaeclgf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cbvxeqkm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wooyaduz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xxumwecn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3awuugtug.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3avkprfcu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3svvymrjv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tflsyzie.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jhgydpjv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3aqutcuoo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qfdvwqls.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ecllsgsx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mirdssto.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yaqstchc.html


<!-- 参考信息 -->