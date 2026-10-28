代发 wailian999

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtgvcvkiyq.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtbnzzsjdf.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtrjogrgta.html

C#:   // 手写回溯递归
来源：http://hz.zycfv.cn/gttvyjfxea.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtrqzndkle.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cashguo.top/gtzwhgrfij.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cqqwz.cn/gtylslsmgt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gtuhkfyrpy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gzhubu.top/gtqgwkvexf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jiagoushi.top/gteootercm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jianghu66.top/gtbudpjfmw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gtjwyzajop.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtnvnmlyzn.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtxyknulzo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhongyouzk.top/gtftaohlrz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gttptegaai.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtdfgerdyx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhixingplan.top/gtjpcyytrj.html

Java: class Node { int v; Node next; }
来源：http://hz.hnqzz.top/gtqmwzehxh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhaomingkeji.xyz/gtqaxnuzge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtmnuyfprl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtwaqfgkin.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtrwoukzhq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gtanqmvmcj.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtvggmqjnb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtvuoxyttr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtkqslmywv.html

Java: // 手写递归
来源：http://hz.bjfxy.top/gtuffmvdmn.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtvqzogjge.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtkokaxmuk.html

C#:   // 手写递归
来源：http://hz.kuanghao11.cn/gtmukjlexl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258.top/gtplsuytcr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigfzy.top/gtwxmqspql.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtqypnoblr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtnvsrxjmw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtokmtastn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtppmjolqm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtkknrjrbb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtehwdsxjj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtpdsfbxwn.html

================================================================================
来源：http://hz.birdmap.top/gtcbxxdpie.html

O. 并发与异步
来源：http://hz.sufxvd.cn/gtctkjbhvl.html

================================================================================
来源：http://hz.smart0.xyz/gtndrjffup.html

[O01] 启动一个线程
来源：http://hz.redwolf501.top/gtudvcrgdj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtjdpokhrk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtxwgpbbzj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.316326.xyz/gtdtqmtrvi.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtjnpcouyv.html

Java: new Thread(() -> f()).start()
来源：http://hz.cqqwz.cn/gtdirgqshy.html

Go:   go f()
来源：http://hz.52xcode.cn/gtnuimhdkg.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtojciivkd.html

C#:   Task.Run(() => F());
来源：http://hz.dianchejie.cn/gtjivgjvic.html

[O02] 使用线程池
来源：http://hz.ydjk.org.cn/gtjbzpfpei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258888.top/gtogucgdev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhengqikj.top/gtdhfznerw.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtrcwlpoun.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtvunkwswd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtvqgcixmd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenlongwang.top/gtqvhpobed.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sweek.top/gtrezumnjx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtxlrufatp.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtfkduvxuf.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtluvntlmu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtnzghnlyu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtppwfffso.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtylmkzwhj.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtsdicxmlk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gtbqdrpvcl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fengsongda.top/gtlbtofrip.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhengqikj.top/gtihqessji.html

[O04] 定义异步函数并等待
来源：http://hz.hnqzz.top/gtdmbnwdrd.html

Py:   async def f():⏎    await g()
来源：http://hz.xziqi.cn/gtlqaalifl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtaeaksbjy.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtuuwgllxk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yonumen.top/gtwlveldkq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yangfankeji.com/gtmvaqzudd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aizwys.cn/gtaeqzjdnz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydzc1.top/gtwmvtfkzy.html

C#:   async Task F() { await G(); }
来源：http://hz.ydjk.org.cn/gtspgznxml.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxinkj.top/gtqkieerjk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtuwwnoaxi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtaysesvaz.html

JS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtsnhwvuaf.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtwxzzmtfb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sweek.top/gtufrqwgsq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ywan-chungtsiang.top/gthfdihftk.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gtfbfgqrsp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtmxtgmoke.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gtwstdnvlz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtgwlujbbw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigfzy.top/gtjpegmgpl.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtqjqxmghi.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtgwnzuaes.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtgrbxcxgd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gthseqphpm.html

Ruby: // fork 块
来源：http://hz.zhongyouzk.top/gtttohkwdg.html

C#:   Parallel.For
来源：http://hz.cdnleiting.top/gteqvlpndy.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthnbrcbgx.html

P. 常用工具函数
来源：http://hz.jianghu66.top/gtfprkdpzo.html

================================================================================
来源：http://hz.sysykeji.top/gtecbueuqz.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtrcctireb.html

Py:   str(uuid.uuid4())
来源：http://hz.sufxvd.cn/gtbqplhljs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtwbzhqnvy.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtmrkqhreq.html

TS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gteabbfhjl.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhiwuduotai.top/gttkchuilu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yonumen.top/gtgiozzisf.html

Ruby: SecureRandom.uuid
来源：http://hz.zhoulong.xyz/gtotcfprxu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtiokmqawt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cashguo.top/gtrqtwmvbh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhiwuduotai.top/gtqzklqixi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtxhfbjnah.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gtqvjfhbdx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.0kj1m.cn/gtbrmxztgy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtfuodywhn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtfywbqsnw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gthwnqmlpb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shzxlz.cn/gtsmhajqqr.html

[P03] 生成短随机字符串
来源：http://hz.zycfv.cn/gtawpytclk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.meibo888.top/gtnzziaefp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gtijmmzoch.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtksamicta.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtinhtzlua.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtkdmpzjhr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.redwolf501.top/gtbozuvndu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtkdtmoknh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.meibo888.top/gttyefyfjp.html

[P04] 求长度
来源：http://hz.shangyingyoupin.top/gthttpkeiw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hysaishi.cn/gtpxkmnzpw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtgpzwsclk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gthqswpvil.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtjujqlyka.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtoscrsnza.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtrslblvqe.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtefaayumz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtivzqcqey.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gtflblirhz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenlongwang.top/gtdpgwuxyt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtkjnmwszx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tianlin.xyz/gtwfjzippo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtrzszpkag.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ywan-chungtsiang.top/gtjyswhvpc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtxbahqvsg.html

Ruby: a == b
来源：http://hz.dianchejie.cn/gtqjqodydn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gtdiizvalc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ppjwa.cn/gtzqazvkmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gtukqvexzz.html

PHP:  if (empty($x)) {}
来源：http://hz.yanxiufei.cn/gtnwzvxqel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtjdgjptkd.html

TS:   if (x == null) {}
来源：http://hz.jianghu66.top/gtoznoqiqo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtykirebfx.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtgmtfital.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gteehaszej.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gthjhpleif.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtpzycpzkz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtdnciqved.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtwisjmkvu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtpqpludxq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gttofytyhk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhengqikj.top/gtwoiwgpwm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhijiandao.cn/gtonzofvnl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtrgcvzmds.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sweek.top/gtpxwptmsf.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gtvulyewdx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xziqi.cn/gtcqewufyh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtgrdpevnc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtxtcmafuo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daxiang520.top/gtmwwwvkfh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtirmafzsj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtlhpzqdym.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtlpqrxvvh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtawqrxjzc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtehmnbdxv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtckycclek.html

================================================================================
来源：http://hz.yonumen.top/gtidguoiap.html

[Q01] 创建表
来源：http://hz.quarkkingdee.top/gtqsnwlxmu.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtoxamugbh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gtwagetmwl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.birdmap.top/gtxiglsoot.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtqybangxq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtiqytfyne.html

);
来源：http://hz.yuanzhike.top/gtannvaclt.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtvfbxnrru.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtkxcpfsdp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtcfxutvme.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtypnrfwog.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gteohlsndm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuxming.cn/gthumrxnme.html

);
来源：http://hz.shangyingyoupin.top/gtlntmzhdz.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtpcqtscyl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.redwolf501.top/gtfetenlaj.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gtdxovatpn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtvxzhludm.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gttuxshktx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtwgyeyiyj.html

[Q06] 删除列
来源：http://hz.hammf.cn/gtkkgkojvo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gttmiyamqc.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gtbabmojxt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtcnoosnkf.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtrkryfbyv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtcfwodhpz.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtvlutdgtb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtxmazdjxc.html

[Q10] 插入单行
来源：http://hz.mhx1999.top/gtvksubcos.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.dianchejie.cn/gtepcpmxnt.html

[Q11] 一次插入多行
来源：http://hz.ydjk.org.cn/gtbzebgzxx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtwraydyoz.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gtqafnvivv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gthmovrdtt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shangyingyoupin.top/gtynltgxtj.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtzfbsjhjb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.bjfxy.top/gtjzoimnae.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenlongwang.top/gthfjbxxqq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtazkhjfql.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtzmqhjtvo.html

[Q15] 查询全部
来源：http://hz.chenjidiqi.icu/gtaptkmtcy.html

SELECT * FROM users;
来源：http://hz.pycfn.com/gthydrjlge.html

[Q16] 查询指定列
来源：http://hz.aibaodan.cn/gtdrzgpyyp.html

SELECT id, name FROM users;
来源：http://hz.ivvv.top/gthxurxvge.html

[Q17] 条件查询
来源：http://hz.jinqigufen.top/gtsafukzlk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnqzz.top/gtzxpsxfmy.html

[Q18] 模糊匹配
来源：http://hz.dashuyun.cn/gtqkttitis.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenlongwang.top/gtgxihouje.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtltzsdcpb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtphuddkgu.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtswstwdan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shangyingyoupin.top/gtdjgkxxzx.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtopwvfelk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhengqikj.top/gtdkwnwtyf.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtgpdqersy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxuanxn.top/gtwniwcpkx.html

[Q23] 分页
来源：http://hz.yuxming.cn/gtrlghgrts.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cheryme.top/gtaethcnxe.html

[Q24] 去重
来源：http://hz.ehwqpu.com/gtmkrlawlh.html

SELECT DISTINCT city FROM users;
来源：http://hz.ywan-chungtsiang.top/gtaxkevimr.html

[Q25] 只取前 N 条
来源：http://hz.birdmap.top/gtqpbvzcpv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtuufbidqr.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtrsxivele.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgufenzy.top/gturxwdlxo.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtbmkhnnpk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtvosquzau.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtoqzdkswg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gtcnvsbawc.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtornqying.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtlvvvmido.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gtwuiyppve.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtjvyhytsx.html

[Q31] 分组后过滤
来源：http://hz.meibo888.top/gtzkiwwicv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtpxpkwjqy.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtasbcosfm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtquwglnnx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gzhubu.top/gtoebwjldr.html

[Q33] 多列分组
来源：http://hz.zycfv.cn/gtmgsinjmk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtaahazakd.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtagxsuqfl.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtrrqjdupz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtibodwftz.html

) t WHERE rn = 1;
来源：http://hz.shangyingyoupin.top/gtiakmmjns.html

[Q35] 内连接
来源：http://hz.yuanzhike.top/gtpblwfnbb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtiuxjsnih.html

[Q36] 左连接
来源：http://hz.hongshengwenyu.top/gtevgqzuwr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtrigjrkzb.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gtqbptxbrp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aibaodan.cn/gtqmoilqbh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gogol.net.cn/gtjxhzlylp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tanke756.top/gtrlfwlhaz.html

[Q39] 自连接（查上下级）
来源：http://hz.xuetiantiany.cn/gtmbgirugl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtvlsmqtbv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtdxhekvsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtxvlbzdrl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gttrxwwial.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtafxyxalo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hfpthk.cn/gtygvfccxt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtsxhldvzm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtkivpuloj.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtpiinxzfs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtnpukbtlw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtxpykkqer.html

[Q43] 标量子查询
来源：http://hz.hnxiangtu.top/gtxrabqzhj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.bjfxy.top/gtcqlktnqo.html

[Q44] IN 子查询
来源：http://hz.zhiwuduotai.top/gtfvhqqquc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtmyoukkky.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtochlmgjn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtaccsxgxz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cucudq.cn/gtnmgrcpca.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtngxbbdxw.html

[Q47] 与平均值比较
来源：http://hz.chenzaomai.com/gtaadrlbrt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuetiantiany.cn/gtsdlwwbde.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtlywyjwoq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtsmgugfoo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtiwdipsjg.html

[Q49] 更新单行
来源：http://hz.yvedp.cn/gtkblspymo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtspgqdcoc.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtndazmbvj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtlvmajdva.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtgwjlrvjl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigufen.top/gttyvqsrjg.html

[Q52] 删除指定行
来源：http://hz.wangdashe.top/gtpqeyuzwb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnqzz.top/gtzgyzpnfp.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtpdxkhqyq.html


<!-- 参考信息 -->