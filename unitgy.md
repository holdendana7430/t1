代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mvyyhrbv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tkrjlyhu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yuohzimb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2amfrpkyu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2shcumliv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cndgzjka.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2upidxhah.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oqxaquex.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2efcepckt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hopaijvb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2knhnijyy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fxezuxgc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mlvwihpt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mzhqaykq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mmosdvnn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2eqbxhpge.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gkkhejia.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hcovyodx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wejxnqza.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pzsgxgia.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chixevim.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ieoggawf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ftjohefi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zjkqwfnw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovhiszfr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pdrgcwft.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hotpiryo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tnpmcixa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tmqzjjdt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qrgxlnxf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jrmixjuh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oxhhttdj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cyjexfgh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yijntlul.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ymadsaof.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyooznkp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jaqbsbkd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tlnbmvea.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kzjajsrz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2unqsznzr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wqoqgrdg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2llkbtemd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hbeaaubl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dxhfnlgv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hautebab.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2alxwsvnw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hfefiazr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pyacybag.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gjixdwqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xzonjjod.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kyqxyksd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dxlxeqip.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ruprobht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ptixleap.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gnvlizec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kpvwwwdw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gcgyjzpi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mvmfgnio.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zzavtudt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qyucvgyr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kwqqxnwq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oikfqmyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jrqyhftt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bopvntpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssmkbqel.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ezzznazv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykgphodg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2movsogrr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zvoaiqvo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kddtliyr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vazlowtz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ylcgkefl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ibeevrzj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bgwdbhuc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ovtkpdgp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ogpfbyqu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sitwtwns.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ztiisthf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mmxwajpu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rosedtvn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uoatkmfh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xlysbicp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ceegsusg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hyrwswqs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qqjplmva.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nngaihnr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqjwztcq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2pzlvqfkq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pmpvxrvv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vdbzdfgn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2imtzxtby.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wvigansl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gzuaqbfh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fftppsww.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jzzxttci.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pgqpcsin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hydsfdry.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ymesxtdj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbgxgdn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2noenvykr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2oylcaxbb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2geugxqry.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehpvmgsj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gkzfybet.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uzechlzi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2heqpybse.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pbmaxrme.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hsazksli.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qkvemnoj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2scpjlktc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rnniltsi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpihdfcz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qquehzpa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zbhawxgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2romextmt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rbxfcdjw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2crgvlgzy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bdtuincf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jkpygpqi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2riaglvoa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vcbxpftk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpltudgk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2gdvkmmsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdhzevni.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2npwwhiab.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pbzqncge.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iyjzlyxm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mothtgvm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pgpdxxki.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ufxqeiqh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jszwbhua.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dnacuwob.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xjfwkdvr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wqrquhwf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jpmcxlvs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwfpiegb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nslpznne.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pbayvcda.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qcgjyhfi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtggucon.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wlocrepl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kzglvnuj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blgwtqgv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nkkizdns.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wxqlfbka.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2avpsxuns.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lylrbgom.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kilwxvql.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hgscxhsl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qjhyfvaj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jreukgtv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2cnaiakht.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jgjbiirg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mbycgwdi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2okcmmlaj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jwhkljml.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pojouxuf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ptxmbfmc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xhoafpov.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wjblrrsi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rqsqwoxr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2iefnedqf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cwskrtfo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eaesfhdu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nvyvyrus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fomjmksv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lieyjsak.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sasxdsrn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aesaynpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zbfzkmwa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2uifyfzao.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiosdplf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vefnzrjj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmoansyr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xsuwtojk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhfkrogw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2movbghyd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2viwfauvl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gctxemcp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2syzxwgig.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lkytrfri.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ptbabrsu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pdrhhwsi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ppkjoybe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2desypwbn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2czrrxbrq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xuoxajgr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hskcvarz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2fytuhkwz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yaxupsxn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2nlhxjxav.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hizwrzsv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2tlnmgvbz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fvvffxgr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gaoyigdm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tyrkeycu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfvqhteh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jiwqypcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lejwzclt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cpfhyaoh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2clheigjv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ygdommym.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2thirbohe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2yoztoclj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rzjjspxs.html

);
来源：http://www.52xcode.cn/Article/details/gt2lljnzoen.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gbzyekmg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yssndrff.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rkfqnuyg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wutzlazp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kmrobleq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mzezeqya.html

);
来源：http://www.52xcode.cn/Article/details/gt2twtwfozy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ykpnddqh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xvtlbsku.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wkvnzhrm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2sflxdrdc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iakaqkey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2lqlvbdwv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ojdvaeif.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bptwbllw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mdgzyxho.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fnazqqwc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ivemfcuc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bztcqmnk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xypluwby.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2upyfalhl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uszkdylq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xmdbhggo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2uhtkdroe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qsacgjxa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2myhttrnw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jbhbbmqt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2imcnzebp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rpfshihd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ofxcgdew.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2whbpsqih.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2fsvfiort.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fxfotdal.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2szcmmzvh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cilhfpuv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zdadbzjo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2babhgczo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hbmnwotz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjxovpbr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dkuxgzzo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wpdkepdl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2knubnqeu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ttrglrvo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zmkpsdgm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2giorcxye.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vgfloifa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aghxwmul.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2swrbgirl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yzcgmvut.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2peovdjnq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yzvzqxar.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ntjwmkrv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2falqhimf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zfzhaiks.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fdexhkhe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gqpihllc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skwuhxcj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rlgdtrbu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vknqrxfz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sktaqivf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hmmtclex.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ehsjlxwe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vqxmdrpc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrtrke.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xxwkbdms.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2irxwxast.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cifdickb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kkdnulcx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cmswjacl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ogoerloq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vtowqfil.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vauxfqng.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tcviqdqs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2oxsumljk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gglscrjs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yvaxfjui.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ttrxqwit.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qbdqsmde.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sojtdhou.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2grfqoful.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ianaqvyu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gsizayuz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hjnzufzv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hxbccwpo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tdvlzeyq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mfdebsmh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2arneukgs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2djmwxuqw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2brxxqgao.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rfefcdpc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cwwadmhv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xnlxajxc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kygrznrr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ancbiema.html


<!-- 参考信息 -->