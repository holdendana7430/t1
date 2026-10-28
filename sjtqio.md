代发 wailian999

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtvxqfftpg.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtcpjogwhe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtcbwqttmz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtgsdswqtd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtzfcgiveb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtwfaqwhhs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gttphxavba.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtoehzyhmo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtnpknxtkr.html

[N06] 判断回文字符串
来源：http://hz.yonumen.top/gtkrfbijel.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtcoemogkn.html

PHP:  $s === strrev($s);
来源：http://hz.xuetiantiany.cn/gtovicvwql.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtwyohkzep.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtortcrlfg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shzxlz.cn/gtumkksnsr.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtxpexbbiy.html

Ruby: s == s.reverse
来源：http://hz.jlsjyb.cn/gthbyfnuad.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtmyuyzhdf.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gtqluxmgco.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258888.top/gtmckdxwmt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj202588.top/gtwyeimwro.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj202588.top/gtgyccffnx.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtmsglpblb.html

Java: // 手写 HashMap
来源：http://hz.shuidangran.top/gtvstciokr.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtjvlszogf.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtjuvuctzg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fengsongda.top/gthtpcezez.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtjhrykdtz.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtfwjvacpj.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gteirjtgmm.html

JS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtkmwmhghc.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtewnedgap.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtzbajulxs.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtfoxuyotu.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtzeacjhko.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtuslkcefc.html

[N09] 栈与队列
来源：http://hz.tanke756.top/gtibukliqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtqsyqoliv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtstmfdydg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtmxdksbgw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zdqjudy.top/gtbecbciez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtdbpzhcpt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtxrhddgbz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtljclgqlk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtqvekqguu.html

[N10] 链表节点定义
来源：http://hz.jinghuilouyu.cn/gtqhkaikrs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jiagoushi.top/gtelgmhfwo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aibaodan.cn/gtdjjpgyex.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtbyafzqxg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cqqwz.cn/gtgbtekiav.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258.top/gtlyximgzk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtchuwcszl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ywan-chungtsiang.top/gtfoqlwlko.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtuahfalip.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gttmerxnqh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtuhnvbipz.html

PHP:  // 手写递归函数
来源：http://hz.c1oappe.top/gtooheurop.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtxnkrkkto.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtyamqcezu.html

Java: // 手写递归
来源：http://hz.nwbrower.top/gtsqooimoe.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtoxkaxeym.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj202588.top/gtktyxpbqm.html

C#:   // 手写递归
来源：http://hz.gaohongyu789.top/gtqknfdegc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.vqdsnc.cn/gtkyptcbeo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtisskuibo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuxming.cn/gtuwwwxyue.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtcforvbfx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtincgaybq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtbqopctvo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gtehskjeni.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenzaomai.com/gtuzsnxgcq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtnahhcyim.html

================================================================================
来源：http://hz.xinyue.icu/gtlbxynytt.html

O. 并发与异步
来源：http://hz.xylfe.cn/gtghblfmfw.html

================================================================================
来源：http://hz.iojbl.cn/gtxdwbkiko.html

[O01] 启动一个线程
来源：http://hz.svipenyu.cn/gtijagpxiv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hongshengwenyu.top/gtquwjetar.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtkbgywlep.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtzbctqypz.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtldnvfkrb.html

Java: new Thread(() -> f()).start()
来源：http://hz.shuidangran.top/gtyodbgpmd.html

Go:   go f()
来源：http://hz.sxryk.cn/gtdduyzcmh.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtvtrptnrb.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtfltundeg.html

[O02] 使用线程池
来源：http://hz.yongpay.top/gtzwcjysfz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.quarkkingdee.top/gtjbrtufvy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daxiang520.top/gtailiiwla.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtcnlerrqy.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtityyqtvd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtwikxaeaq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtsatrqhgy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtnievkjtj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cashguo.top/gtqaiflufo.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtveodfihv.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtlutqdyln.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dianchejie.cn/gtenxuoozf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtqnimtvbh.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtjnngdixr.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtqrxlozgx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinyuanbaomall.cn/gtmufsoyul.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cqqwz.cn/gtzokvhznp.html

C#:   lock (gate) { shared++; }
来源：http://hz.svipenyu.cn/gtwtnogduf.html

[O04] 定义异步函数并等待
来源：http://hz.nanxinkj.top/gtkmhkecir.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gtwwracpoc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.birdmap.top/gtaxqpcxxt.html

JS:   async function f() { await g(); }
来源：http://hz.jiagoushi.top/gtoigzvfpd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtaggssryl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zycfv.cn/gtihhodwxg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtzekjellf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jianghu66.top/gtdlinseik.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtcqbpjfac.html

[O05] 并发执行并等待全部完成
来源：http://hz.xylfe.cn/gtgobjjwer.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangkeji.top/gtkmegvxcl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtpdphbscz.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtpnqbidti.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtnpjqmkdx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtlksymhjd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtqkdhhqrv.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtvhimcfcd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dashuyun.cn/gtsyetjnbr.html

[O06] 使用进程池
来源：http://hz.9152youxi.cn/gteszmuoje.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.9152youxi.cn/gtvrebaacg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jiagoushi.top/gtpmrennbx.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtzhlhxgoy.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtpxommiqp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtfbzgxora.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtubxdylxr.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtsihlyhuu.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtbzhlbvmo.html

================================================================================
来源：http://hz.cheryme.top/gtwzmjucrl.html

P. 常用工具函数
来源：http://hz.pycfn.com/gthpmistap.html

================================================================================
来源：http://hz.guowangkeji.top/gtiiygwtfc.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtvisdcxpo.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtkctfiedd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.snrcjt.cn/gthzkcmixf.html

JS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtmfxftati.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtrsrpigbi.html

Java: UUID.randomUUID().toString()
来源：http://hz.iojbl.cn/gtmzaqbbaw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtrmuzssfy.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gthcgervhe.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xziqi.cn/gtfeyjkagq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gttellpkfq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zycfv.cn/gtmorwfqiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigfzy.top/gtakwvpozl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtprvfnhww.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtfdfxwtxm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtqufjalcl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gteviyrtkk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zdqjudy.top/gtboysadly.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtbkplhjaa.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtseysjoge.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aizwys.cn/gtcbvejwmd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cheryme.top/gtiqilafji.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtaxpqzzeo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtstunblei.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cqqwz.cn/gttzgpzigw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtxcemjxrq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtevcynbjc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gthgmqhucb.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gteqqabjzf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.havefunace.top/gtropnudle.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtrtbypxzv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtxixkjmsd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtzqncdaeq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj202588.top/gtnmnlfxhh.html

Go:   len(arr);  len(m)
来源：http://hz.nanxuanxn.top/gtldlpuoji.html

Ruby: x.length;  x.size
来源：http://hz.shzxlz.cn/gtxfabknce.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daria6918.cn/gtysafeowv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ehwqpu.com/gteifcxnlv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.mhx1999.top/gtlqfbrqne.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtyjcumypi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtuufmikzw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtslbnwjnh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtpbfegslq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangkeji.top/gtthercdai.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtlrughure.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gtqyukladj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gtkvltkrzv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtssvbgbkj.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtxjoammzw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yonumen.top/gtvujizrfm.html

TS:   if (x == null) {}
来源：http://hz.nanxuanxn.top/gtbcgpfkyr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gthacbnoph.html

Go:   if x == nil {}
来源：http://hz.zycfv.cn/gtywpbutnr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtybudkaxn.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtamovojhu.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtkpelfvla.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigufen.top/gtbqbogqbo.html

PHP:  // 手写时间戳比较
来源：http://hz.meibo888.top/gtnfiucdih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtfgtnheos.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtxqvolpgg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.quarkkingdee.top/gtvqvhzbvy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zdqjudy.top/gtpeqbatpv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.52xcode.cn/gtvdggoypl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtbvpabbnc.html

[P08] 处理浮点精度问题
来源：http://hz.nwbrower.top/gtbscdavjt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gtzcxshwll.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yuanzhike.top/gtztburove.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hongshengwenyu.top/gthjqnrwad.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtzznyvtqd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhongyouzk.top/gtvkbtqfxa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtbcyhtabb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtdfjftvop.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gtygryztle.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvdpdepbt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ehwqpu.com/gtvvukzcan.html

================================================================================
来源：http://hz.wangdashe.top/gttvpjkijh.html

[Q01] 创建表
来源：http://hz.cashguo.top/gtqfhqtikx.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtjcdjgylf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtjhpkjbln.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtzsleghap.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gterhhrzlf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pycfn.com/gtynbiohxs.html

);
来源：http://hz.chenzaomai.com/gtmsimfext.html

[Q02] 创建带外键的表
来源：http://hz.nwbrower.top/gtunnxntvr.html

CREATE TABLE orders (
来源：http://hz.andypj.xyz/gtedberirv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtlsonbcvr.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtoszutvom.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtpmxshcqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtuazmymec.html

);
来源：http://hz.jlsjyb.cn/gtqajxgbnt.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gtmkgdhbrp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtjuvyaznn.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gttijgtizy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daria6918.cn/gtlplhkbrc.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtdyguofyb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtvlquxagq.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtixhdbkdy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yanxiufei.cn/gtxclpwfzm.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtqsyqjeem.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tian-w.cn/gtthwogqiz.html

[Q08] 创建普通索引
来源：http://hz.pengpengdd.cyou/gtwfimnewn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtlnfjasht.html

[Q09] 创建唯一索引
来源：http://hz.shangyingyoupin.top/gtwvfwqaod.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtgqqmvbpp.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtetfvfqpj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtzptwxshi.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gteoipdnvd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hysaishi.cn/gtsxbhjpnb.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtorrwizbc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.haohaochexian.top/gtesdyfrvv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuxming.cn/gtrqiluhar.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtcpwxpwvn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtrsuzuiwg.html

[Q14] 存在则更新（upsert）
来源：http://hz.hammf.cn/gtakqrawiw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shuidangran.top/gtgditshln.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtzhchzhbr.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gtnzlswjjd.html

SELECT * FROM users;
来源：http://hz.shzxlz.cn/gtezxzrkdu.html

[Q16] 查询指定列
来源：http://hz.yuanzhike.top/gtbltdjbqv.html

SELECT id, name FROM users;
来源：http://hz.jqgufenzy.top/gtfncwtwgg.html

[Q17] 条件查询
来源：http://hz.shuidangran.top/gtfuzlwnjn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtsrhxolrt.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtrczozydg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gotoacloud.top/gtdhfgdyjq.html

[Q19] 范围查询
来源：http://hz.feifeiyinyue.top/gtfgyeflxy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gtludbrqiy.html

[Q20] IN 列表
来源：http://hz.hfpthk.cn/gtxqsulxrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigfzy.top/gtswqzyuti.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gtgsdkhpuy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhaomingkeji.xyz/gtzjumfnzk.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtzkvnhowr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gzhubu.top/gthllmfqnv.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtgbjeecaf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gttyltwjrc.html

[Q24] 去重
来源：http://hz.c1oappe.top/gtrafobczz.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtvjffgkqi.html

[Q25] 只取前 N 条
来源：http://hz.cqqwz.cn/gtvqrntpnf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gthmheomid.html

[Q26] 计数
来源：http://hz.xziqi.cn/gtjuuxexow.html

SELECT COUNT(*) FROM users;
来源：http://hz.bjfxy.top/gtxvrtiprs.html

[Q27] 条件计数
来源：http://hz.hysaishi.cn/gtemqwoekq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gteddxdcod.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gttcnnhquy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtxixtokrz.html

[Q29] 最大最小值
来源：http://hz.guannengcc.top/gtuhgecgqh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guowangkeji.top/gtjjgxbabg.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtjghtulel.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtdascwqqm.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtlcdhgcke.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tianlin.xyz/gtcodqtyzz.html

[Q32] 分组拼接字符串
来源：http://hz.gaohongyu789.top/gtohwiycmd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtjysjqksi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gtcryfwlch.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtuxonrbpm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtmersovaz.html

[Q34] 每组取第一条
来源：http://hz.kuanghao11.cn/gtiebxxbel.html

SELECT * FROM (
来源：http://hz.cucudq.cn/gtaoydqytk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gtrxgmdgfw.html

) t WHERE rn = 1;
来源：http://hz.ywan-chungtsiang.top/gtifvyjmls.html

[Q35] 内连接
来源：http://hz.jqgufenzy.top/gtxuwbkmsw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtvtjjccik.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gtnxluvhvi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gteocfawyb.html

[Q37] 右连接
来源：http://hz.ybcxt.top/gtzgqrslpj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jyoumei.cn/gtuluwkuqm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtajgqjphx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhoulong.xyz/gtnoomzqju.html

[Q39] 自连接（查上下级）
来源：http://hz.tian-w.cn/gtjoumexer.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtsudgqxal.html


<!-- 参考信息 -->