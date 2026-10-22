代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2altuysgh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2thehxtpt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tlsxsims.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uxxlnwan.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2altyomfc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jvnjvfuk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hiecuqij.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxxfeddg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqoocfqu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qyxrdosv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2crjnnnjz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2giawnxyl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vemxkxuy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eeigiqdz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tvxzfdjk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wzutkcsc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jvfmugfy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tbuwgclp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rldijgmv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ncslmyvt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wnhomogk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lhpempqd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uxrsdjet.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2byltkfsi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mqkoxxkv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wpawjaoe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2byqifsgy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qxtgrwaq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2etsyunzu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tmeolmcx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrrtqzxt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wyskhzjg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kejwrcdu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bncberkp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nkeyoevq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yuvdidqm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gizaecti.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qdbnvumd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lldxzbam.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdahfwgp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gwjtfcvm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2asqfzapn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2oluncpmu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qnehnnpk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2imotmbtc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2acvxkofn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pmmlnoxh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wdigmnwt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lnefgubu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jewbwltg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuoiawqk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hwglktss.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cyyuesvx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpamifd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lvwmwmlj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nziktxqd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gnweetca.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hxuagqqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2adfmmfil.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qgvapcgp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zdzbgupx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pqrtsojm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzlzkaja.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hfdloeyr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lxgpipbw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2skzozlsn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rrapflnw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oztrqrgt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rjuukhdw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbqasazl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmhxeth.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mpgstdkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksxmpvtr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xxrzausk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znmwudua.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bzsmtomu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xqfcraee.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2emvlwfxd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ammqnckx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qhqwmiai.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bitmvebz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gkywersh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ghpclvhn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xnzbxozy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yhzufdxi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yonoanqz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2exftsvlk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2chaermrk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2drfjviad.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wglfgxne.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aadawkfe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yvvfujpi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2axijprgz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qwmzeuzl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eyqsaxfp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xeakqzyx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2unelrtoz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ugeyerle.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2njlrkqlh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hncpbckl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ykciwjwh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eemkfndc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tyiscecz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vpeawovt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yzxilrfy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cxoztnwl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tyshtdeu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kohbdycn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ccqpiyvp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lrqgheml.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoowxdne.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2njunbrar.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2owdhzshm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2reboufka.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxochk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vvkjozrn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2inflevbv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2gnqqzfpi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iokweouk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yhrgzzzt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uarcdrbg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2sqcmufbv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2aemacjks.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2akkecjna.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bqoohqje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vsznkzkg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zruoziqt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vcdjucgn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fxwcfcep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afjlppsb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bigwqrpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axsgrnfu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pptwfidr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2piupudxv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2djehgrwd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vcdjfcvz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ryphfbbl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ragjxlhk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pucisrby.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jytovrpp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ojqhzpgp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zypqwmwx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pohtdszu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mroqmnyj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jjsoelbk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wbuaagev.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ullgkike.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oajgwpez.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vddqwzhh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wkmuutwp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dlldslwd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zxpvyacp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qaeahgys.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2midwjvwu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxzczsmm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ocuoqmhz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cmgrztpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkoqeeg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zunrlygw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lrcztpot.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cjqbyglv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2byccywuz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tvdduobd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ezapsgum.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nsvgvlec.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rbiaedxc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2izajumez.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lafvjgjd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2climcntv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ehnccaod.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gaidivwf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2faqtwnug.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bhifanok.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yclbcyha.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ekmkazux.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2smniwqay.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ektvzodg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vaieqtco.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qepspudw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2appgbvtz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qzxbipbd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2puzwilfy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aviluqth.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2utvdcemk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2kjpegktq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htvavjxz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2klanclot.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2caalxtdw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fzkjwiko.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tystbgwd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jrthcrnz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqezokly.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xdabozsr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cmtgxdyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2cnvqaiwk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ugbzcysk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2epoxeibo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xzxnueoy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wbfllebb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2shaoekud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dgayjqeg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2abrdrbkp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2efrmqucx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2naqqugqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwffctuh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2axicqwzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dahgvvkd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mndnbrrl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wzyrqpkg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bdvxqauj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lvbwszbn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cxxefgjq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2sybyhzcu.html

);
来源：http://www.52xcode.cn/Article/details/gt2ejqglose.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zhubrcvm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cekwjlto.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pfxxyetj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ilbyefuf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2akogvdkt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kclzrfgt.html

);
来源：http://www.52xcode.cn/Article/details/gt2nfanuell.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ploutpus.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2honfmdgh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wwovgvzk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2stjrzrid.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lndlvcym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2nbfyojdb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wyvjappf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lryotrvj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2quocbidt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gjtmrkqs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2asubusnx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xjlxtkht.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vsbmcafz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ygwqiebg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nqvhwsbq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hjorxoah.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mvtqxjzy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zbqjjenm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bcztofia.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gduwikoi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2joedlgyj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xoeptyrb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2njhlrzle.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ayprrotq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pkzghnmb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hufppgji.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ylggqpks.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikebjjtg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nihlfzwm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlgkljxd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ncoeycfa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2arscmyjw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2erjfnhrh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ootxckkz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dqihmdlq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jdnknanb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2loxcieru.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zpjrxtqx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gibdowfb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2diwokkwi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rjpsazop.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwpskii.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tvxqyjea.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hbwfrrpj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rvzyefnu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mivursxe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ghrddpau.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kceacrhz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xtnhgyye.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhpmdgxr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jyicybgt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxvuik.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kesevxmw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bencfxdh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bypkidxf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pofcjmsz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2repaurle.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eamldezb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ugsfiuoz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rbqyzcbp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pivqqueu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2srewtiij.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hhbcsfwi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2iffkzkqu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ojbzphcs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wiexlxdx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xommbeab.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2syzemoyu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fodgctie.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wiurmjsz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2psljlqpw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2moffxhtw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2akematia.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qszjqhcj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xpwdbgji.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2iqiulwim.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wwtjghci.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nnmuwsqb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2endtanfl.html


<!-- 参考信息 -->