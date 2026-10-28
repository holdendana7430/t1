代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.yvedp.cn/gtdeznehzu.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtpdhnfclp.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtkutkfcfp.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtnclqviln.html

Java: // 手写回溯递归
来源：http://hz.52xcode.cn/gtacxuzgrb.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtgntjfdqs.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtfumxhrgi.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtktqpisxt.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtacxcwglh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guowangkeji.top/gtwxfkbpbf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtjvhbgsex.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtxvneoszt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenlongwang.top/gtfnujzbmh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtcfznrwme.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gotoacloud.top/gtvfswpxck.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtcwughhug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shuidangran.top/gtlemdzfmy.html

[N10] 链表节点定义
来源：http://hz.meibo888.top/gtctgucboc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenzaomai.com/gtfwtxvvpu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhoulong.xyz/gtfqqgxmnk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtgvmzsirm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.smart0.xyz/gtbsqtskhz.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxinkj.top/gtcltchxis.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtuogdqovj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtznttocwo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtlylzwssi.html

[N11] 二叉树中序遍历
来源：http://hz.hywenlv.cn/gtvnjkoozt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenjidiqi.icu/gtnyltdepf.html

PHP:  // 手写递归函数
来源：http://hz.guowangkeji.top/gtcfbcbnsd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtbccoexyd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtthgxjmmu.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtzkxcywbu.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtrumduinc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtuiomecbp.html

C#:   // 手写递归
来源：http://hz.yonumen.top/gtytddevxq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gotoacloud.top/gtjmkyslly.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gtfrxoluxx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gthrrzoiyd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtoopollki.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtpavhsgoo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtjyodfygk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sxryk.cn/gtjvpjtmfp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xingfuxueyuan.xyz/gtfrdmkkwt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtytpzkfue.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttrosfegf.html

O. 并发与异步
来源：http://hz.ivvv.top/gtbnpwqahf.html

================================================================================
来源：http://hz.hammf.cn/gtgsrkwhzq.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtypvjnhmw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yanxiufei.cn/gthswzdcno.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sxryk.cn/gtdvwpialx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tianlin.xyz/gtfecxzyib.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtikpcihwd.html

Java: new Thread(() -> f()).start()
来源：http://hz.gzhubu.top/gtmxhjtifc.html

Go:   go f()
来源：http://hz.vqdsnc.cn/gtvjfvsoys.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtapnsoltu.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtouictnkf.html

[O02] 使用线程池
来源：http://hz.aizwys.cn/gtrifqjkcm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtqgqthufr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gogol.net.cn/gtpnzmmbhv.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtnmjmlggp.html

TS:   // worker_threads 线程池
来源：http://hz.pycfn.com/gtstaqmcxq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.redwolf501.top/gtvftdpmdj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258.top/gtaxdxqoad.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gtyyogaegq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtvilufthc.html

[O03] 加锁保护共享数据
来源：http://hz.jianghu66.top/gtszyznjmm.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtzvreglck.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtgovguruq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gttacijgpx.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtziryqdhl.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gtktdkpntu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtsnppbsew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtrwrcwvhr.html

C#:   lock (gate) { shared++; }
来源：http://hz.xziqi.cn/gtbzqbcsli.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtnikngglm.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtrtbrdfog.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jiagoushi.top/gtjheeclvm.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtcpraraqi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pycfn.com/gtypuozouc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gtwgofqieu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtztwbsroz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtduxkxpug.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtvmgnrogm.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gtapypogam.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yanxiufei.cn/gtkperqpab.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gtreasjyoe.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtpzgngpmk.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtzxpavbxu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xylfe.cn/gtpiwtxtfk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtnhwjlzek.html

Ruby: threads.map(&:join)
来源：http://hz.316326.xyz/gtgusatneb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtukerodcf.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtpyieyxcw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtlwxupstk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtrmdxxxhr.html

JS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtskbsqmng.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtrvoyhmce.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtxuhognzj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gtqdnggchw.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtifrngdra.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtthwyblyv.html

================================================================================
来源：http://hz.52xcode.cn/gtujviuodb.html

P. 常用工具函数
来源：http://hz.shanyushiyangkeji.top/gtcsfaooct.html

================================================================================
来源：http://hz.yj202588.top/gtrwbgxhbf.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtjaqyjljx.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtfzciwyjp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtzqteiqpa.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtwykbryam.html

TS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtvgafyubp.html

Java: UUID.randomUUID().toString()
来源：http://hz.jiagoushi.top/gtqlyctklr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.redwolf501.top/gtdavwoypt.html

Ruby: SecureRandom.uuid
来源：http://hz.ybcxt.top/gthffxllfo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtyezwcmky.html

[P02] MD5 / SHA256 摘要
来源：http://hz.316326.xyz/gthnirvxrn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtzqzgbgbr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gtercayfho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtizzctpgz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gtbwzeavyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtwefsdptg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtcmzyztyr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yangfankeji.com/gtweujmtfm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zycfv.cn/gtbuslscym.html

[P03] 生成短随机字符串
来源：http://hz.zhijiandao.cn/gtvrimpeyg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zdqjudy.top/gtbtkrjkdt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtipiezyme.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtypypajic.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtpzxpbkfl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuanzx.com/gtpknglamv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtvrulfscc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sufxvd.cn/gtmmidnefa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gtyiikxmsv.html

[P04] 求长度
来源：http://hz.fengsongda.top/gtoyzkjwwp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dianchejie.cn/gtqmponury.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtblyvwdxr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtwrwilxqk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtxyqmhzxz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gtqxmcibry.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtolvkrwoi.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtsmyhnplz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtripylpad.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gtnfgzwwvy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgfzy.top/gtkfnaaqys.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtdgoebqtk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtfzruivww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtphqrlncw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tian-w.cn/gtcyufmlas.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gtklfzvwiz.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtgvjxljrc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgfzy.top/gtgwassksy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtxrbxvmsb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgfzy.top/gtjwponnix.html

PHP:  if (empty($x)) {}
来源：http://hz.yuanzhike.top/gtlffpjtjv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gtfaiidebl.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtkxakgkre.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fengsongda.top/gtpnthvlak.html

Go:   if x == nil {}
来源：http://hz.hnqzz.top/gtjcnjtcei.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtvffsajnw.html

C#:   if (x is null) {}
来源：http://hz.sufxvd.cn/gtmbtybpuf.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtpbxtqujh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gzhubu.top/gtvkrhaeda.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtrtipezns.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtvyilihtg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtpurgzzlf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nwbrower.top/gtuzsffipt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtxruudmhm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtfzfxzdia.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtlaheecth.html

[P08] 处理浮点精度问题
来源：http://hz.316326.xyz/gtegqdnman.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinyuanbaomall.cn/gtlgdwyhao.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xinyue.icu/gtvgzmthsd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtcxyjvaju.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhiwuduotai.top/gttzjywyft.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gttmpmprqg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gtytqoauau.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.c1oappe.top/gtcxiyuesu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtjbyvqxsy.html

================================================================================
来源：http://hz.bjfxy.top/gtrofbbdli.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ehwqpu.com/gtwtkfzzzp.html

================================================================================
来源：http://hz.fengsongda.top/gtgkzvzgcg.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtadodvdyd.html

CREATE TABLE users (
来源：http://hz.ydjk.org.cn/gtnvwgydba.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtxpxfvlpl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnqzz.top/gtjhrfqpvp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtynodwsqc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtxqwnjxdk.html

);
来源：http://hz.yuanzhike.top/gtalksgnse.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtzkxmdjix.html

CREATE TABLE orders (
来源：http://hz.cucudq.cn/gtlxwhukvw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtvyfskzhp.html

user_id INT NOT NULL,
来源：http://hz.zhixingplan.top/gtdonbvasm.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtjqsvtjnz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtmeewcjhv.html

);
来源：http://hz.nanxuanxn.top/gtzfepstdi.html

[Q03] 增加列
来源：http://hz.ydzc1.top/gtcplovhdk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuxming.cn/gtnarmoqzl.html

[Q04] 修改列类型
来源：http://hz.hnxiangtu.top/gtayremlfw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ivvv.top/gtiyfvktzf.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gtmaqsxfka.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtduboljoh.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gtxploedwr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gthibkitlm.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gtpkdcvmtp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtxoyhjgwc.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtzalawmvg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtsreapepn.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtuscrqbrr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtafvpkfyu.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtcvwiiawz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtgdbyjlgv.html

[Q11] 一次插入多行
来源：http://hz.cucudq.cn/gtuhhdtdzp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gaohongyu789.top/gtlfwcmovf.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtvgauskjs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtdzhytllb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhoulong.xyz/gtlsspxuim.html

[Q13] 忽略重复插入
来源：http://hz.birdmap.top/gtqblffpgf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtyittulte.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtqafyczuk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtablttnld.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.havefunace.top/gtcyrrqgsf.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gtnfthwync.html

SELECT * FROM users;
来源：http://hz.iojbl.cn/gtmdmhvrqk.html

[Q16] 查询指定列
来源：http://hz.vqdsnc.cn/gtwiznqbmi.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtcoulsmmr.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gtieqtfrci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shuidangran.top/gtiaclfnoq.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangtech.top/gtjeppnywk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtigkxdcty.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtdnxavura.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cucudq.cn/gtwpowxcbd.html

[Q20] IN 列表
来源：http://hz.zhaomingkeji.xyz/gtevxxxclz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zycfv.cn/gtmlfphlih.html

[Q21] 空值判断
来源：http://hz.shanyushiyangtech.top/gtgwatgxxc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtnwtrhxjs.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtbjxnhqmx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtpcvepkmt.html

[Q23] 分页
来源：http://hz.cqqwz.cn/gtpxtdjryg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hysaishi.cn/gtdhcdnupt.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gtpyakvfnh.html

SELECT DISTINCT city FROM users;
来源：http://hz.haohaochexian.top/gtfvpqapyi.html

[Q25] 只取前 N 条
来源：http://hz.ydjk.org.cn/gtftydvydm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtiparantb.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gthgtfmpso.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtbkqofybw.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtlurfysau.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtshjcaiip.html

[Q28] 求和与平均
来源：http://hz.jinyuanbaomall.cn/gtfillizes.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtohpdsrqp.html

[Q29] 最大最小值
来源：http://hz.fengsongda.top/gtkewlsykd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtgzyzggil.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtxxfwgxph.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtznoauavt.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gtaqnmyomz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dashuyun.cn/gtbiyiueus.html

[Q32] 分组拼接字符串
来源：http://hz.zhijiandao.cn/gtwslqxqpx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtgdgrxfbt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gtdqajcjsx.html

[Q33] 多列分组
来源：http://hz.yvedp.cn/gtxxjemtao.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtimsowdzm.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gtfjcxsbzk.html

SELECT * FROM (
来源：http://hz.pycfn.com/gthoxkzoma.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cucudq.cn/gtlzoowxbs.html

) t WHERE rn = 1;
来源：http://hz.ywan-chungtsiang.top/gtwknjjywd.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtivlpgmtf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtwoaczjbd.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtomiwepkh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtwydeevja.html

[Q37] 右连接
来源：http://hz.ydzc1.top/gtlxpczvur.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtyfrpizya.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.svipenyu.cn/gtiuhtzslp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxinkj.top/gtskqgeqzd.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtaolganpj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cqqwz.cn/gtjgovhtrg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhixingplan.top/gtbwsozjrh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aizwys.cn/gtxdgnhgtw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangshuangyany.cn/gtpaveoqcf.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtudwqskms.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhijiandao.cn/gtdeaghoat.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aibaodan.cn/gtdlrwlcpx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tianlin.xyz/gtcwnyckbe.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangkeji.top/gtpxfmiynw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtyavxtxez.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtqueaehze.html

[Q43] 标量子查询
来源：http://hz.xingfuxueyuan.xyz/gtxkvyoqxe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtlrefbnvb.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gtqyczbiwq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtnvksqqpx.html

[Q45] EXISTS 判断存在
来源：http://hz.0kj1m.cn/gtnwcvcrfu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtzomkhlcy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yangfankeji.com/gtxpdsvtsf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtuyfirjkb.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtgwesxlkf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gthjqmrhqb.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtaycytovg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sysykeji.top/gtjsdrksav.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtazkwhvfj.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtrmclzgmf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtuxacempc.html

[Q50] 批量更新
来源：http://hz.gzhubu.top/gtoyijsiho.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtsjewepgl.html

[Q51] 用子查询更新
来源：http://hz.zhengqikj.top/gtdatgfqwb.html


<!-- 参考信息 -->