代发 wailian999

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/gxymjcuxj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqxtqlhag.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoefptai.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdsxtkhik.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqfttqdrf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fanxiaobao.xyz/Article/details/giljdejmb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fanxiaobao.xyz/Article/details/grllsoeda.sHtML

Ruby: a.gcd(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gnklqrfss.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzxebab.sHtML

[N06] 判断回文字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glgmxktuo.sHtML

Py:   s == s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gzfylnhbv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvqbjxon.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/grhgnzlir.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/guxqoczqs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasioilgm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gccmgyjli.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdukagkp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gchapghfk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/givcujuzi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwzcwfvw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxbjxdk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhyncdev.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjxigvex.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszivkzgq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gywuzqatf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gupuwknzy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gciplineb.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gvwqmkbqt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtmpiijo.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fanxiaobao.xyz/Article/details/gggijlvla.sHtML

JS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gamiovtre.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gvnldvmqj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajnpqteo.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/guduynyjg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gyebbcdnn.sHtML

C#:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gxklmjljh.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gdwgxiyey.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqoehjna.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gmxfmlmck.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gmpervaty.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gravzepzj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhbgillj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhdqjjwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdgldgzr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/grupjsudp.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqrscrkw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeeattfj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gszotjeww.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqqslcls.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzijvrcdl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvtxpfqe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbrkvasz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsqbbvh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdugzoctv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gjnoeygtn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fanxiaobao.xyz/Article/details/gczsoarve.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqohbmpza.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfqesdii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmbnapuq.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxywttmv.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gbjqzsxel.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfaxjqrp.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gqoqwmgoy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkksukxq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gswupawad.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxfqholb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gbuzywpjd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxialbfvk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugwxxxex.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gizvffdvf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzavpnifg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gfgrbckmv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjmhniyak.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gialnufvy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxucnovk.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkztdamv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/ggzwenywz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofvjfzjp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkunbxpz.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gmyckthuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuvequpx.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyunqqowr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqleqmbbi.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gqempyptt.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gxexzfxxq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtngefod.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/glsdoaomz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gqxrrnhan.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbrykres.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gywitfdrt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/geaqwthwd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/geaevyapp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/giytvcyal.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjaeplmn.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcvhwsig.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gqocbtweh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfhaduxl.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbxuusun.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmmfwprsh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytztbizt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtznvuav.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/ginzzttut.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdqyovps.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/gatgjftrx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gesbefxmo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsevbmptr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnvnuewsg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/grpttirxi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmswxex.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/grjtoviid.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goqhlksxt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/guepkhxik.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/grevzhvwy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbdvfpeu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykaxibog.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczyrkway.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtbcubxk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrqkvpvr.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlspzakj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbsklbnr.sHtML

[O06] 使用进程池
来源：http://3g.fanxiaobao.xyz/Article/details/gtcvficzm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gxfczbffv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fanxiaobao.xyz/Article/details/gcxrucuwp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/guvhantrd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfshzqdm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcphduax.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsrtgatw.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/goqoiqggb.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttzdnmy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvirragpk.sHtML

P. 常用工具函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdycbfdjz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvulnvj.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/geulphzty.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gmtgfglrj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnlilwkb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsraeljdc.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gufourvfx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gggrxlzle.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gnbxnpdel.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnnfyoij.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/golblmdvy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbjiggkj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxjhsvrc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gwympfjhx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfldgzopr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/ghijlrnfc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/glrnupqbj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkntzajds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gusycxxnj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gianvykmy.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtfclzjmv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gokpokrqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gxyeboksz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gezeuwdav.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gschieyzc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymagsnml.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjlzazyp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gsxahuyzl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gpzczndhv.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzggjtrdc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/grgggwhdn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/grsarawyi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gychblgjz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/galhcbwqc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcgnwufh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhcizhhf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gehuhtaoq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gldirrvmg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhqqopt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiradulw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/gvqembody.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/gxeosyxfo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvotbbebs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/goezmmmnn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbukarhjd.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/gpauoomev.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gdycxffzi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/gegnjmrha.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gljoikupr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgqwydr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/glzsbfykk.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjhbhgf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwutqmcty.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gifjtaluu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoqpmqbt.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gedtbhzef.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/grgnxcuei.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fanxiaobao.xyz/Article/details/gsijpijgc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzvgsnmg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjvirkqq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gulekhyub.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbvqwnacb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxrcmyk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gdbltcexg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gwwmbteqi.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gppovitgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gwjdyjads.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpazchbv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gjikjfrxj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwtyppba.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gbgytfxyn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gdvmmitph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyayamucq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/ggmmfpaxk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtmawwxoj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/giyvxyeon.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/galloywzk.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdinmhill.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/geyeufgqy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gnikafkvn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuuzsouk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrjghowd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztwtbfc.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gxrycoenz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmrzkxtv.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbkuwewe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxnhorhi.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/galbizywp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/grfdoevub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/glyeoiokn.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gittgkxhf.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwvjnace.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gkjwyzddr.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/gspwrrlxx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqqfazfa.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gbrxkhyev.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/gjxmqqcfr.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliynojij.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/glhuyrios.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gcmlxxznf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsldunacf.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwuminvgh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjiblhfp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeercfza.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gyouqjxxy.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxxqnwd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gqfcfxszc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniktihdy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrxgyflz.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhbohnrc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfqhzbjr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gynqpcmra.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyckwsky.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gykzkfhli.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxiacxgv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpvoolcd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlbnsaha.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gzejjbjjr.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnggbykvb.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsfgfph.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomtkwczq.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gouvwotxb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gigagqyfx.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gonypitpf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeyzbzns.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gaxhtxjtf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gicxziayc.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gszlmyivg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomsxvsdr.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqrersotf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gyurdxxhj.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggwawubgr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gbddsoocd.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gjretythh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjrzosk.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhitdobu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkubjpshy.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihyfqewb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/ggfaeeqzb.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxnmuhxq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmnoknpua.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnsogzt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpgprzvqm.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gfxyrolwd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemdgpobn.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gqbsbzsii.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqflhtqni.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhdsqidq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiumicmo.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzviytuxt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucerehjx.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/guxsbavhr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlbicgdr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gpckgljay.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvijatueu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyadghrv.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gcluhleon.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjazepoac.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaxdizmn.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzidmmciz.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/glxheebhl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkvrtkvpy.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilxwicpf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gubpybvog.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gfwalqsnc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnwpktdk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrigqiae.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrprdxju.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gepcoykcw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gnlucxnod.sHtML


<!-- 参考信息 -->