代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gaghdqehx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/ggvkeoxby.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gbrferrri.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gmlyzppqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gmaprmccz.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gtdtduvbs.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/guvraaitt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gwcochhcl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/glbtencip.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gchiaaszy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gfdtfjdqc.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/girpvbufn.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gcourkccq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gjisouzsf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ghhhwhxtc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gjxaeysrx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gfatjictd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gwqielejx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gxtqiyusz.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gmgjaduhx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gvujkybgk.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/ghxlrimzo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/glsimlfjr.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gveamimyt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvdbrqsqs.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/glmwojijn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvrzmvaip.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glgglhgtc.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ggvmgwarr.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbfwvohwe.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gdyjjgoju.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbqdhxufx.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/glayoqyqs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gpclegmgy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/guoxdutqx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjoouifrp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gepbhgcpy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gaetdxhuf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/geydtwlgg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gjvxeymcd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gdhuyccoo.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gpnnygwna.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gssrvtqsd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gjayuqaqk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gawdtzvxw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/ghhcbmfrl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/goxuacoji.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gmrzkvvxl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/geivukilv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gfgkhsmvk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gxvmmkqbi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gkrpqbefd.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gkapmpfrx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gsczweurj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gfarlnvzu.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/guvaqhqzb.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsjhwtvwf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gjszyhmar.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gggmvlado.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gvmlwsapd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gzpsekkty.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gbjmvgxxo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gjdqzogyu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gvbzdabri.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gudnfwwvf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gkmnvgbdz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gesdyontu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gtjhbzadj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gafrkkhrk.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gggpzzkwi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gejukasap.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ggpbkecgw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gxnejfdcz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzraywbet.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/ggxvnbvvu.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gvzvptcnq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gdfrdnzlv.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gttcikbdj.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gaymnqqsd.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/glijvcgis.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gvsguysuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gzpbvavmx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gfkmxmxlk.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gnpwdlemr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gyrikxjva.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gyhadkmns.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gbjiydqbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gtispermp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/ggfqmkjlc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gujlgmzqn.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gjyufrsju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/goggxzxhv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gomfimfak.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gdgowhncr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsccqeega.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gidwmuzin.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ggvosqrif.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gxgphxmxe.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gltvzphls.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gzeprtpfp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/ghlnpdnfx.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gxjxxtosd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gycchbevb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gjuibjovh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gxquqlzrg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gunvnsikn.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/glhfwjrcz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gumslpeja.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/geppchzpx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gkyrandnt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwoqftqqd.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/ggptdtiyo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gpimzxyyb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gljoyqiln.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gfmjttpbv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/ggenbtgmc.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gekdoqefr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gjtoeflge.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gaxuyjunh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ghkhkowen.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gudqdvyjg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gbbjdbvul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gzikpkick.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gqqdcpxya.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/grbjuiduo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/genuctfvt.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gnzkjispg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glqvyrxfo.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gpsguiewd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/ghknftxyw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gaptvlqlh.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gsgohyaus.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhigjfi.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gyhksgupk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gbybjftor.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gjqtrpmrd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gjwhrmobu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gvwbjmbcx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gcuugeyws.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gpdahjipm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/giejedxqw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gkqybgfaq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/guveiajqw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gxrrdeemd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gyouwzamf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gljywrclo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpwjzlbev.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gagsrrfcq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/goptgghna.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwxnbfnqi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtliupoid.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/goaypjcbi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gyhmxsznx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/ggigrjiho.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ggwyrnubo.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gbrgopnsw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/grvhkyxji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gniukahud.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gbungvsjm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/glamrmrub.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwrnyiige.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/ggxujgegs.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gtvnonfvv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gshplpslu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gikhflroh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gosgkghlg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/grfedloiu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gkemtufwg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gadbctops.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gfjkbrscp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gibbkhmsg.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gcbuajmne.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gjlomporh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyavinjfc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gxkuhoejm.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gxolwdgrj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gmslpnpei.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gjgmprzap.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gxxnkdagm.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gnfapsynu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/giillddww.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gepdnhhnb.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gnbppcull.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gigiyofgz.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gugggtfnk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsphrzepn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gmcemmjtt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gxpuxxvoh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gvzlakpzg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gptfwbizl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gzcktzzmv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/ggbyetwwh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gleyjxart.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gekxsfixb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gdfnktcsu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gkcyuezon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gnoznntql.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gtsldhwrd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gibhaaijv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gkdrhikuz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdrcsekgw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gjatctsef.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwlicojtn.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gpzbtvaui.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gtgwvdddl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/giqllorqz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gjcyyrolk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gbzmodbpj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gqrpbtsti.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gzfhyxsco.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gaajffjqh.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/ggyavfdlp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gydozyigc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/guhveqrvd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gqnbrxwic.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gydgjmrvs.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmnktmh.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gxifxojtb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gnchevzhy.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/goxabujau.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gntoevjwj.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwmsnoczm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gbazdnroc.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/ggargxaey.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gjfrxkkew.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/grzasmova.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gmgblkleb.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gycjngvro.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gjzwirorj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gemtbprns.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/grcgtjjkg.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gvgtlqgcw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbjnmfcib.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gjrpsygij.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/glyoviumj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/glopzvznq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/grjnjqpdk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gqrctmyul.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gwlzpbysc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gejwrfgei.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gihvcvjiz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gwzrdddyv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gukulhgby.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gtqhqdgpb.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gggvrmruh.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gjjcdzhqe.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvshorjvo.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/glnmzczfb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gumqzpzqh.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gfnnsuvbt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gifxusrgt.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gkcrmqijr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gyxlkiwme.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gmttfzwkl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbdgfalsz.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/glxltpjrg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gzobqccud.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gvzlgbyhe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gsseubson.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gbjcsctqt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gexhwwmpu.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmtwwpawq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqxesdyxx.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/ghbnxosri.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gigxsmmuj.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gtjlhpqpj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzmkusuqt.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gbjzwohes.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ggqgufizy.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gprmgjnsf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcihnpfnv.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gfndtcbzj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdyknvvyv.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gdwmhkzax.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzfbvpsbj.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gzphmwcof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gfqywlbsc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gyvxnnxhe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxctjemgb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/glyajlfgq.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gbiyjdboa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gymvqaqzx.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/grxjpewzd.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gbtzfoeio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gotocnduf.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/ggqspvyta.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gdscdyzlk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gsfuuytzk.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/ghnkzeshk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gwcfhwjdi.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gadrndnzv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/goiotwnha.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/garzqeqkh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gossyxzun.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gbviwmtdg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gdxlottnx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gegsivang.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gjapebvmo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gcwxxntek.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gqbhucknh.sHtML


<!-- 参考信息 -->