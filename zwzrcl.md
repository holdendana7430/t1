代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2csxoxpmr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nzrvsnzq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yrzsxbkf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2blcakdtz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zakomwdq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uvbvcjsa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qopksxwj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xcgmhdka.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kluoqyjh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aonbhiuu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qpjphlcq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zltrfblx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2aoucryqa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcmkspl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lnpppszr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xwubqqvc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ltwtqxqp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gzkdujzt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tzirpaof.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2owkgbjbp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqnseybb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gcljwybm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2axfbunqg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gtrjmzhf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ameyncdd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ntactecp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ztuifbgv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bvfnuvip.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2knwcejik.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jorwsxib.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mksfliip.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mylhuncu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zbjtijkl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mnfvarpx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rcmqdxor.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hkjqckid.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ozukvfmb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wabeljpo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2joqfdewd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jcdpsilp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fzsxwyqu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nardvjzd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nxtllqhh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hmtkfeay.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mwwmcdth.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxtplnm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hhgurwep.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2remxxnhx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2smrbldhs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xdcxxqep.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kyhyckeg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2raogbain.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gifqbbge.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ubfdduej.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kblfnymn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bqlnyfcd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2iojhdwms.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dyhpersq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vcmsfzjs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jrhegbrj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bgmkymrk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lgbujouw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qjvxspin.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cthxxmsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbelajks.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dkgdotbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2siguthwe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2texyjihd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2diolgtgb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xrngvhis.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mskspcyd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xddibqez.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vpiiqnzw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ybqepunm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jqaqmsbw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lqklnljc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hpcyesbw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pakdupov.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2phbkxvcc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2alnorios.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2roumxnik.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rfpbsavx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ampfhfxz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jecihmrb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2agfueiqx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ufhmrift.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nkarjwhg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kcdbbtiz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2auewbqdo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2snhebdlc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmzkxyns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dhsyxsib.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxrtfinq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejaykijy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dydzprwh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2swemjeut.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hcwxccll.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqrviek.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gppwhgbj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2iuluckze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pasjoomt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fyxrlpid.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2glznuyqu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2saztlgnz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdpfgqr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pobraufi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pmkwzcho.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2inqhdxfz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xummevhp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wxcbcgjx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yfycvgfw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jizgmpdh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lioiitmi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2oyafdrds.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2aogedfto.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qeouqwgg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xmaagglf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ygcttyse.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2srltojoi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zybqhdia.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pvaladca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgtgwojs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ifezgcgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylebokpc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cyfftbse.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2exxnpwfc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qyjeyboi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tdovkkkl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zqypdlfy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2njmbusbv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hpkkqrte.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rdeynufw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oppydnvs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dazaxqot.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kdeasgtb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpfniugz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2opktccnk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cztnvuse.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sksrdeys.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2trotzgxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqddpjc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ahcbzomx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wwpjtrxx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ppzgqhgl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zbofrngc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2srpryxjm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2njtjuatd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2onjnydwm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xnrlzpdu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrqltpx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2eddibpkp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bnpujtku.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hmkddfnz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ncomvcuy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uyelkdga.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lsjmhcyh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ldockdom.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2uukmzckf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qfadqmvg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oqxvncdn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rfnecjdm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2oevqdpfj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cpllqibw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dbokrhwx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ziqjpbth.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2sqdvjpnw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxnufjm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mncnxfjx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qkajqhsi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uvjxowqc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2glnbwuow.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qjaqfltx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xjxikuqk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wpvsrkpn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqdhvmmk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2svyqyywc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2delpbhmy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2giwpyvoh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dosspdep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kouqygeg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vjspajnp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2azlibpfh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ocyoxzfk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grujhasm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vzknqhvu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mhbsxojf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xouckfxl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wkswozdh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2hskibtqz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ehqfkbhi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wxhxhjub.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hfksvflo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yslkjznz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hqbfmhpx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dqedezmm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mfghuyee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2boicrbxj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2auaxyyub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqtiurcu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpenux.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hyukklzp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gzjppjsq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qfnmitwb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wkwdysaa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uldtpcny.html

);
来源：http://www.52xcode.cn/Article/details/gt2xbhgivzf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kdmowihe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2oufodswp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vfwijnzl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2napdwncl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2cosrxjyw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yyxmkopp.html

);
来源：http://www.52xcode.cn/Article/details/gt2arrapyfp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jzhunozp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fnzkyqhi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mvexwxed.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xpwvrors.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ulburvjw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2unxdikyq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2anxmigew.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qnnpcxfg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hxetrlnl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bmwtxssz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xbxgfnso.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bmycuqin.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2umscwngt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cqlwwgun.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wpoeigoq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2inxfsmof.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bzkkismn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wxsvarjq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2skizcijc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zpxvhfqp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2stusckal.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2looeximp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bawduexy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wmwcjebb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2netzrldl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2evpltgkj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gezwdiuo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2blotdvwc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nkltyfpx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yerxoxsg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lqptaidj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ezzuotaj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uuuxzqkm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2jkigapbf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ucanklpo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cexzylrl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2catslobj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2raytmlqd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yxrcahqu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gboeezxi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nekwcbiz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ytezzgxv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yvcvmdfc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2elgvdtef.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zlyufavj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yezqpoyw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ounsjxhj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mqpeuqzp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wmifzeih.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kzycmawy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dxsvqyqi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dnxwkbhn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rfxnpxar.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kimujjjd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2atdajfuq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sjpsdsta.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2krnmpeon.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fikxapiv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2abvesaug.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2srlanpnp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqykroxk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hazdmkff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ahzxpdws.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2edvdjqvt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2uqawlzuf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jtkdeyds.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kndkvtdb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fgqxbvfn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lphgrghw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fzbjnasb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wkgmlzni.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rdqxhcoh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jdzneuug.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oobxgwjq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vuyshtqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qfococck.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2siazhdyl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2oexmtrke.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wwakqlyb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pwmnvryr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2taafzgmu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2muyrzmxo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dhgayrsq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ptrxdqky.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2snysnygp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gxobzlmt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ryehjtih.html


<!-- 参考信息 -->