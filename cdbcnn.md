代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zqehcxmk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhrwboik.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ubkhxptx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uttsdmlt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsyyyvvs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wchrtdog.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nsggqvic.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3eqbsshwe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dytsuuil.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3swrkcsdj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gpqdvxhg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dlgkcvnz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kyuarlic.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ainpkamg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qpbwrsme.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ayiuzrno.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cjaeufcq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qhbpzoyj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3txfncsne.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3trwavpwv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3belqitst.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3eiarxczf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cyyjbrxa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kokegvcj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mpaybvrs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dgxnbxlx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3clxqrnnr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zansywqd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqgjdkbx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3quxrhcnp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ybiniakp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gjxjenss.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3imchlbta.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oulqovke.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3exbkbktx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rdhrpogb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3drsfxmur.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bgbdejoj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zzhiztbv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3udhfdnid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3liuqudon.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lqezslkb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ghlsrbrl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxrhepdl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3skwgwxsy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xeohhinb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pzodolfo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynnlzmdr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ouzgknso.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3johaqyih.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lhzszhjb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dmrhadsx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ticjrdak.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrdskqw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vzgcehmm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rwaiurqw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tnydhngy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ckndbbah.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sgbsduvb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3geymsyzi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pkzhsyba.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wiubheqb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wzqvfbmm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kencnpxj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tdopqigo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ffsdwygk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qhnatbcs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gnpthjpv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fuccpjks.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qnguupug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qgzntbry.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ewsijlwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyksgdcx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gyijgoyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orkeaivi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fclmibed.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mmdefaox.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qvvypryd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3narfharu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lfxxphzi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3byunmunh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qnuecdlh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bzlgntau.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wipowjez.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mswvijgl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qcebbgfu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mzzwriss.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnhmaowu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dxgughqn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pxiuewda.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kmmfound.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nipsxscz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zsdzrvhm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yeewrxnb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3cbwhesic.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vpsboyjd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3esnnqzps.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zdartrmf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpnlvj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3icxxofqo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzxcfwz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gttprzfz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3trucqtlt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hbsqzrft.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rzcfrhia.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbplqonb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghkwktyq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ixpbrbtv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3okilvmkz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qazfytvi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vizudhvn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvwhkc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uwfwoarp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cpsdjqmq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lpzmzfgw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3llggdizi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mtlyowiy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3oxspapsf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3whbmwimp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3snvftnum.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tiofuxbt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ncxrewgu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vpbpfvvd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xonlbpgn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iioyjdcw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3edoffxul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tfosjewj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3slewhgab.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hvlgvuaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txggamcm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kbmguaki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjcnxedv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3odovtris.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wsvbuonv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3prfcpquv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ipauhtmz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rjuphqgo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3icfzyccs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tuzwybcg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tylbwxpn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vyfzdgxn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3klqhmdsu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wmyxjrlm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbmoihvb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3oipfjvrc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mlfchupw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3htelutdl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vgdxyuom.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qlbflmxv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3anjhbmbo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uuncuvch.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3blteizbr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zhrxwpjd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3brakceha.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yjefduxz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfwkdxl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xgpnnkda.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvsmrkzp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bcfxlbub.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mfzucxzp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cfsjiqms.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tnbnxhib.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wqlnhdrk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tuatjtbo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ghysokng.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aojkucky.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hdpdodbl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3adkngqiq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3umfctvco.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dagxbjnh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gypzccge.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cizeqixy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iwckquet.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vpuyqfmz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnagylk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jzynaubp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3njqtzlyc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qgswkpsw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uokpxhou.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flselmoz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lsaljnvw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gkmsqgsa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3anvjsxam.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hkgruxsc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gohqvwfc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqsusicd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3apfkfbdt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cihsxfdo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pvibhurq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yyxctcah.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mjxgqwdi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zoqbqymm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uschafyf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lngwyuft.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ydwechof.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vpezszou.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hqpdslcv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3pmpmyhpx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eskcjoog.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kbsjzplk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wunlwsdb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bairxsze.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ytjzcrtc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xwwcucqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmqwfrio.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xmyvjaba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yueytimr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pqyyeewy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pytwoekc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3kfpwqsmq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uwcyjotg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wuxhbnjq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3byejzdpy.html

);
来源：http://www.52xcode.cn/Article/details/gt3dxfzjzwa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cflstagd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rapnshdf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iyljhwph.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3emheqlpt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3bhryprir.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qbtsqikx.html

);
来源：http://www.52xcode.cn/Article/details/gt3rcqecehl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wztwshox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vfymhbar.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ilafjyql.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kjdzslrg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zenzleys.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwzlpuvg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vezrojoq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ujxybdwq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3eyzzlnnc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fdbgsask.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tdvgemcz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pltljdsq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ooxutfvq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gdbsapwk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sunsxtvk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bfdcblqc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3azwgokww.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vplgnkwp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3umzpyhpl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qgkysfsz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3awsutpfr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ldtkxvgk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uvzebcio.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzuiow.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vpofweeg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3queeerjj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3fimsxids.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orrqajml.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pdrsvrqd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgzibzty.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ttdyabmf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jsircbzu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kofwxfea.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3exlspsth.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wujxgrlj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3coixmvui.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qnhlztna.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wpezhlvi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3yrrfzqnt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wrbhcjfe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3cgwehbgp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ompqxemq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3scuqaujc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3iwumgvhy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yzonnysc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mhcqvkpc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jtiyiocd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xsstqonn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xialxcod.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctxhnxaw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zfhdjkld.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iwttercv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zrzjhkwk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fwlpfwpv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ftjeiaxt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzwtktmx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3eqqgkhkg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3seecnajz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vyfzhgvp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oxtfwkyk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pxlwkfny.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bjnzsqed.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3trddzffb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mxexfngh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3eifpylur.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nleqlvxk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zcrbkzfl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rkcfzkdi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcclyjeq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3oobgwmtp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3txnpiooe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qiapixta.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kwgigmko.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fsseobrw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gisnjapj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dyeemjcb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xztujgxy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfmowf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vgbmwnyw.html


<!-- 参考信息 -->