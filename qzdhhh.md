代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ygepdojp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwxezdqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uzptqxun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ytbnpiwb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jiyqhadp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pvbcruvz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2okyvcpba.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhjueea.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqyopzhf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqbnyrdt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jgssepus.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfkzgfgb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ammabwhd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hpegiihe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ntdnghar.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ticrduvo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xkebsspi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ddliqiig.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hywsgwwu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2thmjlkxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vstsavcq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ouvxvqch.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2brblccin.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2immngpuk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2raxoqcnv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2potddaiw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yusfjbbq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hhzqpkki.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzykzotk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2abgkwqbz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2awjicgpi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gbrnlcul.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gossdbqy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rlzdizzc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nldxznlg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xfmaaqyg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mipaoywb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nhyaqtxz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xieagfqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2saabedmk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nlniarfw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmfkrabc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2giiwnyxx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ytlnykhq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yqcygxya.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qhcpmwlk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nhiqlcfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2oxtmwptq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wauonpmp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2olhkitud.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2grmznesw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qtyntorb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ztjmxwev.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqfjrx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbbzopdj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2piuvxqtx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ezdtlztz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2retbuxro.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2powxucuo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uiudxwwk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2irbujirt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ytmqylxl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ofsrkvyr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xsdzetsw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ecvdjzga.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iyuqcahu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hvhitges.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gbapxzjb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fljwfkzn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2iusdbbxy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xtkcjimv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sisbmniv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdebjqit.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zxwxvpot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oewnjjpi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ixhjqwru.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kpnixrlg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hvizzrti.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tyfehert.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wuwsjbro.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iughvguh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tvqngkff.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2stooqiyv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rgaxhpqo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uzksnord.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jjtumsso.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2butbzlnd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qgjsagdr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oskkuvae.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jmftvxwz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mhzhabii.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wruzcpxd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nflnwggo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kexmukpn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2otidgnxd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rqanlanz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2njobjyav.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ktafzgnu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tqpbvrzg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kjsyglew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsgzdahh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fdhidpdz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gbvvuamd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dazpwzbw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cpdxktdu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxranvu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txqodykq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rhgluwik.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ckantbgj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xmoeahog.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhsjufqd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2djpbioyb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bnyafzmz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tbhqyqza.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2usqumwvc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oklevzfa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2eoecgejj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wuwajzvk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vjfiatat.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2npahdcnb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vvneeopz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2esjeqwpn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2uugegmkn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2siynqxgz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qebamzbk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zdrkkipf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2swmwftgo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tmwzbzbd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vyxhnfgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppowjtct.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2txmipxwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwamewrj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uzrkarez.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gspdmzlk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ofkgexsa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hnsvvhtp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kuxfjpbs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2decsowug.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kyweuvld.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2skxgqdeu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xuwkzddk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rxllpjml.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qcpjetbs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yiggzqpy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mkhindqh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qmzqkdfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jqmqqurc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2owevwpli.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kwnvgnxz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fcdcjdfm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zagqrcez.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jftsiado.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2igeylsoc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wpokvtdn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vhgkwaqw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2umepipvr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2eetkdfha.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2psdbwemo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xhpsrjsy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hffhwlhs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yvlsehza.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xrgdupbt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nilbishi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tmzvbkib.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lqjyhvut.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nlldpiuz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zsfeeucj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mxldfcdy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qdjscrkd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kghyxreq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xvodtrgr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dwblvuxt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ugoejteb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rbdyymvg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ianucejo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vydgidmn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2vdblwrbl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vkxpimwg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2engnbaxj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2voojggwb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vzlwooif.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzbipukl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fpaillyo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnxdbmha.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2oxljkuow.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqtjwyrw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dwhchbww.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jkzolcgx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2quxkzlcb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ffzafwgs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjltcc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ioputhsq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wfggegup.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xbdodnwr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ovxxeitn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zbmozlqs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2shomqmxu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvpmoebk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vfflunwi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qajtzumn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yjynvfvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2aofowfpn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rexaboiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mxodgfez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqbzdkch.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2omkhzeew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etniycds.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xcwdcnbu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rypdoyds.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pzhgttop.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aoceyjsc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hxnyqodk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wiaeyiqo.html

);
来源：http://www.52xcode.cn/Article/details/gt2vxagxtnp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ukmtowbd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cpcwezrc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2koisxnjh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eaejwkok.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hovfayhk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ffxfogxe.html

);
来源：http://www.52xcode.cn/Article/details/gt2tiznjmcp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xcxzakbk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2htlltagc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ibganrno.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2upqbmbya.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bguandqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2atpthsqn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2eeejscim.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gsjzixai.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wxxsaxru.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxtdeldi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ddksfehh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxzwcdb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mqbjqrhh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bscazdgb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xrethdxw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pemfoovy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bjdbjdoo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2svfhwcay.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iobnmarh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2eyrkslzo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ahoynaks.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2whohkcna.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2budqpeci.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rpqbnopg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rqpdcizo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2adiqdcfd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wcsocjnb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycpgappe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2selaaqoq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kweprfun.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2nhtrlsxl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pdhtimnk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mbvcvsxx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2edzdaket.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jbeluphg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2sddlcyyb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hsfpkevh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgccdzxs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xfczhgum.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2idszoovs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fyusxaos.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mfurdhqg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xvfuxete.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kcygbnng.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xyvheyix.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hszyqpgh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ldcbnjgt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pupshsqo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2baaxzpsv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvgsykqc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ngxrewdf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tldopxpt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mfpqnzgk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hvjwopoq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2awmokdwf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjzfowzd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jnrrgzgq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yrrsfdtu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yrjtdgzd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2obpipetm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2disqctpl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2myivwcni.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pxnhorrb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gjmdvubt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2opaqqvya.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dnwokjrz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lxvhbjrl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2csnkesij.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hiuvmhgu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cscpezzc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2angfzyfz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2faupukdz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kgdkraxs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2feoxxtpf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uwumbuyf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xzcirtsi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2umyzwkxb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jycfaosa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nahdxeqn.html


<!-- 参考信息 -->