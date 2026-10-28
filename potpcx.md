代发 wailian999

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtpggresnu.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gthbpkmvps.html

Ruby: arr.permutation.to_a
来源：http://hz.0kj1m.cn/gtbujdebcq.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtkmifnklz.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gtnenmlruq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtgzwwbmow.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtgwhamlxo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtibkxhzqy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtkodnspox.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhoulong.xyz/gtlacqdbxw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.havefunace.top/gtryumxtba.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zycfv.cn/gtvglbcwza.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guowangkeji.top/gtqlrjclhq.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtkzgbdzdr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtkjhlkuhn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtartbwgka.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtmkbytxaf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jianghu66.top/gtiuaxgsrq.html

Java: class Node { int v; Node next; }
来源：http://hz.svipenyu.cn/gtdjfjiwdq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtlfnnpmhw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtctzurvdp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtbiuklzlp.html

[N11] 二叉树中序遍历
来源：http://hz.zhixingplan.top/gtbiqyqgds.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nwbrower.top/gtxerarmhr.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtvurogyar.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtvjtwpqld.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtuzkwmhlp.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gthcbdcfye.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtxaodenpg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtlozdsmbn.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtxnintvpi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtgvoxixan.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtkjkdcnyp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtsuzszbsk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gtdrtstsxc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtgvykhxzn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtaplaiami.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fengsongda.top/gtxbqgynuu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtfdjypdca.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtqvkfzmjp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxvglgagi.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtfrufwqof.html

================================================================================
来源：http://hz.snrcjt.cn/gtnpoxpezu.html

[O01] 启动一个线程
来源：http://hz.hnqzz.top/gtkibaawpu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtwvjbzksx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtedavtgbb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gtqdixofhg.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtmiduleju.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gthfwkmfgk.html

Go:   go f()
来源：http://hz.cqqwz.cn/gttifzhrng.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gtnhhzwoba.html

C#:   Task.Run(() => F());
来源：http://hz.sysykeji.top/gtbfggmdgo.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtansnmpog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.havefunace.top/gtsnxvjqwh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuetiantiany.cn/gtsmyvktyp.html

JS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtpjavddmv.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtprgxhcqc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shuidangran.top/gtzambwble.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.meibo888.top/gtdpbrfnej.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cashguo.top/gthiawaana.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtmquungip.html

[O03] 加锁保护共享数据
来源：http://hz.zhoulong.xyz/gtzoknbfpu.html

Py:   with lock: shared += 1
来源：http://hz.tianlin.xyz/gtbtjujtql.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuanzhike.top/gtkhuqucxs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtuoceyydt.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtaxbnrnnh.html

Java: synchronized (this) { shared++; }
来源：http://hz.shzxlz.cn/gttddkhozb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jianghu66.top/gtzjxaqkqb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yvedp.cn/gtqpysbvkq.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtqlrbabwe.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gticrdedme.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtixlylypj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtkpaexsdb.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gtxrzgtzxr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.c1oappe.top/gtqeddkmro.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtnvahtbum.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hfpthk.cn/gtekdwnkcm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shangyingyoupin.top/gtegzqwdzu.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtphnggvsy.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgfzy.top/gtzzszdtqd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ehwqpu.com/gtehpgxfpm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jyoumei.cn/gtxsksfrdz.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtoeussadi.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtcvuccwtq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dianchejie.cn/gtbkxhsfis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nwbrower.top/gtarpvlzmo.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtxpixlgut.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtqlzdsjrj.html

[O06] 使用进程池
来源：http://hz.chenjidiqi.icu/gtfpubwpbm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtvmaoczrt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ppjwa.cn/gtrmimwpch.html

JS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtuldhuiel.html

TS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtproezznx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gthbvfhvpw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hongshengwenyu.top/gtftcqzylg.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtoldvshcg.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtzfnlabtv.html

================================================================================
来源：http://hz.nanxinkj.top/gtazxaxajo.html

P. 常用工具函数
来源：http://hz.aizwys.cn/gtgddmzqtw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtswcqskwr.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gteacozldv.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtdatphewg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtzznbpbhs.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtibqbfwev.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtdfhdslex.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gtrimmjsnd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenzaomai.com/gtwguvkftr.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtknddxmfa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtfodxxoud.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtgbtpvijd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangdashe.top/gtiohasotk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daria6918.cn/gtsofsukzq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtbtxyvmew.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gtwivzuaoq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yangfankeji.com/gtkvzhbwyj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtqcfioydg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hammf.cn/gtpikipupb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gtdcmktyxb.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtsqyotubf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhixingplan.top/gtcwrcwlqq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtlplyqvmn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtjniymuwt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtoqcuipbt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtksisctag.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtjfkgzjbz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sysykeji.top/gtnayppcuz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtydxofqhr.html

[P04] 求长度
来源：http://hz.shuidangran.top/gtdfymdldu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtnducaqub.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtmwtznhai.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtzpywhznz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gthajtwmqw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtxgvarapz.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtvahwdtpc.html

Ruby: x.length;  x.size
来源：http://hz.xuanzx.com/gtdbyujedu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtfyvmpxph.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gttrxfodvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daxiang520.top/gtphxwngdd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pycfn.com/gtijuvqikh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guannengcc.top/gtoyjyyouh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtnozxkbxc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtvduqczzj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gteobmotsu.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtosnwlxow.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtrjrafnyu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtmpnuskux.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hammf.cn/gtymptznfc.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gtukfwmykv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fzhhl.top/gtahbpqdgd.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gteacgilth.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxinkj.top/gtysrceelb.html

Go:   if x == nil {}
来源：http://hz.yj202588.top/gtmstyabqa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtihxmjthl.html

C#:   if (x is null) {}
来源：http://hz.hywenlv.cn/gtecrnmzcb.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtnjykjxbn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cdnleiting.top/gtugtdcuhy.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgufenzy.top/gtihjdxnes.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtfejinuwp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtaddkfydt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtpvhwybfs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tian-w.cn/gtxrqkdygc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtwfalgzzt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ppjwa.cn/gtlphfkden.html

[P08] 处理浮点精度问题
来源：http://hz.xuetiantiany.cn/gtnvjmjgnb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xylfe.cn/gtzlnqbrxf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cucudq.cn/gtfaxieout.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gteuucbtwp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtpspiyefi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtcuqhakeb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtbavcljpp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtdvwsytcr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtjpepxyjn.html

================================================================================
来源：http://hz.cheryme.top/gtyjxgihrr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.snrcjt.cn/gttifdonrd.html

================================================================================
来源：http://hz.ehwqpu.com/gttsdhygxd.html

[Q01] 创建表
来源：http://hz.meibo888.top/gtufollexr.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtldwgzenu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtrulwhvsf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gtetbidaiw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtcrpedbvn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtsorxqfjg.html

);
来源：http://hz.sxryk.cn/gtlxslhsbn.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gtaasinpnd.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtmiyklejp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gthidjrjxq.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtfcraxpgh.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gthhzqzoyc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gthiivjrjm.html

);
来源：http://hz.nanxuanxn.top/gtqdgpsltr.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtrstztduh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xylfe.cn/gtqeaqzsda.html

[Q04] 修改列类型
来源：http://hz.havefunace.top/gtmjjzqbuv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtxfinkzzj.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtfafntnpf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtjsukjjzq.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtmcfpdtaf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtsxmvhass.html

[Q07] 删除表
来源：http://hz.feifeiyinyue.top/gtzefewzdu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhijiandao.cn/gtwowbuivb.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtzeqjzhbm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nwbrower.top/gtwepoyfoo.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtnylqdqyx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtxjvimdcx.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtyifuoryg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yueranfly.top/gtsijsbulb.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtstqglsuj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ivvv.top/gtiimwcuxw.html

[Q12] 插入后取自增 ID
来源：http://hz.feifeiyinyue.top/gtnwoqohqa.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtuhtwdziv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gotoacloud.top/gtnovscpsw.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtvzicfhbi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangtech.top/gtrpdgevow.html

[Q14] 存在则更新（upsert）
来源：http://hz.dashuyun.cn/gtghmqaozc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinghuilouyu.cn/gthszxzoax.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.daria6918.cn/gtvujkmivq.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtoqnraeqo.html

SELECT * FROM users;
来源：http://hz.andypj.xyz/gtjesgbgca.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtvgzlysqo.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtwszemlcj.html

[Q17] 条件查询
来源：http://hz.xuetiantiany.cn/gtilbzvndr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gtvcriwlrd.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtubfkurgo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daria6918.cn/gtawiiokqn.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtbqrzatjk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenzaomai.com/gtmlptyopn.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gthjvpdloh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtxhimljdw.html

[Q21] 空值判断
来源：http://hz.gogol.net.cn/gtqckhroka.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxinkj.top/gtdvojerny.html

[Q22] 排序
来源：http://hz.ivvv.top/gtajdpbdxq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigufen.top/gtikamvgtr.html

[Q23] 分页
来源：http://hz.aibaodan.cn/gtyrikirru.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gotoacloud.top/gtqdwolybj.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtypcpxome.html

SELECT DISTINCT city FROM users;
来源：http://hz.havefunace.top/gtygngfisr.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtsaxxrtxb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtzovzrguk.html

[Q26] 计数
来源：http://hz.meibo888.top/gtweynogmr.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtetfupudf.html

[Q27] 条件计数
来源：http://hz.gotoacloud.top/gtelhlhyyz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daria6918.cn/gtmufovrwx.html

[Q28] 求和与平均
来源：http://hz.hywenlv.cn/gtsjsulqro.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jyoumei.cn/gtioofufyz.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gtwzhfyyno.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtoexhsofa.html

[Q30] 分组统计
来源：http://hz.tianlin.xyz/gtqmflojxn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gthpsdhapt.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtbbqyhnmk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xylfe.cn/gtibjkvaja.html

[Q32] 分组拼接字符串
来源：http://hz.ybcxt.top/gtldzpavnm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtmkdgbbgr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtspewxcwp.html

[Q33] 多列分组
来源：http://hz.redwolf501.top/gttbxwnqth.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenzaomai.com/gtlsrtjvuj.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtxkxbqcbj.html

SELECT * FROM (
来源：http://hz.shangyingyoupin.top/gtcptccqtf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yangfankeji.com/gtmshfpwgg.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtfxcwdsfa.html

[Q35] 内连接
来源：http://hz.andypj.xyz/gtuwrohhmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtznautyxv.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtbljxhbgm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtzuuffsfv.html

[Q37] 右连接
来源：http://hz.cashguo.top/gteylsfulm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xziqi.cn/gtjgcxpjyd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daxiang520.top/gtxuxrdlsz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tanke756.top/gtrzzzygdk.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtfeidhady.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daxiang520.top/gtjnnxgamo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yonumen.top/gtadvlgvwb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ivvv.top/gtyflkywky.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hongshengwenyu.top/gtiyoaqaik.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtzdvafukb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gotoacloud.top/gtrmihwlsj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhengqikj.top/gtsnffjjkw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ehwqpu.com/gtcjceshaz.html

[Q42] 连接条件附加过滤
来源：http://hz.haohaochexian.top/gtqxdorpox.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtdzkarnfl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtabfdxjmo.html

[Q43] 标量子查询
来源：http://hz.yj20258888.top/gtbwrrpsua.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtnpalivdc.html

[Q44] IN 子查询
来源：http://hz.yangfankeji.com/gtmyeflzpb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cqqwz.cn/gtrcyvhhpj.html

[Q45] EXISTS 判断存在
来源：http://hz.chenjidiqi.icu/gtmsnktkgt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenjidiqi.icu/gtllacdekr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtdchisquw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtarkbminj.html

[Q47] 与平均值比较
来源：http://hz.zhaomingkeji.xyz/gtsmiwdltm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zycfv.cn/gtgwzctlpq.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtdnqanjvm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtcagukhzk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xinyue.icu/gtkwdnjcni.html

[Q49] 更新单行
来源：http://hz.aizwys.cn/gtnzszektz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtarebjskf.html

[Q50] 批量更新
来源：http://hz.yanxiufei.cn/gtbrpvkgae.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gtffbvaocp.html

[Q51] 用子查询更新
来源：http://hz.mhx1999.top/gtififrvot.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtxrlcoxcg.html

[Q52] 删除指定行
来源：http://hz.wangshuangyany.cn/gtckxihunm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gtwdeimvlc.html

[Q53] 按条件删除
来源：http://hz.ydjk.org.cn/gtphqtgjhl.html


<!-- 参考信息 -->