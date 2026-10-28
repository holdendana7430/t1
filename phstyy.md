代发 wailian999

[N09] 栈与队列
来源：http://hz.yonumen.top/gtbpklzdpt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xuanzx.com/gtljsnjaqj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtmwlhugdc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtlvskusis.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtyzfhoqzi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.haohaochexian.top/gtgsgytmfj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dianchejie.cn/gtocaijtgd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtfxdommkr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gthiluocdh.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtavczpcyw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hfpthk.cn/gtwdpswdoc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinghuilouyu.cn/gtriiycljr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtlhyhomot.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cqqwz.cn/gtskxuzodf.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtlwbxpuwd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gtgyhqqebj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangkeji.top/gtxeyjqorz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gtxzmckgen.html

[N11] 二叉树中序遍历
来源：http://hz.gaohongyu789.top/gtlhgthogo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydzc1.top/gtpsauyehg.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtistctjaj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gtsbbdargz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtvzuqftal.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtqnlwdqfa.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtshuywbbw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.mhx1999.top/gtgwsmeepv.html

C#:   // 手写递归
来源：http://hz.9152youxi.cn/gtoodaywgv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yvedp.cn/gtqanjnbtb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hongshengwenyu.top/gtqmotadkk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gzhubu.top/gthfyvubvz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtjrkqsfwo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtbtospsxx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtlliwzmgn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gtphxxtwux.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aibaodan.cn/gtqflhkpal.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtesrztukg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtrhrupgzs.html

O. 并发与异步
来源：http://hz.xylfe.cn/gteovxsuqr.html

================================================================================
来源：http://hz.yuanzhike.top/gtaiswsiva.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtnitawrgb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtbirxeioe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gthwtnctox.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.havefunace.top/gtvmcxedan.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gthbnlxkye.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenlongwang.top/gtbdctoxgx.html

Go:   go f()
来源：http://hz.yongpay.top/gtcczkblra.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtmpzhqexm.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtekrkbqrs.html

[O02] 使用线程池
来源：http://hz.jinghuilouyu.cn/gthxvkfose.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtmrlgsuzq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangtech.top/gthtnavlqz.html

JS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtcjttcfuj.html

TS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gthwcfaezh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtigbdqfkd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gtugjqbfsx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dashuyun.cn/gtembczket.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtcfvhdcas.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtzwaspvhg.html

Py:   with lock: shared += 1
来源：http://hz.wangshuangyany.cn/gtedczmudx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigufen.top/gtgsqnvnei.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fengsongda.top/gtpnjefkdw.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtuvuatbko.html

Java: synchronized (this) { shared++; }
来源：http://hz.yvedp.cn/gtsurpjzmv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydzc1.top/gtcshhpkkj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuetiantiany.cn/gtybziqidn.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gtafaofxrg.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtpsabdobp.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtmtejrham.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hongshengwenyu.top/gtpqvyftbx.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtnbcpruvc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hywenlv.cn/gtmqdtakdn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtdqtyiuwm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gtwxezigts.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cheryme.top/gtaidzjkzc.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gthvfszvrw.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gttjmonnza.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fzhhl.top/gtivmkbouc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhaomingkeji.xyz/gtetipelmw.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtvbgjifki.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gthoxvjpec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gtnqudtcve.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtzlkgkzcl.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtfncpqwqx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yueranfly.top/gtwcynrahq.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gtmgngkckn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.feifeiyinyue.top/gtneqnhhhs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tianlin.xyz/gtqbfurxly.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtgxasejol.html

TS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtosfspslb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigfzy.top/gtspgthhaz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aibaodan.cn/gtoilwirkq.html

Ruby: // fork 块
来源：http://hz.zhoulong.xyz/gtuqrenaem.html

C#:   Parallel.For
来源：http://hz.pycfn.com/gtjytxstpu.html

================================================================================
来源：http://hz.nwbrower.top/gtnjxghxdj.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gteajhjdqi.html

================================================================================
来源：http://hz.yj20258.top/gtrddnyqqe.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtnxfqppau.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtqecszjzh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yonumen.top/gtygsrzvji.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtybisdpwn.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gthppzbodu.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangkeji.top/gtzntprpvk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydjk.org.cn/gttaibekjx.html

Ruby: SecureRandom.uuid
来源：http://hz.iojbl.cn/gthowzsbhp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.smart0.xyz/gtmprpgsgl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.quarkkingdee.top/gtgrrqvswe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.havefunace.top/gtbiyuecss.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtemxkiyrq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hywenlv.cn/gtlmlumdkq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.andypj.xyz/gtctymthzv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangshuangyany.cn/gtbuedlazk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj202588.top/gtvugacgja.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gtdkkcnksw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.9152youxi.cn/gteogtmugn.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtkavgqwrz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gtvbsyxpmk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtpycbzxfl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtzyfnkxiu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtytcadeux.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangshuangyany.cn/gtgkmsqabq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jlsjyb.cn/gtctnxuykj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.0kj1m.cn/gtambrlyxq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ywan-chungtsiang.top/gtpqsvswep.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtgzvfdgha.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinyuanbaomall.cn/gtjginjoqx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtlobsivbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigfzy.top/gtyetxluuf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtksqzfvco.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gtbrmqkjra.html

Go:   len(arr);  len(m)
来源：http://hz.zhoulong.xyz/gtpbdwzdmh.html

Ruby: x.length;  x.size
来源：http://hz.shuidangran.top/gtmspdmfsz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtofixcnzp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gtwgzswrkb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fzhhl.top/gtsggqalda.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jyoumei.cn/gtzvendyql.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xinyue.icu/gtnygvqrcf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtfeyrcdcp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangtech.top/gtxvauliyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gzhubu.top/gtdwmlodrm.html

Ruby: a == b
来源：http://hz.sysykeji.top/gthaizayyk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gzhubu.top/gtbffqboum.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daxiang520.top/gtfkmdzpkn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.c1oappe.top/gtacexvjzm.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gtymxnmern.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinghuilouyu.cn/gtltetpcxt.html

TS:   if (x == null) {}
来源：http://hz.cdnleiting.top/gtxzpehlfb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtqggsoesn.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtjdqebkeg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ppjwa.cn/gtcvhwbrov.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gtkqugbape.html

[P07] 防抖与节流
来源：http://hz.xylfe.cn/gtekzoypeu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gtumktogew.html

PHP:  // 手写时间戳比较
来源：http://hz.sysykeji.top/gtcpztfqnd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtocwbvugg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtplepnfaf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gtbssethvv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pengpengdd.cyou/gtugkahhop.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtyaawmsce.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtilewtuau.html

[P08] 处理浮点精度问题
来源：http://hz.zhengqikj.top/gtwtqkzzir.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gtirmvwtey.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sufxvd.cn/gtnqjkwfyr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gthtrzglbc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtripambsp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guannengcc.top/gtqiraflri.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtfnliwsqg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydjk.org.cn/gtbcheqbhn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtipgyjgxq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwvtxxrmw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.bjfxy.top/gtapkoltzm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjumexizj.html

[Q01] 创建表
来源：http://hz.wangdashe.top/gtpobwoyav.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtzwmqmzta.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtgtnhcian.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtahpcfdvp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yvedp.cn/gtkpnajisd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtqnekwrfo.html

);
来源：http://hz.nwbrower.top/gtwffikeev.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtzkmuzhux.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gtwnlnbfkh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtrebrbekw.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtpimvnvcv.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtifcclavq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtjzyuudiv.html

);
来源：http://hz.wangdashe.top/gtvmqaveha.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtvaopzmhp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtteyubtln.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtenzsaehk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtsbhqmwjz.html

[Q05] 重命名列
来源：http://hz.vqdsnc.cn/gtdakapjbd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aibaodan.cn/gtorufsriv.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtrsovthsi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gteobaajpu.html

[Q07] 删除表
来源：http://hz.tanke756.top/gtyilzarrl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hysaishi.cn/gtjjnlxwxe.html

[Q08] 创建普通索引
来源：http://hz.smart0.xyz/gtrcqjnkcc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gthxkniipt.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gttzknzezr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258.top/gtltlsnrro.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtmadcojqy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnxiangtu.top/gtosddgcla.html

[Q11] 一次插入多行
来源：http://hz.gzhubu.top/gtdpxkeyml.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtztbzzwkr.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtxhhnvphl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtmxbsbeuc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangtech.top/gtbgtmdlyv.html

[Q13] 忽略重复插入
来源：http://hz.xziqi.cn/gttiajuqab.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gttcduycep.html

[Q14] 存在则更新（upsert）
来源：http://hz.tanke756.top/gtpappcwyn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydjk.org.cn/gtyzmjlsib.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtduaapism.html

[Q15] 查询全部
来源：http://hz.yj202588.top/gtppgahxql.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gtfiylwxjj.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtvwdewvar.html

SELECT id, name FROM users;
来源：http://hz.xylfe.cn/gtzgaxchfp.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtoetueous.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gtxjemhikp.html

[Q18] 模糊匹配
来源：http://hz.nanxinkj.top/gtcitatxta.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtcizljkrd.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gtdzeoulbs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhaomingkeji.xyz/gtbjmpalip.html

[Q20] IN 列表
来源：http://hz.jlsjyb.cn/gtmwcipctj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gtrmcjandq.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gthwtuaxkx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gtlrnthwvs.html

[Q22] 排序
来源：http://hz.hammf.cn/gtzpgejuws.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ehwqpu.com/gtderoiutl.html

[Q23] 分页
来源：http://hz.sxryk.cn/gtltcovqzd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydjk.org.cn/gthtiepwhi.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtdkypalnx.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtvjprtsju.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtqlbgrhil.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.316326.xyz/gtbhpiaobc.html

[Q26] 计数
来源：http://hz.gogol.net.cn/gtkjcqkaoj.html

SELECT COUNT(*) FROM users;
来源：http://hz.shuidangran.top/gtjkaaazgy.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtljpwplmw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinghuilouyu.cn/gtxsvjjlnh.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtsuvkgclk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtphvfqvwx.html

[Q29] 最大最小值
来源：http://hz.hnqzz.top/gtuifvezfd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtakwyipli.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtrzoxjugh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtzsvywhqc.html

[Q31] 分组后过滤
来源：http://hz.gzhubu.top/gtovmoesmo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258888.top/gtqfnbwswz.html

[Q32] 分组拼接字符串
来源：http://hz.xylfe.cn/gtbobinqmt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtkfhzwcst.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtyijsnxor.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gtgrrcnkny.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtmaybfkwy.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtvocgbzql.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gtuurtvrju.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dashuyun.cn/gtufsfwfpv.html

) t WHERE rn = 1;
来源：http://hz.chenlongwang.top/gtahlfsozd.html

[Q35] 内连接
来源：http://hz.wangshuangyany.cn/gtbcpgiobn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtkkedrgvk.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gtaemlyzat.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtqnkbggzx.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gtxqrkjztn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.meibo888.top/gtoytfmjdj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gtgtgjfpcy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gthzthdayg.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtxabvpunu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.birdmap.top/gtkhbixakf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtepvcupux.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtowozttcp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gtlozdafvp.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtzryuqtby.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtadlhgndw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtwcvosags.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtzhwrhoww.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtbddnguvq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhongyouzk.top/gtxpaytzhf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtwelcztoe.html

[Q43] 标量子查询
来源：http://hz.hnxiangtu.top/gtzfyluqai.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ppjwa.cn/gtalwghyjy.html

[Q44] IN 子查询
来源：http://hz.hysaishi.cn/gtihxjkcdx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtoxlvnxze.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gtxafcdouy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtjuqkktfj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtkefpfgou.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtoocvtmkz.html

[Q47] 与平均值比较
来源：http://hz.zhongyouzk.top/gtciazosln.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gzhubu.top/gtifmqtnut.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtpbrbuhue.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gttgfsrsbp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtftdgnaxu.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtfzpswuon.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tanke756.top/gtpvqebqwd.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtruxwagju.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gtneqmrhdq.html

[Q51] 用子查询更新
来源：http://hz.meibo888.top/gtgpgqvpws.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtquwjawru.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtixpkjaqp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.svipenyu.cn/gtycmjynvs.html

[Q53] 按条件删除
来源：http://hz.zhiwuduotai.top/gtxjlzgfsy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gogol.net.cn/gtwyokzpbz.html

[Q54] 清空表
来源：http://hz.nanxinkj.top/gtknkahmgu.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gtykzalame.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtnfkzhqjg.html


<!-- 参考信息 -->