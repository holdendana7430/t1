代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.jinyuanbaomall.cn/gtxncjlvtm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gtezipbmgs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtegohhule.html

Java: // 手写递归
来源：http://hz.yj202588.top/gtcobmenbo.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtckjzqmot.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtnzdbdnqz.html

C#:   // 手写递归
来源：http://hz.birdmap.top/gtkjhbxlox.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydjk.org.cn/gtefxhbxqg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtisqjjabm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtkafoueyq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gthalioyfm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtvzsybowc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtqxuudbvh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtjiadzhpc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtajjfvczs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtgtbppkkt.html

================================================================================
来源：http://hz.kuanghao11.cn/gthzvnachu.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtuvpsmthd.html

================================================================================
来源：http://hz.guannengcc.top/gtvtyyjdzz.html

[O01] 启动一个线程
来源：http://hz.hnxiangtu.top/gtdqzzusie.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zdqjudy.top/gtrjffytsi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtyqqjtfvo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sxryk.cn/gtfzdeurwq.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtiuppszbq.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtelmtgbsn.html

Go:   go f()
来源：http://hz.wangdashe.top/gtbykrzhmf.html

Ruby: Thread.new { f }
来源：http://hz.xziqi.cn/gtzcmcehbi.html

C#:   Task.Run(() => F());
来源：http://hz.dianchejie.cn/gtzafqspei.html

[O02] 使用线程池
来源：http://hz.yuanzhike.top/gtpvzkjgpi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtimxgpjmr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dianchejie.cn/gtvolgloay.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtakmrrbpg.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtaebwjblp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtbtqcgjqr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guowangkeji.top/gtclbcaoek.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtkrmnapgv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtqmauzbox.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtnpqiidkx.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gtridvnulu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangshuangyany.cn/gttxmpfmvt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtjkktaqgw.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtyjfmbvmt.html

Java: synchronized (this) { shared++; }
来源：http://hz.cdnleiting.top/gtzcwyojfc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtlmjoaiif.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guannengcc.top/gtwaclvlrx.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj202588.top/gtmlfslcns.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtylgmijxs.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gtiwhernfi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenzaomai.com/gtqswdpyue.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtlllbwhsg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zdqjudy.top/gtpjejdhpl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtayxcqwmr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.havefunace.top/gtugujljyr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydzc1.top/gtnuvwtpxh.html

C#:   async Task F() { await G(); }
来源：http://hz.gaohongyu789.top/gtiiaqivwz.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnqzz.top/gtmiqxyvwg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhengqikj.top/gtbrzflceu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtwhhulmjs.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtmmoixnlr.html

TS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtpbfkomsb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtendvwaml.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtmnpwcnnp.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtzjqolitq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhongyouzk.top/gtzwnvqtcw.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtqgsxvxni.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gteoldrmks.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtsfgyuwsb.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtxaswcriq.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtxcgvmokl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigfzy.top/gtplhirhvi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pycfn.com/gtllnfwxqs.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gtqlduaovw.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtufioemqd.html

================================================================================
来源：http://hz.hysaishi.cn/gtcdtolvot.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gtqikficun.html

================================================================================
来源：http://hz.zhoulong.xyz/gtaeomomdw.html

[P01] 生成 UUID
来源：http://hz.dianchejie.cn/gtncysphai.html

Py:   str(uuid.uuid4())
来源：http://hz.wangdashe.top/gtgliviyco.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydzc1.top/gtczjugpdx.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtkbpudkjm.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtadgkrjiz.html

Java: UUID.randomUUID().toString()
来源：http://hz.xuetiantiany.cn/gttmfjmvwg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.kuanghao11.cn/gtlcrkvtok.html

Ruby: SecureRandom.uuid
来源：http://hz.cqqwz.cn/gtjydjxacu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.mhx1999.top/gtvwxurvqw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnqzz.top/gtfffytbvu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.dashuyun.cn/gtaxxbikgw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtxlbrtdfl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.svipenyu.cn/gtojjopzac.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtfsltfuxb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cdnleiting.top/gtvaifwzul.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xinyue.icu/gtvytwugms.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtjaqtmgok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.52xcode.cn/gtsdtbburq.html

[P03] 生成短随机字符串
来源：http://hz.ybcxt.top/gtngisctny.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tian-w.cn/gtilfqjykc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yonumen.top/gtpnnucugq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtexhwoxix.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gthkumzdpy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtimpwjkij.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangshuangyany.cn/gtpmwswdld.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yonumen.top/gthprscwae.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenzaomai.com/gtbzzlnjow.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gtetjjntpw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gttoavjcgl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gtbkmrqcwy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtqcmkmnff.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtojgncihm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtkxwcvnfs.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtrblkhanr.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtsthapsvj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtcfdcalda.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ehwqpu.com/gtzsoclbra.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtqfhylylw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtrtjezwrg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtkaeoxihc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtacyumdtk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xingfuxueyuan.xyz/gtfnrvlyaj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtxvjnnrpo.html

Ruby: a == b
来源：http://hz.havefunace.top/gtpmwbsqxq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtrokwtcbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gtxvjwvatb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtbsuzwrms.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gtxogptrng.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtvrxyjxdi.html

TS:   if (x == null) {}
来源：http://hz.c1oappe.top/gtanvgwunt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gthvjvuefj.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtylwgewqi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenjidiqi.icu/gtorekcmfn.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtavkcuxdg.html

[P07] 防抖与节流
来源：http://hz.zhijiandao.cn/gtvvhlvwec.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtwrvdaujv.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtsaedkpwt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtbutxmwoh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtlahzukxh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtbusjozbx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guannengcc.top/gtjscinxcn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangkeji.top/gtlibuvxny.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenzaomai.com/gtoufcpdxh.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtmmdaljii.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuetiantiany.cn/gttcmdnqtu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtkyblpifz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtsgmuolfo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jianghu66.top/gtflhjhhfx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gteuqkozvy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtltlzbski.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtmnkhzypi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnxiangtu.top/gtghcqdqwd.html

================================================================================
来源：http://hz.chenzaomai.com/gtosqrgkqw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtvarzdlkr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtrhwxnbja.html

[Q01] 创建表
来源：http://hz.haohaochexian.top/gtwgfboltn.html

CREATE TABLE users (
来源：http://hz.ivvv.top/gtwmeziuqx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtqkpbqsuy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtgozjetko.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtfetbnxuw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cashguo.top/gthmcseayx.html

);
来源：http://hz.zhoulong.xyz/gtcfyuuzrb.html

[Q02] 创建带外键的表
来源：http://hz.316326.xyz/gttntlxgwy.html

CREATE TABLE orders (
来源：http://hz.jinqigfzy.top/gtilliiwtr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtrnrdfohn.html

user_id INT NOT NULL,
来源：http://hz.hammf.cn/gtbqdfvqyg.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtjrchgofq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigufen.top/gtxsvigilh.html

);
来源：http://hz.ydjk.org.cn/gtmslfbdha.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gtixathvgb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.c1oappe.top/gtulrfypxm.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtzelmtlhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtsxlgrxog.html

[Q05] 重命名列
来源：http://hz.pengpengdd.cyou/gtzsufwnht.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangshuangyany.cn/gtsiekctoy.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtqmelqcxr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shuidangran.top/gtlgsulkxm.html

[Q07] 删除表
来源：http://hz.9152youxi.cn/gtyoygkcan.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhiwuduotai.top/gtrcurgfrv.html

[Q08] 创建普通索引
来源：http://hz.cucudq.cn/gtvasqpxdb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtpelhagry.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gtcobjwkjg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtsxxaqych.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtgiwoagab.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtajurwyog.html

[Q11] 一次插入多行
来源：http://hz.nanxinkj.top/gtwgysumkn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtnzfkiibj.html

[Q12] 插入后取自增 ID
来源：http://hz.yonumen.top/gtdcoamrpo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gttsdcxxua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gttmnrtzfr.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtuvdrzyim.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aibaodan.cn/gtugrlqecp.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtvfgfygei.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cashguo.top/gtwjgzlabd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtlgdhcjlj.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtuqvlzsfx.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtcqxchlbj.html

[Q16] 查询指定列
来源：http://hz.daxiang520.top/gtzaqbfobt.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtjngkurzy.html

[Q17] 条件查询
来源：http://hz.9152youxi.cn/gttizsbplu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtogzojgdu.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtlptrtzjv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtnpnllurs.html

[Q19] 范围查询
来源：http://hz.ywan-chungtsiang.top/gtjrxcjcug.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtodfzredm.html

[Q20] IN 列表
来源：http://hz.jinyuanbaomall.cn/gtknstazyg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtnthuadad.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gttqxythja.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aizwys.cn/gtqftxojnq.html

[Q22] 排序
来源：http://hz.jinghuilouyu.cn/gtwdnlzffp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yvedp.cn/gtsgutqiiu.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtlomfnqqv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtbtjawkhi.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gticolblse.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtconcrtke.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtqyvvqrbz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gthtdcxkyb.html

[Q26] 计数
来源：http://hz.ywan-chungtsiang.top/gtymutsqna.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtyvcujxmd.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtehjmcyyl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtamknrvpg.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtdxdbqgfz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtyonavonq.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtwhdicaaq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gtzrkaudyq.html

[Q30] 分组统计
来源：http://hz.zhijiandao.cn/gtvzwxqqds.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gttefuthxy.html

[Q31] 分组后过滤
来源：http://hz.jiagoushi.top/gtdwxetamq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tian-w.cn/gtpeaegeyq.html

[Q32] 分组拼接字符串
来源：http://hz.jqgufenzy.top/gtcizsadpy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtrsaqcnmk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gttpppoxou.html

[Q33] 多列分组
来源：http://hz.yuxming.cn/gtmuqlufnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guowangkeji.top/gtzjsmgmyn.html

[Q34] 每组取第一条
来源：http://hz.hongshengwenyu.top/gtuzkzelii.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gtzplrjurh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj202588.top/gthvwuwhtj.html

) t WHERE rn = 1;
来源：http://hz.zdqjudy.top/gtmexpkfya.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtdyqwnekj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtppawzpmj.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtsncmxibr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtxffrpmct.html

[Q37] 右连接
来源：http://hz.iojbl.cn/gtwunfeeuq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gtckcpotfz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ppjwa.cn/gtisycrfip.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cdnleiting.top/gtptwfddil.html

[Q39] 自连接（查上下级）
来源：http://hz.sxryk.cn/gtkbxtsfkf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtvkglfudm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtrbzkirjn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnqzz.top/gtqgkremrp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.smart0.xyz/gtosbcqnyn.html

[Q41] 多表连接
来源：http://hz.zdqjudy.top/gtrpvxjlvw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtiiyweaug.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtigmfqzxo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtpaftstmm.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gtiysekmdp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtjdkrdlbo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gteogxzrkg.html

[Q43] 标量子查询
来源：http://hz.guowangkeji.top/gtsjhbhxec.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sweek.top/gtbqrpgtgb.html

[Q44] IN 子查询
来源：http://hz.yueranfly.top/gtfkbpvebi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtauhnrfdz.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxinkj.top/gtluopofoj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtzncsbifh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gtzsgelhcb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gttwedpzrx.html

[Q47] 与平均值比较
来源：http://hz.shangyingyoupin.top/gtxdzbvlkp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gtvrvspbib.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtbcbgowcf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtkskvbayw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhongyouzk.top/gtnzlfvzns.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtijvutdxm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxinkj.top/gtxzxfcsrp.html

[Q50] 批量更新
来源：http://hz.hfpthk.cn/gtkxmvubhq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zdqjudy.top/gtwpdlvaoa.html

[Q51] 用子查询更新
来源：http://hz.ywan-chungtsiang.top/gtilwzphky.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtdopeajkg.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtnowphlza.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fengsongda.top/gtffxtbxat.html

[Q53] 按条件删除
来源：http://hz.gzhubu.top/gtcshgggun.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jlsjyb.cn/gtgrbsgqxv.html

[Q54] 清空表
来源：http://hz.sweek.top/gtgrpzxgzt.html

TRUNCATE TABLE logs;
来源：http://hz.havefunace.top/gtuwatynqt.html

[Q55] 排名（并列占位）
来源：http://hz.zhixingplan.top/gtpptkrkij.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtvbjefdrs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhengqikj.top/gtslrsfysp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtvokjjdjz.html

[Q57] 行号
来源：http://hz.jinyuanbaomall.cn/gttsxblumu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yanxiufei.cn/gtgiodegcn.html

[Q58] 累计求和
来源：http://hz.gotoacloud.top/gtykondyvb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gtvvniunxs.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtcrxczvbs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtsdmrweow.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gttwgwpwwg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtgexmhbhp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtcffljsdh.html

[Q61] 移动平均
来源：http://hz.daxiang520.top/gtcitczvdf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yongpay.top/gtqfqkmyug.html

[Q62] 分组占比
来源：http://hz.jinqigufen.top/gthmsybnko.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtffrapxek.html

[Q63] 开启事务
来源：http://hz.aibaodan.cn/gtsrcogtlq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gtlowkpbdx.html

[Q64] 提交事务
来源：http://hz.shzxlz.cn/gtipuvlrav.html

COMMIT;
来源：http://hz.daria6918.cn/gtxnlwowcf.html


<!-- 参考信息 -->