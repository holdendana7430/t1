代发 wailian999

Go:   // 手写递归
来源：http://hz.9152youxi.cn/gtoilanfrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gzhubu.top/gtfzhzboux.html

C#:   // 手写递归
来源：http://hz.haohaochexian.top/gtuhnnuthu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.mhx1999.top/gtagqdhmxj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daxiang520.top/gtreijvfod.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cucudq.cn/gtxwqrrepn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gttxixtoxn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtcisahjbc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtldzsgkea.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtzqpnjfrt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.52xcode.cn/gtmkkskrak.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtmtgzaohl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgxkxcmaw.html

O. 并发与异步
来源：http://hz.yanxiufei.cn/gthrohftth.html

================================================================================
来源：http://hz.dianchejie.cn/gtnlgghnrx.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gthkgfyrol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtfnhtwbig.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cucudq.cn/gtxtapwyah.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.havefunace.top/gtoahjlwrr.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtmcopyduy.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtguihctkx.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtuwkjtdiq.html

Ruby: Thread.new { f }
来源：http://hz.ydjk.org.cn/gttodxvqeq.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtbivaqwnw.html

[O02] 使用线程池
来源：http://hz.yj20258888.top/gtheywhvxt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtkgtrqjul.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhiwuduotai.top/gtzfdonqqv.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gteuwtimrf.html

TS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtbekpvhrg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtqhaeujog.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gogol.net.cn/gtlxddfasv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gttthfarjb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtrczdnymv.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gttoyreeyh.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtbeumggwu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtbxnaxjkh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ppjwa.cn/gtogmyaylx.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtbacuvgbs.html

Java: synchronized (this) { shared++; }
来源：http://hz.hongshengwenyu.top/gtbawradps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtjbsnsubw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtmhgcmsub.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtlcienbpl.html

[O04] 定义异步函数并等待
来源：http://hz.svipenyu.cn/gtppeujzxp.html

Py:   async def f():⏎    await g()
来源：http://hz.bjfxy.top/gtmzwsacoi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gtlufxmjhs.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtfzvmtgfo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenlongwang.top/gtvpsarsge.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtxywtbdqk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtjtzinrmh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sufxvd.cn/gtdhaxocfk.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gthykmywgp.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtotwplgcw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258.top/gtisywfeuu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yongpay.top/gterddlfhf.html

JS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtpuhddlcu.html

TS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtewdfmgtt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtlqemttrk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtjcvqzbsv.html

Ruby: threads.map(&:join)
来源：http://hz.jqgfzy.top/gtclcosqmv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jiagoushi.top/gtkorunjjt.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtcpaewdja.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gtjwbzhmsp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gtpfkjwxam.html

JS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtprmvpokr.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtlttirieu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtkaasblox.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtuirpykpy.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gtmquewjup.html

C#:   Parallel.For
来源：http://hz.yj20258.top/gtunadqozf.html

================================================================================
来源：http://hz.tanke756.top/gtgdlerzde.html

P. 常用工具函数
来源：http://hz.ydzc1.top/gtlkoteyqp.html

================================================================================
来源：http://hz.bjfxy.top/gtphfgtwvv.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtscvriiom.html

Py:   str(uuid.uuid4())
来源：http://hz.jinqigufen.top/gtmgxhnhtn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtuugjezem.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtchbvspdn.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtmysjundg.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtyyqzgmlu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.smart0.xyz/gtjxguqtqk.html

Ruby: SecureRandom.uuid
来源：http://hz.sysykeji.top/gtulxngcbs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yvedp.cn/gtkjeiresi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.kuanghao11.cn/gtureshizg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ivvv.top/gtyqarlnus.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fzhhl.top/gtelwmhbix.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ywan-chungtsiang.top/gtstmyaqwh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtwsuotfal.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zycfv.cn/gtxdhzvczw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gtxjsrialc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtokgwqzhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gtpkkbzdoi.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtqbtbocwy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtxyrbxqlo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hammf.cn/gtamlehzbm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtxguhaany.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtzaseozir.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cheryme.top/gtvfzrnyvn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gtbdsnskju.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtntbwcldg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hammf.cn/gtmxkdajnh.html

[P04] 求长度
来源：http://hz.zycfv.cn/gttxofucmx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yueranfly.top/gtmtzrsjzp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtyqpmjzgz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtbojvjnjv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtpluesdds.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shangyingyoupin.top/gthajitolx.html

Go:   len(arr);  len(m)
来源：http://hz.nanxuanxn.top/gtbkybnzdx.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtknfoqnye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtobwrvrfe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gtvxgubkqe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cdnleiting.top/gttblheeqd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xziqi.cn/gthhfdmvhp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gogol.net.cn/gtojexyrvl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gthoyckfuf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fengsongda.top/gtamnndald.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtjsziazqh.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtnpfmmixs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.haohaochexian.top/gtrvxsbsch.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtcuxwyezy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtqfndxygd.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gtgnuwvlxm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gtfmynqrts.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtvuabilis.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sxryk.cn/gtsoofdwqf.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtolrpggcg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gtwgiehset.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gturkadwdw.html

[P07] 防抖与节流
来源：http://hz.chenjidiqi.icu/gtyilujkba.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zycfv.cn/gtjzsykxmu.html

PHP:  // 手写时间戳比较
来源：http://hz.andypj.xyz/gtcytgkiuo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtlcfocqvj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtwwqzvjsl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangshuangyany.cn/gtxtherkix.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.c1oappe.top/gtpwzblqjj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gtgfopkgez.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ivvv.top/gtoiemeqjg.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtebmdzyyi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gogol.net.cn/gtfaxjaftw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jianghu66.top/gtsjkvupyj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtwnobopzo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtkfucbxli.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhengqikj.top/gtvxyujcqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sxryk.cn/gtpvuycvwt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aizwys.cn/gtojftywxq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gtztfuerfk.html

================================================================================
来源：http://hz.yueranfly.top/gtiombwkrg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dashuyun.cn/gtnuarygcj.html

================================================================================
来源：http://hz.aibaodan.cn/gtdsqyddag.html

[Q01] 创建表
来源：http://hz.hnxiangtu.top/gtdzpkizab.html

CREATE TABLE users (
来源：http://hz.ydjk.org.cn/gtbonuvzoq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtecntgqvv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtqbppavlh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenjidiqi.icu/gtswmpwled.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.andypj.xyz/gtelgugkcg.html

);
来源：http://hz.sysykeji.top/gtpfyfqdep.html

[Q02] 创建带外键的表
来源：http://hz.zhongyouzk.top/gtuxmgomuy.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtpsrajlsy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtjschexsw.html

user_id INT NOT NULL,
来源：http://hz.zhengqikj.top/gtbamywcbm.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtxekfwklg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cashguo.top/gtjyxakdmc.html

);
来源：http://hz.nanxuanxn.top/gtlhnugbar.html

[Q03] 增加列
来源：http://hz.havefunace.top/gtaijudbxz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jyoumei.cn/gtlniovnjo.html

[Q04] 修改列类型
来源：http://hz.yj20258888.top/gtfcmyjrnu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.feifeiyinyue.top/gthjsbqera.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtmuwfuhup.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fengsongda.top/gtpszogktx.html

[Q06] 删除列
来源：http://hz.xinyue.icu/gtdmgqytan.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258888.top/gtybnmfvli.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtxlsxdtcp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yanxiufei.cn/gttdfegljq.html

[Q08] 创建普通索引
来源：http://hz.jinqigfzy.top/gtyjeyqojq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtxfzrjrag.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtucxdrhov.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ehwqpu.com/gttlcxagem.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtdzqeimlb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.dashuyun.cn/gtzcybqwhu.html

[Q11] 一次插入多行
来源：http://hz.gzhubu.top/gtswmruxtk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtwqcxwvui.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtidgarasv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aizwys.cn/gtmiyvyjmv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xinyue.icu/gtazirrnjo.html

[Q13] 忽略重复插入
来源：http://hz.ybcxt.top/gtvrobjibt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yangfankeji.com/gtybthqgtx.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtjxyzumxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtewaihlpo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtezvckzcy.html

[Q15] 查询全部
来源：http://hz.yangfankeji.com/gtqdspkkqw.html

SELECT * FROM users;
来源：http://hz.andypj.xyz/gtejbnjuzs.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gtgumkshrn.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtovkpctan.html

[Q17] 条件查询
来源：http://hz.havefunace.top/gtnzuvsvde.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gtbcpculbk.html

[Q18] 模糊匹配
来源：http://hz.cqqwz.cn/gtqkkcjipg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgufenzy.top/gtkybglrzz.html

[Q19] 范围查询
来源：http://hz.cheryme.top/gtoppwowkf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gaohongyu789.top/gtmefgijhm.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtgmixskua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtkaymdlxq.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtxqkensoo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xingfuxueyuan.xyz/gtoiuqcvfn.html

[Q22] 排序
来源：http://hz.guannengcc.top/gthgqmzmsk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gturvqhbnx.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtkbhwycsx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtcoibzldb.html

[Q24] 去重
来源：http://hz.ybcxt.top/gtbjtprgxn.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtyopnfghv.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtxwxzcntw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pengpengdd.cyou/gtyeqqkggb.html

[Q26] 计数
来源：http://hz.9152youxi.cn/gtcjaesloo.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtojkqeibs.html

[Q27] 条件计数
来源：http://hz.yvedp.cn/gtgjekuydz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtttmmwyky.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtfjyijuis.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gogol.net.cn/gtfbrkjsio.html

[Q29] 最大最小值
来源：http://hz.svipenyu.cn/gtktsaeywu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gthgyrrehp.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gtlitrtzrv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtdrrkwnqq.html

[Q31] 分组后过滤
来源：http://hz.chenlongwang.top/gtkvgxhyhh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtmuiarzld.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtpdtahubn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtdisimryu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtaverwnvv.html

[Q33] 多列分组
来源：http://hz.nanxinkj.top/gtjzgmnmwd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtdmlzfeqa.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtursrsrjv.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtpjmfndpz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtuhbxpowy.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtprdxfvkq.html

[Q35] 内连接
来源：http://hz.jqgufenzy.top/gtzvvnsnmn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtwhoqiphl.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtwngqsonj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtbyhniitj.html

[Q37] 右连接
来源：http://hz.chenlongwang.top/gtrmhprbcb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtrpyqzqhp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtomssetjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hongshengwenyu.top/gtegxhwqix.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gtirakbypt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sweek.top/gtzpblkhnq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtktpdggru.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtrvsqhdsh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtfwzbkpev.html

[Q41] 多表连接
来源：http://hz.aibaodan.cn/gtplrqxixc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258888.top/gtsjixaouz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtatkdwpzd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ppjwa.cn/gtpgihxqnu.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtjazzqdlv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtaahvrtlj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtknticxkb.html

[Q43] 标量子查询
来源：http://hz.kuanghao11.cn/gteodanufl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.birdmap.top/gtlovishfs.html

[Q44] IN 子查询
来源：http://hz.guannengcc.top/gtjvjcsjpe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtvwgsplpy.html

[Q45] EXISTS 判断存在
来源：http://hz.yueranfly.top/gtlznakess.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.kuanghao11.cn/gtlmagcpsv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dashuyun.cn/gtlabuuaxm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gtoyzfrxtf.html

[Q47] 与平均值比较
来源：http://hz.yvedp.cn/gteqcotopb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yanxiufei.cn/gtsahglykw.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtrdpabrnm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtdrqfcynq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gtxjgehxee.html

[Q49] 更新单行
来源：http://hz.gzhubu.top/gtqjiewsbe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtpskapkdp.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtutmtkyka.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258888.top/gtrixqrcdl.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtctjgkdox.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtdpmucprx.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtmodffwag.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gthttjugsw.html

[Q53] 按条件删除
来源：http://hz.daxiang520.top/gtzmxkdoek.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtrnjrluje.html

[Q54] 清空表
来源：http://hz.zhijiandao.cn/gtbaigucfh.html

TRUNCATE TABLE logs;
来源：http://hz.gogol.net.cn/gtqvkccofm.html

[Q55] 排名（并列占位）
来源：http://hz.ydzc1.top/gtzjgzswus.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gthvjbhnce.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinghuilouyu.cn/gtixqlnelf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtgumkcytg.html

[Q57] 行号
来源：http://hz.daria6918.cn/gtxqavpesn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hfpthk.cn/gttikudrie.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gtskzyhxab.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtslelfcbi.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtbhgtxiuo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtfqqhopxf.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtlbhlfxhz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gttlorpafn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gttkcsgbix.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtihhxpszz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtnggwxxod.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtybslotkc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtfzdzqqgc.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtsjqjcywq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtpawiunoe.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gtjknrtbtu.html

COMMIT;
来源：http://hz.cheryme.top/gtruqfuqkl.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtcbvyiixt.html

ROLLBACK;
来源：http://hz.sweek.top/gtdwkhmthd.html

[Q66] 行锁查询
来源：http://hz.pycfn.com/gtcxjwxbkc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cashguo.top/gtzgoksglu.html


<!-- 参考信息 -->