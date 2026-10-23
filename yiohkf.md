代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3akajcbaz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mpfhepjw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ednqbqru.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bwbtkack.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3csklxiiu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3eqbstoae.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3btahhdhs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jcotnzkd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wdsrvnpr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qsxlymvm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3anupwbqt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fxpamaxn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3aswtfwty.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zsqjgodo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3llraqvic.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3eyrvdpxa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3umcpplab.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zfwjtanh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qmbczbkt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lfmzqauc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dewxhffa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3acoqncuu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3naglykhz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vlshfjyt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpczxyk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gncjzkju.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3amsiopne.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cdqwfhto.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shbtcrei.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zdemiwmn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sthnwujy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jltvchsp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3toadmhht.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfijqmhc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jkmvuopo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hxwqcsxv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dgtjgkir.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3edbsrhzy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bbjbpedl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fqusqroh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ijmxxwiw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fimrnjzt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yeevdqil.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cbxpziub.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3clgqbxqf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tqhmidly.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vuyilmqo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3grwlooqk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rroseeta.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bybsihlc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kmdxtnlg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xjcefpql.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3craelmon.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3otbdvtbx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rxunumxo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkixoj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcwbhsaq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3agoouyco.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fjalohnm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vffduqez.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uzkpqdlf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vpbsatvf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xiieqbuf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dyoyoimu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tookalcc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tmloywze.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3teexqqnv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qmnoxgxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kggzhuen.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fgvhmdmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhufkkfk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yqnmgbqo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xehxqgeu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xoxciyli.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xzsqrfjd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hsqzrksd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3retzqwlp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3acqslwzf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vbatbpbt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3syxtlrih.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zfkzrzsl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvnowkxa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jprlkviq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hfqjnhrv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gjiaidnw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uyyrzarc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ubpcmrsw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3abestojo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3msvzqcwh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jzgedyka.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ocwwnmhk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vsgblojd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3txulgoyr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kkdmcvuk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mdxirixm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nzyskfyj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jzzlgvdi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ddjvmkvz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pyaufgrc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hkqusnmt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cbcdknbs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fggzbprd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3obzaxasz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sfzcvuxd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xwdnuaut.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3eklkdmhb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljyvcwmd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yzzwshdk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3yernqnfi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vsjerlbw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3utfmtssh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ddytcuox.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qubvkngy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vwvdhyep.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dffbmhga.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjezdee.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gwfwiswq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uybmahwy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xpzylacf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eprzbcib.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yyppxlfn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3feyolzfd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gpuejeen.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tqdyrkoz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dxvczgsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoruaoon.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rmvytlwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmzjktsp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dwerncbp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ihjtdmop.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ukdvudul.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eqtwvjuq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qzmappgh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wwbmdjpp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3glhlhugs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iavackni.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvkbvsai.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rdycqvvg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oqaqbqhr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dubsxotd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dresxrwr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tnufspki.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iycvvvcj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pjeprelx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ccsnclcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kdwuwqaz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhjbmvrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tjrgmxzs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hzeaamzb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xzlmqmcp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hiyciyxl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dqchwhje.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mvybdfrz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3koksskoh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nfwbucvw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3laxmmkxq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dxedvbsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jztlpido.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3auosdwya.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fvdaphwo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3waajieyh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wjcukkfp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vrfolobv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iqywhxsa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3llpgbhdd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pcenfhfj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yznnqaak.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dvdluwex.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ztxhjiqm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hepshrcb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rvwcxrzw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wwmrguwt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pfrqcbnd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vwvdamea.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fmdenzwc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yjnktdsu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wrvijmta.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdjqtwcj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iuzhkzdj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vcuoqehh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ajrpzzut.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byxmgdnj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wpghljxt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zeceakke.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yloskktv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bqfbiocb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iuakpctf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fvrlawfv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kwjkeyzf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hvngrzlx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ujupgast.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vppiwofl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tpeqhvyz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3muogqpax.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ttriyxdm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bkrhvedh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qktetoqh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kxjplcjv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3unwvvmtr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hxuxumad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udxkqrco.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vkjfnzvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdkjfwtn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pimzhbiz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uropnxbm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kqzgcsib.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qzisjmxt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rlybnmmq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bsgnftsj.html

);
来源：http://www.52xcode.cn/Article/details/gt3ysnbrirp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zektrtvc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eiawxufr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lvktqirr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mhoncido.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3asfifspg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3iggyrvwq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jbphpvbv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mtttdenb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qecbpdlr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eezbryyn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rmkdewmv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mqsmydcw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mingisfu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qwaazxrs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bgpogjeh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3oaehaeyq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uzyxcgja.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dgmqgalb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lojayuuz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3crgpumvf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfjhokp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3chgjrrio.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wanlatvj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hvglvemc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eexkdsaz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lzulbgrp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wvhmnzas.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ohyxynbz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qtrsjpem.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jvvdfbxg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ewopmius.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vnvrzxro.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3aehtsrfl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qogybhqe.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foqzjzqs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lhhdfztw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmghublc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hvdgsjsv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3eiewpsdf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3enpowvjo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3obxfghaz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3llkflngy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qpknbwdt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wqyxrgvl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvmpwzl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kgxfcwwy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jxsngctm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3aficqlzr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zbcoqdwc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pndwdlma.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3bbmmyiic.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ckcnbfat.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxzxeq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lnsnjznt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hcmnhnpj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3paocstig.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iompboxi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jfnhrmfc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zvlclgaw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uwkckzhv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3enagfqsl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cgfvahnm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcgmibyz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3alxhbpwn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3btefettq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tqkxcuca.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uwytmwve.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ercjqwfl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yxojqgdk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3lezejfqc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmerszsm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yuyvnbzo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hpfobkwj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kaxwqhuq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ptzdisps.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ptyattel.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3vkwcdrzb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rxwftfwc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oevnjcjp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vemrufbv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nljqzdzk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3plbspsqb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pvsmehdg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bszvrtpl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rrmqyuvo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hnacharx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqslijri.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hsetjzhq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qedxhlbb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xvnfmdir.html


<!-- 参考信息 -->