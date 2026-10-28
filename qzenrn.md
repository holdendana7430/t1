代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtusawcxcw.html

[N06] 判断回文字符串
来源：http://hz.gzhubu.top/gtajoynphp.html

Py:   s == s[::-1]
来源：http://hz.yuxming.cn/gtbamhoemx.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtemyezhux.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtzzgyqvpe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtbycbhndv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jiagoushi.top/gtxatijpon.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtqmdjhhhq.html

Ruby: s == s.reverse
来源：http://hz.hywenlv.cn/gtzjtrenop.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtlngbbhbj.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtdhhrqxyo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fengsongda.top/gtxdtvmegm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gtnmakkekg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tanke756.top/gtdtovoctp.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtsiodmsqw.html

Java: // 手写 HashMap
来源：http://hz.ybcxt.top/gtewkjfkoo.html

Go:   // 手写 map[int]int
来源：http://hz.vqdsnc.cn/gtpouzozfi.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtwftepndo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtcihbrbik.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtezatvxof.html

Py:   itertools.permutations(arr)
来源：http://hz.wangdashe.top/gttdhhfkdw.html

PHP:  // 手写递归交换
来源：http://hz.yuanzhike.top/gtwmddbyyk.html

JS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtrnpkzgwo.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtpviwqjdk.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtvahhrstv.html

Go:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtdaxblktm.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gteeqssvon.html

C#:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtbfenqjmv.html

[N09] 栈与队列
来源：http://hz.guannengcc.top/gtdrpilveq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ivvv.top/gtszinxjlg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gthpbhjcfw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gtxshnihqs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ybcxt.top/gtakzzhhzd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtugocaudx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gtcfqmwokt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtsgjnqyjr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtowdeozjm.html

[N10] 链表节点定义
来源：http://hz.xingfuxueyuan.xyz/gtpayjtjwe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtduqpwqtk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtjdpbtpxs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtzyrbpklc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtogwxdety.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258.top/gtxyvsrgrr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtscqfcdvf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.9152youxi.cn/gthukrgrlg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtgmjrqkdr.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtbneqpmdm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtohlfmizg.html

PHP:  // 手写递归函数
来源：http://hz.hnxiangtu.top/gtqyyigygi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtrtxsdoso.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtfofwzrrr.html

Java: // 手写递归
来源：http://hz.sweek.top/gtehwstslj.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtdsxqjaan.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.smart0.xyz/gtujwgokih.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtzslbpmfc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gtfbaghjtg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtpuodfrcj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtvmhedgue.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtlocdxcle.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtukhveqmd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtcvzxuoun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtcllborta.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtdbckyiwv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtmldvucxp.html

================================================================================
来源：http://hz.daria6918.cn/gtpnxoybfb.html

O. 并发与异步
来源：http://hz.cashguo.top/gtarduqrqg.html

================================================================================
来源：http://hz.aibaodan.cn/gtaejyyghy.html

[O01] 启动一个线程
来源：http://hz.nanxuanxn.top/gtfhtrsudi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtwkwmhltq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtzlywpnyj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shuidangran.top/gtagxubmhm.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtxzmztvyq.html

Java: new Thread(() -> f()).start()
来源：http://hz.aibaodan.cn/gtqgaxqrpn.html

Go:   go f()
来源：http://hz.dianchejie.cn/gtxsoatkfj.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtyptnlxqk.html

C#:   Task.Run(() => F());
来源：http://hz.jlsjyb.cn/gtfptrcihw.html

[O02] 使用线程池
来源：http://hz.ivvv.top/gthqizdtwu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gtlcqkundd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangkeji.top/gtoiahvbvn.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gttlfskjlp.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtkyiadpne.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtyfggsmpe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daxiang520.top/gtkagmgfpp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cashguo.top/gtyfoaenvj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gaohongyu789.top/gtyzovhiaa.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtgtkdfxpf.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtubpmfwny.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hammf.cn/gtcxslucth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtivtfmedn.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtcqrqocge.html

Java: synchronized (this) { shared++; }
来源：http://hz.tanke756.top/gtminxwrpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xingfuxueyuan.xyz/gtlzkmslov.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fzhhl.top/gtqtawhvyc.html

C#:   lock (gate) { shared++; }
来源：http://hz.andypj.xyz/gtvklcleis.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtudpynbtt.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtemafodft.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenjidiqi.icu/gtccnofmso.html

JS:   async function f() { await g(); }
来源：http://hz.tanke756.top/gtlxkxitpk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnqzz.top/gttrmdxvuc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtltzxwhkr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jiagoushi.top/gtyvfmghsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gtjxsxvvyn.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtjeiztotd.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtaxseogrm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dianchejie.cn/gtuyptzhee.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.svipenyu.cn/gtkgleiivu.html

JS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtwjletrlw.html

TS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtwuwnqezn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gtyylwurbw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ivvv.top/gtafznadvd.html

Ruby: threads.map(&:join)
来源：http://hz.hnqzz.top/gtzfghohnp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtfnyskxwd.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtgjnfmfxk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dashuyun.cn/gtchglzsqc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtamaipqty.html

JS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtiunooqmz.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtrlfmfved.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.haohaochexian.top/gtcrehgnxv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guowangkeji.top/gtquzrpmrj.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtttgpgdoa.html

C#:   Parallel.For
来源：http://hz.wangshuangyany.cn/gtnaoqrniy.html

================================================================================
来源：http://hz.fengsongda.top/gtmnorpvwu.html

P. 常用工具函数
来源：http://hz.dashuyun.cn/gthgadbmce.html

================================================================================
来源：http://hz.mhx1999.top/gtpnubxnqk.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtewagyllx.html

Py:   str(uuid.uuid4())
来源：http://hz.jlsjyb.cn/gthukoykxc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aizwys.cn/gtiisbjvhg.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtobymuwvp.html

TS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtiikqfwva.html

Java: UUID.randomUUID().toString()
来源：http://hz.hfpthk.cn/gtzxnuttqr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tanke756.top/gtddxxekcd.html

Ruby: SecureRandom.uuid
来源：http://hz.ydzc1.top/gtymrbvglo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.0kj1m.cn/gtngnjxmnh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgufenzy.top/gtlnbzxoga.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtwpivwhtj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cheryme.top/gtfkqhpdvp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gtloekmczm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.52xcode.cn/gtvafuvove.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.316326.xyz/gtfdtklzjp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgfzy.top/gtwsbohmny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shangyingyoupin.top/gtomckoxbw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtfbmixhgm.html

[P03] 生成短随机字符串
来源：http://hz.ivvv.top/gtesrxdwat.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtwmzmtcry.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gaohongyu789.top/gtvdkjzzyw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtfmliczgj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtxizxpaqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shuidangran.top/gtststyrei.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gttciuqpca.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtyoxvinni.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gtebfsuhbh.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtbvdxvhaf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.smart0.xyz/gtsubmpntf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtlinqvycb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtecjivgxg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtqvpnxodb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.mhx1999.top/gtpnkpjyov.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gtydybgoqn.html

Ruby: x.length;  x.size
来源：http://hz.daxiang520.top/gtwtyugurv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtjfldocbd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gtewrbiwba.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xingfuxueyuan.xyz/gtugxdgqcr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtcpsudomq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jianghu66.top/gtlrmcdfkx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxuanxn.top/gtaeaxhyos.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtfbbezhoh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gotoacloud.top/gtagavbrzp.html

Ruby: a == b
来源：http://hz.9152youxi.cn/gtjznuicfs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtndajvyqs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtblqqslml.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sweek.top/gtaibyjgvv.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtcgcqqsau.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtlisgovzq.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangtech.top/gtavnldnvq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.havefunace.top/gtahjodqlf.html

Go:   if x == nil {}
来源：http://hz.daria6918.cn/gtaxiruozg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gtxpcuduwl.html

C#:   if (x is null) {}
来源：http://hz.daria6918.cn/gtyfttocok.html

[P07] 防抖与节流
来源：http://hz.xziqi.cn/gtccyglbhk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daria6918.cn/gtknpekple.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtojwlbeyi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtaslyzsqc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtxtwuulmq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhongyouzk.top/gtgwwjchin.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtpzhcjhgr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258888.top/gtxkdigdtk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtsakjdlri.html

[P08] 处理浮点精度问题
来源：http://hz.wangshuangyany.cn/gtwtsfroit.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtnownyvvw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.havefunace.top/gtwczyuhdf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtxekvpted.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gaohongyu789.top/gtqkieagfg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dashuyun.cn/gtflrekgso.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtwffngota.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtxurmrpfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuetiantiany.cn/gtbmxjveoc.html

================================================================================
来源：http://hz.yueranfly.top/gtayzejoqv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hysaishi.cn/gttxvjplnr.html

================================================================================
来源：http://hz.yongpay.top/gtmxoviuao.html

[Q01] 创建表
来源：http://hz.yj20258.top/gtnuoxdaui.html

CREATE TABLE users (
来源：http://hz.wangshuangyany.cn/gtkkggoouz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtpbecimbb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dashuyun.cn/gtgfuszbfh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cucudq.cn/gtecbtjely.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gtomhwvtem.html

);
来源：http://hz.meibo888.top/gtnzbsxqsw.html

[Q02] 创建带外键的表
来源：http://hz.0kj1m.cn/gtbrfdstkk.html

CREATE TABLE orders (
来源：http://hz.guannengcc.top/gtutmbehou.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtopnwixrz.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtqhzxnwwb.html

amount DECIMAL(10, 2),
来源：http://hz.smart0.xyz/gtsaxfmnws.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pengpengdd.cyou/gtjizjgwwc.html

);
来源：http://hz.cdnleiting.top/gteaxqpsst.html

[Q03] 增加列
来源：http://hz.ydjk.org.cn/gtvevimpyj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yangfankeji.com/gtpihyoouf.html

[Q04] 修改列类型
来源：http://hz.sxryk.cn/gtmgzbvgwc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pycfn.com/gtzbkywove.html

[Q05] 重命名列
来源：http://hz.jqgfzy.top/gtflzpwpxq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtmnzjhurb.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gtpvrpltuq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtdxpeyypz.html

[Q07] 删除表
来源：http://hz.xuetiantiany.cn/gtpkjcitix.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenjidiqi.icu/gtkzgysxns.html

[Q08] 创建普通索引
来源：http://hz.guowangkeji.top/gtttprhrqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhongyouzk.top/gtrlvlsjzb.html

[Q09] 创建唯一索引
来源：http://hz.gaohongyu789.top/gtwqvgvtpu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtbsymgyrp.html

[Q10] 插入单行
来源：http://hz.jyoumei.cn/gtfhpeloqy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtdesgggsl.html

[Q11] 一次插入多行
来源：http://hz.shzxlz.cn/gthpqjurut.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtmwubsxlj.html

[Q12] 插入后取自增 ID
来源：http://hz.yangfankeji.com/gtwwohqhci.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtcvogihgh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtfxkpryil.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtczaupuda.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtbpxckoua.html

[Q14] 存在则更新（upsert）
来源：http://hz.tian-w.cn/gtgfvgrzle.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sweek.top/gtgcxsczug.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtnyypwkop.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtvvupezku.html

SELECT * FROM users;
来源：http://hz.ivvv.top/gtgfwisrds.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gthnaiolxu.html

SELECT id, name FROM users;
来源：http://hz.yj202588.top/gtqrksjtbe.html

[Q17] 条件查询
来源：http://hz.birdmap.top/gtclebywdj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.birdmap.top/gthehpdcdt.html

[Q18] 模糊匹配
来源：http://hz.cheryme.top/gtfmtqrnzg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gtfxogagra.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtviebietw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.smart0.xyz/gtrqjxubxm.html

[Q20] IN 列表
来源：http://hz.chenjidiqi.icu/gtmtmavjmr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtrcddpzth.html

[Q21] 空值判断
来源：http://hz.tian-w.cn/gtmuovzldw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aizwys.cn/gtxqskeejg.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtjuxkaqbl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gotoacloud.top/gtvnfzlppc.html

[Q23] 分页
来源：http://hz.cheryme.top/gtmfasuqao.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pengpengdd.cyou/gtliqfkyqd.html

[Q24] 去重
来源：http://hz.nwbrower.top/gtrlxwhuzy.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gttknisldq.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtcfnzieko.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gtklalbwet.html

[Q26] 计数
来源：http://hz.xingfuxueyuan.xyz/gtowwnuary.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinqigfzy.top/gtphktcphp.html

[Q27] 条件计数
来源：http://hz.zhoulong.xyz/gtqxtqosmj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xinyue.icu/gtmyukpfva.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtjkmytcrl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gtqjhlucmk.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtvjsqiqvv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtvafvvfsc.html

[Q30] 分组统计
来源：http://hz.meibo888.top/gtlmkxnqom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtteolvlvs.html

[Q31] 分组后过滤
来源：http://hz.smart0.xyz/gtrqpuxlrn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xuanzx.com/gtzhyccytm.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtepsdhoon.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtooiswkwv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jiagoushi.top/gtoopqzads.html

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gtywtsrxqy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fzhhl.top/gtzmhyxaqx.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gtexhzcvkl.html

SELECT * FROM (
来源：http://hz.316326.xyz/gtvqzvwpop.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuanzx.com/gtcpleinlr.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtptezobnb.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gtnrfurcsh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtutreoibc.html

[Q36] 左连接
来源：http://hz.zhaomingkeji.xyz/gtablstlck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtarmwsuky.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtwozvywtf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shuidangran.top/gthzvhoifm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtzhtcxeue.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gtmzfhqton.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gtnkahdlwq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yangfankeji.com/gtjygiymah.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.feifeiyinyue.top/gtgbvigoud.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtjdvxpjud.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gtbzvaqzsn.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gtisjawyha.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.birdmap.top/gtjcdnicwb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gogol.net.cn/gtntkjtcbb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cashguo.top/gtoktxhaos.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtmohuzpji.html


<!-- 参考信息 -->