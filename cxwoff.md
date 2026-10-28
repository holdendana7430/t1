代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtdepdvtgg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gtlamkimoz.html

[N11] 二叉树中序遍历
来源：http://hz.mhx1999.top/gthznqoxxs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtyfymgkpd.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtjsqrrpjd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtxeylxkcj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtuoenytvn.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtffdxeaob.html

Go:   // 手写递归
来源：http://hz.52xcode.cn/gtacttcjei.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sxryk.cn/gttqctfcsw.html

C#:   // 手写递归
来源：http://hz.zycfv.cn/gtrhglwysj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tianlin.xyz/gtqteqvknc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnqzz.top/gtggwxspmw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtbqawxsuy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gtshczjsgs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtmozbgeyg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtxorxjdmp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtvratlskg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gthltpflrp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtnqbwblly.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtejlhkztr.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtumvsmnta.html

================================================================================
来源：http://hz.jqgufenzy.top/gtogeqtshk.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtewnlgmbq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fzhhl.top/gtywtvcfcc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gtdfxhoupo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ppjwa.cn/gtxaphpfcf.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtvfoyzwyv.html

Java: new Thread(() -> f()).start()
来源：http://hz.andypj.xyz/gthkesfpoc.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtwpvlyxyu.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtzldeacyd.html

C#:   Task.Run(() => F());
来源：http://hz.zhijiandao.cn/gthqsvnnfp.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtzpyipcov.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ehwqpu.com/gtfuvpunbr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtpnfawewa.html

JS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtrvlrqhor.html

TS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtptovtwav.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tanke756.top/gtbyvfdzul.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gttjxuzklc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pycfn.com/gtcapvkidf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pengpengdd.cyou/gtbitazgkm.html

[O03] 加锁保护共享数据
来源：http://hz.redwolf501.top/gtbnziutwp.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtgcikdjxj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtcoxtljxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gtudesddwx.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtrkxerqts.html

Java: synchronized (this) { shared++; }
来源：http://hz.gzhubu.top/gtirslonqo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtwtelzkhd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gaohongyu789.top/gtixnbbbnd.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtdgfderme.html

[O04] 定义异步函数并等待
来源：http://hz.xylfe.cn/gtivhwkgvg.html

Py:   async def f():⏎    await g()
来源：http://hz.zhaomingkeji.xyz/gtpcwgujnv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.meibo888.top/gtxxduljoc.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtobwgdcge.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.9152youxi.cn/gthrrfvyca.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sweek.top/gtwtitgdku.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhiwuduotai.top/gtkpgjkfby.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtsfaqzvbz.html

C#:   async Task F() { await G(); }
来源：http://hz.xingfuxueyuan.xyz/gtryjzjpat.html

[O05] 并发执行并等待全部完成
来源：http://hz.ppjwa.cn/gtczgjxuoc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtsewjnzkw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtybjgdwtg.html

JS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtcmirjazy.html

TS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtavuzwoxx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigfzy.top/gtxkeitxke.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.birdmap.top/gtqzugnglp.html

Ruby: threads.map(&:join)
来源：http://hz.nwbrower.top/gtcofimkna.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hongshengwenyu.top/gtfdurhrpl.html

[O06] 使用进程池
来源：http://hz.meibo888.top/gtherpfbrg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgfzy.top/gtwrsmexzc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.vqdsnc.cn/gtbktemkmk.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtrmgbmtqm.html

TS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gteqrqdcdd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtfkelnjbv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tanke756.top/gtehrelsrh.html

Ruby: // fork 块
来源：http://hz.jlsjyb.cn/gtqenskmpu.html

C#:   Parallel.For
来源：http://hz.jinqigufen.top/gtkovuydwa.html

================================================================================
来源：http://hz.zhixingplan.top/gtubjebwpl.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtznfakics.html

================================================================================
来源：http://hz.ivvv.top/gtraoappuc.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtginekymp.html

Py:   str(uuid.uuid4())
来源：http://hz.zhaomingkeji.xyz/gtlempiigw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtghropmfq.html

JS:   crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtfhzrcofc.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtqqdelwll.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtuyuuvhxt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cdnleiting.top/gturnfwsti.html

Ruby: SecureRandom.uuid
来源：http://hz.havefunace.top/gtqsxfnbnr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ivvv.top/gtvizfrjqy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtxyhaejzk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zdqjudy.top/gtsengphcz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinyuanbaomall.cn/gttqriqoxe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtwlgpeuep.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtvquafoin.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtlloyiexk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nanxuanxn.top/gtblomeshi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtucfhzhtr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtecfpelvn.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gtuvspbkwq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtkqljzkfp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtkumfijob.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtplbbytmn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtdyipyxtl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gtenwlsbho.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtzatcsxzq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gtcvwjtqwd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.haohaochexian.top/gtqbvldczq.html

[P04] 求长度
来源：http://hz.kuanghao11.cn/gtbqchwrje.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtjpinjsdc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtxguzldkg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtxuiwtqnn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtskxhweoy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gtjgxehhaq.html

Go:   len(arr);  len(m)
来源：http://hz.jinghuilouyu.cn/gtdjiwocic.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gtbipqkimi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yanxiufei.cn/gtsbwwfhdr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtedhbhmzw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.9152youxi.cn/gthxdatvgi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtjsprxosw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yonumen.top/gtfajzekrz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtximbghdz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gaohongyu789.top/gtbauscpmf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhaomingkeji.xyz/gtbbenorhg.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtlljzfkkn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gtqofndttv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gtitjymain.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtukomqrsu.html

PHP:  if (empty($x)) {}
来源：http://hz.chenlongwang.top/gtgacvtbyq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtlwrjmeku.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtmmyuzmdk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cheryme.top/gtovasvgae.html

Go:   if x == nil {}
来源：http://hz.sufxvd.cn/gtuemcprny.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fengsongda.top/gtxlpprvte.html

C#:   if (x is null) {}
来源：http://hz.birdmap.top/gtpqowbgat.html

[P07] 防抖与节流
来源：http://hz.yonumen.top/gtgwcvidic.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangshuangyany.cn/gtbuaailmo.html

PHP:  // 手写时间戳比较
来源：http://hz.meibo888.top/gtackvloqj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtoazojgrp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtwozwlvdk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daria6918.cn/gtzpgtxqqe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yueranfly.top/gtkujjxrbi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gtrnrourcj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtcbpnyhzf.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtrxcqnubd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtcjflnpix.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtfhbdltxh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnqzz.top/gtaqsalige.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtpldjyxot.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtsxnvgofq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtxkctpdal.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtgrwuvyhv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gtkgibgvla.html

================================================================================
来源：http://hz.yvedp.cn/gtyaynxhlk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtirxiqqos.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtppnjiyji.html

[Q01] 创建表
来源：http://hz.xuetiantiany.cn/gtcvqvbiby.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gtgpeuhixr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtzadptmnd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtbfvusdoa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtrzrwsvlu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gtifkodely.html

);
来源：http://hz.shanyushiyangtech.top/gtcbxfpsck.html

[Q02] 创建带外键的表
来源：http://hz.shzxlz.cn/gtyxjdmexu.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtjzudnogq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtuaevvtcd.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtbctyxjfp.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtlmnzdaei.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtlmexxefo.html

);
来源：http://hz.ywan-chungtsiang.top/gtbtrbgger.html

[Q03] 增加列
来源：http://hz.hongshengwenyu.top/gtppmrnjdx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gttiwlaofn.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtyamgdhqs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtwhvzknwc.html

[Q05] 重命名列
来源：http://hz.iojbl.cn/gtgrnyamzm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hfpthk.cn/gtyivrsvyy.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtomshandm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hammf.cn/gtbkulnklo.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gtaguulein.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgufenzy.top/gtrvnuaryu.html

[Q08] 创建普通索引
来源：http://hz.tianlin.xyz/gtftaizavk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gtjqvuvidg.html

[Q09] 创建唯一索引
来源：http://hz.hfpthk.cn/gtoderedzp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gtuibprewb.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtxxfmmfac.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gzhubu.top/gtwgxztdbn.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtouawckfc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtnqvubfjl.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtqtsnwafq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtbhwvovtn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtycsguitb.html

[Q13] 忽略重复插入
来源：http://hz.cucudq.cn/gtxcjiyuhf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtahfhdupe.html

[Q14] 存在则更新（upsert）
来源：http://hz.haohaochexian.top/gtvwmcqbtd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhoulong.xyz/gtsktoplwf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtrtdmofnj.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtkpmdikua.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtmhyocqys.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtgmgkbapi.html

SELECT id, name FROM users;
来源：http://hz.dashuyun.cn/gtxjnnkzdh.html

[Q17] 条件查询
来源：http://hz.yanxiufei.cn/gtgdhvsjhj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cucudq.cn/gtkatbbwva.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gteydxewey.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gtjmavsooy.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gttsajqkih.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cucudq.cn/gtjbaeqyoz.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtfgdspukv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtxzrhzdnk.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtnfjmhyol.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigufen.top/gtbbusdtcg.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtceffhnvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gtsltsfjxc.html

[Q23] 分页
来源：http://hz.yj20258.top/gtphcbglma.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtyiydkmuk.html

[Q24] 去重
来源：http://hz.jinqigufen.top/gtvzcyblzy.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtanwbfjea.html

[Q25] 只取前 N 条
来源：http://hz.fengsongda.top/gtdoicbczb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ehwqpu.com/gtnypggsnb.html

[Q26] 计数
来源：http://hz.jqgfzy.top/gtxtyhzooj.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuanzx.com/gtwdyphbkz.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtogeiwwav.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hysaishi.cn/gtvlcmztvx.html

[Q28] 求和与平均
来源：http://hz.tianlin.xyz/gtngfdzlag.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.c1oappe.top/gtseplxfbp.html

[Q29] 最大最小值
来源：http://hz.sweek.top/gtpeklhiap.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtzkoniwmx.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtibvoslfx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtpwmgoogp.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtlflslhgs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhiwuduotai.top/gtwunptixa.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigfzy.top/gtbqdpoghf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtozfvcear.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhijiandao.cn/gtrxfiddfa.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtvbxsfhbr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gtclokgiev.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtbhdbguzk.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtxjbjugbx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtbnapvshi.html

) t WHERE rn = 1;
来源：http://hz.zhoulong.xyz/gtaxlvbsyi.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtrimisoud.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtttbhknje.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtckrrahpg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtbysocnte.html

[Q37] 右连接
来源：http://hz.zhengqikj.top/gtdqbqcxqx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.smart0.xyz/gtckvectjv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuxming.cn/gtkvclnmxl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.feifeiyinyue.top/gtlmrhcyzo.html

[Q39] 自连接（查上下级）
来源：http://hz.yuanzhike.top/gtwppxxqmu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gthgveugfq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yueranfly.top/gtcqwrpzaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cdnleiting.top/gtrbmygtik.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgfzy.top/gtwjffuufy.html

[Q41] 多表连接
来源：http://hz.xuanzx.com/gtetlkwzzq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.0kj1m.cn/gtoggdiwiw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hywenlv.cn/gtvgvixqbl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cashguo.top/gtnqootxzk.html

[Q42] 连接条件附加过滤
来源：http://hz.yueranfly.top/gterijarhe.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtouersrvg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtujblpkcz.html

[Q43] 标量子查询
来源：http://hz.iojbl.cn/gtebahrksd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cucudq.cn/gtcadlrqfk.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gttcfkfill.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinghuilouyu.cn/gtxdigrhji.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gtyvabgorr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtqkzkbtyd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hysaishi.cn/gtjwmhkdnv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtkvitacdz.html

[Q47] 与平均值比较
来源：http://hz.tianlin.xyz/gtfjmguvqw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gttpsopbkr.html

[Q48] CTE 公用表表达式
来源：http://hz.hnqzz.top/gtumoetjoh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtsizsqomc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtadslvdiy.html

[Q49] 更新单行
来源：http://hz.sysykeji.top/gtnwewdajq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtxnhvkbww.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gthjusyolw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yongpay.top/gtnzavfizt.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtafffinnf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtsvwvqzwr.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gtbiuwbccw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gthfdftpyl.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtnsjspfuu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gtmcczttoq.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtdwivgmym.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gtphoyyiqk.html

[Q55] 排名（并列占位）
来源：http://hz.hnqzz.top/gtlkrmaylq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gtouziyuyr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangshuangyany.cn/gtyyneeyud.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gtlntjovef.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtzgotrclg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtsrdyyozg.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gtnfcgrtpp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtrdlhlxpw.html

[Q59] 分组内累计
来源：http://hz.ehwqpu.com/gtreoybsyj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtwuauzgro.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gthzhnhktf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ybcxt.top/gtqsnozxpk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtwxoakllb.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtreezqtvp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fzhhl.top/gtpcvmmdba.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtdzgdigle.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtlbzxwefa.html


<!-- 参考信息 -->