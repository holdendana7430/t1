代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3aksnrsgh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xkweuyod.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qfvaobvr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lloofkzl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djvpxekh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dnnfwzrq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pzkupvqp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xljswagl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fhwthehr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ggzromtp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ahhzfjhr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ntmjpvix.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jkwlgywy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ljsbjkme.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gbxqsivd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tvgxupre.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xwjuotnt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozsmvqvw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tbhrmwym.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yyjedofh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fzlbqqsm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yeqnmkcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ezaailhd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdxjaff.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtalojzl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ysdizjfh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sngkskeq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ohwzwabj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwcwwdr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qyfbucyu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ebbyhazx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qxcopvtg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlewspiy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wnlvuypj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yjwvlzeg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3veigvrma.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eruurrki.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3opichemj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hucomwlp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cxuqydmo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dkhnhlhq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ckfuxenp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qityexsz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xoyoelxk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nksvimiv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xrufrvgi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jpdoffzw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uqzstsmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwxlkvpo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3umwtrhyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfjidcyx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3nhmwwbds.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hycsdhrk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jvdlmjey.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ozpphiwj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pdhbtfzb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3plodrcvh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3oksbjzva.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ywzmqngz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3iipkrwzc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yolpyghc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3bludrxxs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tpslfizr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wcxvrvzl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wwlanrtz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vektokqu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3tkzxfmzh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vxydmezm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3chcxtkhp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hhaglpfj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xlkttvsf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hwzncaqe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hnicntek.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tofoatqb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mftjojac.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lpntoczr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fegsuatt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifsxylxw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sdsfvvot.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ddcsxeuy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ztzgzrzp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bhlmjiil.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fybxokkj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3psgjuitw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3albsokao.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fudqpdgt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3scklodmf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ahwesddq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvovuxq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bignhder.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqpkzti.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hkvmuqjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dlrnrcnd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3losjtpcp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mfzvxdrk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzkmajb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3megttjkg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ieyfbvwa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cubvgvjh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iyiltpto.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bzslgqej.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3geicuoqs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rwydhgpr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ulhxioux.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3npduukau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgmnygsw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3chfvykqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izfdlhxm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3alglwiyg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3aejttbtn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gbnrgljz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zmgqrsnj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gsxxpdjh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3itshpdcx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ebsezkgp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iquywjmg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mflafrgn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ybetayhi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dfgthbqq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xymousbc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vvphobsv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3foumsauo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xwlndmdx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wrmjoite.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpwkvgub.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mbxorurv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jowjsxer.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3yifgozyk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3udqhigjc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3whgalulv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ginzwegk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcsasaa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jigitpgm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sinotlrz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3sjrjuqlf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xrhrdgba.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3whhyyvzr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cdduspen.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3myexeryt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mqkadqrs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pgubzlcc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aqtsoncr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nhyxrptu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ytipoick.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gaqkcoum.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3vapjfzvu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xwirfekg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3aqeugwod.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yyiwjmeb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3rycfksqr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtstvpu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ragzqtno.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xoivfffm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rypzzpbr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3bxmoidfc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xuagntwp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tmyfqwij.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xrofhfep.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jqvbrhwe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3eqildvfl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pbtirosh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lsfykxkf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hzqnumdk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3adtjtffx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uipocnxb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3grdsdbsr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hqahbqdj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfdegvw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cgqjdaad.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dzdhvrsm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vsbnixyv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pfghomjy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tlrtgrqc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eyafyfat.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lgdusxsi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jxzwgvwj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ireeudqw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3czyiaibv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rbhshsjd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ctdxvqpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlelihxc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dlzyzybu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hahspgqo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dflxkvhq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qnnszxfd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ciswcttg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fhwmenit.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tfcpspxe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vmltooqs.html

);
来源：http://www.52xcode.cn/Article/details/gt3zeomkgyy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3domxxnms.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kxwomoha.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vzlcbhpr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rdreyjhh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tgkhdzzr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wybfrnqp.html

);
来源：http://www.52xcode.cn/Article/details/gt3xpiklskl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vcybatli.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dferbtjl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pafmxmxw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3coclbazq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qotowkdz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3enxtqjlv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kummgark.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jbambfks.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yntrhpdu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3nukqhlfo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qkbzochb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ulloubsj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3umtjvmop.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3drtamrws.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vmobcnzz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nuhmzyil.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3utrjvmtg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3onmyqicf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qwsmtiix.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lrfqabke.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3clerndsj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zbfqzjas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cqhtjhia.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ionerddz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ancwwuof.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gsbsmlnw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3heefrlzl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zuauzwnk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hhdzidia.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnlhslus.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cxyqgqfd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gwnejbri.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3casiprte.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ocieuici.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ezwxdpoq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vvebyzvi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bufhzieb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3txufohhk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3khpzvqqs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gvvcckhr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pbajmqlz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yxizkvap.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zwbzbajg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3iqicthzy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3axzfajtg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rnceasns.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3bnrzttzk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ugrwhpvs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nwzkwxub.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdwtdlbk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3trywbafz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfmanvrs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zwxaxwfq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ftvyqcdt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mecmcjsg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uhgiccak.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rrvkhukx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tkvvpnep.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cseqxovm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3daqxgbkh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktvmypxr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tvcyllat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gwfhmpmw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3caypvkkz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gaoivkys.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3udhuqwya.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3elcqrwix.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ytlcneui.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3txteebeg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rhivllwf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gmseegkw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oqwnpzup.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bdqzojkj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dxuiivat.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fyegtzsc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zqgtmpbq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dxghcimx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sixjwwio.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kxicfkor.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dlhcpuhf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3znupjhmm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dijjsvbg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tgccvvoc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ldbuxtas.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tljdryqw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xjyhywtm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ctyaaoai.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zicdjxlr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qclstigu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xqeiactf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bdlfdjel.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ovkkohmy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kjrkeika.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3egjaqlts.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eotfbttz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3uuitlsgu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kqdcgphc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfgrcrpd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ypemytkd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3debqemag.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xuteoyqg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lfduojkn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zddxgqzm.html


<!-- 参考信息 -->