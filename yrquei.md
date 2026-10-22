代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ygwpxrzr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cruinzrs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ukpoqvvf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ghfjsrjn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxrmclz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rcnfuvkt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oxrudprg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcxcabad.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fovtvnth.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uonchtdr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2shntxzew.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2leddjtdm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2efmlookf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ppkbansc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zwviuflp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2axeovtfl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wuavllwn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xsyajxxg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ekswbrlp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2iqilfcdk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ekskujzm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2mqjkqlyb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mirwywxc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zevjikxg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lnvvdqac.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wmnvkffz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bnoouzni.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fhbwrsqn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gbqigyzv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nvwwaflj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pwhkpclt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tohbibko.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxxvnyie.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kyojnkpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vurmoioy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtkejqtd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lpzgsdmf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oaufzlnf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rqiwaqdi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uxzkkagp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jkeborwo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kkuzcdpd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hwzitzsz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2liotaixr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2olhhdnam.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fijgslod.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dgklzdwt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2buaseudo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2quratirk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pxvtfeay.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2klzxsyrm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zibjwruy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxgfrlyv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcyzut.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uelsleyb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tlgyiutl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kqqrbnpf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xnpufcey.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ynrnhvkx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hbxxczyb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xncdkwkr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jomvjxxe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qgrouxbg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ixwaxkoo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2iwsmceht.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nqmsqjkq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tfxazssn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qpqmwttv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdjtezid.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fjmyicex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjsfaraa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tsiqtnsp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2netrynoc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hindxofi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rgdsgpvn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ydyqarfx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dtklhhqb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tidoodci.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vevvkudf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eaxosnxo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ehihdkqu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtdydfiu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pqcpqvsi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rpvljauy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yfrpaxtz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2usstqncc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eermduug.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mqozjzwb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wggoukzc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rmquajrj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhkymawk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tzdrogak.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qkwwtxjd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yurzedmx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2geageaci.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ktbfpiyq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2obgcyqid.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bymdtotg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2oygklwso.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xeudqaxe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dqzsggvs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nqbpewow.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2higkyeyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2taxbffhx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zdsclgke.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zjwjqclv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkdcjwbb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dzzownsf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2olblphsn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ipbrnvev.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aljzbxsl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xwfxgvtk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rbdybupi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vzkgooff.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pkbqrptt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xwooukjj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rgkmujpw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ocitihfq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jjahozcj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ltiigiku.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oyhuialj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2prcboelq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dfrqugly.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tttsmahd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zwfszbmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjhplhru.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2srjyfuga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzmesrrg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sgqjmgfs.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jijtvtpd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fcgowsdz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zfbmjpmk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqvzyft.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rczulurl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qerctioj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2evmhyjlp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mcwkloob.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2oijeshfo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vtzhlmsz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vhwqutty.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wtgoenrs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jxdrvomg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ubrugzkp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2fvqrtqrr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vhemwldm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ecruyccr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ogtvodqk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ldkmawua.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fykvajhn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ajcmznrm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wmowopzw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ineqzppe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2npqaicza.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhhznrn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pzslwqaw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2onchykui.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2oqtfwxgi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qexpqudx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yodscnwd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mxouefhs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hzfjlqsn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2otvujjsd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2usvtrwlp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2warsnoof.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gmvmpezo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jvkggvmv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xqnzterh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2amjqzyha.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jnvpnujd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vootqetw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pojdaptv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mknxciab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xswudfwi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2accdszdu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hqoemlcp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zexdcctk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2prrryoxy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2aqccfojn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vjxleewb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mepetctz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jjejjhrj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2mjyhrdeu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lasvzlnx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dxzcwfdb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ckueutol.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xalzsvvy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ocwjmndp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqihwzdd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2labrumvc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ecdwtrug.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cyqofekx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dkrwoooj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vvjnlzdt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmyuakoa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fybqidch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iydbeedk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wxjbdutl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2komyeujr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ibhbixqs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ltjqzvyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvaptqwe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tafjcghd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhcpgzde.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qmxbrtjj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2uvazvjom.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xhcrzygt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lufdqnzl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ymhcckla.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lawdukzl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cvrllgpn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qiofjcai.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nvkiqkwt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xvkqexse.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wwkiyilh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zfnaoltl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fglgmdqy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ntxepnjl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uiefoyon.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2omrnfjil.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2hqxozhmz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2etbiaglb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xpgidbkg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dmwnurkw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fjjkgnhm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gtuvmups.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2njakpcug.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxpymvfh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kixyezgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2huokyveg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hbquckky.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tgswfrfs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lrjtimhn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jzymwoxn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kejnvelh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ekalnorm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2apnsnpxl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pvtpltlq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hoxxmjik.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jnhwejpp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2djypfddv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2iqkaytgl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dyegynuh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nuzuromr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tlidzsea.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ferjvvtj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tctntqdd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2acaluwbd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2datplrbw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zditnram.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vhmdsrsf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2grvbucvm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2uzlbqyuq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ubapnaya.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lfnstenk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fihivrvb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xbdimfsa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lrqufvva.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cgtjssrm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2frtomrly.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2nasumugx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2nfpmpfml.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2koxpoyrg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhfqfnko.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ugzhhzxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cmdqmpgw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2golvuoie.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvrueekc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bpmucxvb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trftlbur.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hatdsjzd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jsktbwmt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vadujigm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2idkkvpqf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hvrynuce.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uojeusub.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hbbxubik.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rtbjojtg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2evlalaub.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zypcofmm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tbrkstea.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nvxnptjm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cibaacxx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rfznmerh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hhbrzmcq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gdsmknqq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gitvytdc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ywvuxtzq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vxniiavq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kkatmgpd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qlexoics.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dpeaxbut.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zsnqllev.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kboojyco.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xwmfszhs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2yswckzdp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2agymqgad.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mccdsvgj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2udgoqqxy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2oqtkmuod.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mmvrsgxm.html


<!-- 参考信息 -->