代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtqagnjrwk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtsxqnvdzs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtetygmmnp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgufenzy.top/gtphiinyjo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xingfuxueyuan.xyz/gtdupzpson.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gogol.net.cn/gtyiuiopaq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtdzisisbr.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtmmhvgajy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtjcrvpqim.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtvazvyvkd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtprslhgby.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtlmxygkmw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xylfe.cn/gtfwsjzlsa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtexdykinc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtsjnemrqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.meibo888.top/gtznskbtek.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtarrtxqwm.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gtujyokkvz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtwmejmtjx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtrbtbabdx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtddhiqqeb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtmgpiabvw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dashuyun.cn/gtbndenshm.html

Ruby: a.gcd(b)
来源：http://hz.9152youxi.cn/gtibbvnokm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guannengcc.top/gtzgoearna.html

[N06] 判断回文字符串
来源：http://hz.feifeiyinyue.top/gttxydgmfu.html

Py:   s == s[::-1]
来源：http://hz.gaohongyu789.top/gtunnnnfxv.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigfzy.top/gtdfakxovg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtdhfawwao.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtxmwcjeua.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtnedvqgfl.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtaaaimfwk.html

Ruby: s == s.reverse
来源：http://hz.hongshengwenyu.top/gtavjyasyj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtelwjwzap.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtyjrlqoiz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtvybwxxsl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtoliyprar.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gtzrmgvxpg.html

TS:   // 手写 Map<string, number>
来源：http://hz.birdmap.top/gtojbetvvz.html

Java: // 手写 HashMap
来源：http://hz.cheryme.top/gtrmahzzcx.html

Go:   // 手写 map[int]int
来源：http://hz.jinyuanbaomall.cn/gtfkgbunea.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtvpgcmgqf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gtdpxynzyc.html

[N08] 生成全排列
来源：http://hz.jinyuanbaomall.cn/gtjkvbvosu.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxuanxn.top/gttnmbqsnu.html

PHP:  // 手写递归交换
来源：http://hz.wangshuangyany.cn/gtyhujrhir.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtpsqchngg.html

TS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtlmdlwzpu.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtxntjzsua.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtspxgumfe.html

Ruby: arr.permutation.to_a
来源：http://hz.zhixingplan.top/gtrrjelcgn.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtqavcyckc.html

[N09] 栈与队列
来源：http://hz.bjfxy.top/gtmrrpzwnl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtdqbphbtn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtknqxqtte.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gthvvxlnua.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtnghzctng.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtlhbkxoll.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtlvbzyfxw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtjzurjcki.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtbcqeikfy.html

[N10] 链表节点定义
来源：http://hz.sufxvd.cn/gtagvwauri.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gtbvxcdwyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gtcmwmhzhv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtafdkbhde.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.svipenyu.cn/gtadicjqgz.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtyktzcxim.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gtmjzqvgfs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtpqitvkkd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gaohongyu789.top/gtvwnrfyjb.html

[N11] 二叉树中序遍历
来源：http://hz.andypj.xyz/gtmrludccw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.meibo888.top/gtfcdsoqhj.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtkfkkqkca.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gttkqutpoy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtdojzxxme.html

Java: // 手写递归
来源：http://hz.dashuyun.cn/gtmrfjbizw.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtwycmkhlo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shangyingyoupin.top/gtvfnasmif.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gtlnijprtk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtmcyblscn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aizwys.cn/gtdrwaulmy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtaoqhoffj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtfbjgyyfa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtdlymhbbl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gteihcfxyh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtcjcmnkqj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtbdawigcr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtmmtlpjee.html

================================================================================
来源：http://hz.cqqwz.cn/gtmnlgruof.html

O. 并发与异步
来源：http://hz.nanxuanxn.top/gtrexcumzg.html

================================================================================
来源：http://hz.ydzc1.top/gtqnooebme.html

[O01] 启动一个线程
来源：http://hz.yvedp.cn/gtblouwfhs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tianlin.xyz/gtsijeisxb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtoiksxbxy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gtromejuoq.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtmcoytsgf.html

Java: new Thread(() -> f()).start()
来源：http://hz.ppjwa.cn/gtjsarxsnz.html

Go:   go f()
来源：http://hz.jiagoushi.top/gturpthpsf.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gtkuxzyywi.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangtech.top/gtgxieuhat.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtcxekzvpn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.feifeiyinyue.top/gtbkglclvh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhengqikj.top/gtfohzdjoz.html

JS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtbzvwatoc.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtkjtobpkt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guannengcc.top/gtsrrysaln.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jianghu66.top/gtrcmouwpg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtauqnjkrd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtusmjwkhh.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtjrntfhrp.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtvxkovcvf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hongshengwenyu.top/gtecbaokfu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj20258.top/gtfsfehcdt.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtphchtlqx.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhiwuduotai.top/gtmozvdxkk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.mhx1999.top/gttpqkmgya.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shangyingyoupin.top/gtydruliqy.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtaynscmdg.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gteqcyzymf.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gthlihhtwp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shuidangran.top/gtjamjmnse.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtodxeengx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangdashe.top/gtjzyuymai.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tanke756.top/gtgtkshrrj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtmfkejweg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtvuipjxiv.html

C#:   async Task F() { await G(); }
来源：http://hz.redwolf501.top/gtsbwonezn.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxuanxn.top/gtfivwfijz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guannengcc.top/gtlbgtyzsa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtmbimyzzj.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtjmqsmzyk.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtyiozwybi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gtyawtuafz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtdmgyhdio.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtsddwrvpp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.0kj1m.cn/gttksorogl.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtkrewprse.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtnufeiimw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenjidiqi.icu/gtyivamtyz.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtoywrbmut.html

TS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtxbnvtnmw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtuvszhizh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtchplkunm.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gttvwotojd.html

C#:   Parallel.For
来源：http://hz.wangshuangyany.cn/gtvsqhtgxf.html

================================================================================
来源：http://hz.yuanzhike.top/gtlesgkdhg.html

P. 常用工具函数
来源：http://hz.chenjidiqi.icu/gtwdzxhgmj.html

================================================================================
来源：http://hz.tianlin.xyz/gtewdtolgu.html

[P01] 生成 UUID
来源：http://hz.zhengqikj.top/gtasbkktyh.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtrsvinjwb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gtmjtacesi.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gthepqrfkm.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtmfenkemx.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtpwcnhrex.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtsohbxsid.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtvwgttssb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtzytoluje.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangshuangyany.cn/gtaamcbuks.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gtmozuxzxv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtzesvlppk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pycfn.com/gtqoykwugk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.havefunace.top/gttbrcuopc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yongpay.top/gtimilyzgd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gttsgrndpx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sweek.top/gtptzxqclg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xziqi.cn/gtapnxsakb.html

[P03] 生成短随机字符串
来源：http://hz.gaohongyu789.top/gtkzlwsfvz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigfzy.top/gtscjkupfv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtivovqdhn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtmpgyqnid.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtenxrljzn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gthqmhsoav.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.andypj.xyz/gtpfydcvkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtslkwexbh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtkgvsilkc.html

[P04] 求长度
来源：http://hz.mhx1999.top/gtioqpxxqj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtyrueegay.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtvwhobuik.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtsmexkiaz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtpxaucztb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.birdmap.top/gtkthmkmbq.html

Go:   len(arr);  len(m)
来源：http://hz.xinyue.icu/gtvkhxllcm.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gthbbkxrmz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtkceywvcs.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtwuvwwyzb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtxuwzvtyi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.52xcode.cn/gtklmeorjz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtzvxzpbmq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtczpdhrtx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtfcwhprxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guowangkeji.top/gtcjyujpfe.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtnamizbgg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.svipenyu.cn/gtrrqvlayk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhongyouzk.top/gtgsjtbzuy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.mhx1999.top/gtwsbikmrg.html

PHP:  if (empty($x)) {}
来源：http://hz.smart0.xyz/gtxoltcpvq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.9152youxi.cn/gtaefmedge.html

TS:   if (x == null) {}
来源：http://hz.jlsjyb.cn/gtgcuufudb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.bjfxy.top/gtgsngpgmq.html

Go:   if x == nil {}
来源：http://hz.zycfv.cn/gtriyrstzv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj202588.top/gtzntedslk.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtspvesdwi.html

[P07] 防抖与节流
来源：http://hz.jinyuanbaomall.cn/gtkszgnjmf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ivvv.top/gtwcixxwns.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtyobfudyd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtyzrikoxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtkzvguqhn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtsqxcttjy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtgatmsalb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hammf.cn/gtvtojexqg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtrewocsxc.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtdcjgplny.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtcsvzucrr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gttmgkacbs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gthggkunav.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhixingplan.top/gtyxcvhrix.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtghpwrioi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtiqxizkgo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtmslvxoli.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gtlbdhqqfz.html

================================================================================
来源：http://hz.jlsjyb.cn/gttgsbybbn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtamxoadkf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthwzoamin.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtjkrmnttw.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtwixlzeff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtjqwdvzzv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigfzy.top/gtfzgedfja.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gtcccueghp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtzkbmbgjc.html

);
来源：http://hz.yangfankeji.com/gtiunhgrhx.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gtgreoqwru.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtbhblwygl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gthxzdjkma.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtkgkbgurb.html

amount DECIMAL(10, 2),
来源：http://hz.aizwys.cn/gtbtgjjtat.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.316326.xyz/gtagxamsuw.html

);
来源：http://hz.shzxlz.cn/gtneeejiaz.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtatdperia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtmtjfrbet.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtxuwpzhrg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.9152youxi.cn/gtdbqjgxed.html

[Q05] 重命名列
来源：http://hz.jinyuanbaomall.cn/gtvgtodipm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.redwolf501.top/gtictloywz.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gtkhjjwwso.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtpphgtgid.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtxleriekx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtcqusxxpj.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gtnpffwfwt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtunpckodo.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gtorrqqceh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuanzx.com/gtjkcygxoi.html

[Q10] 插入单行
来源：http://hz.daria6918.cn/gtihtaqvsg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nwbrower.top/gtozqbvnvp.html

[Q11] 一次插入多行
来源：http://hz.52xcode.cn/gtrleyuvdc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangdashe.top/gtcyqlyuaz.html

[Q12] 插入后取自增 ID
来源：http://hz.havefunace.top/gtgtunmdhv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.52xcode.cn/gtlmwdlset.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtczbaubkb.html

[Q13] 忽略重复插入
来源：http://hz.yueranfly.top/gtdakyhjtb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fzhhl.top/gtmxexkpnp.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj202588.top/gtaxtbnbry.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yangfankeji.com/gtxbqbvozh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuanzhike.top/gtdsrumvnn.html

[Q15] 查询全部
来源：http://hz.wangdashe.top/gtquelkeyy.html

SELECT * FROM users;
来源：http://hz.c1oappe.top/gtyuqqrsac.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtxewiqxuz.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtqitbbiuc.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gthtdzvnsw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigfzy.top/gtygeoeijm.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtctyvyrri.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jyoumei.cn/gtljbhalhg.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtazjlhjem.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.iojbl.cn/gtkasafdot.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtyczyxfka.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gtazjwmcsa.html

[Q21] 空值判断
来源：http://hz.tianlin.xyz/gtqxrfbdrj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtcuemexth.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gthvfdwagv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aizwys.cn/gtvenazsnt.html

[Q23] 分页
来源：http://hz.tianlin.xyz/gtugghxxsa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtjwudckss.html

[Q24] 去重
来源：http://hz.jianghu66.top/gtbagqchps.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gtysixokln.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtthjqlume.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtwlpjuglx.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtzrtveghx.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenzaomai.com/gtfvrbmtrw.html

[Q27] 条件计数
来源：http://hz.meibo888.top/gtxhwdluec.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gttfkghqie.html

[Q28] 求和与平均
来源：http://hz.cucudq.cn/gtqitygqgt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gotoacloud.top/gtatgitqtr.html

[Q29] 最大最小值
来源：http://hz.zdqjudy.top/gthhilafgd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtvsopiyob.html

[Q30] 分组统计
来源：http://hz.ivvv.top/gthtgqsvdi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtwbyaaqqm.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtnblivjup.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtlcigdexk.html

[Q32] 分组拼接字符串
来源：http://hz.cdnleiting.top/gtjzaxqore.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtaqllpytn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtbhhdhsdw.html


<!-- 参考信息 -->