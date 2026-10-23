代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fklgukif.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zcewcbeq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cygejuzp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3betyupwx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yfztvsnc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3juwvzwiz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3somtbmze.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sfauueuk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vcwlfydk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zazbjwjn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xxmwfsvs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pdukdtty.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3peulvrqi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3euvjpcau.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gfetctld.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zhkskuha.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwvorwtc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmwuqszo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ykrthcxs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vbleltbk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ykmnbmpl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kgkybrop.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3djsgehcr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bzmqrvek.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vimhpvog.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3nxghrhgz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cmmjuwof.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mqafexmc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lrtsnkgz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jwxesljq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ycdyteyk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bcocjqhb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bzfzmyni.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cporsuck.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3brkhwjeo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nwtjyznh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3yaxibegi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3azwisvyn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vimrmmzk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrvntawr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sgpkxfvd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3shpptilr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ydwfrpef.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ncszfnqx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gbrlmqae.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3thowvgtg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qlkmiytv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ztlsgffy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kfgyqomw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fosvchqc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lomxgyrf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ecmmemui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlccbgxi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tslpdvog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blmkdfxw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dzgdqiwm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gauwjpkx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gpilcyvt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ulwzoumu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jklviagv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kbhdgtwo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gseqmhym.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3awtyotah.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3kpmqcjzt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mbsqgpzd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xxonixrw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3oxvkxxos.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bgwszdvv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yrxqvcqj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bclehimk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ybqbsjti.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mmsjlqjv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nvduwqoi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wlrwbuzr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3opjuxlzv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sfdfaqpj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tkzahrch.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lqrczret.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmkhpdk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zyhtqvga.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ktpbakbk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxnydhp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ozhghcem.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3aqitrydg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fchdobop.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugaqixlt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxcuoqug.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jzpgpzyg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mhngmday.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ovvjtypt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gwpedkjb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kwfymwzh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wzayfolb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qjneaxuh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pbziidsy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bffpwmfn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3eyebgjrs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rucvmfbr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ihjkatqf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcdigwd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3luimhbzs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qqjdccnm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yhluokqk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pzjadocm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xljcbyhj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xvqtoxiq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gwqviiwr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3aezfjwwv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zcaumzkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rthbhklx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3uhuzuijy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnvljaan.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kvambzty.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bqfmczau.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mlbxvwnd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hdhupbhh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vumdtflf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xsxebqsy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3afvndvdu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pftbuwbe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vctavfch.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cdtrwydc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xuciigxt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qxzcjqhr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zslawfqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xiwqsvud.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uywhplgt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3iztdhoyq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azcmslgu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3kffhsqar.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dsuqxxjt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mhsdbwuf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mwbmcigv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hkbglvkk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qwtlcgli.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3klpqpcdg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pgilwfyz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lpnlbzxg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ysthykmr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bmoqzkhu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3obxzbwin.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3osnxboat.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bobzraih.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gaaumjbg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zoktkbrk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vrwbzmyr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eowsipbr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tjcxmkgh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3maptgtnh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gijrscib.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wzmdzuuu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qtsvvxdn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqntbxbs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pulfpkwc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cibbuxut.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cwpeodgr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xgbpvdct.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3euhwcids.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rdpuxoqb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3haenhdhb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rnryyege.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zfjsjffd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgmhqqdu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwzihzfk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbltbvq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xabnipbp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3uwkvmwle.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gjqmhjfh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xkvoizrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gfdjodnw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3frdkkxnw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxovqkdj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yviakwcn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bzvhbtid.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mbpinzro.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3meulsndd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cswmclbr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zcrseukl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ahqiglxz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtlmjfig.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3huclnmwb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3paoodxhx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rihuglpb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mebbxubm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlypmntk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3olrsjpwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edexngvs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qyxlzvmi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3netqykvl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nqsunoce.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3imagpozp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ippnpucd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3eoiafygk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nkicbifv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3uvrfbdri.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fezelwal.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jfhpwbrl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tghjmuwn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rkhgxjsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bkepcpwf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mvhvrdev.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kwyvimvd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3flsvcxcw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ftzwmybf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hntakgtq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mjodmonv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nuguckec.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3miplotex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ydqhgmwl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dnhnnjxp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ayhqegda.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jivsewqx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gqkdnkwk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3hklrrggo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3osajakht.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gmfgeyoy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xfqgacqw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3sdawboqp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ihdhfqsc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zgrvhwhc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ujsfdlld.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3brkxhmvw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qpvsxxkv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fczolsao.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jjmevqlz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bnqkuomb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jbsdbwzg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3quwohchl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ciuqzcjj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qgnkgihk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgjhwtyv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xcmrbial.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yawavwso.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kzubmhtk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lffxxtph.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rmmazeni.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rqxpzbrd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3prrqszdy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3iljjhcwd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ltpvsvvt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ywgmfwdx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3djwedngh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3owjtewbi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dcmxdcvi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3mkdpzidb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3iramqgqw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcqaogor.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xkxebtbr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hlrgcgyt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yhwpoucn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdzwscdc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3piolrcus.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muuvsdkp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lguzbyfy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xkvnnisx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zaxecnyh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uxgqdfiy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3uakhtwbz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3plaxjoyt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nfeaavej.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3faqlywwi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fbiuqift.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xlhsxnew.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qsrupohr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kyarkmua.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3faifvmsw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gxnwwfiy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3epaynrtf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3upikgvil.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nweigxdo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jnchylae.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bajlolen.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pclimvcb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eprjkgua.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gybfwizs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lckppamv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xswxgecd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zksyokwb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zoeiarou.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jfifgdjp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mdpirclo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rellqanh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3sjiniofn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dfvjcgpd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jqecbhrq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jdrluvak.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hrdzdoax.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nbrgydir.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dwenxqvr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fsavrxke.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cnpzcgbp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xwfiakmq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lxpstudj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cjvhcvnz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gaqvrkqj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cuatgyso.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mtrdqqfk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dzmqlilf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nkqgjvfq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dxjlieyw.html


<!-- 参考信息 -->