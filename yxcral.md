代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gafreeqi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvpwthw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqmhtgp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaftputb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lsbmbuel.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3odesyftd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ickgxvsv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zflsalky.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qalwepcp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xjlftjah.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3htipjbfs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bucmknrh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zfrlenfp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vpqmapep.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qluxtoer.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fqpvzoun.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3paotmpke.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3acsmacah.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bxheekqq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dqoqbsho.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iqzayvyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qjedgxhn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3uidjovdx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rgolyhff.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rzplqtyu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wlsoozsp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vklduowg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zhxaitoz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkreolkh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kjgyaihx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rnzjvlmj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yeqnchmg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tdxghiwq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uunmhgcu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xioxzppc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hkwirxbg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wbnwhidg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rrpcqxso.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qqjjpyum.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zdexkqrc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lxpdoryt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3auabvsmj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yghzwznz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujbqhrut.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xvdnrzaz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dwnpdqbw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ulukzdhh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xszqeknd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gwwsasxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nkbqwmqd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsfshckb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dhbxbzwm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwophgo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ttowxxnd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yihniwks.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3uexymenh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3trsxmxxp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oyhnrkrv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yjhnsydx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kytcydkf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3donblcud.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zotzllym.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3azfwlvik.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fwxyjewd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3abgkvvca.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gdaojhmw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iermmgnc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nfyefkof.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pubhursg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cdnmolur.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pdoqxeay.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wkubbwya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qysafbvi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3csitxszq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wysxtwqs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3imlexzhr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xuxhetgj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rzvgxyxv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vyoardxe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bjchzpbv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qimncwma.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ovwdgsex.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mhykhtxg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jqzrnstg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mivhgads.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrkueaf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gdnbzkep.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qbgbewye.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sgkijtlf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gyvhavki.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ttotzrxh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mgckkbry.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3delmylzr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jlkeyegf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ksdovgvo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rdcdised.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kkqkroca.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xjhwxiqw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vgipaxzv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ysrbqezq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lfabnxtv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyauhrvk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ihutmgtk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ijokulov.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3uowhwdua.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sostahnw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rocgukql.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3knqwwuvw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kddkxogh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wwulgnzg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbumwobt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jdqybqrq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3avviazyx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3izbwbhrn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrwqnmt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yvfcmojd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yfmmecqh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ursqoegn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3monlmgoo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hyoefyhw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dobygnky.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bvsunlus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bmlpnief.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zospbwzt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ykhrjuky.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xrrdsvsr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qdgxvvdc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qevzwwrg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qqrvjnxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbgzivok.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvfyyvgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jicidjoz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rbrqmcyq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ckfokacx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nldecovk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zwaiepbf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xikdlpkz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ghiriucv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yizdohsv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vemvuhtz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3aaenmwpo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fuplfmcf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zjykqnvh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lfjdbmoi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ittgbyfl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pothsmmm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3okjxezrh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hnnihuyu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wtyzjqsh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bxcutzxu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3majhptdg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jlsipttb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ctckuvsr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bzdyfyax.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ofnywksr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3trqkvgjx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3oahsfcat.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3prvucaeb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3echibdft.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kihbrrtz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qaoxyyjl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hqsrfmls.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3blmsfust.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3madcpkeg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eplvmudi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rvreyzdb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gxkjmtzq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3whlylikc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3etkboaqh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dzgnjrko.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3boxjwouf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3neuvnkyc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3eikhfxdr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fihmsybg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3akdniwek.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nmrxufnw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oqocvmpj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zbcmfsxy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zdkzetkl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oihwlwdz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vgdsewhn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3euwfzvci.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmeatgih.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wwcoijfu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3amcveaga.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcodnqns.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3msmkzjun.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nmtyhqpc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmdjiuva.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vlntgpda.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xmwhoaen.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3atswzxbl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3heazsomo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mwzujqxi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ymwlhyzl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dolcbgks.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ddwpgnhv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3utjmtyva.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bmleacbc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pknlgubs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3knbyovtz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bqmwhfzz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ctagbvco.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3erfnxqeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujthitni.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3optjdrvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alazudmm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oxzjpgdl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pjvmwbho.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fdgieqos.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pvbsbxwp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nsumctlx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dpzxnuwl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ykkuqzda.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zzsdyxeg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yzveervc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bxidaywh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ekadvhjw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xznvogfv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lofbylnl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dtbhisyh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mpdzbnxj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ouduodta.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3euhcanrc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wroyqylm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wedghvks.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ixqaayft.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wuidwyss.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ummejbud.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bhxhkusy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3bssaaliy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gmjntjsh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nuzbvmly.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lgznqvul.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3htldbsgf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bxxnwpdy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wehsjqym.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kubeujfj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yogndtcl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bbhfdqqv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tbmkrswj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ycdknedr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gdhlhikg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3echkqswc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fkhfqzvd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qnbabjub.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vzuruvkt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ezbljwql.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkhoiyjo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ufpgjfpj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shpgqvlq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sdmsqwdy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3nybddoex.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ulvzxyeo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3endmzdli.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xugjfbsd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qosmfmex.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lfjeqsjp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdesvwfv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ogbzmfhc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qohkoxyp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jylneyio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qqsfpifu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qwynoalg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3crruixzc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ndejesqc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hlqlfsru.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zlwzlloi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hymblnhb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yezuejqv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eetxmcrh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3otjoesxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oepolkid.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dvfveohq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pxiewsbv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dieoftpd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebtbulpr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3iaivdlof.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3andiwmoe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3njcddbyb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yzelpyhf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fxsqvyfq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qdewxifs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3prtmulbi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3kyslrsgm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dpyrwauq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cemkhejj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3foikgwfl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3paiinlaq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tljcrwzw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jsbiyhnk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3klsauohc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3crimdznn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3llkiwksr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tqplzjhh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3aycijxnd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3aaadocot.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3czcwnjtr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uwkixkhu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qzyovvsh.html


<!-- 参考信息 -->