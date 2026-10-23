代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oiyzjpwl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rihwkboa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jbmmuyxr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dbrqehdx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pnftvbhl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pyakwejx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zsfavxcj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rcdzejey.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xnpysqgp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pftmrpqg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mgaydusn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ukvigrrt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ysqindmk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qaejyfdw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zyhpcpyu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bqpsgkuu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhbhoirf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbalamu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqedpxej.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3owcrqdci.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3khmxethh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ticpdvvn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vwywqtdc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pcwpmpkf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oxkafbeu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sdswlovj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yezvaosz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pjgdsxen.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zgxpgnmo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hmjnesle.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lzdodzga.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vtklodqk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xbmbvmuf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jscpryah.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gvmaevbe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vqdmspyd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3chxiohgr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qzrymzcx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3exzelycb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uhsdsgvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdtdwpln.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jlhkcrfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyzcwecp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vdhvuphv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3luoqoewk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qvximndi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3eowumptk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tjficxam.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3aylphbst.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nlfpoisg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dnafctjb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wbygamtz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iezwxint.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3exmgxnor.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3buaqduoe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zxjalcqz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3woyhzpae.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qfcckoly.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yhfmywim.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ymxuprgq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xobtnxxt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lkgwecvg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hxmvrqnc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jsaeutnq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mffijtyu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tlmtlvjl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3moluydua.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bepxmfgi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3secgurce.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjkfqkwy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jppvztrh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xvpfjyhs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3onglgquz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opozauph.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjrgrixw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mudbyqsw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jpzpxxlh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dlculsyv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtjnzej.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zwfgogyo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hrikkcco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3aitwqvft.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uspfbrba.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cudndcuu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3czaglxjp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tlkseufm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fbcinncx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xhejsuay.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3csqbdnyz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3usmszewi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3guzqfhgc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mxybmmzf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ktgohnca.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3pegckqvh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fzhliapy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uttccgss.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jxpfzkgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjjchkml.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oytnxzsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqxbfqfl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iaqtrrnt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3neopjcbf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3igumdoyb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tpopeyhz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eqoatzpe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3oeeimwnw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dqyflsrl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vmkpohmt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3drdmnhvt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nvdbkotx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3sovhtcfq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pbyvpbfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qgglclko.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zkuyafti.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kuvnvxqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kpddkhei.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ioedfzld.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ztuteymd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tbocxsoa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mqntqbjp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bxgduyco.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3grphzdlh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dipqyjja.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3omvdyumm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vwedlgzv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vhcrhily.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xpoiuarn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3clohadyv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3trdkzkwp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kvzcsxwp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3etcddert.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pjypelwr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oxbtebuf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jahtawxe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dnnwdoib.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wvdvbjwo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xuihycwl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cfaiwjjh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gartrkfe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gjxqeuhf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkufplnw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wgefxyuv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3popvyogx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yaabdzzd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3glxsrdlj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3uwqtvvxj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yqbnjxcs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yyeumajy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cvhvpsey.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjrraxkh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obwtcrbq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vhppmetz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qfdjmbug.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fpuwczpa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3iwyisswa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fstesbtg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vgzfzxfu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cldbfhzu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vgoparfl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zedlakfw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yowzebqz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ierrwueu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ryycdcoa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vcbbuagh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rdruocpu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ebclbhez.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mgdwabuz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yujsoivv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tbarkheg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3aizvjisa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nypptlpm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bhuguidf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsrnhyoy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wzxyyyog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgzjwnej.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hkssmyif.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3goaegvxp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wipvntow.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dzqammck.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3atdhepuw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cyysayin.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3iqyfgqra.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gygudcdh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3skoclzsd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kywwbfoz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fxpzgolu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uxcpmiqw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mjeetbwz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dulmkwbt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bcrbdadu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3uypzfoaz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hhdcvien.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kzkmdbcm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3frszprrf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dbqrpnnm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3aphuptfe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kgrlwrdw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vndinmpe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kzoervqs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ylfheegm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3amzckzlv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3huawwydv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dnhgdstk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ynmynmsq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uachksxx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ztfmfllw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ovdhzyuo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mgmksfwy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hjwylbxa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xwfrafix.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3niiupgct.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tnwlvvaw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jvllxrfd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nfrkwjwh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fsnlcujw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pnzklnpy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxvbbqyw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yvuiqvjv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qxgnnafc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3swklzlqc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ulonsncl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3unofdddn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wbpqfpfi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dfhbqyxk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hbqwslma.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dgzycdgr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tjbmhgay.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3svginoee.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3eilfqkbr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3odmnhinz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mezirpur.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uhyeuyjm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3apqdngqt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3aakugadv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cmuvbebk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3svojbznl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mbaxhrrj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3oujkbdqo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zhgqmtjm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uswbshht.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aairuprz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qlcwplsl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aghdepma.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xsuapjpi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwxldhhn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3eneogabv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3atgmiuyl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wlxhbcpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yuoctqpe.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqcbugoo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zjagenqc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ihrnjbwx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ktgvirzk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mbpkmbgx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qlybddzk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ihpeqyus.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tvqxffqd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lqjgdnux.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nbtmafec.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nwyheeae.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3qhnvjcmo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3agnabxlq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3focsujia.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tcvmjfoe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3alxmhtyq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rqlfascz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rpwoovpm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zzahcojr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jeefmbzx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wrmwqmrb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oswhbfts.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3oslsvdce.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kqhwoaox.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3onnunyiq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cljabltl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fpjsrmya.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3gwachmtn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qewxqnub.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3suourotm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ypuhzxbq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lxsaxnhh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qhefmmso.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3spyrnavg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yuylnkez.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lkntzrby.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kjxhpxjp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hhacegpq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3druttafp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wgtfsoku.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3itkqdbms.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3klbqkzwp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3arjhwijq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tduzdwzu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3owdnmugt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gkcthanj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xiufoufs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmljvult.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ssojobwq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hkoxjezg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wfcarpnq.html


<!-- 参考信息 -->