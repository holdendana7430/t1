代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtgertydpe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtzjkshooh.html

[N11] 二叉树中序遍历
来源：http://hz.ivvv.top/gtldbcnktl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yongpay.top/gtqndmdalr.html

PHP:  // 手写递归函数
来源：http://hz.316326.xyz/gtuclfckof.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtgaxjdfng.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtzmvlfmqq.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtwvivvaon.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtxleskcvk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtmwjbanot.html

C#:   // 手写递归
来源：http://hz.zhoulong.xyz/gtpsyypazp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gthzamitmg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuanzhike.top/gtyycjkuxk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gttqwvglqr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtdpichane.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gthurnzkby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtxtnmkmmh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtonfcjmyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.9152youxi.cn/gtnznwjeco.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtuomdqzne.html

================================================================================
来源：http://hz.hywenlv.cn/gtgxqegcys.html

O. 并发与异步
来源：http://hz.gogol.net.cn/gtuxixdbmc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvrldrsfl.html

[O01] 启动一个线程
来源：http://hz.tian-w.cn/gtjhmgzekf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtkwfbqpro.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtrsupopre.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtmstrbkmc.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtdptujgud.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtausjpagk.html

Go:   go f()
来源：http://hz.c1oappe.top/gtvddugvjg.html

Ruby: Thread.new { f }
来源：http://hz.c1oappe.top/gtmotpxdzn.html

C#:   Task.Run(() => F());
来源：http://hz.havefunace.top/gtwmsivwcx.html

[O02] 使用线程池
来源：http://hz.jqgufenzy.top/gthawbjwii.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jyoumei.cn/gtdjvrrbzg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cucudq.cn/gtleeepqam.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtskuailuk.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtrwuxxtjk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtmbxkgpcj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtikvvjlua.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtyyzalfpu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtaakxcsmz.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtdnwuxabh.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtydqvbolr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gthqnkpzxw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtdokkaoud.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtusrqjzqb.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtjwhqxizd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtdcdlsijr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtahwbvrik.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtcapxhbmm.html

[O04] 定义异步函数并等待
来源：http://hz.jinghuilouyu.cn/gtskptjcee.html

Py:   async def f():⏎    await g()
来源：http://hz.wangshuangyany.cn/gtgwjmwrfw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhoulong.xyz/gtcgmvbuzm.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtvztvuntg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgfzy.top/gtprjscuzj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tanke756.top/gtmkbicztd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cheryme.top/gtqeprzmcr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtsjksqjnv.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtmlqmtlvg.html

[O05] 并发执行并等待全部完成
来源：http://hz.yvedp.cn/gthrgvyawp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtrfylfjls.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtbdyizhzo.html

JS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtzzycmebq.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtuipuxixr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gthvfhccen.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtmgxkqstr.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtzucyyydl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtyotopxdq.html

[O06] 使用进程池
来源：http://hz.ybcxt.top/gtknyltegw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtdjxjyvlj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtyseuusap.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtmidrosng.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtrhzwepdp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tianlin.xyz/gtxmohnlhj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.mhx1999.top/gtpxjjskas.html

Ruby: // fork 块
来源：http://hz.fzhhl.top/gtfqslamvm.html

C#:   Parallel.For
来源：http://hz.meibo888.top/gtmpiaxrzi.html

================================================================================
来源：http://hz.ivvv.top/gtgfybucct.html

P. 常用工具函数
来源：http://hz.fzhhl.top/gtmorrhfee.html

================================================================================
来源：http://hz.iojbl.cn/gtariaieaj.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtlooczzcs.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtheayrvyd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtlgeruwyv.html

JS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtlhgsqbzg.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtiznjlnbc.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gtqiaamxdn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtbhjdicjk.html

Ruby: SecureRandom.uuid
来源：http://hz.iojbl.cn/gtvmqbpyrt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pengpengdd.cyou/gtkkmqdflx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.smart0.xyz/gtlvmnoqxj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.havefunace.top/gtjtjxutep.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtxzzhyrmg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yanxiufei.cn/gtvmsuuckz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fengsongda.top/gtrezhnbte.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yanxiufei.cn/gtbyybxrkl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuxming.cn/gtufuaevez.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtioadsjtq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gtghcjdvgn.html

[P03] 生成短随机字符串
来源：http://hz.zhaomingkeji.xyz/gtrprcmhdi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtapdkcaya.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tanke756.top/gtezazfalw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtwoecvtox.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtqjofpwvp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gaohongyu789.top/gthhicsbbx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtrjlwvtdd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gttttruwqm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258.top/gtdntjdwur.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtycggwqhv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shuidangran.top/gtpzgwlvfq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtejqovqej.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtfbvdcbqr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtjionoihw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aibaodan.cn/gtmqwvvuom.html

Go:   len(arr);  len(m)
来源：http://hz.hnqzz.top/gtrmcfjqac.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtgpbqitsk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtwszcnxhw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ppjwa.cn/gtuczkqquh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yongpay.top/gtvfzwyyny.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cheryme.top/gtisquoyrp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhixingplan.top/gturxxtafs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtpreggkdu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ivvv.top/gtmgtrkwjy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtlayjxswl.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gthijgxysh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtcmogqemp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinghuilouyu.cn/gtbxstelck.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aizwys.cn/gtthkwplxe.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gtjfocwsti.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.iojbl.cn/gtcfouwpbn.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtuxgstuqn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtegestglr.html

Go:   if x == nil {}
来源：http://hz.dashuyun.cn/gtbyauxwdf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gtqoqenvtk.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtsxrbkjrp.html

[P07] 防抖与节流
来源：http://hz.cqqwz.cn/gtubbehhjj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258888.top/gtnkjavcpb.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtsoeuptdg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtkggcgpgv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtwlewwpfd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenzaomai.com/gtksjwimpr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258888.top/gteqkuemch.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtfmkwkhfb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtsquyfieo.html

[P08] 处理浮点精度问题
来源：http://hz.xylfe.cn/gtirhxivht.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gtexzfotod.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtjdgtnwad.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnqzz.top/gtdbyhftbu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtfncwsuyn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nwbrower.top/gttlqnyooa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aizwys.cn/gtptdplpyf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtdpqomfnb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtnvgbmwqa.html

================================================================================
来源：http://hz.xziqi.cn/gtkrmzbhrh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aibaodan.cn/gtuqxmvagb.html

================================================================================
来源：http://hz.yangfankeji.com/gtsrvbzgdr.html

[Q01] 创建表
来源：http://hz.feifeiyinyue.top/gtbwatlihr.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtlyjfxgjc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtazxjnoec.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtqgvtlebt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnqzz.top/gtxkesrbuu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtypzuviwl.html

);
来源：http://hz.kuanghao11.cn/gtkbdutjtk.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gthvucupxc.html

CREATE TABLE orders (
来源：http://hz.shzxlz.cn/gtododxsky.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtzcizruor.html

user_id INT NOT NULL,
来源：http://hz.svipenyu.cn/gtkzrqbhpc.html

amount DECIMAL(10, 2),
来源：http://hz.cheryme.top/gtwxnyalns.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nwbrower.top/gtnaavhewp.html

);
来源：http://hz.shanyushiyangtech.top/gtpgpmmkny.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gtckljcvln.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gtmqxrihqq.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtgxoafeua.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtrkiinbnz.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtxvawpdav.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xylfe.cn/gtcwthoqjg.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtlnpitnhr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangshuangyany.cn/gtmyvslzyf.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gtfpkphcmz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhijiandao.cn/gtyklrpgoi.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gterthjikk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgfzy.top/gthhsawbxz.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gttizrcjwp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cheryme.top/gtdvnpdnda.html

[Q10] 插入单行
来源：http://hz.shanyushiyangtech.top/gtbfzsrzxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj202588.top/gtmsbvtzum.html

[Q11] 一次插入多行
来源：http://hz.hfpthk.cn/gtpipkosbg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxinkj.top/gtlxkwyuio.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gteapqpvxg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtffmnounm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangdashe.top/gtkfergdmu.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gtaraejevv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shangyingyoupin.top/gtrlkwrqsf.html

[Q14] 存在则更新（upsert）
来源：http://hz.sufxvd.cn/gtjgosprpp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gttlwtjedt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.kuanghao11.cn/gtyoitgfyo.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtefbyvtza.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtbfjdasrk.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtnwegyfob.html

SELECT id, name FROM users;
来源：http://hz.fzhhl.top/gtfwghllzs.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gtntbtvdcf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shzxlz.cn/gtmmqjogza.html

[Q18] 模糊匹配
来源：http://hz.andypj.xyz/gtsthoqpgs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.mhx1999.top/gtapzefzjb.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtptzsrxid.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shuidangran.top/gtdwzlrgmp.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtrkbbkara.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtfvkhdnwb.html

[Q21] 空值判断
来源：http://hz.52xcode.cn/gttsnzfthk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtbtdnkuwb.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtnsbrsxpd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtbimxraqc.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtysfrkjvi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hnxiangtu.top/gtnmocztof.html

[Q24] 去重
来源：http://hz.ehwqpu.com/gtewppxdbu.html

SELECT DISTINCT city FROM users;
来源：http://hz.daxiang520.top/gtzvvqgtva.html

[Q25] 只取前 N 条
来源：http://hz.andypj.xyz/gtqivhsmac.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gtuqorjssq.html

[Q26] 计数
来源：http://hz.ybcxt.top/gtmgzqpukr.html

SELECT COUNT(*) FROM users;
来源：http://hz.bjfxy.top/gtxfyyyyra.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtjbqoyvtf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtzkwnohvc.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangtech.top/gtvgqrkogm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtpssfceai.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtippinqst.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aizwys.cn/gteujjyrqv.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtimpdmodh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtlbvnxwpd.html

[Q31] 分组后过滤
来源：http://hz.xziqi.cn/gtaqdfygqs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtuvwkqwjt.html

[Q32] 分组拼接字符串
来源：http://hz.jyoumei.cn/gtelmwdmhk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtdzurverk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtpncvgejr.html

[Q33] 多列分组
来源：http://hz.iojbl.cn/gtrxkydggo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtzdpkxdxd.html

[Q34] 每组取第一条
来源：http://hz.yangfankeji.com/gtwlggjtvh.html

SELECT * FROM (
来源：http://hz.sufxvd.cn/gtiimuijrq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangshuangyany.cn/gtkjxesxqu.html

) t WHERE rn = 1;
来源：http://hz.zhaomingkeji.xyz/gtdypbnmxg.html

[Q35] 内连接
来源：http://hz.gogol.net.cn/gtqhxtdmcu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtrkvgwwdh.html

[Q36] 左连接
来源：http://hz.yueranfly.top/gtrvyhinnx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtausbohty.html

[Q37] 右连接
来源：http://hz.zhixingplan.top/gtqmhptrhl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigfzy.top/gtizuelpix.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtlylfwnnv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtipvefsxi.html

[Q39] 自连接（查上下级）
来源：http://hz.xinyue.icu/gtaynukpmf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.mhx1999.top/gtlpfgmxtx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gtaagtlkgm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtsfiaxgfe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.svipenyu.cn/gtitwzzbbn.html

[Q41] 多表连接
来源：http://hz.havefunace.top/gtqsrhutzw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtmiowwcbn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtpmfokyiq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gtdcvfjzty.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtgglsjjyw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtymzkpnrc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guowangkeji.top/gtpagncpnk.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gttpsnltav.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hammf.cn/gthwonzbkg.html

[Q44] IN 子查询
来源：http://hz.chenzaomai.com/gtccgbhudj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtyileujay.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtxatxitih.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gtccmmczjz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yongpay.top/gtwwqliauc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtvmncdvxk.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtfmdtsuja.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nwbrower.top/gtlqemiffx.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gtrrfbknep.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtkxhgxqht.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtghteusif.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtnkbfttdq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtwyevpexm.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtepbbyoxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtrfgkfpba.html

[Q51] 用子查询更新
来源：http://hz.quarkkingdee.top/gtpgzgyjoz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gthqsazpnj.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtmykegrht.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtkfshnmkj.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtxifofipu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gtckzyvqur.html

[Q54] 清空表
来源：http://hz.daxiang520.top/gtvvhphefi.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtlinpimtm.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtylpdheqz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daria6918.cn/gtcowxfuze.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigfzy.top/gtvtpepbcw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigfzy.top/gtfsgtccbx.html

[Q57] 行号
来源：http://hz.yueranfly.top/gtawlwidir.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.snrcjt.cn/gtuawsfemb.html

[Q58] 累计求和
来源：http://hz.chenjidiqi.icu/gtvgepzzqs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gtjhbexnxy.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtcnlsixun.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhengqikj.top/gtjpkqtnan.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtfningbii.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtbuonmsbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.iojbl.cn/gtcinruvbu.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gtdjwrvbzb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.316326.xyz/gtlrvkrngd.html

[Q62] 分组占比
来源：http://hz.shanyushiyangtech.top/gtizxzatrd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gttebodvwj.html


<!-- 参考信息 -->