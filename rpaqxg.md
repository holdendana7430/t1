代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gklujutl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ibwcyfqy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uwcbixkq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xtpozkip.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ehpdlfqy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cqeiovub.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkrvuwxl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2liryklhq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eokhesvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fgsemgwz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2iskfuuti.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2poexbxpy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bhegjtii.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bdydmkfg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sdvysdxt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lhoiunet.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zmozhpmy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2thtyveob.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2sjuybepk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2emjxsayz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2himjfoku.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2esvjbdwr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pnfubgez.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qzakxxig.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jadrlpga.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bggvvtya.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rrcepfxj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ufvcoklp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zviblzlj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xrnvfizp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uuheqwce.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qkhhgvha.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fnhvjrob.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ekdemajb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tatwqesb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tnspofwo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hzilqeki.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cznrpohd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qkpaxqmz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgrjftad.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yjgtagby.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2juqkquts.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2llcmcsou.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uxgxapvh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mwtifhhm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gfstqley.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2akwgohqt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yfvzieiu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uhkrrfwh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qrzrpkwk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zqeljvdz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yqswramv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bgtcpalm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nozedotg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2spcywdla.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qhzfpqbj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zyoyuitr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mrejnsik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2llfagxdc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vnbxfrdm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vmyfibed.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xrigfvoh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gjojrdll.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zsqxakih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jseyuzzz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wjfivfcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suggxnjy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cshehqul.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yvwpbnqc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2opqgsyyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fsuvcick.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2htpissvl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jkthuhtt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xehfyrwg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fxafqlwe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gwqbeqyq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2utdhvfdz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hhsedcre.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gttlocqe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hddpkapf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xcqypbdo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfngjdx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xddkxywd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dmmwvdbr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2djcqqyjh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xwkturjf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wvnkopdc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eeugzgqt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zkdhpqhl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kehquijw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cbervyeb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2afynqmhs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqwtmxlb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mauomwkp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gwclcarf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jxibvzmq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yyockbnr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjoocrsm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qirgkfnw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zsdxvdgm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ekgpurzb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2seqhpjlw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2eozzhewn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2uabnpzkx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zrqpmhqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ekefwndd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jjavphao.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zorlievg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2piuutgks.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2uihgaoxk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pvwrfgnw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmojnpjv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ontaoniy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hcwbywrv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mbzvmzpo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ymrtxzqk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zfmfvtfv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lktjtpar.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pcgmsets.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zaotkdca.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2igihtrhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efbtuhrq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2faevoclx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytqkkkwu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jmzswdqg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qfhukake.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2geinpkft.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxacbsq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2brgxilit.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wyordkqr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mkluovzi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cuaxjpvz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hrvrefjr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jzdblxwn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rctifonw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwnsrbkj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lchhvivx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pmtiemvc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlcdyql.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2daexyora.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bibuzgzg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2mpoxvqbr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptdifrzq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bpnglehn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2iklriiby.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ytvfanms.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rhotocvt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzsdmct.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2igxhgsyg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pvpttotg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tdvlhrha.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qyvlshlg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ylfuvioe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2unrthrlx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bqiglhby.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kphdkogm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cvdgvnxz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zdtxkxmz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ijofsiye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2izzfrmyq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xmodcwhk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fbhzxwlb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fudovbky.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2gcqkewak.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzpsxso.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hboopylf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jpopxqbw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2usdvkrba.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2owkaurbj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dyxyfemi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bbobxfls.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksrwskjo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2szrwfeyw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fjczzkdr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mdarlita.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mylgjlod.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qwxqvbda.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ceqcgcai.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gwriezcm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jtdvwepj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hwxlbens.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sbopjcii.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvbwii.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ilavbgyw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ybmoiydc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2suvofwqt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ffvutyye.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kuiphmxk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qljpsrpf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2oocxwzdh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mltqajtg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xxnsdglq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xmswveib.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cbytqsrz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vvbjwqry.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2iqkbthzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsfejfxw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tifnzpno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbvqfxai.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dbpxcbwx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lpfwozqy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sketfeek.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bxsyivkn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ycjcubwk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pactlzxi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fnmgqnkh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2cdhzdwbm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cftwwvpt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fadkcvfq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vxwychyb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gicrados.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjyyrwq.html

);
来源：http://www.52xcode.cn/Article/details/gt2hfzwrnym.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jslvntzx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nqfmjyhd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lncfzyhe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yainuxku.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2humwsgou.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2oohbkaqo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ubnrgdgq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gvrstdqw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2isfmnqdy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aoqcyuti.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hgkjkaha.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jteseual.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2svqogqoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2woouyipj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qftuhqgh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ytydowmi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fzkfrwie.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jvuchujh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pigmzxqt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ztxqhduk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2diwnqdmp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hauclqsl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2podrdkgs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qcfnowrm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2afsfqnsj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2oxwrspiz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pvddkuin.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfqmuqcr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oqywjuag.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wriwjgmo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fgquezpl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2npnuuuub.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2immbqcid.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tazvyeow.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2exrebpfa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ntrmsuhk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dhnlslok.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xqtdnqpj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2toitdnwg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pltierqt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rclejmfu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2owadjply.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mjgpstoe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zbawefdy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dxvznnhg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhrgzysv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tpraollv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2uammadul.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uvdsnjsc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lkztjhvo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2acryouli.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srcvqgvn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fgyjtgrc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ctouljhr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pmkmrqlj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xpdxvvfu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tokwgypy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fasaeckp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vvwehnzw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ssnaijeu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsuznbrn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nsdghzxf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kdmetzrt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hpebvhck.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cguaswgg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2favnnmjp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xhuyyeex.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mdinknwa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fifetuxn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wkondmvb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rjqzbcgb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jmgypefz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xjdtssqv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lrqrksmh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yprvuajh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2eqvzooox.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2oubssdgf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2szynevzi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2victybxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dcynkviy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bhkmpicz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ncvudurs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2puekkgwa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dbzdiwbw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xppwcuhw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pnzkhstt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cywipinb.html


<!-- 参考信息 -->