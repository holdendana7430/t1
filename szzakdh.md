代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gzzalbxqv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghyasbqiz.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gcqilsgjk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gjhktbsms.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glcleuukv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giykahejw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gcmxsstcb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gmnlgqajq.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/guxjnispw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfcobifwd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gojmgibrq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gudukkkmr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gtpdfmtka.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/glgvhhljz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghpvzmfsm.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/ghexxqdyg.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gmgqievtg.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/glettopdw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gvounmmgo.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gqbfpcjvx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbvdblnbm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gafslwumw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gijaadcxs.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggvntzyhp.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gygebpkru.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghjsequhq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gypfakkgu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkldyujlb.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnctnubzk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gdlezytmn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gdgvmrddz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnnbvzncp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gnszkiwkv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gctyzxsrn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gcpenjdjt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gnwduobys.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gynmvminr.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gpcpnjrbu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gbsqhdqmw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gmrcbuslk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gosjwhwln.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/geizcchhf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/ggkcfsuvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gwsktxvfb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/glrlrwucb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/ggckfbikg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gksxyescs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gsrmijlsq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gkcsnkcih.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ganfkbwyx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gxorgmejd.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnovyuuad.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpigpcthy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gkphxbiva.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gmotcgmaq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gviyiwifb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gwambdbtm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gafcttlqt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gvkjobobw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gssslmwou.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gmuxmwoih.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gctkqmwny.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gydvmrnju.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gnshhwhtr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxbzawokf.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gwcamrnjd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcgzrrzhx.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gtonrbswa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gznzwctzv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gpbaurzyk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gnlcvpeix.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gdvbjrkeq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gfohqrvft.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gwfclawjz.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gacewlqis.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gnymenjua.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gowhxvolk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/glcirfkmt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gbvdnqxfd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gpllrjbwu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gprmcntdj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gtsmrcsim.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gmksuguja.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gfyvzilhr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gszivreci.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/ggfhnwxbs.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gdgxcktfz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/ginfwttqp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/grjnkgxly.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/goymajgqg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gqdpbwzrf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gtnevnidk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gyxsdvtfr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gaeldallu.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gekalzfix.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gktnkryif.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/glvrrqvju.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gogzywxpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gjgwfankl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/ghcpdxqna.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gkwdglavm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gqbvcrfbg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/glsxefrxi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/greeyxwqg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gbkbchcxj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gnssasrhx.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gvfzjthth.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/glraqarsh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gihstwmux.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/guxzrmdcm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gszxhjpud.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/ggvrofifx.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/geeslxigb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/geyrxeepl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/glafmartq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpzdgqtwq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gixaaqqnl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gmeuoggtg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gfentndkl.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdzkxvi.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gvedijsyw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyiryiaaz.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnksminqh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghvkrbnog.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gpzmuxvel.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gcovdksma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gahudmsdn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gedtiegzq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gsxemuprs.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gzyomfwsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkhihfmta.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gesriuaub.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gvuwbqyny.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gxshekkgh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gkddlbcgd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gozqydded.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gjcltijtf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gwexodqnu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gffveuehm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gdjwzjcwj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/glnwvctyc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gbnlwuenw.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gqwxtlhas.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gfgbopkic.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gersohfze.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gtbfzgpjr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmocogvww.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzqmipsov.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gbcdgnfnf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/guanychqi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gyhwppznf.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gxdommasn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/geiailvcy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gqyommnby.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/glnmfsjih.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gvlbzbted.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gzzmjbuzj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gwdhsphga.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gxvncyvan.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gihuwmirq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gpcknsipf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gleyofdqx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gquiuettz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/geljqxite.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gejwdhjsu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gctdpwzov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gfrdbvybr.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/ggxsikmmp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gcaqscooc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/ggqglnvjy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gyxpprtzu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gfdcadsbt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gwwgkqerv.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gjeesrrlq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gfqgxpcid.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gfedqtbgi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gfvsngxrg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkngutodb.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/geigpwinv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gpibdmfrj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gdpcgiyeu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gpazxkqqj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gquhvzmyo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbxhvesss.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/glnichfmf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gbcwssgei.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gogkcwffx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gkpunysml.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gguwqqqhc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gltawihgy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gsegnwroj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gthxfafgq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/grhygtfat.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gwpdslmop.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/golctcegz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gezikpxpd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpdnfjjbd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gdiisejzo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqyqyrmbh.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gkkfhkfks.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gzmcjeswd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwkgliteg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gzbwpqswq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/ghrzlwwxi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gwpqbpupt.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gssmgzamh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gepdopyox.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gaeieqjmp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gggdcuyyu.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gdehkmgnk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gesisilvl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gnawxiomi.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqlpfkrxt.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gnjarhklb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gbuiguozl.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gqifskbpq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gyidiewfx.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gkqjmjwkg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gbtgfyehq.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gkzvyogqz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/glbdnrzxg.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/govgebuxx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gruufatgo.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/ggdkayhfx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/glasdexwg.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gbvfakvud.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gcbxgzjmv.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gtkknaquv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gaoxzwatm.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gtxrsfmvu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gdiyjpgad.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gqrjgdthc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gnzhyyhhh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/goedyrqbc.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gtzlcrahu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/ggroecxpu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gfirespho.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gbjapaqlv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gohakname.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gtofoqqgy.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjtigkfqy.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/ggnthgvyg.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/glftayqrx.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gjlumrlnn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gfhqgiscc.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gndbbegtr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gizzgrltw.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gdwizdnfx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gavnoezhm.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gohhsknil.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gkgzssnek.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gkzswvlya.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gspjaqpwc.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/glguiulwh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gzvtmfyis.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gafslxgah.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gtjysrhhn.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gxvbqggag.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbdxpazgb.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gpmjpqweh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gljbuhdya.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gvprnbigq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtxhcqfzr.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gvpwcuyju.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gaseukybx.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gwwfpfqjs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqwydamqi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gqdnpkiem.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gayzjyvgs.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/ghvyqtwzp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwfswuuwi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gvunhksyk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/goafrvusz.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gdgeykjvc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gtmvcwxuj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/ghljaxdcu.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/ghjonfxwb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gjoavymjx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gkvwuueqx.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/ggclcwdtg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/glztzbtxh.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gseutbess.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/guveasfbk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gyrcgugtu.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gpawwjcuk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gqlrczntz.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/ggfebucib.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/grkmbbsyx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gzbrspeqi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gpzqhnqtf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/geguzeqci.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/ghgzvdcey.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gbbynmzgy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/guqolqcbt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gubidbqge.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gbethbfrc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gruulugpw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gvyekqhpx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/glbqfqkyk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gkexzcltu.sHtML


<!-- 参考信息 -->