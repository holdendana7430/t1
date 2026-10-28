代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtmqdywjiq.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtbeoihubf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gtbkygvyyw.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtbqqjcqfu.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258.top/gthfifcaxo.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtcmrxccbw.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gttxigwegc.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtftfkcann.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtdvajgaum.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtwmekpsvz.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtzqszurag.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtnvftoykg.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtfuybmuru.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtxtxmnwcz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gtzhhhidnc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hysaishi.cn/gtizhyvnrt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtjykkinyi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yvedp.cn/gttnyaurre.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gtefjofgvs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gzhubu.top/gtaeyvpxsv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.snrcjt.cn/gtbhezkplr.html

[N10] 链表节点定义
来源：http://hz.cashguo.top/gtmvxgswta.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gteknqihvj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gtyqiksqlk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtmzcznfab.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuanzx.com/gtejbdlbgx.html

Java: class Node { int v; Node next; }
来源：http://hz.xuanzx.com/gttnjrnvlr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtbnoysbei.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtkqmdcsxd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtqyqoqsnw.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtnnzxfvvy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtiwvycmxg.html

PHP:  // 手写递归函数
来源：http://hz.haohaochexian.top/gtlrsxpcry.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtdelzotzj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtbjwvoacs.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gtmqlbwumo.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gttmvjofoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgfzy.top/gtyjbttgmo.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtkwpjiwlb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtjqwhalhd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xingfuxueyuan.xyz/gtopfuttax.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtjpyyrhxj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gtgyvpmfdq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gteytnyzua.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.quarkkingdee.top/gtcrzrbqfx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gtyozobwsq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangshuangyany.cn/gtbmfjrncq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtnqpdzugo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcljqnrlz.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtyynovgfp.html

================================================================================
来源：http://hz.xziqi.cn/gtgfcvytkp.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtbehcpzvr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtulaihdox.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nwbrower.top/gtdqoluzeg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yongpay.top/gthicromyi.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtfdmjozbv.html

Java: new Thread(() -> f()).start()
来源：http://hz.fzhhl.top/gtkdtexthi.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtkhshahao.html

Ruby: Thread.new { f }
来源：http://hz.zhixingplan.top/gtxutbdlnu.html

C#:   Task.Run(() => F());
来源：http://hz.hongshengwenyu.top/gtzufqplwi.html

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtxgmlzyhh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigfzy.top/gtpnqwcjbl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuanzhike.top/gtlikrfvhm.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtxydtpiii.html

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtfsihbdwg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtvxrzguex.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtnmaaoynz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.52xcode.cn/gtcwrvzity.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenzaomai.com/gttigkumph.html

[O03] 加锁保护共享数据
来源：http://hz.jlsjyb.cn/gtqugfwmkv.html

Py:   with lock: shared += 1
来源：http://hz.chenlongwang.top/gtgvrinifq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtvwubbysu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtruivtzgb.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtmcrehrxv.html

Java: synchronized (this) { shared++; }
来源：http://hz.shzxlz.cn/gtjugaaixg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gtcjkmuurk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhijiandao.cn/gtndvjtqcw.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtcauugjqs.html

[O04] 定义异步函数并等待
来源：http://hz.nanxinkj.top/gtrkirkuam.html

Py:   async def f():⏎    await g()
来源：http://hz.cdnleiting.top/gtyjxksxdh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jlsjyb.cn/gtfzpeznct.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtcqbkcqko.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aizwys.cn/gtradnynbe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtqcdazfnv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhongyouzk.top/gtzaqizasc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtjmnrgjay.html

C#:   async Task F() { await G(); }
来源：http://hz.yangfankeji.com/gtjpavtvus.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtvehoajmh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gtxmxltaib.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangkeji.top/gtbhpdvyvt.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtbbdmdolg.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtauslthtp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gttxdznalh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgfzy.top/gtpeciymbn.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtossvhwnu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gtxjomgpun.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtdgcvvjro.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cashguo.top/gtshhnzagv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtgavfwsew.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtznrkgbnd.html

TS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtupgqjeey.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtpndeauym.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zycfv.cn/gtzwyncfrt.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gtlziwicnb.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtptdecrzo.html

================================================================================
来源：http://hz.cheryme.top/gtmeykjsop.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtbjwbdjvk.html

================================================================================
来源：http://hz.haohaochexian.top/gtebzgmsfp.html

[P01] 生成 UUID
来源：http://hz.guowangkeji.top/gtfxkjhlnt.html

Py:   str(uuid.uuid4())
来源：http://hz.jianghu66.top/gtehxghxre.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258.top/gtbwpsfemv.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtyyllrhwp.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtvtcinwqi.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhoulong.xyz/gtfqiraojd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ivvv.top/gtisryjeht.html

Ruby: SecureRandom.uuid
来源：http://hz.guannengcc.top/gtwhufabdi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gttyinintm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtxmeikxck.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gtybshqhvo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.mhx1999.top/gtodrwhpuo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtarqqrqgp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtkxpepfto.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.vqdsnc.cn/gteaibnuqk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangkeji.top/gtntftlzfw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yanxiufei.cn/gtbybzwglm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtsfivlsfc.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtxepuccyq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtvdgpegvd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gtepnukymd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtlyajcwst.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtcqxwipnj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.havefunace.top/gtjvqbjvbp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sysykeji.top/gthfpbmosd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtdmnlcqhx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yonumen.top/gtdxqrlhjc.html

[P04] 求长度
来源：http://hz.kuanghao11.cn/gtzcqsinrc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gttoujjdcg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtkqeovlsc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtpwvvjaub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtstdbporq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtdxmorimo.html

Go:   len(arr);  len(m)
来源：http://hz.aizwys.cn/gtsoauuuno.html

Ruby: x.length;  x.size
来源：http://hz.ydzc1.top/gttzvgmynn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtxteazrbq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigfzy.top/gthdxudcsv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gotoacloud.top/gtacjwgmxd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fengsongda.top/gtcrkrwyqr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gterrexcqz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtkfsxyafh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.52xcode.cn/gtatvdestv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtermvlzwx.html

Ruby: a == b
来源：http://hz.dashuyun.cn/gtpdvacbbw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gttwseyeuv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gtcfcqfbzy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtcicmdepj.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtsbtberyt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnxiangtu.top/gttfgydcgx.html

TS:   if (x == null) {}
来源：http://hz.dianchejie.cn/gtaxdsodor.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aizwys.cn/gtdkeaqllk.html

Go:   if x == nil {}
来源：http://hz.iojbl.cn/gtwpxppnca.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtyjwypkuc.html

C#:   if (x is null) {}
来源：http://hz.hammf.cn/gttpsghhkm.html

[P07] 防抖与节流
来源：http://hz.cdnleiting.top/gtrfwvistv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtwtaglqvi.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtzltpsfhj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtfwjlmcqj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gthbcoryjr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gteziymfzd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtifnjfxkx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtnrjacbkd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dashuyun.cn/gtyfrxjzrw.html

[P08] 处理浮点精度问题
来源：http://hz.daria6918.cn/gtticzbnuz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.iojbl.cn/gtypwaynoy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigfzy.top/gtogujqvka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.9152youxi.cn/gtupxcoluh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gthwkmjovk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gttdxzpeei.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtkduohgxq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gtywmbxshf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gthaxerttn.html

================================================================================
来源：http://hz.0kj1m.cn/gtjjtxbmne.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cqqwz.cn/gtjikaqnty.html

================================================================================
来源：http://hz.pycfn.com/gtnxgjvaox.html

[Q01] 创建表
来源：http://hz.zycfv.cn/gtzrktpfry.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtmazarujp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtwhwkbqqv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxinkj.top/gtllbpbivo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtyivazgne.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gttggdyjdp.html

);
来源：http://hz.shangyingyoupin.top/gtkajtiadk.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtsnjghywd.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gtorlqpxww.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtxljjaqfr.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtbxehnjfy.html

amount DECIMAL(10, 2),
来源：http://hz.sxryk.cn/gtbakkaetv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gtpdmrksmu.html

);
来源：http://hz.c1oappe.top/gtxsiaecdw.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtdbigpjfy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtjnwmgjpu.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtcwltpgzd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.iojbl.cn/gtxfhmkcul.html

[Q05] 重命名列
来源：http://hz.jianghu66.top/gtwxanqkgd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtghjzkzot.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtchsyyeyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtzzmncxuc.html

[Q07] 删除表
来源：http://hz.svipenyu.cn/gtipergkoq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtghauwsvg.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtinrxggjp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtflakvtyr.html

[Q09] 创建唯一索引
来源：http://hz.svipenyu.cn/gtqbtlqwzn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtnexkrtpp.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtnupuxzex.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hysaishi.cn/gtplmjgkxt.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtbqwafydr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cheryme.top/gtiivdldyc.html

[Q12] 插入后取自增 ID
来源：http://hz.shzxlz.cn/gtjbhmmgqh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydzc1.top/gtsgjyfror.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.snrcjt.cn/gthhygkwrl.html

[Q13] 忽略重复插入
来源：http://hz.chenlongwang.top/gtjcfewntz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jiagoushi.top/gtypbezkci.html

[Q14] 存在则更新（upsert）
来源：http://hz.gaohongyu789.top/gtihoiktng.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtqjylnlsv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtrrjijokj.html

[Q15] 查询全部
来源：http://hz.mhx1999.top/gtlxtrqwlg.html

SELECT * FROM users;
来源：http://hz.zhijiandao.cn/gtmilhftss.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtklfpxfxc.html

SELECT id, name FROM users;
来源：http://hz.ydjk.org.cn/gtobmzgglf.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtguwtqjxv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtpzspfluq.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gtxwpklunx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gtnscvukjm.html

[Q19] 范围查询
来源：http://hz.316326.xyz/gteleozqcw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gotoacloud.top/gtjotwgfjj.html

[Q20] IN 列表
来源：http://hz.havefunace.top/gtrvjfwvlz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhongyouzk.top/gtnglzmbtj.html

[Q21] 空值判断
来源：http://hz.ydjk.org.cn/gtfpfgtynr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtkrjszcrn.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtrgqfqtfl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigufen.top/gtjzkpvkhu.html

[Q23] 分页
来源：http://hz.cqqwz.cn/gtkrbmlbqk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtiuautyia.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtfyextfke.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgfzy.top/gteanaizkb.html

[Q25] 只取前 N 条
来源：http://hz.xziqi.cn/gtgfsjhypu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigfzy.top/gtynprycmp.html

[Q26] 计数
来源：http://hz.jlsjyb.cn/gtyyojtoms.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtizglkjys.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtqdovpuor.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtxzhjwwcj.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtjmabpjpl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydjk.org.cn/gtabniusny.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gthneagjek.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gthzvipsrv.html

[Q30] 分组统计
来源：http://hz.xinyue.icu/gtfjdcfkcq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtsjgjbuua.html

[Q31] 分组后过滤
来源：http://hz.jyoumei.cn/gtmcrekgga.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtjiivqsar.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtjxylsfza.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtvfjznthl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhoulong.xyz/gtrwhxcauc.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtnhsaxumh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.kuanghao11.cn/gtlprxiuzh.html

[Q34] 每组取第一条
来源：http://hz.hywenlv.cn/gtzovxibfd.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtzwwrdhcz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hfpthk.cn/gtbzlddpak.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtsffxvpvo.html

[Q35] 内连接
来源：http://hz.quarkkingdee.top/gtyyqsctkz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gthpytiacr.html

[Q36] 左连接
来源：http://hz.zhongyouzk.top/gtgqahgfnx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenzaomai.com/gtdkiyqlbs.html

[Q37] 右连接
来源：http://hz.jqgufenzy.top/gtjpbeujqf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.andypj.xyz/gtqhldqted.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.0kj1m.cn/gtiqepuxza.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenzaomai.com/gtnkczhhjd.html

[Q39] 自连接（查上下级）
来源：http://hz.zhongyouzk.top/gtvohhdfoj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtrmvrajry.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cdnleiting.top/gtwxbyboma.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tianlin.xyz/gtybxuehej.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtsbytqlbn.html

[Q41] 多表连接
来源：http://hz.ydzc1.top/gtvxqpdtox.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtacbekfkd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuanzhike.top/gtneiialyc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pengpengdd.cyou/gtaersdncw.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258.top/gtwppqruvl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.birdmap.top/gtlewffwih.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hywenlv.cn/gtdrtqtrsp.html

[Q43] 标量子查询
来源：http://hz.shanyushiyangtech.top/gtwbvrcfmg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jlsjyb.cn/gtqukewzhq.html

[Q44] IN 子查询
来源：http://hz.chenjidiqi.icu/gtijhilmso.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gthnqmbszv.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtogjyubwp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtdazklqnl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenjidiqi.icu/gtnogfcorv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtunmspkij.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtnygssugd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gttkazsdqc.html

[Q48] CTE 公用表表达式
来源：http://hz.ydzc1.top/gtrfrlaqli.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtiunzicdp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtpphsovkj.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtjijtzgmh.html


<!-- 参考信息 -->