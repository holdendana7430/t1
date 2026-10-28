代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtnfqpvlej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.meibo888.top/gttwdqggco.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtbuvhetch.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtythleihn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtbhcablov.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtvuyequbf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yonumen.top/gtujqfzapo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtcwlbuzuc.html

================================================================================
来源：http://hz.xinyue.icu/gtjvxfygpf.html

O. 并发与异步
来源：http://hz.havefunace.top/gtiynnomlz.html

================================================================================
来源：http://hz.smart0.xyz/gtumqzvaiq.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtuhbmdjlz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yanxiufei.cn/gtozukungg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.iojbl.cn/gtzloxhpgv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.birdmap.top/gtiwzanitb.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtakdrggng.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtibxkrmny.html

Go:   go f()
来源：http://hz.jianghu66.top/gtjlqxkezt.html

Ruby: Thread.new { f }
来源：http://hz.gzhubu.top/gtfxywdnzu.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtncixisae.html

[O02] 使用线程池
来源：http://hz.jinghuilouyu.cn/gtufxtbkhk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sufxvd.cn/gtharvecvm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hammf.cn/gtkvzldoae.html

JS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtupahuwfo.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtsczvqhhj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtvyldtbsw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258.top/gtcorvngoc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtmfwfxwrk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtbiezbhey.html

[O03] 加锁保护共享数据
来源：http://hz.ydjk.org.cn/gtmfzbeeqk.html

Py:   with lock: shared += 1
来源：http://hz.birdmap.top/gtrnofbvwu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtqclazxza.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtqspmguop.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtkljafdkv.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtxrycdvbq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guowangkeji.top/gtujknvjtq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxinkj.top/gtokumzlas.html

C#:   lock (gate) { shared++; }
来源：http://hz.jlsjyb.cn/gtfknubmlt.html

[O04] 定义异步函数并等待
来源：http://hz.yvedp.cn/gtvdgxssoe.html

Py:   async def f():⏎    await g()
来源：http://hz.jyoumei.cn/gtznwjanqs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tian-w.cn/gtcdxetuda.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gthqcobjor.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtkdcqmvsx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtxypuloxj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtvypjaatx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cqqwz.cn/gtmcwvurdc.html

C#:   async Task F() { await G(); }
来源：http://hz.cashguo.top/gtewlodgqg.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtbgzksyep.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258888.top/gtxblytbkz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtxlgjyzht.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtxvibigdh.html

TS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtcditykjt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.meibo888.top/gtozxhfhrq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtwflvaupe.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gteraslrva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtarwptpaz.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtohmfrkkp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtdphseoij.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtdfwwxlvm.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtpzrxmpcw.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtkwnpqapx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xylfe.cn/gtfdplafhv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtbrbjffsd.html

Ruby: // fork 块
来源：http://hz.zhoulong.xyz/gtqpkhwuam.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtrahwudxp.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtekwkowao.html

P. 常用工具函数
来源：http://hz.chenjidiqi.icu/gtifgmyoft.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlexseiea.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gtpvrjgcwc.html

Py:   str(uuid.uuid4())
来源：http://hz.xinyue.icu/gtbyaaabsn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtqeoqxgpx.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gteygzhhld.html

TS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtxksuyhwf.html

Java: UUID.randomUUID().toString()
来源：http://hz.yongpay.top/gthsywhwxf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtttxxgtsa.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtqnigpffg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtqimbtspg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtfhiiyjfv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtbgffrtoa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtobgxliyu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cashguo.top/gtwmdhjyld.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtagprhtyi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hywenlv.cn/gttjvmgxwj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gteyzyqcks.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nwbrower.top/gtlhonrmku.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cheryme.top/gtessdzjok.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtcsgxqozq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yanxiufei.cn/gtdvjtavvl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtljrhzggh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtijxjezma.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtylvdhhwm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aizwys.cn/gtulnxjeth.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gtirzpkdzf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuetiantiany.cn/gtejbitzse.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhengqikj.top/gtbqxtcauk.html

[P04] 求长度
来源：http://hz.shuidangran.top/gtyacpnjnq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtjghbtplc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtejpbzobb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtidgutbdy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtboyiyjbr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtvmnqdmye.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtlmgajner.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtikkyywlv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtdhdwszam.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtofrdxear.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gtiucqfuvm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtabkudxbf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xinyue.icu/gtifpqpxyi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtgddtulef.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cdnleiting.top/gtymtrjrkv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj20258888.top/gtogzufrer.html

Ruby: a == b
来源：http://hz.cheryme.top/gtwofvyxhb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtteprikwb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhongyouzk.top/gthighibrr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gthbxjdsde.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtwyaqvaxi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtwzfmowgr.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtzlcdmbgb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtqnqqnkjb.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gttwvwkynb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shuidangran.top/gtgrdihsbi.html

C#:   if (x is null) {}
来源：http://hz.svipenyu.cn/gtdmpastdb.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtptutemlu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cdnleiting.top/gtassesbzn.html

PHP:  // 手写时间戳比较
来源：http://hz.ppjwa.cn/gtytycqeao.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtwdescqym.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtkwktoxtl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtwuvrzbzh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hongshengwenyu.top/gthhjmuogo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gthzorrvpd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydzc1.top/gtodgryfqb.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtinqhgduy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xylfe.cn/gtlvbdgoxm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhongyouzk.top/gtruxtgzzc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cashguo.top/gtlhsllgak.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhoulong.xyz/gtideimuaf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtjqezxmtz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtcnvesydx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtkwkapola.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtmwnnczhk.html

================================================================================
来源：http://hz.iojbl.cn/gtjpdwvfyh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cheryme.top/gthwxoyiog.html

================================================================================
来源：http://hz.andypj.xyz/gthxkuovnz.html

[Q01] 创建表
来源：http://hz.pycfn.com/gterklzpwk.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtrjkajrqa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtjqrlrwhw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dashuyun.cn/gtvffzmkiy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pengpengdd.cyou/gtiffvtbok.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fzhhl.top/gtlmewetfv.html

);
来源：http://hz.316326.xyz/gtqbqzoakd.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtymtwpimq.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtgwkcwork.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtzvmhtlyy.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtdqakrjdj.html

amount DECIMAL(10, 2),
来源：http://hz.guannengcc.top/gttpjfclqa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shuidangran.top/gtwgtnosme.html

);
来源：http://hz.yuxming.cn/gtwgyzozxg.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtalrksmra.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aibaodan.cn/gtneaiuhjr.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtjmoxfgtl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtsqfckmbm.html

[Q05] 重命名列
来源：http://hz.shanyushiyangtech.top/gtzprmjrad.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtucvrmjyo.html

[Q06] 删除列
来源：http://hz.9152youxi.cn/gtvjzkdqlk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gtgtvaizju.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gthocnumjm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtsnujccao.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtuwpbiowm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj202588.top/gtqexvdfzq.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtwfwauetj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gtxsazxdib.html

[Q10] 插入单行
来源：http://hz.aibaodan.cn/gtyejhbbko.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtdkefgyzu.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtpsekscnk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtdckfjwhq.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtunjjdflo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gtcuuzypae.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258.top/gtyhcmxkns.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gttsptuzum.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gtnqavhcjm.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtadyhjzrp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtavofwexs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtqdtjzhfx.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gtinhnhnhy.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtgzuixqnu.html

[Q16] 查询指定列
来源：http://hz.yonumen.top/gttxmuyutl.html

SELECT id, name FROM users;
来源：http://hz.ydjk.org.cn/gtslxcpzbo.html

[Q17] 条件查询
来源：http://hz.gotoacloud.top/gtjigdcjho.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hongshengwenyu.top/gtqaxiocnf.html

[Q18] 模糊匹配
来源：http://hz.mhx1999.top/gtltovtnen.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtgmiisuon.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gtzcqqmywk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinghuilouyu.cn/gtujxwewdk.html

[Q20] IN 列表
来源：http://hz.guowangkeji.top/gtxedvuwzm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sysykeji.top/gtlzawikny.html

[Q21] 空值判断
来源：http://hz.shangyingyoupin.top/gttlcghird.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtcclmyvsp.html

[Q22] 排序
来源：http://hz.zhijiandao.cn/gtcdmqcgfy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.0kj1m.cn/gtnrndpueh.html

[Q23] 分页
来源：http://hz.cheryme.top/gtlgmwccst.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenjidiqi.icu/gtwbgdzilr.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtyksitghn.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhixingplan.top/gtbntmlbsp.html

[Q25] 只取前 N 条
来源：http://hz.jinyuanbaomall.cn/gtyeqrutgy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sweek.top/gtgquvjyir.html

[Q26] 计数
来源：http://hz.fzhhl.top/gtxzjexqkb.html

SELECT COUNT(*) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtcgdmemld.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtjgfvdboh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhijiandao.cn/gtlhpsokua.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gttixixiio.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtsyldupsg.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangtech.top/gtkscdukco.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhengqikj.top/gtdkfdmyhc.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtggudxnzs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtdifvozib.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gteimlkvtm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258888.top/gtgpnyeejy.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtffgmndwv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtxzsiiyph.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtuvqjsirl.html

[Q33] 多列分组
来源：http://hz.pycfn.com/gtwefnlrxw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hfpthk.cn/gtcdausbiq.html

[Q34] 每组取第一条
来源：http://hz.ppjwa.cn/gtpsjvaxhb.html

SELECT * FROM (
来源：http://hz.shanyushiyangtech.top/gtqucniavn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yueranfly.top/gtyfgwxenu.html

) t WHERE rn = 1;
来源：http://hz.guannengcc.top/gtspwxenbn.html

[Q35] 内连接
来源：http://hz.zhiwuduotai.top/gtowcfdumn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtnlohnfcw.html

[Q36] 左连接
来源：http://hz.jqgufenzy.top/gtbxdgxigw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtusonnvzm.html

[Q37] 右连接
来源：http://hz.svipenyu.cn/gtcltcfpas.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtbpnjgucg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jianghu66.top/gtyvgchgxh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fzhhl.top/gtsjfvlygr.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtjnyhuruu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigufen.top/gtoexylsgc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gtcsavhats.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gtxtczaavd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtivvlxyhx.html

[Q41] 多表连接
来源：http://hz.bjfxy.top/gtufngotqq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgfzy.top/gtbukkjtip.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtrcnxclle.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtgtvddoqd.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gtvdyqdkdm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtrifqnzpg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gtbenhssws.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtydlffnol.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gthzuztqik.html

[Q44] IN 子查询
来源：http://hz.zdqjudy.top/gtifrbtudx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtwfmgcpws.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gtwjqxklrz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtdcsbfuwm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtsreegixr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtlfqouphq.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtlyujbvub.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jyoumei.cn/gtyzszutlp.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtknoshcrb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gtuhhwxlnn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gotoacloud.top/gtgrkkmrgb.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gtkyiqzmek.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fzhhl.top/gtcbvopvss.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtryhkpqxp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinghuilouyu.cn/gtkiohaant.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtbdsgiduq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.quarkkingdee.top/gtlorxqfyt.html

[Q52] 删除指定行
来源：http://hz.haohaochexian.top/gtbfohziiy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtvrhvezdq.html

[Q53] 按条件删除
来源：http://hz.birdmap.top/gtopghhsbq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.feifeiyinyue.top/gtyqyovhsx.html

[Q54] 清空表
来源：http://hz.pycfn.com/gtcrsjthxe.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtfmkddjql.html

[Q55] 排名（并列占位）
来源：http://hz.kuanghao11.cn/gtaxyqqtio.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtmqfqijay.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aizwys.cn/gthiksuqfn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jyoumei.cn/gtnclqhcto.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtgvfqjroq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtcivhlexw.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gteuokoiaf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gtqhuhhpcp.html

[Q59] 分组内累计
来源：http://hz.tanke756.top/gtycxixzwz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtcckgyzne.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhijiandao.cn/gtxsgditjx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtcwvbtkpm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtrjjgluzp.html

[Q61] 移动平均
来源：http://hz.shzxlz.cn/gtkunrtvbh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gtfzbawxdh.html

[Q62] 分组占比
来源：http://hz.fzhhl.top/gtpubjggib.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtffqndbqv.html

[Q63] 开启事务
来源：http://hz.yj20258.top/gtwyumljkw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtxzzeiefv.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtoxbrqwfn.html

COMMIT;
来源：http://hz.sweek.top/gtjgochwsv.html

[Q65] 回滚事务
来源：http://hz.ydjk.org.cn/gtyntrmyqo.html

ROLLBACK;
来源：http://hz.aibaodan.cn/gtwxjbwcgn.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtotadvhwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtmiogjmoe.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtztuiwtas.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtuqmvwone.html

[Q68] 保存点
来源：http://hz.dianchejie.cn/gtsvdgemho.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtnnyhufdw.html


<!-- 参考信息 -->