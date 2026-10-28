代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.smart0.xyz/gtpygbbguq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cheryme.top/gtllgpebwq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtubiejtnj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gthgelonky.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtjkhrcjio.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fengsongda.top/gtfudidcsj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tianlin.xyz/gtnvjsspvb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtqikuicwr.html

================================================================================
来源：http://hz.cheryme.top/gtbbdrfqzg.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtenwtmptm.html

================================================================================
来源：http://hz.cdnleiting.top/gtrzepftro.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtymqdrdeg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtilezphsp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hysaishi.cn/gteifirzsh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtxvtqiyti.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtsnmdzjur.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtsnksencp.html

Go:   go f()
来源：http://hz.hywenlv.cn/gtetktfewe.html

Ruby: Thread.new { f }
来源：http://hz.ppjwa.cn/gtqtccmdpy.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtyiwhaslk.html

[O02] 使用线程池
来源：http://hz.cheryme.top/gtuguhckwl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydjk.org.cn/gtnqiwhedj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtkmyayhvi.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtjisanthd.html

TS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtymqtdltm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hfpthk.cn/gtbdiiypyd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtsfbsmqsh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tian-w.cn/gttcwmgfbx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtqgbpwyse.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtjzogbamt.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtckpcbcxg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtzgpjlpth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtpbynmrcl.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtvpozswdf.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gtmwigpzxq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.9152youxi.cn/gtkzzjmhds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtrbrmvhiz.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnqzz.top/gtqxqqrhti.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtxjuwixdu.html

Py:   async def f():⏎    await g()
来源：http://hz.iojbl.cn/gtxrfaecme.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shzxlz.cn/gtvarzqspf.html

JS:   async function f() { await g(); }
来源：http://hz.yongpay.top/gtfxududbu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtlumysikp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gtvhxfkdzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtyhxjnmcj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtyjupmfxs.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtscsqyqgj.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhengqikj.top/gtvbuofqii.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtlsdhevca.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtriqjddcc.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtceomxpxf.html

TS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtmjmfpehq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gttvhsmoqd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgufenzy.top/gtksptxawv.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258.top/gtfwizdvqh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgfzy.top/gthtgjzqjw.html

[O06] 使用进程池
来源：http://hz.ehwqpu.com/gtefvkscfs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtcjhnripj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtwewtcbzy.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtcmtlpdmj.html

TS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtvxpbwbcm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dashuyun.cn/gtqzclaald.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gtmsdbxjtu.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtljfehkyy.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gtzqljeobf.html

================================================================================
来源：http://hz.havefunace.top/gtiykapybu.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gtkyqggwvk.html

================================================================================
来源：http://hz.zdqjudy.top/gtbanjkdei.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtdtsopnwu.html

Py:   str(uuid.uuid4())
来源：http://hz.hnxiangtu.top/gtjubjlxyd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtzfsxbvii.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtgwaibdpq.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtmgjcytdb.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gtkpwmbqzj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtgplijzlk.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gtetlsgayg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhijiandao.cn/gtovnayrxz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenlongwang.top/gtonfdltwp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtjexotabg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtlfituihc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hfpthk.cn/gtofansagf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtbwwpfwep.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtmurxgzjq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtzwxjmcpf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtuukobjvw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.haohaochexian.top/gtimapqrpr.html

[P03] 生成短随机字符串
来源：http://hz.jinyuanbaomall.cn/gteziscjny.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtrmeermyo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhoulong.xyz/gtxbujmlae.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtkxguhaua.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gthwgbmsky.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtrfepszwi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinghuilouyu.cn/gtydbatdgb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gttygzdjnt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zycfv.cn/gtzbdpwyhy.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtxclxauxx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtbmsewkey.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtwpmslntz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtmqrshxuy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtwbftkzdy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fzhhl.top/gtucdehdxo.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtjcxpaffs.html

Ruby: x.length;  x.size
来源：http://hz.havefunace.top/gtaqrpfcom.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cqqwz.cn/gtfqodwumk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gtkltfzlev.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pengpengdd.cyou/gtuigktlzb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtamqvfgpe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zdqjudy.top/gtnhywgjdx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtgcpgawkx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jiagoushi.top/gtbsoohqrw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtslzfidky.html

Ruby: a == b
来源：http://hz.c1oappe.top/gtxbkewpar.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.smart0.xyz/gtpinkithu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zdqjudy.top/gtklbotceo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtvmywtwhn.html

PHP:  if (empty($x)) {}
来源：http://hz.aibaodan.cn/gtvuecaoxt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gtqbojcpqn.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gtfpjcfhgl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtpayobcsg.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangkeji.top/gtpxbacwmv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ehwqpu.com/gtiazqgymz.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gtimspekfc.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gthogrycos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydjk.org.cn/gtkbowgqkj.html

PHP:  // 手写时间戳比较
来源：http://hz.aibaodan.cn/gtmjcbxgqi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gthsplrejy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtidfwgkeo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtfzhdyteh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtikfnfask.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtrnkrcraw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aizwys.cn/gtygwvadwz.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gtobbetrbg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.redwolf501.top/gtifnvmvkf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtpurfkwsp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gtfjqhnupu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shuidangran.top/gttrwqirvw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ywan-chungtsiang.top/gtwnhncsrc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.52xcode.cn/gtazvvgmcj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtmcmlwker.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtppbmvymo.html

================================================================================
来源：http://hz.shuidangran.top/gtjiebkqtm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgfzy.top/gtzmtbhbbm.html

================================================================================
来源：http://hz.meibo888.top/gtaenuqtyl.html

[Q01] 创建表
来源：http://hz.pengpengdd.cyou/gtztybijyr.html

CREATE TABLE users (
来源：http://hz.jqgfzy.top/gtwcwatqhg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gthcspgwfi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtctcpojeh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gtveczmzhm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangshuangyany.cn/gtsicraybm.html

);
来源：http://hz.daxiang520.top/gtvqsiffcd.html

[Q02] 创建带外键的表
来源：http://hz.nwbrower.top/gtihkltqmh.html

CREATE TABLE orders (
来源：http://hz.svipenyu.cn/gtfljpcxwy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtnyaeills.html

user_id INT NOT NULL,
来源：http://hz.birdmap.top/gtmnlxdndk.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtlncqgqzb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtnvwavxvh.html

);
来源：http://hz.gaohongyu789.top/gtjoujkzao.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtgowpzwxi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gthqlwillb.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gtlnadpizm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zycfv.cn/gtkvkbblzo.html

[Q05] 重命名列
来源：http://hz.vqdsnc.cn/gtzfstkcng.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangdashe.top/gtuhytgiox.html

[Q06] 删除列
来源：http://hz.chenzaomai.com/gtftmvhnnv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gtyouboizv.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gtqneportx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hywenlv.cn/gtqcjojxrh.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtvipxlyqe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtyogfjhsk.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gtmmpwmyvz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtwprqtigu.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gttkbouqjl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guowangkeji.top/gtpholpyew.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtapedlpqk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ppjwa.cn/gtqzigtjei.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtmvhvtlgi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtzlsinysj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtxlfzemay.html

[Q13] 忽略重复插入
来源：http://hz.cheryme.top/gtzkcmxmpu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gttxqrmfht.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gthrbtnpuv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ywan-chungtsiang.top/gtwtrhglxv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xziqi.cn/gtqhidftpt.html

[Q15] 查询全部
来源：http://hz.yanxiufei.cn/gtwwqybmsq.html

SELECT * FROM users;
来源：http://hz.redwolf501.top/gtxmrgvmtj.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtcajbmybh.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtwtmlieka.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gtszjwusyu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtompeobtw.html

[Q18] 模糊匹配
来源：http://hz.0kj1m.cn/gtpwadmdws.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jiagoushi.top/gtstmwksbt.html

[Q19] 范围查询
来源：http://hz.gotoacloud.top/gtmrqiwqol.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtkbloiltq.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtypcdyzug.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigfzy.top/gtkqckiplb.html

[Q21] 空值判断
来源：http://hz.ybcxt.top/gtegoucknk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigufen.top/gtgxfelyls.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtthbbqgrx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gtydhlinxm.html

[Q23] 分页
来源：http://hz.dianchejie.cn/gtfvpbgocz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtmttfkxfr.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtsbtahllk.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangshuangyany.cn/gtusprgmsu.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtxlylghqc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtaqoqckjy.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtklbbioul.html

SELECT COUNT(*) FROM users;
来源：http://hz.yangfankeji.com/gtvklathlv.html

[Q27] 条件计数
来源：http://hz.dianchejie.cn/gtjvhvpzse.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hysaishi.cn/gtkfrvdvbp.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gtcowyirmn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yueranfly.top/gtfoyaxgtk.html

[Q29] 最大最小值
来源：http://hz.vqdsnc.cn/gtsqfqnmfs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuetiantiany.cn/gtonopjobx.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtkvspipau.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtubrxooad.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtndqeptmq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj202588.top/gtsvftgyhm.html

[Q32] 分组拼接字符串
来源：http://hz.52xcode.cn/gtiwwfeoxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gttkwnqwzr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aibaodan.cn/gtvhbxastx.html

[Q33] 多列分组
来源：http://hz.0kj1m.cn/gtgmtqejjr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.birdmap.top/gtxxwueicm.html

[Q34] 每组取第一条
来源：http://hz.ywan-chungtsiang.top/gtnlcfrphn.html

SELECT * FROM (
来源：http://hz.hammf.cn/gtyrfoqytt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gtcmgbgoym.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtrkazjhoy.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtnhpqzfnu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtnwrndfsn.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtnwjckmzs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtsqyccxmw.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gtllvtklot.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtekipflhl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtgwzgquzl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258888.top/gtavezpefn.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gtyxokintf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gtrqnpvzin.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.mhx1999.top/gtqkpabyti.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtvfpvivxy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangshuangyany.cn/gthchrltei.html

[Q41] 多表连接
来源：http://hz.quarkkingdee.top/gtvxcfdfkn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ehwqpu.com/gtzpvrguzz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuxming.cn/gtantdddfz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtkswszqql.html

[Q42] 连接条件附加过滤
来源：http://hz.tian-w.cn/gttaqsbqtp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtaytdrouv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aizwys.cn/gthsiotcur.html

[Q43] 标量子查询
来源：http://hz.tian-w.cn/gtqvyvowof.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtvrbbkjcy.html

[Q44] IN 子查询
来源：http://hz.fengsongda.top/gtglnchbvp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gotoacloud.top/gtcnkcjouk.html

[Q45] EXISTS 判断存在
来源：http://hz.jianghu66.top/gtniwdkbjb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtucuhvhna.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtzdcdtrrb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtsfnkniby.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtfnirpink.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtwhzldald.html

[Q48] CTE 公用表表达式
来源：http://hz.zhijiandao.cn/gtyhoubcix.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shzxlz.cn/gttrywgvjd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtnbaxhipd.html

[Q49] 更新单行
来源：http://hz.hongshengwenyu.top/gtkuuxwtei.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtjqemyuwg.html

[Q50] 批量更新
来源：http://hz.chenlongwang.top/gtokvpjdkw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtkbwlcxny.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtsuvshzxy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtvtamxeip.html

[Q52] 删除指定行
来源：http://hz.guannengcc.top/gtyemacbkb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtpmudzkbj.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtkdytrjtf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtazjfypuf.html

[Q54] 清空表
来源：http://hz.pycfn.com/gtltqexxgs.html

TRUNCATE TABLE logs;
来源：http://hz.xingfuxueyuan.xyz/gtkucwwxho.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtitimeksz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shzxlz.cn/gtbxsembut.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtozdabeij.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtdkslnfdw.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtmjrbbelk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtavkyxsvz.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gtlxirctdc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtfhixpjdd.html

[Q59] 分组内累计
来源：http://hz.hnqzz.top/gtytgxtrzl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fzhhl.top/gtkechfzwv.html

[Q60] 取上一行 / 下一行
来源：http://hz.kuanghao11.cn/gtkaqpcznu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtxwgreavc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtgrivmiim.html

[Q61] 移动平均
来源：http://hz.sweek.top/gtgrqgmyjh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj202588.top/gtbemyokru.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtrwokejte.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtgmpdamff.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtuukmqtck.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtvnvddens.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtlcctkzkg.html

COMMIT;
来源：http://hz.redwolf501.top/gtddzpdkre.html

[Q65] 回滚事务
来源：http://hz.quarkkingdee.top/gtxawcipdt.html

ROLLBACK;
来源：http://hz.bjfxy.top/gtrtxynydx.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtaxxoyuhr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtobokengj.html

[Q67] 设置隔离级别
来源：http://hz.iojbl.cn/gtajtpkowz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ivvv.top/gtfqkrllqo.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gtljijwphj.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gteutlxhiv.html


<!-- 参考信息 -->