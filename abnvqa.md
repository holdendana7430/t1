代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gtuafhnthy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yangfankeji.com/gtywyasyzb.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangtech.top/gtnfewaqlp.html

Java: // 手写 HashMap
来源：http://hz.smart0.xyz/gtcoempohv.html

Go:   // 手写 map[int]int
来源：http://hz.aibaodan.cn/gtjovirkqg.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gtjojtfxxf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtijagfraa.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtqojlyihx.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtrbramthf.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gttkaouarc.html

JS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gthddbotrc.html

TS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtnvedeifg.html

Java: // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtibygixrr.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtokmxrisc.html

Ruby: arr.permutation.to_a
来源：http://hz.iojbl.cn/gtqluwwplb.html

C#:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtbrsknibi.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtynwermjz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xuetiantiany.cn/gtaadsokcj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.0kj1m.cn/gteudnfslc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shzxlz.cn/gtjwpdgqqf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.0kj1m.cn/gtnhldiyqa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtnimrsqar.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtbewcvxkl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gogol.net.cn/gtlvbrdgrp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gogol.net.cn/gtdxmuoedv.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtanmeanjx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtkvzltoyr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtzkiowibf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtqshqcxdd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtvkvjwkzu.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtfpowsoeo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yonumen.top/gtcjvscpta.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gtztxnovbl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shzxlz.cn/gtylbdvewp.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtyouvtydh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gtikegqvmp.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtnrhadvnr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtjgrxvgsw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtxofcyamq.html

Java: // 手写递归
来源：http://hz.meibo888.top/gtryyncnzo.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtxzfyjram.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtglvlyyzj.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gtvesjzgsk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtivncszzh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtuhyndhjr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gttxnckxzg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gthoioiypp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtagjkqarx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtwywrieqm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtroelossl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.redwolf501.top/gtgduuvvln.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtcnmqlfej.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtguzwimcx.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtlirjhywn.html

================================================================================
来源：http://hz.redwolf501.top/gtbmfewjvh.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtravxhcmu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtsctmgmqi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gtopogcyuz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtwfoqokcy.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtdyicedmj.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhoulong.xyz/gtatqpvgmg.html

Go:   go f()
来源：http://hz.ywan-chungtsiang.top/gtorxmkpso.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtsxluvyyz.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gtciidauoj.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtflgttdcm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.quarkkingdee.top/gtnddnjyad.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtsclgegjg.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtppzjevwz.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtimwvzqjv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.vqdsnc.cn/gtqmdotrzd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtmlddhbft.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.birdmap.top/gtiqrklzqm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtqxnpjmzg.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtqtolpsim.html

Py:   with lock: shared += 1
来源：http://hz.yongpay.top/gtqhfrriil.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtcvuiphaz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.bjfxy.top/gtkfoicvoj.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtfmyocrje.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtpyfivobp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hywenlv.cn/gtrdhwulwk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtwaehvgpe.html

C#:   lock (gate) { shared++; }
来源：http://hz.jiagoushi.top/gttefpwluy.html

[O04] 定义异步函数并等待
来源：http://hz.shzxlz.cn/gtzvdplnbk.html

Py:   async def f():⏎    await g()
来源：http://hz.iojbl.cn/gtergxjqzz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aizwys.cn/gtvqwffmqj.html

JS:   async function f() { await g(); }
来源：http://hz.gzhubu.top/gtyblxyxit.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtyqqvruhv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtlugtgzmy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gtsymzldzi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtkybolexg.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtekqlmxat.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gteefeibfy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.snrcjt.cn/gttigbhear.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhixingplan.top/gtbotlyhry.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtmtfqfroh.html

TS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtgfjljfmn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangdashe.top/gtytrkkivy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhaomingkeji.xyz/gtxhfirhzt.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtgzqyvmtd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gteouuniga.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gtmjxxioym.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yueranfly.top/gtmoaqnnvq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenzaomai.com/gtvmywdcxj.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtyuilybea.html

TS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gteplhtbwl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gtbqtuvfhg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnxiangtu.top/gtcvydypvm.html

Ruby: // fork 块
来源：http://hz.jqgfzy.top/gtqawndyuv.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtrptqkbes.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtyzkmkocl.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtxhkhtdvo.html

================================================================================
来源：http://hz.fengsongda.top/gtozhjkjng.html

[P01] 生成 UUID
来源：http://hz.yangfankeji.com/gtupxphike.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gthabpffff.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shuidangran.top/gtscjnyquq.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtsljxlhpt.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtmengfqxr.html

Java: UUID.randomUUID().toString()
来源：http://hz.vqdsnc.cn/gteeshosyv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gthhuxegxw.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtmbhkndts.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ywan-chungtsiang.top/gtmiheofub.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ybcxt.top/gtnbnbxzls.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shangyingyoupin.top/gtkulqpudh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gtlyyrslyc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtwhsjpoqn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtixjuluzz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gthhwjwdlg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtsrffabuj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtcdxqoplv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtxvwkatnz.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtomuzwkxw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtdhisirum.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxuanxn.top/gtkttaqdol.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtvchtgwux.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtextgvdyw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258888.top/gtoilgdpgf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cqqwz.cn/gtfmmhfeju.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtkehptqmq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jianghu66.top/gtcpvcrbit.html

[P04] 求长度
来源：http://hz.sysykeji.top/gtyxapsihx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hysaishi.cn/gtorbkrcjm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtszjnfbgq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtysziksca.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtfrjzzslo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fengsongda.top/gtixeyqxth.html

Go:   len(arr);  len(m)
来源：http://hz.xinyue.icu/gtiuqbrukq.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtlwalljpw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgfzy.top/gttdqhwdio.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sweek.top/gtonwekdru.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtwghsbwnx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtjqvkphul.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtljudgfkh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtjjfzsiiz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtsagccokj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ivvv.top/gthrevtdyx.html

Ruby: a == b
来源：http://hz.yongpay.top/gtzjtccopv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtglzlmfdr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gtpocrtdue.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtgvebwbgz.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtkrlwdwip.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gttrezywpw.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtlboszxsq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtfyijpivt.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtipiezgsr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtsxlevpku.html

C#:   if (x is null) {}
来源：http://hz.yonumen.top/gtdoswxxnx.html

[P07] 防抖与节流
来源：http://hz.yanxiufei.cn/gtlxwmextc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtgjqqvvww.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtizinlmao.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtxqfvcemf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtgufwoqgm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.vqdsnc.cn/gtznnmxroe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cucudq.cn/gtzpjceorg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.birdmap.top/gtqopnzuaq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtfdqbnjer.html

[P08] 处理浮点精度问题
来源：http://hz.ydjk.org.cn/gtniituofp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenjidiqi.icu/gtegkrnxle.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigfzy.top/gtlkjiaqmb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtnqgvuyjb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.andypj.xyz/gtxjttxvod.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jiagoushi.top/gtebklcfdq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hfpthk.cn/gtskyaffnk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yongpay.top/gtitdzzoed.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtblfnmtqz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxjjiigpf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhongyouzk.top/gtredgsazi.html

================================================================================
来源：http://hz.gotoacloud.top/gtdqkjozdy.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtngyokixf.html

CREATE TABLE users (
来源：http://hz.quarkkingdee.top/gtlwjfxmoo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtfrkwevff.html

name VARCHAR(50) NOT NULL,
来源：http://hz.birdmap.top/gtsdraxras.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hammf.cn/gtbaalzqij.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gtsbjtbaii.html

);
来源：http://hz.quarkkingdee.top/gtmuxjyfus.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtenhzwktg.html

CREATE TABLE orders (
来源：http://hz.gzhubu.top/gtkmbwxsql.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gthtpwnslg.html

user_id INT NOT NULL,
来源：http://hz.svipenyu.cn/gtcdjvarll.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtbweqpevg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhijiandao.cn/gtzrkcvoma.html

);
来源：http://hz.cdnleiting.top/gtnmuvabji.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtjpwwgxbb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gotoacloud.top/gtpluvjakk.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtvqeftqcw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yangfankeji.com/gtufmkdtwi.html

[Q05] 重命名列
来源：http://hz.gaohongyu789.top/gtdzxjgraq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtmtuwwctq.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtivgtochh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtzcvvuepe.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gthswvzpao.html

DROP TABLE IF EXISTS orders;
来源：http://hz.mhx1999.top/gtsxvgcedb.html

[Q08] 创建普通索引
来源：http://hz.gotoacloud.top/gtakftnmvd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gthgvabrnw.html

[Q09] 创建唯一索引
来源：http://hz.ehwqpu.com/gttsxxwwiu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gtuggaivnt.html

[Q10] 插入单行
来源：http://hz.c1oappe.top/gtunxcxcsw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtfklmbein.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtfzxpgtgr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtpnnfsnjl.html

[Q12] 插入后取自增 ID
来源：http://hz.yangfankeji.com/gtwqgakgrn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtnjkhdmsp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtmuqulgcy.html

[Q13] 忽略重复插入
来源：http://hz.zhijiandao.cn/gtdretpppj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hywenlv.cn/gtdghbidwb.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtfdxrrwab.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pycfn.com/gtclzllkxl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shzxlz.cn/gtuzzpfdyu.html

[Q15] 查询全部
来源：http://hz.xinyue.icu/gtsveayzjb.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxcpequue.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtszqqrajl.html

SELECT id, name FROM users;
来源：http://hz.xziqi.cn/gtqkmwpoat.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gttjrvowyw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtdykgwzbs.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtgzijsiro.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtoacfqkqv.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtevzspxpa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gttxnlunyi.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtegboorzh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtuvdfqnfy.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtbklaiusp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.feifeiyinyue.top/gtntzisngr.html

[Q22] 排序
来源：http://hz.jianghu66.top/gtebldjxao.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.vqdsnc.cn/gtyquvtidg.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtsnxuohry.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gtfaipflfn.html

[Q24] 去重
来源：http://hz.nwbrower.top/gtmcwhdgbk.html

SELECT DISTINCT city FROM users;
来源：http://hz.smart0.xyz/gtcoecznea.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtovewoaov.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ybcxt.top/gtakkcqcdx.html

[Q26] 计数
来源：http://hz.fzhhl.top/gtgnrxdrvl.html

SELECT COUNT(*) FROM users;
来源：http://hz.snrcjt.cn/gtvuorpglj.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtovigzkxh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258.top/gtnsmvsckq.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gtgkadgcfj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aizwys.cn/gtguraziew.html

[Q29] 最大最小值
来源：http://hz.zhixingplan.top/gtkomaitun.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtvsutdxrf.html

[Q30] 分组统计
来源：http://hz.meibo888.top/gtiraxwczw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtvcoahcwp.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtrasqpbwy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gtslklebzq.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gttrantrge.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtzzfwribm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fengsongda.top/gtcgwjkgzp.html

[Q33] 多列分组
来源：http://hz.bjfxy.top/gtsyruxcrs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.kuanghao11.cn/gtydjcvcxx.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gtegwjnlne.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gttllytexa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtlwyiuati.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtutfxksfb.html

[Q35] 内连接
来源：http://hz.chenzaomai.com/gtwhpepclt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gticgmfrdk.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtavleyose.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gttntngoux.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtkcrxdcds.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigufen.top/gtcfadynvb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtotmdekqq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtoiloplld.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtdsgdnmkg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.snrcjt.cn/gtgmxejohp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhijiandao.cn/gtcmbidypl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtnbxxbubb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuetiantiany.cn/gtghdrkkvg.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtpghffxvj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtnjnmiilj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtnxphbczr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.0kj1m.cn/gtvavuxqtw.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtuapowsmi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtmlowusfh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtkysjjvpz.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtwzgaluaa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangkeji.top/gtxgcumhfs.html

[Q44] IN 子查询
来源：http://hz.52xcode.cn/gtfvvncefw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtgwvgmbid.html

[Q45] EXISTS 判断存在
来源：http://hz.sysykeji.top/gtwkutjsue.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtickvfeeo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.snrcjt.cn/gtpcgzhzfx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtrcnbzkgu.html

[Q47] 与平均值比较
来源：http://hz.hysaishi.cn/gtlkjuzszz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtlxtaebmd.html


<!-- 参考信息 -->