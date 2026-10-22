代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nyiisvaw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yiwdjpnm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2iixfafpo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2clebmfma.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tdcnjtsn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2swzfztlm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bpfenatb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vpyfahuj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rfzhsjrh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vvtqbvhx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2msaymatz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfvnpwjr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2agfkrzeq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wldwyvaz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lariwmmz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjetcgij.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kxvbnfhq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfmzpkad.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kpcvucia.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gdstiadc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2belirsai.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dcozjhpo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2grwjixak.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mobphayl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ehgzridr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2azjwajxp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2alncihqc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2soozlsvl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcisvqz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kzqjrmbd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2czrhchrj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bzgxinis.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dqufspyc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dbdfjapv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ssyvucmp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2trxhbbgb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2iyqgytjd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uhorkemy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uidcoqhp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmyrfcib.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2necknbth.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rbattlmu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xpgtnjco.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pdwrhlcc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rqofgkpg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wwnwsohc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ukilbnwq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbzeqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oiacsrnf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2eukllgcc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rdhpuufb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2egygwnle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzroqiit.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wtzwucth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybbougjd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ypzsxtni.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ckepezio.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ncsadepf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2sditrfmf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jwywcstc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tfyromgm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2igowsaxr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ynhcmaow.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xhenzwoz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mxlnkttg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxorxdkz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bpghzqzd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ccvowbus.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pflgpbqq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqmocou.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2knjxjemd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wibhchle.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2esexrrsj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2diwtcbfm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukgjeauu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qoegmlcg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ttzjzsyw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nhiarxoa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tsvvukbq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2clagiuje.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mbdarapq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrhqrxgz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2obsopwxf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mysieylv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bcgfamvz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbqpzqyu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oscpqzmp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ibczjstk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tanldqxu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ohmpicvv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xiztgiud.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kychjrqe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qalwtnub.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xtjzsrtx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2juxetvsx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tjxsjdxa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zqxgdzvl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fdamwmga.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ryuhztva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qpklzjaw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hklmigzt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fpdwfemq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2iuxogyeh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gfjezplh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2egufjkhd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lgzausgh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ufkrypfr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gkjhctjt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hxnfurcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owrgadcb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jocguqnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kszrptxd.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xrrocnpt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pqaapoal.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gdeprspw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ethrkpef.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xvdebrzh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pjitawcx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2oeyifdzo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rdbxcdie.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rqdeflpp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gnhllekq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ogzeqxcn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pziumzzp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xeczktlw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tuxbatad.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pdaoscda.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gnrxzkxz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vbbqczrs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zgootyuj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjidxc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vqrxugtt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lsatddku.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zvarafzb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2giamreyz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2luazzfww.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nxnbcpnu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kzekeaue.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hgjoojmv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jyyhgjfp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ozxyouyk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ifrrmnvy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2joqraprx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2szttjskc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ltpbbovf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nlottbjb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zumwygds.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bbpkadnj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jambiync.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vhhtihhe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yamcfckd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lxonkvwm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yaynihek.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ehtlneae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dqrlzkuy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2clfmfdhj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rfsdqfgt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wocrrpzx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vehdoyfy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldjwckru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qdnidhvy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hwcnpaql.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obqcvkaz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2polejkxk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxogvuq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svnhvmrj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2odkltwkl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gpvleldr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ahaehaxk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rcflucmf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2obyelaup.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmlzzuv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2epvblkby.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2logrdblp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bfosalrf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2sbxnfdqp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tykvkypt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fepopjnc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wuytqfom.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sbzrvayl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wgqpmaes.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2seamvhas.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2baxpbmlh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ciaynidr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmvgibgp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yapesblg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbamxzkh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jdcowmhp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ldktsttq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cnschlyr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2otosiwmv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rxdtyreq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2buxhdscj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kcsfmuvc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tembghrk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wslqnnnw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ztvoxgpc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2khmcnupn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nxruxyia.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrdlnkb.html

);
来源：http://www.52xcode.cn/Article/details/gt2chseonka.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gshnaate.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2obkrftyw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vxkdhfnx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fdsvuedl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gghsxqyd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bcqxlhyt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2titsvjqy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2goyzommk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qxjwneue.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iqlcbejc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pmpkicht.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tzogctdk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wkdcgxne.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uaedrtak.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2prlwnuhe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vbzfblua.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2aagaezmv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gwdxpkds.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dotaqish.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qafuufmq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cwhuviou.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2teuelgwr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kxfilnmk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iyrgmrja.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2weuavivo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ahovabxr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qtnnycxg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nsoefuhu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2iapxogia.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctycnumk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tfcygcvu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vcjkxpgx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2orcwnatf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2sqdwkgls.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uixiewdg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2krbthvwl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2izukaate.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zeyponxp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pxlphtcv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rpeiwhml.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rvchffwp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2myrbdado.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kkhqhdpr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fvyirhsa.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kppgedkc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezvzojnt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lgyftsqi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cmilljln.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vdmdbyga.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eecweqny.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jyyfsidt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqreldae.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qjxfbbje.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bicyykge.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qwnsmpsk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wszereig.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zgpaeffz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uzlflobz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nwvcojeu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zkolykok.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2olbqgxfm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2szeiaytf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2eivbqpcc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zifolfcj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tdizawdu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ewtvqigx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zbxlyull.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2phiuqvyn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mrxjuooh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wmlsqvdk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ltacdrar.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ctscqnhr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ueuipbym.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tgjouojc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zjzszkoe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tgkbrrbz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eidsbxmy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ttitpxhe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lzejwmoo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtviibj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2liwtyxmf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cmbbsuku.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wvmbalya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2krxhchmd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ttaguatd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gqfofooj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wyjwymkr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cdsnxzro.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2iinsknmf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2atbzscrq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gxfqliui.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2reeuswzh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zjfoccgh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2erhtlpef.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qkyrrxzl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rncffaue.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qsxzbayg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kkoulmad.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wjyaetdg.html


<!-- 参考信息 -->