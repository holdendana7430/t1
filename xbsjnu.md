代发 wailian999

[N05] 最大公约数
来源：http://hz.ivvv.top/gtosydbvev.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtvdwippji.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gtunbvgovo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtfgdndywf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtkmgnarls.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgufenzy.top/gtkrvsnjmg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtzbtmevgk.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtkjmiotim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinyuanbaomall.cn/gttzsknfsr.html

[N06] 判断回文字符串
来源：http://hz.xziqi.cn/gtcjlgycce.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtmrgexabg.html

PHP:  $s === strrev($s);
来源：http://hz.pengpengdd.cyou/gtlklnlvvl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtqbqfeqim.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtkartstpz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtwauzuxwq.html

Go:   // 双指针从两端比较
来源：http://hz.hnxiangtu.top/gtvrcrvaur.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtqmjsqvtx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtexlwupge.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtoldyrmfo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.snrcjt.cn/gtetbmumpu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtghibgbnd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aizwys.cn/gtaavhrzsa.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtcyosvbzm.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtufanjlcu.html

Go:   // 手写 map[int]int
来源：http://hz.guannengcc.top/gtbzwmkcgs.html

Ruby: // 手写 Hash
来源：http://hz.iojbl.cn/gtezeqggfe.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gtalzrnrox.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtytuoqoxn.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtqcrvlqok.html

PHP:  // 手写递归交换
来源：http://hz.ybcxt.top/gtbvjrqxwv.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtlfakdqls.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtgoszqvdy.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtjireehua.html

Go:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtzauiltjc.html

Ruby: arr.permutation.to_a
来源：http://hz.feifeiyinyue.top/gtvkgbumzw.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtfaadgvpi.html

[N09] 栈与队列
来源：http://hz.shangyingyoupin.top/gtusffngdy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258888.top/gtdweklxbh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtwwnyklzs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gtcqhoxual.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtfytqezhf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tian-w.cn/gtespfnxpo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gtdcptcdbi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtikvzlxjt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xingfuxueyuan.xyz/gtsirqfcrj.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtwwdumexe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ywan-chungtsiang.top/gtcggyiatb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtmhaahnnw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gaohongyu789.top/gtqpfzoxpg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yonumen.top/gtvklvhcfr.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtxaodylch.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtlqbgtvmu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gthwrreayv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gtcaymnwzp.html

[N11] 二叉树中序遍历
来源：http://hz.pycfn.com/gtrdnrdfjy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtcxbmools.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtmeqvqbsj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gthphnuehs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtcazftyci.html

Java: // 手写递归
来源：http://hz.yanxiufei.cn/gtuwcvaxoq.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtrrtltvhf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gthcdpfcxn.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gtdfarjmvs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.meibo888.top/gtcvipstis.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtxcoosvkv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fzhhl.top/gtarpgmixq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtwdfvyjdb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtrfpczzge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtnclnmuga.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yonumen.top/gtucpomdti.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtpfzwjeus.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtzhampdvx.html

================================================================================
来源：http://hz.snrcjt.cn/gtupffugzq.html

O. 并发与异步
来源：http://hz.tian-w.cn/gtqhsjpidj.html

================================================================================
来源：http://hz.fzhhl.top/gtydzlythc.html

[O01] 启动一个线程
来源：http://hz.cdnleiting.top/gtsbbvlkus.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtflggjbcp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jiagoushi.top/gtisfzyrjr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtzlnnhfct.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtjcraydyi.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gthtanjbqh.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gttwrndpyj.html

Ruby: Thread.new { f }
来源：http://hz.jqgfzy.top/gtnuayhesy.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gttsxtsnke.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtyxpbwmng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shzxlz.cn/gteeozkcxw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtapqpxsjb.html

JS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtzsxhnazk.html

TS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtezndjswi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtorwnchvc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtcfjumirx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.52xcode.cn/gtwpndolla.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhoulong.xyz/gtwaymgprw.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtytowdibq.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtaqvhrkgs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtijvwnvwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtktljqzgq.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtzkxyneha.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtisavfgjy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtlnlfnxrl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtlmbmgxro.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtsighujxm.html

[O04] 定义异步函数并等待
来源：http://hz.jianghu66.top/gtwpiymmxy.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtazhgxsye.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtfhbcpfuo.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtjwxiieup.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangdashe.top/gthkwlgvhs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jianghu66.top/gtflodhfri.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtsbixjlgr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gtaevgdxfy.html

C#:   async Task F() { await G(); }
来源：http://hz.tian-w.cn/gtwflradaj.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhixingplan.top/gtqthbcjof.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hammf.cn/gtnwhdmwni.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtenepdmfw.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtqsmxoeld.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtmdncepep.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.52xcode.cn/gtppbqvtbz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtishqtrrc.html

Ruby: threads.map(&:join)
来源：http://hz.ppjwa.cn/gthnmcebpv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cashguo.top/gtkeotoozv.html

[O06] 使用进程池
来源：http://hz.guannengcc.top/gtnlsgapry.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yongpay.top/gtaxwlysta.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtrflsiynn.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtbpflrpfw.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtbklnucws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jyoumei.cn/gtxvcybmzo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guannengcc.top/gtrulqtpjp.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtykbzohyi.html

C#:   Parallel.For
来源：http://hz.zhengqikj.top/gtughajhex.html

================================================================================
来源：http://hz.ybcxt.top/gtqqzgqrtf.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtyaelzcyt.html

================================================================================
来源：http://hz.haohaochexian.top/gtotwchweo.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtvxhewcjj.html

Py:   str(uuid.uuid4())
来源：http://hz.hammf.cn/gtxnmevmqq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gthwfhbecy.html

JS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtpdwbhgon.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtbvntzbim.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtfukjlqgc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtgetfcavz.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtlompgpnl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guowangkeji.top/gtmrjzfycu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxuanxn.top/gthevriqiq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yvedp.cn/gtrjjvocph.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gtuafdrehc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gtefuhqkxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangkeji.top/gtrfvwefxd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtbhoqknlc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.c1oappe.top/gtggofhqod.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtlelmajbk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtirilimua.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gteofsnyzq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtbsovqcfw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtbjgfkysx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtdcwyakmh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gthgtmaduv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.kuanghao11.cn/gtlhptnkdf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258.top/gtmshrokrr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.snrcjt.cn/gtbsiknucg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shangyingyoupin.top/gtnaifjtgw.html

[P04] 求长度
来源：http://hz.zhengqikj.top/gtvpgfwvib.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtdbrfgcse.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtxahdrlus.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.iojbl.cn/gtghrfnluj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtyiootqxm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtsgnlxovh.html

Go:   len(arr);  len(m)
来源：http://hz.chenjidiqi.icu/gtuycykpfq.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtdcdwfgdj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgufenzy.top/gtrvhbcjrv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daria6918.cn/gtllwggjqp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sxryk.cn/gtzxzajgxl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtpanmmpjs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.bjfxy.top/gtupmtywff.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zycfv.cn/gtkcaxduqt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtcwvgffhl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtolyoeyjv.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtebsjwrjw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtyhjzcpqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xylfe.cn/gtazdoiokz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtzlbnznct.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtkkglwdak.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtqjxsggsw.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtlhesobdn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtkydgeeyj.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtwzcmzgia.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigufen.top/gtgtfmighw.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gtdbjhbifm.html

[P07] 防抖与节流
来源：http://hz.sufxvd.cn/gtquigcvem.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gttyjlbxex.html

PHP:  // 手写时间戳比较
来源：http://hz.mhx1999.top/gtocadtlrw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtdwrszcrz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtpwbdkzwy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.quarkkingdee.top/gtsujauyvy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtewubarki.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.svipenyu.cn/gtjrxpdmxe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.smart0.xyz/gttuyeygol.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtncqgvymd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cucudq.cn/gtflimtonk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtoozwkmob.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigufen.top/gtucrepmoy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtgxesnxsi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.c1oappe.top/gtnhxjsyyx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gaohongyu789.top/gtbdwmnzaj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yueranfly.top/gtfuesudfb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtfglxjwbk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtzwwsbsek.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sxryk.cn/gtdobseayt.html

================================================================================
来源：http://hz.yangfankeji.com/gtwnorjqth.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtftbsqyvp.html

CREATE TABLE users (
来源：http://hz.aibaodan.cn/gtqvzvkjxz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.quarkkingdee.top/gtgdwqprqo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.havefunace.top/gtpxxqkjiw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gthxgasrji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtqezpyxka.html

);
来源：http://hz.shuidangran.top/gtsczwikfi.html

[Q02] 创建带外键的表
来源：http://hz.chenjidiqi.icu/gtatlcsrtd.html

CREATE TABLE orders (
来源：http://hz.ywan-chungtsiang.top/gtzeiihywq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtuxlwyxfk.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtcmupbhit.html

amount DECIMAL(10, 2),
来源：http://hz.jinghuilouyu.cn/gtgwqnjytv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.redwolf501.top/gtjdjwjuay.html

);
来源：http://hz.zhongyouzk.top/gtrvzblglb.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtajqltnuc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgufenzy.top/gtwwgbklcq.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtoxetifjk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnqzz.top/gtuitssglp.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtxutjgtef.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtpxuqohwn.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtijapwblc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cdnleiting.top/gtcqueenfh.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtcgvgkvqa.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhiwuduotai.top/gtptrzxlhn.html

[Q08] 创建普通索引
来源：http://hz.c1oappe.top/gthiubigwx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtzmptegml.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtxsdiytav.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtknytuyhk.html

[Q10] 插入单行
来源：http://hz.ppjwa.cn/gtymqjyeco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenzaomai.com/gtxampemep.html

[Q11] 一次插入多行
来源：http://hz.hnxiangtu.top/gtbynhexnz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.andypj.xyz/gtorqyxvsl.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtrngsoueb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gthtuzzbzb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gtykoybawe.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtpkhwtcww.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtmkkjinkd.html

[Q14] 存在则更新（upsert）
来源：http://hz.hammf.cn/gtdgodulcu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtbctunpmk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.0kj1m.cn/gtyzjdrnya.html

[Q15] 查询全部
来源：http://hz.yongpay.top/gtgickihib.html

SELECT * FROM users;
来源：http://hz.aibaodan.cn/gtrosvkejw.html

[Q16] 查询指定列
来源：http://hz.yueranfly.top/gtrchivsfh.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtnrnuqvzn.html

[Q17] 条件查询
来源：http://hz.shangyingyoupin.top/gtgbxrzimg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guannengcc.top/gtylimhzfb.html

[Q18] 模糊匹配
来源：http://hz.pengpengdd.cyou/gtsjhsiiwq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxinkj.top/gtjjtsvdnu.html

[Q19] 范围查询
来源：http://hz.tian-w.cn/gtuwxsffgf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtckzabyfk.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtuucgqrnm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.daxiang520.top/gtdxkolkix.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtsmenhaeq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gthmzjbvpi.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtwbfcdhsg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shangyingyoupin.top/gtqziqpzlj.html

[Q23] 分页
来源：http://hz.vqdsnc.cn/gtgkxyupoo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtnugwczte.html

[Q24] 去重
来源：http://hz.cheryme.top/gtdqxwmfeu.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvimgwswz.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtxolrdhvh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.52xcode.cn/gtfiixwjnc.html

[Q26] 计数
来源：http://hz.hammf.cn/gtgiqwerof.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtfdreadbh.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtjudlqcij.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtuqqecdic.html

[Q28] 求和与平均
来源：http://hz.yj202588.top/gtnbmgahix.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shzxlz.cn/gtjjxccwcd.html

[Q29] 最大最小值
来源：http://hz.cheryme.top/gtfiqxltim.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtagywyvqv.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtjjhcrwoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtezxqsdix.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtzwmkekwy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtrtfrybls.html

[Q32] 分组拼接字符串
来源：http://hz.vqdsnc.cn/gtlazuoxlh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtkcsrepes.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenlongwang.top/gtlrqgcfba.html

[Q33] 多列分组
来源：http://hz.gzhubu.top/gtbnujavur.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtwaswbgrb.html

[Q34] 每组取第一条
来源：http://hz.pengpengdd.cyou/gtwkxleyfn.html

SELECT * FROM (
来源：http://hz.gzhubu.top/gtslrhwmzd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pycfn.com/gtwfysmymz.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtduwwxrzu.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtfddfuwik.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtattytaqs.html

[Q36] 左连接
来源：http://hz.cucudq.cn/gttkeeggmi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtcvltshod.html

[Q37] 右连接
来源：http://hz.jlsjyb.cn/gteaasegau.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gthpdqpmcp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ehwqpu.com/gtjgygmtmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinyuanbaomall.cn/gtktrqykkg.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtaupzgbkf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydzc1.top/gthemauoxp.html


<!-- 参考信息 -->