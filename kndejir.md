代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghyvwoxnj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/glsfruvxv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gzbjzesvr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gbppjsams.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gutuxckmr.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gkkmzvclt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gewdlcgwt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gsbztdbmq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqybucrkb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbzvbibtj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gdmxomtsw.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gvgveeumd.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gxjplrfwl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gyvglxjrf.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gekffjbvj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gegrsuiqm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gztuntren.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gatjontgq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gislywdvr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/giyipsevo.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gdodrkuzl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gifdtjrsv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gaxanjggt.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gljccggwo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzscbqyvt.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gyicivslp.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdrznoipg.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghfcomcxa.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwwwkxepw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwgbjzrqx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gwodtlrex.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggjyzixoh.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gyiqdksul.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqxsdma.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/guztrpndq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gzouudclj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gqhxwwrlw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gfauqbqjs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gwbzpezeg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glqkazdtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gtruszeuu.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gaepoexmg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gwxtvwlli.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gihiclgub.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gtbnspoew.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gcrbndcgm.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gowwokyqr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gbqtvtdqn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gjvyrrkzz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gjksuohtq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gxilvdehz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gtegxihbt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/ggeasxvwd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gqjhhvipf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gsuqmbcrh.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxacraseq.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqtyayvxp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gnegvchpe.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/glonvvziy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gjujpxozd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gpacfsxqd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/grfojoukt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gmsqcwykc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gjihpmphf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gmefedqyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/ghlumltss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/glanvhysv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gsmlidarf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gffyyoiat.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gddywzjbk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghgpauuoi.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gkobmukzs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/genulybxr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gcyqxdyzw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gvvdzwnsy.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwgsxyssx.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gfnbclfeh.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gbdxlsphb.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gkymzrdhg.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gtbpluyho.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gdxgxizfm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gqhlitmhb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gsudataqy.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gtzurricr.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gxymjkqvq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ghltgztia.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/geqstcsel.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gtfqjrjag.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gvtxobvna.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gqgrbcsju.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/ghhdrkdeh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gaktjnhip.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gtpnxlufw.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ggfpcgvjs.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gbylitpgw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gefvvqoni.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gtikcorwj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gasmyrphm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/geetrayvq.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gxcukfaxt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gbuirooym.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gbfmesqqc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkzdvkkxh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gcbeqbibc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gpjtlfcku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/grxqgchwz.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gdligxinc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gsspxpzas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtydktgia.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gmsbvhycc.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gofojjdrq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gfmehkwnd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gpziiwqfg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gwdyctaer.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gasccrihn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gmsutjdzv.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gblqhioyn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/grqcyiwtf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/ggktsdozz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjasyquzq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ggbjxmtrd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gwdxjuuop.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gnykihcwm.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/grwajdcjr.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gazfdzfaj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsbkbtehd.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gfxirkwrz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghozrlnta.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gbrisdysx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gxfppxfdh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gxaapbmfl.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gqktumohw.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gxqfqxlgd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gvhmregwn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gndjmfnsg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gesoulnhh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gruopquzy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/grndtrwkc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gzodluyji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gbldvqewp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/grhcoeiqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gaviwxffe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gwdiybcwe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gdegygxgf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gldydgmla.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/ggdncdwwo.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gqwodrfci.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gdzfikzrw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gtvfxhptd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gwibpfveu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gsfsqyasu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/goyouxwsh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gcntcpffz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/geewkxhtl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/grgsacdrm.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gltcgkfmm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gqrcdauir.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gbautoaxs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gemveeiti.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gtftjtymd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gvsamntgq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gsrecxhwn.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjggfczxl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzcvlaaig.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gkleunfus.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gdrlbqufa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gzemkmnwr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/grifwlqih.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwhqhzrjs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gjumuisqe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gvhgtajbm.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gootyoxds.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gnspcilcs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/ghpksdcup.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gfyxosesi.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/giyexuhgm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gadkbkkes.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/ghqkptxtw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gtzjmsfki.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmghmzi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gnpsyvlnd.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gagwxrtic.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gksykzkzo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gclziahcj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gqjuwqrtk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gkhleeqcl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggzambadp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gbjilwfta.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gvdrgqogr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gcivvzxzr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/guuvdivcq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/ganwjzjfn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gzdrddiji.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gbxmrqidm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gukfpkqog.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gjuwikywa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gkafpciin.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gdvvcdils.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gylerlsaa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gslystqkj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gncttlxei.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gqzjplzxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbtinwdcw.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gnjhadock.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/grlsgqowa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gzmccpqgy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gtcglfnfd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gtcxsvpwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gvubudpeg.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gavegxvyi.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gtgmurgas.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/ghxijdzdj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gpetioudz.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gjoophlwy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gufvxzrox.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gstnjgnes.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gceyrzrew.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gvdmyncnz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gntoepwta.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gdqosfjxa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gdpgfppmy.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gvmncqagp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gzjnrwwuf.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gutmqgcjk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gzrmgldiu.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gviklhyvt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gousfnzub.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gtpzpchjg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gbmefpoui.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gzuekzmkc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/goxvrwolx.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gjfglbcws.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gpvczfbyk.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gsqzodktl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gjycmencn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gqrgjzbvs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gorolnkvw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gobozduut.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gxhelmljc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gruhzuxxt.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gousgfkom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gymdleqjo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gznqvprhn.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gwtprljgt.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gilaimxww.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gfxdtujwq.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gnxlnswle.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gsnxkqjqf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gghiitdlc.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gjxxclmev.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gcstrhybg.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gzluyqvzi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/grlyvepcm.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gmluzgmbw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/grncmeluu.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gnjiygdyv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gcrtlgmkp.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/grfrvdqtf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/ghdfvpzoe.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gkhiwhems.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gvetqpyje.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/ghrvgmfdw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gafquxcan.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gaqtucpjh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gdcdqacqm.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gvdcrjgta.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmzhysdqr.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gmllkvstm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gvvegxlct.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gubdmlzxb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gcrydpqnk.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gmgkcmwsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfpyryxpy.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gwaftawad.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gpwaisuog.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gdhmgkskl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtlnheiqt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gquubzuba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gqddrsjvl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/genokbxpm.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gssvzgxqs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gqvhclowk.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/guzrdrdea.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gnnfwfmha.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gkyksdxcz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfjmfferx.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gphyzejnz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gfuxohvhd.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gfjthzqiy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gzefqsjtg.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gfaidehdx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gzwewuhim.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gtigcjljc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gisxdjkxi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gjidwueca.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gtddhqosu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gkahmkmlx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gfawexgpb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/geigftemt.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gmoyufpiy.sHtML


<!-- 参考信息 -->