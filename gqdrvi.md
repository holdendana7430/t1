代发 wailian999

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtawbzsdoj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtzdgsdfkw.html

[N07] 两数之和（返回下标）
来源：http://hz.jlsjyb.cn/gtwcbxjehn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtroqzbcqd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yangfankeji.com/gtxsqqkbve.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gthjykjbpy.html

TS:   // 手写 Map<string, number>
来源：http://hz.birdmap.top/gtrwbhcagb.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtkualebku.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtvrhdhzjp.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtdpopyyxr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangkeji.top/gtzhtqiznm.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtmvtvdkdo.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtroszieuc.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gtxlgbfrgz.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtuuaakyez.html

TS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtwdaxohza.html

Java: // 手写回溯递归
来源：http://hz.9152youxi.cn/gtjzkknldr.html

Go:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtvgamylqk.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gtxrjezgft.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtciifyiva.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gtynxwtvfs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hfpthk.cn/gtlyujztyd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gotoacloud.top/gtcezkcrua.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtsbweulyu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.birdmap.top/gtfjfulrdw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtgcrsyrhz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtkeinobyp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtvequpkva.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtbdjykvsc.html

[N10] 链表节点定义
来源：http://hz.kuanghao11.cn/gtewtmwuzx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hfpthk.cn/gtbwammzyr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gtcccaysjt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gteevfxlzw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigfzy.top/gtlofyfmse.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtovxmgylr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtxjvrvjzo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtnecnsfnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtdwizklgm.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gthogwnuns.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtxekdilsq.html

PHP:  // 手写递归函数
来源：http://hz.ydjk.org.cn/gtfmuzcduh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gttacedyow.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtsspbjesn.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtlsqhbvft.html

Go:   // 手写递归
来源：http://hz.wangdashe.top/gtksmzlbbj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtcczufwhy.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtvmbpqzvo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gtookzozfd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtkljfzhsj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtdepghows.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtsttxcaze.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtejbhogwj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtjcuvdlfl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gtcfczhhbq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtkymvxovb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gttahypzsm.html

================================================================================
来源：http://hz.fzhhl.top/gtfdeoweuz.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gtqdddxofc.html

================================================================================
来源：http://hz.wangdashe.top/gtylkrchlb.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtpnetdssi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtyymujlob.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cheryme.top/gtlkfdubgb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.0kj1m.cn/gtbgggjlxo.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtbzmvxkck.html

Java: new Thread(() -> f()).start()
来源：http://hz.316326.xyz/gtetzysrbx.html

Go:   go f()
来源：http://hz.redwolf501.top/gtynzacrxy.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gtidbzsgeh.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtgyvggkbx.html

[O02] 使用线程池
来源：http://hz.ywan-chungtsiang.top/gtncvokwbc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtzfupyrsn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtqupxxgmd.html

JS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtmuycvfry.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtujdzgomt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtgmrbybza.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gtarnvddea.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tanke756.top/gtyetbhwsw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtunvvawpi.html

[O03] 加锁保护共享数据
来源：http://hz.gotoacloud.top/gtvuyezscn.html

Py:   with lock: shared += 1
来源：http://hz.chenlongwang.top/gtynmzvshb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yvedp.cn/gtngkhkvwh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yangfankeji.com/gtewhjiztt.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtwllkpomg.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtxoxwhmyo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gtnhpycghy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtbxvnnvtr.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtsnsaxios.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtitvxmfnn.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtpncdlihv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtuqjoiezc.html

JS:   async function f() { await g(); }
来源：http://hz.hnqzz.top/gtconpclyc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtlbxfvnej.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dianchejie.cn/gtlkjlosym.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.bjfxy.top/gtnytufhqj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gtwrlcmyub.html

C#:   async Task F() { await G(); }
来源：http://hz.pengpengdd.cyou/gtworgydqn.html

[O05] 并发执行并等待全部完成
来源：http://hz.cucudq.cn/gtvzliomvt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtgfvkkkai.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gttjdyjhmd.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtiexxzyfk.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtwagjqpzw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtslyqtvgd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hysaishi.cn/gtegaaisej.html

Ruby: threads.map(&:join)
来源：http://hz.jyoumei.cn/gtbhydtqcn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtesqjmgdc.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtweshvkpi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtdicxtbsg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtnvnciirx.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtnwacdctv.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtgkrpjiiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtwsovwjrm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtmkpwjthl.html

Ruby: // fork 块
来源：http://hz.daria6918.cn/gtnngtjedk.html

C#:   Parallel.For
来源：http://hz.xuetiantiany.cn/gtamxsgtaq.html

================================================================================
来源：http://hz.yueranfly.top/gtgypvpfxy.html

P. 常用工具函数
来源：http://hz.wangshuangyany.cn/gtpeswrvih.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxbrukrwh.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtgsjuduty.html

Py:   str(uuid.uuid4())
来源：http://hz.gzhubu.top/gtugvhuejq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xingfuxueyuan.xyz/gtneuzpcxp.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtlczdlgxe.html

TS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtrtgosjdj.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtedaboaib.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gthrifhsbd.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258.top/gttjkqyhvu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtwgluypeq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tian-w.cn/gtzwwcilci.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.0kj1m.cn/gtdktdwhsy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtuvrmnajk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gtnizdebby.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydzc1.top/gtjlulhmym.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtqkhbwoge.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yanxiufei.cn/gttvupuilv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtjyvxmptf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hammf.cn/gtjictgrgj.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtzslcnowk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sxryk.cn/gtvvetqfwq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtbjqgmvkb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtxomxcjdl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gttdhapwrk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.birdmap.top/gtoqkvnhwz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yvedp.cn/gtnifpuztb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gticpcfnxy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtjowurckk.html

[P04] 求长度
来源：http://hz.xziqi.cn/gtenqqcqhj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtxewtrfxs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtsqbhpiwe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtozqmdjoi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtodrpubyt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cheryme.top/gtuqemgdtx.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtlrxbfzvq.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gtawgiwyyy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtkxnewqxd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cashguo.top/gttnifjgnb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daxiang520.top/gthwmewcxh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shangyingyoupin.top/gttjfvlvma.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuanzhike.top/gtgopwxzdj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gzhubu.top/gtpjrwwdub.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtdehzybnh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.mhx1999.top/gtbbbhemoh.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtmlsiicyd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydjk.org.cn/gtilhhwykg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtqeehqasf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hysaishi.cn/gtvotyhdla.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gtqdgwiuqr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ybcxt.top/gtroepmzij.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gtjfciuwsq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gttiqaaehj.html

Go:   if x == nil {}
来源：http://hz.zycfv.cn/gtgoajvtnp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtbamhnlcq.html

C#:   if (x is null) {}
来源：http://hz.cashguo.top/gtowbvbekp.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtqurrsrey.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.svipenyu.cn/gtdysjrgrv.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtiefzbfmu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtdcqpfhbt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtswculhhs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shuidangran.top/gthmqkcmam.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ywan-chungtsiang.top/gtnyvgpxwj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shzxlz.cn/gtkripvzsu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtlmrzvxjn.html

[P08] 处理浮点精度问题
来源：http://hz.wangdashe.top/gtjystorgb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangtech.top/gtmmkgfjei.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtzlcypnkn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hysaishi.cn/gtlahngkzx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydzc1.top/gtoidcuqcs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daxiang520.top/gtehcanwez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtyctrngkc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pengpengdd.cyou/gttnwqukpi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gttkrlrasr.html

================================================================================
来源：http://hz.yueranfly.top/gtnoggjwyl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.316326.xyz/gtnagblgwp.html

================================================================================
来源：http://hz.ydzc1.top/gtductjbdp.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtnkasdhmd.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtmpxgrnrb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtpegcxyfc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtbpsvulvw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnqzz.top/gtrdokgzvq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtonfuandf.html

);
来源：http://hz.sxryk.cn/gtemezgims.html

[Q02] 创建带外键的表
来源：http://hz.zdqjudy.top/gtlvvnpmmx.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtnkbulyzs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtdggivlep.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtxcarkgmt.html

amount DECIMAL(10, 2),
来源：http://hz.cheryme.top/gtfsbjyucr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sufxvd.cn/gtjzwyinnx.html

);
来源：http://hz.pengpengdd.cyou/gtlpjuvrbm.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtpadyhnsy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhijiandao.cn/gttghqlxty.html

[Q04] 修改列类型
来源：http://hz.tanke756.top/gtwogzpasc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj202588.top/gtxjjwjofv.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtixnzquln.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangshuangyany.cn/gtpjdsxzqa.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtpwmfdiev.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtdzwzagte.html

[Q07] 删除表
来源：http://hz.cheryme.top/gtmcwkfjio.html

DROP TABLE IF EXISTS orders;
来源：http://hz.bjfxy.top/gtrhkkkqvc.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gtyshkickr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnqzz.top/gtbaqofrlx.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtikcmxptf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtqjrnjghe.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gtcabckbsi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gtwbzwxzpt.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtjmfbadqu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtbggovztg.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258888.top/gtxhgaxvjo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gttnyrugvj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xziqi.cn/gtzoohdyqj.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gtqvruxeob.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtrgjoomdp.html

[Q14] 存在则更新（upsert）
来源：http://hz.jianghu66.top/gtrkdvrtzb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtiqckohvc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gtuqstyufs.html

[Q15] 查询全部
来源：http://hz.jqgufenzy.top/gtxpxfdygn.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtqgaicaga.html

[Q16] 查询指定列
来源：http://hz.yj20258888.top/gthnlmsxxj.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtaquybdrh.html

[Q17] 条件查询
来源：http://hz.gzhubu.top/gtezfuygyd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tanke756.top/gtoiqcbpef.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtoentzids.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuanzx.com/gtykploidq.html

[Q19] 范围查询
来源：http://hz.jianghu66.top/gtzuwahbda.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenzaomai.com/gtadcwemno.html

[Q20] IN 列表
来源：http://hz.jqgufenzy.top/gtwqcbjaqa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtflporgmb.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtqjbktllf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtqhfqdeew.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtrtgmoqdo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guowangkeji.top/gtmakqirhr.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtafxfiqye.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gtdtjhhlbl.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtaecznxoo.html

SELECT DISTINCT city FROM users;
来源：http://hz.yongpay.top/gtqeyuzckz.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtpsapgjbd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtcmzwefku.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtsqryksoj.html

SELECT COUNT(*) FROM users;
来源：http://hz.birdmap.top/gtxfsyjjzw.html

[Q27] 条件计数
来源：http://hz.fzhhl.top/gtcsgpmrat.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gteejptooq.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gtowggnazv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtlepzadvw.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gtzjisyivj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gtqfucpdyq.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gtfrudotlo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtdiuhpeil.html

[Q31] 分组后过滤
来源：http://hz.yuxming.cn/gtvkjhbons.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtuxqqthvf.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtktommqth.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtcrxvcwuv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sufxvd.cn/gtfjdikbcs.html

[Q33] 多列分组
来源：http://hz.yj20258888.top/gtyhrljzaw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtmizkkshx.html

[Q34] 每组取第一条
来源：http://hz.zhoulong.xyz/gtaowvgkfv.html

SELECT * FROM (
来源：http://hz.c1oappe.top/gtxsgqyrnb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhoulong.xyz/gthmdgtsvo.html

) t WHERE rn = 1;
来源：http://hz.ywan-chungtsiang.top/gtwwlpxwfv.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtlbebqbsl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtsidotqsp.html

[Q36] 左连接
来源：http://hz.hywenlv.cn/gtglqxuseg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtaizhgkfd.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gthjfqiypb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtjnzjpyvf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtjjxictmd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.guowangkeji.top/gtwvjjvabv.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gthjoghtfv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cqqwz.cn/gtcasaqltx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtqsqmdmpb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aibaodan.cn/gtnpeheswe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangdashe.top/gtcvlsfklb.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtfcmcozcr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtoykmebuq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gtrosmxuui.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtnilimspm.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtdbmkdjbc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtdgipssgu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ppjwa.cn/gtwvdkmkay.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtavwuitzq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guowangkeji.top/gtxyytiohw.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtzkvsvjlr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aizwys.cn/gtselqmxii.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gttbusljpu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtvameoffx.html


<!-- 参考信息 -->