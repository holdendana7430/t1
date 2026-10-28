代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtcgueovia.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtkmexmmdi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtjmkxvrul.html

Go:   slices.Sort(arr)
来源：http://hz.hammf.cn/gtfvzarccu.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtabwyzfyu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtvmjpbrfs.html

[N03] 快速排序（分治示例）
来源：http://hz.hnqzz.top/gtgrmlqohr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtzwvwqtnc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtttulzagn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtsdtphsgn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtqmtefezm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtpcahxlni.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.52xcode.cn/gtubpaetqt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dianchejie.cn/gtiwuljmmi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtgxymvhfm.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gtpxepwvsq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtxeecgdna.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtufvdzbqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtdcridlte.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtwrvigdzx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtxxrienwm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gtgpslqvtm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtjnisjqdd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuxming.cn/gtbbruurjn.html

[N05] 最大公约数
来源：http://hz.guannengcc.top/gtubjilmxx.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtqdueihbd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtfphifwjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtglzfhzse.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtkdvsbnkh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yvedp.cn/gtfnwozkhc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtrprieyqc.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtlqcbdgdm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hfpthk.cn/gtlnfonljb.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangkeji.top/gttfidbdlr.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtswistqoy.html

PHP:  $s === strrev($s);
来源：http://hz.feifeiyinyue.top/gthjwkzmsb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtxgcdsmtg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtukkcmocf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xziqi.cn/gtyzidrwmg.html

Go:   // 双指针从两端比较
来源：http://hz.zdqjudy.top/gtzfvslahv.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtseaukvau.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtolpqluer.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtkpmegegz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtyxavwtpr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.316326.xyz/gtfqxzknfc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtfnmxnlty.html

TS:   // 手写 Map<string, number>
来源：http://hz.ywan-chungtsiang.top/gtnwsshnuw.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtbgwtppqb.html

Go:   // 手写 map[int]int
来源：http://hz.chenlongwang.top/gtphnstauy.html

Ruby: // 手写 Hash
来源：http://hz.pengpengdd.cyou/gtuyxivoof.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sysykeji.top/gtvbfmdjww.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtnfeoenlj.html

Py:   itertools.permutations(arr)
来源：http://hz.chenlongwang.top/gtrcvwqwiz.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtnuuwxodt.html

JS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtriplkkhy.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtxtkjgbjs.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtsglepjbt.html

Go:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtxzelcggi.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gtfhoghnqe.html

C#:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtzkynncxi.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gtvvlytynt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.vqdsnc.cn/gtjuagyubw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.snrcjt.cn/gtgfehwjlc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.redwolf501.top/gtboisxpih.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hammf.cn/gtukomcmel.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtwpyzdshg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gtdcbmkcsv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guannengcc.top/gtawzoehze.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.snrcjt.cn/gtokobnvni.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtehqbzlfm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtgioumsym.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gtdnnjrxcr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtgixpwggp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtbbxsvtbm.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtiospdmhx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtjzxpvaul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guannengcc.top/gtzvgamytx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.kuanghao11.cn/gtfofwtdgc.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtgyuihtuv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tianlin.xyz/gtrjfirxmy.html

PHP:  // 手写递归函数
来源：http://hz.dianchejie.cn/gtekaipodv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtzhnvzyej.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtyemliklr.html

Java: // 手写递归
来源：http://hz.zhengqikj.top/gtvyvhygeg.html

Go:   // 手写递归
来源：http://hz.jyoumei.cn/gtqojqmirq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinyuanbaomall.cn/gtlirfdrxm.html

C#:   // 手写递归
来源：http://hz.jqgufenzy.top/gtfvvymuxa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtfudwkzey.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daxiang520.top/gtljfjzjgq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtrzjfygji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtpnzwlgre.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtczvmdaxg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtpsgdfwxk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gtirkepfvt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtlqpxprlv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtlkbpdmix.html

================================================================================
来源：http://hz.iojbl.cn/gtztzgbbth.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtocnmsrrp.html

================================================================================
来源：http://hz.yj202588.top/gtsoqgwouf.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtzxjhzvsc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtninprkzr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xziqi.cn/gtsugqzfgb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtcetamvqi.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtclbuisfr.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtsfocyxof.html

Go:   go f()
来源：http://hz.guannengcc.top/gtxojuwkkv.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangkeji.top/gtcdrnzkbt.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtljywuwiz.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gthujdmzxp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtqnfovaso.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtpiwyadnu.html

JS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtxwtbwfnp.html

TS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtoabfbxjg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cashguo.top/gtlpurviat.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guowangkeji.top/gthdprddlf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.9152youxi.cn/gtuomfiqag.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.0kj1m.cn/gtgvwxcoii.html

[O03] 加锁保护共享数据
来源：http://hz.hywenlv.cn/gtymkmslit.html

Py:   with lock: shared += 1
来源：http://hz.smart0.xyz/gttfvecuuy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yueranfly.top/gtrcqzzexy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtcfnkfcsv.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtoqxtrwdg.html

Java: synchronized (this) { shared++; }
来源：http://hz.shzxlz.cn/gtmomjyjmy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gttprbxutx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtsjtjsmeo.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtlgbogyjh.html

[O04] 定义异步函数并等待
来源：http://hz.zhixingplan.top/gtqpjoteyt.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtuhjhadjp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtrzihdfcv.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtlqhvsybv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cheryme.top/gtcfbcxmbk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtoxljrngc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aizwys.cn/gtsjzuvrgl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtmhdrelus.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtyufrslly.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtcnvewbyf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtopqovdwh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtxrwuehwj.html

JS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtcwevqneg.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtnavjnffo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gtllmnvgzf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtpbnybucu.html

Ruby: threads.map(&:join)
来源：http://hz.hywenlv.cn/gtjsoycltg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gtjpbaekrz.html

[O06] 使用进程池
来源：http://hz.hnqzz.top/gtghfdmrjy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtzqnviacv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtddjthmdw.html

JS:   // child_process / cluster 模块
来源：http://hz.yongpay.top/gtrcdfdjzh.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtypxyrtgj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtucubmhmp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gthtlogbbm.html

Ruby: // fork 块
来源：http://hz.vqdsnc.cn/gteqwhtokz.html

C#:   Parallel.For
来源：http://hz.jinyuanbaomall.cn/gtglsescjz.html

================================================================================
来源：http://hz.cqqwz.cn/gtsbyvjvbq.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtfhzlmccv.html

================================================================================
来源：http://hz.tian-w.cn/gtoiilrpqe.html

[P01] 生成 UUID
来源：http://hz.yangfankeji.com/gthmnwuhpp.html

Py:   str(uuid.uuid4())
来源：http://hz.gogol.net.cn/gtjjevuzwl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuanzx.com/gtzqdolvcf.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtazittqwe.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtsegrblao.html

Java: UUID.randomUUID().toString()
来源：http://hz.pengpengdd.cyou/gtxyodqtvv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtubnfpmgx.html

Ruby: SecureRandom.uuid
来源：http://hz.9152youxi.cn/gtynzbjxkf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guowangkeji.top/gtuolstwuz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhongyouzk.top/gtulahnkqn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtwaizncca.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtplvikknh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fengsongda.top/gtzjrxngkd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.redwolf501.top/gtodpdfilo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxuanxn.top/gtqdejsrua.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.9152youxi.cn/gtszgbhhjj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtwjlpdmvt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.0kj1m.cn/gtbjyyhrck.html

[P03] 生成短随机字符串
来源：http://hz.ybcxt.top/gttkmtyoid.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtbathozoa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenjidiqi.icu/gtooeaykwt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtkjjkimhy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtsxtebiur.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtlwtawuic.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhaomingkeji.xyz/gtcqxtutbk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.316326.xyz/gtxwcyqykn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtgsmtljli.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtpmxakwlu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtkhzhjwmw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtzyvrmarn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtyexeulik.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtbfthgjbk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.mhx1999.top/gtzucmtvcu.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtiwedpsns.html

Ruby: x.length;  x.size
来源：http://hz.dashuyun.cn/gtrtprxbme.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ybcxt.top/gtubagqcmh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gttiagzqvf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtmkxfsadt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtsbhtdggt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtvxawcfiq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigfzy.top/gthfyoocnp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gtksieohja.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ybcxt.top/gtnytmlhgx.html

Ruby: a == b
来源：http://hz.aizwys.cn/gtaggvslaj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtpxfttksg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnqzz.top/gtxxrgmndp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtlamlxuqq.html

PHP:  if (empty($x)) {}
来源：http://hz.shuidangran.top/gtgqastdsy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cashguo.top/gtcpjrgwvm.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtgcazulrz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuanzx.com/gtiqbnmhis.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtwvszkjfb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ivvv.top/gtzzwodvvv.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtyxheruww.html

[P07] 防抖与节流
来源：http://hz.ybcxt.top/gtmbzfpelu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtoxztrlsp.html

PHP:  // 手写时间戳比较
来源：http://hz.sufxvd.cn/gtfncpjcxh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtchfkinjs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtdupwqhhh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtokykiuaw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtqeqrogaa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gtftznkxer.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtzwmfxhsd.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtdshtwlev.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtybmvugwk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtesrcvlck.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtzxanwmjb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhengqikj.top/gtnkijqimg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtruzvjhif.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtolubyyte.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj202588.top/gtdzntywga.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtzdatdfvg.html

================================================================================
来源：http://hz.tianlin.xyz/gtbkxzyzxw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cheryme.top/gtjtlxrwrx.html

================================================================================
来源：http://hz.svipenyu.cn/gtstpdiojf.html

[Q01] 创建表
来源：http://hz.shanyushiyangkeji.top/gtbzygehgg.html

CREATE TABLE users (
来源：http://hz.9152youxi.cn/gtbzeydrst.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtmejqwifa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhengqikj.top/gtynnrxzmg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtkpwxmwfb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtguwgawvf.html

);
来源：http://hz.hammf.cn/gtogfprfna.html

[Q02] 创建带外键的表
来源：http://hz.xuanzx.com/gtyyizfmrn.html

CREATE TABLE orders (
来源：http://hz.hfpthk.cn/gtegnlulhr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtmmwkmqfe.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtamlaghyq.html

amount DECIMAL(10, 2),
来源：http://hz.yonumen.top/gtplzksbyy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guannengcc.top/gtmnpcqxar.html

);
来源：http://hz.jqgufenzy.top/gtfwyaslxs.html

[Q03] 增加列
来源：http://hz.jinghuilouyu.cn/gtehosulht.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtbjdjfmti.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtawxhnmnh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yangfankeji.com/gtivwbgojp.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtggmfrnhm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sysykeji.top/gtgnqkjoml.html

[Q06] 删除列
来源：http://hz.cucudq.cn/gtojrblvcw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yvedp.cn/gtqakcjuvs.html

[Q07] 删除表
来源：http://hz.yanxiufei.cn/gtynzxzifv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zycfv.cn/gtruzwtntj.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtoekhzzmq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtobdjhuff.html

[Q09] 创建唯一索引
来源：http://hz.yj20258888.top/gtkwdpcyad.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gttdosnuuk.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtceckndin.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtvqmmnrsl.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtzmugyzpb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gzhubu.top/gtpmpoefbu.html

[Q12] 插入后取自增 ID
来源：http://hz.ydjk.org.cn/gtxloyeyqm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtgjxkondr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gtddpczhtn.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtksyefshj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gotoacloud.top/gtbfjatsys.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtamjuzprf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtejomuxcy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.pengpengdd.cyou/gttvitszro.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gtxujreykj.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtjmbsogfp.html

[Q16] 查询指定列
来源：http://hz.fengsongda.top/gtciigoplp.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtfjchxgww.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gteykdtmdr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtflzrvvly.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtukkncwvz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuanzx.com/gtcsadlver.html

[Q19] 范围查询
来源：http://hz.hysaishi.cn/gtaitznqnh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shzxlz.cn/gtxcidxhcx.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtmkrhebjz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.mhx1999.top/gtnhadxcmi.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtnhnaewho.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.birdmap.top/gtypklgxfc.html

[Q22] 排序
来源：http://hz.gotoacloud.top/gtwevosxai.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtwdnealov.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtikqpfycv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtthgcixpj.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gtwkjduikc.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtdyklktgb.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gtoelgmytw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shuidangran.top/gtoophijhf.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtgemzfggk.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtvmibofmk.html

[Q27] 条件计数
来源：http://hz.cheryme.top/gtiautmgog.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtvrdoxysd.html

[Q28] 求和与平均
来源：http://hz.fzhhl.top/gtjqlmwujv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtphvmornu.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gtktswudqe.html


<!-- 参考信息 -->