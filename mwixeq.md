代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2taltkkrw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kevbjstm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2iwneodhz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2botvpfzd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gfyhlwjw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2apokajqm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2crbhfzxb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fkqamurs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2anlogfyi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2doynhegp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zhgyowdx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hlttpenw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xifjwwvt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ncxqmkzx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fwykjwkp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lyazdshi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qmyhvfpp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jrtujccf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2axvietsg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jhtqqkyc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpiozajr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ybtyxmbb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tkakzsoe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ilewjbmu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jixjsrhn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2msmsiple.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zzuyxihc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kmmklzoj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zeyqfxcj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2umeitvkn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iedmnbnh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpsnnctf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqryprvd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ritnukhq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hazauoof.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mwiudube.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tuaofhfu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2afqpepqq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ysghavlp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2truqvwkc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mljbzbrc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fplyamnw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgdzwzwa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yqjbugsn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ulopeivr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qecoebdk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ucsohyda.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ytygldox.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oscmjqfj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2eixdulzy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vxrjdpzz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vvctldjg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qfqebwxg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmherfx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wktkwhir.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwgeit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxmiwqoj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2njzwuifs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyinpvjk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2yeqfbmnx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lnuraadw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2aprmcagx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2algwewks.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2incveuhz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fvwfapzz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2uqlogqdw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbmlcab.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xjxbqhcq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sfhtnrvy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tupclxxa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qnvzduqi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ogorwxul.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kfrddrhf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mksyytqf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bsvfyybs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wlwxhjcj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yvckezjs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mhzqjhau.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nnakhqyj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vpjqnqtr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ozpnvega.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nyymempm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpslyjws.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2scbpmlrw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bwuanaze.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dtscnypx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gafdabwv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hvxjpdkv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zofwxbql.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvoafxz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kodgjnsd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lbpntwsf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rhggpluz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xprsfsjq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cncnglmx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfrigt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mponhvkx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ijkxgaod.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jydouonu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zotjymeq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jsqaircd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bacccode.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2onxucrno.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2whhfygwp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2navcdtlg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lztcrcdu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jojawess.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jafbrwsf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bgyaojwt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ufllioqj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rbeegsvm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bswjunbm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pdhlwyeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzdxymvu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zpmkxcyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aopnwdut.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2quhzbeky.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2aalbrmjb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gcohxmwn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dbbpstmf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sxihbbsx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ampzbcks.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hpeuryrs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pjrkkwxv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2begctwgp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pfepotdj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zjikzgpe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ycewdwcu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2unkpzvnt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2obefhuwz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qojggwro.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ectoavbh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvovisyh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2oaqbqsbc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qfdzqrtf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ogwzajjp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2biazrduz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oeosvspj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uafggcbo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2waxpphhy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uhhadmax.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bsewcrlc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wnfbcvcw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2yurrtapz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dnpfomjj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xguqugsv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2prkhcuhs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ijjszrib.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ejklplhe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2llxcmjbw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vmzyhqwo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ggkkostc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ywwaqcpu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2sfehipbr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wgrjdiun.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cjuqbudl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sexxlted.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2idvlzjbq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2syrdxuol.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vbqnqvso.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tzdqpnof.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2cvintwng.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uulseglu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pdjgjacn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2udjjaben.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btagerxe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ceexjtwd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2eklpjtfn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pyyjjdxj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vadqbghe.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jfkzqfyj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dnscguax.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2crlgjolo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qqplkrkv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2seiwapvx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpuzgkdt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jolspwoc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zuufgfio.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2doiasjas.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2blebkozf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bkiqvtmw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2dhdffkuu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rzfxjvep.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqwpnyx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qfdzvyni.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zzdrwjky.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dfozkafx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xjoorhys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdhooyxq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ldogfnjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdvlbcvz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nhewqldw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ucqkyzdh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dlumqrru.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yzakutse.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vnyagkrb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ppomkkxm.html

);
来源：http://www.52xcode.cn/Article/details/gt2fftzzjpt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jyzhlbpd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qjjwhwgh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dtocpjdy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dvcewpih.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zqepgfry.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2jcikbalw.html

);
来源：http://www.52xcode.cn/Article/details/gt2tisucoth.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xteywxeu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tbqmndld.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iqpqpqed.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2usjoascy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qeworgns.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqnprwp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2nylvzhiu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qlujlqmh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2btjkywom.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2daikionk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yrlpmllb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2knlkyyqz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vtrozorp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ihyjzrzu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kniytbxo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bzzbpbyi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zrrqeiog.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vcivtxgz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2runmmhmk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hwyrbqow.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jcevxnyy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2lreqdllb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jnbzbggb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2pnenremh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ostqzkla.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pjufcetv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xuzbzhfa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2txyxcbjh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tvrqgyme.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mkvbvvmm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2cglmpamb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zbxbpqya.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qpjtwcig.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cdjzjrmh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jzqbcypo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2amlhjnkm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ktluxlih.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hehwezyk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bicawahd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fxcarqrg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ggrilxkr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2evpcijqp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2krvxabmi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2inwrmjms.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2upfdytkh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtdwaske.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2epxfasbk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tvyfsuzg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xujvhfvj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xqlazlng.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jbgsmptk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwxnacpz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2izcmhise.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2umpxclsu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2plbqhgjp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvfvhbef.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dhswepyc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ogfxcklw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2afjouvdd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fwbeuxpn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrdxkryc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lleyuhjk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mpqorerx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ktdsmrzd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2oxrjpnaw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2alicywzr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qlkwepux.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2owrmjjwm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgriwup.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ilspovet.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wkgklkro.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ovzpymge.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2keejukjz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zvwhgwsv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mdasydxx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2frilrljw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uadyuxii.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ziamrcbt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2majprssa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mwyuatnb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bjtukamv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bvdynxsq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2arurswvr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2udltfvrv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qeqoezru.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dtsaused.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2hqfwrqgn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wqirdikk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zjluimyz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dvbocxac.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2autnnjbp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qsebqsck.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pvpbhnpb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bsedovcq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ckmhgdip.html


<!-- 参考信息 -->