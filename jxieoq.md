代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.birdmap.top/gtwychkinn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtkfyfrbkc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtflzikzyh.html

Java: // 手写递归
来源：http://hz.fzhhl.top/gtoqlioswd.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtvjfqwqvw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtatjsnino.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtrvyveawi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtqofdldos.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cucudq.cn/gtowbhafiu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtsjpsphrr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtxgzrfwvl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gttfhonjyz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtzkvadqzj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtnoedhxek.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtpaxozkpp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtbyinuzxk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtaswduaut.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtsoejbvaa.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtoficpkor.html

[O01] 启动一个线程
来源：http://hz.haohaochexian.top/gtnmqmiptz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgfzy.top/gtimraxvyb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhengqikj.top/gtcceicdru.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnxiangtu.top/gtojnvdwou.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtoimkdrrm.html

Java: new Thread(() -> f()).start()
来源：http://hz.fzhhl.top/gtunkxjcvy.html

Go:   go f()
来源：http://hz.daxiang520.top/gtaywmzhen.html

Ruby: Thread.new { f }
来源：http://hz.jiagoushi.top/gtolewytiz.html

C#:   Task.Run(() => F());
来源：http://hz.yuxming.cn/gtrprkrvoa.html

[O02] 使用线程池
来源：http://hz.sweek.top/gtejlubjxu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtozpmimio.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gtawdaabik.html

JS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtwvancakf.html

TS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gthgleooqo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtyujbnsed.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gttkaxwxkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtwcqapeye.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yonumen.top/gtxacojrlc.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtbqryxvlg.html

Py:   with lock: shared += 1
来源：http://hz.nanxinkj.top/gtwlsouqrd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gthixokjla.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gthassfryj.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtanhhewlq.html

Java: synchronized (this) { shared++; }
来源：http://hz.gotoacloud.top/gtkhyweiqx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtreoqkalu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtozfibdxi.html

C#:   lock (gate) { shared++; }
来源：http://hz.redwolf501.top/gtqejnscst.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtcqmynjrx.html

Py:   async def f():⏎    await g()
来源：http://hz.jinyuanbaomall.cn/gtdfkuahpj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtmaoegjlm.html

JS:   async function f() { await g(); }
来源：http://hz.meibo888.top/gtpfsrsqzl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ybcxt.top/gtyckswvxs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yueranfly.top/gtfktvkrkl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinyuanbaomall.cn/gteuxbezji.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhengqikj.top/gtvpltkxdn.html

C#:   async Task F() { await G(); }
来源：http://hz.vqdsnc.cn/gtplfebssn.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtftwerhmh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gtfjrlwhrb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cashguo.top/gtsdbqxcdx.html

JS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtfixklfkl.html

TS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtcpqkqnts.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhoulong.xyz/gtetcoagne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtgeqsovgc.html

Ruby: threads.map(&:join)
来源：http://hz.jyoumei.cn/gtevnksrrp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtddhalcrl.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtqozluxpn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gaohongyu789.top/gtlvqlsolx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtzjaydspb.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtjdurdxud.html

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtracwxigh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtgomfahtv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.9152youxi.cn/gtikbtljqx.html

Ruby: // fork 块
来源：http://hz.dianchejie.cn/gtvfnjbxut.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtttckbrlz.html

================================================================================
来源：http://hz.yj20258.top/gtymomiruz.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtcjjmvcdm.html

================================================================================
来源：http://hz.zhongyouzk.top/gtubqdukyp.html

[P01] 生成 UUID
来源：http://hz.shangyingyoupin.top/gtgoqikijb.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtelipfzfh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cucudq.cn/gtzxcgeziy.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gteirnfecj.html

TS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtzmzlsvto.html

Java: UUID.randomUUID().toString()
来源：http://hz.guannengcc.top/gtxoattqyr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hywenlv.cn/gtjpdpafgy.html

Ruby: SecureRandom.uuid
来源：http://hz.feifeiyinyue.top/gturkhzjpa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtxaivowrp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnxiangtu.top/gtryycryck.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj202588.top/gtwaakwyuy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cheryme.top/gtjwwzlerq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sxryk.cn/gtqbsboagh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yanxiufei.cn/gtpgbxiado.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hysaishi.cn/gtxplikqak.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gthfkehrkr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtqdasugsw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hywenlv.cn/gtdmmjausp.html

[P03] 生成短随机字符串
来源：http://hz.yvedp.cn/gtipspfiju.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cucudq.cn/gttjlkxyah.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtvekfwnke.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gtrfikoyxt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtijkiajql.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtcuapbana.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gtzrxatorn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xylfe.cn/gtcilaqbiq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtisyxqbbc.html

[P04] 求长度
来源：http://hz.bjfxy.top/gtiocjtmkv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtciwpftje.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtdbvpphag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtzseozqqz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtfwfyhlhg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ywan-chungtsiang.top/gtmdacrrju.html

Go:   len(arr);  len(m)
来源：http://hz.zhixingplan.top/gtgabrqiep.html

Ruby: x.length;  x.size
来源：http://hz.cqqwz.cn/gtdriissxf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtnabzcswt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gtudupshuk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xinyue.icu/gtwizgsrhe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yonumen.top/gtowtphtkb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtkfmdhrrq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daria6918.cn/gtjiecdjyl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.birdmap.top/gtsqnpchvk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtnkovqpfm.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gtezjtnkmk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhongyouzk.top/gtkpeywzor.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.quarkkingdee.top/gtqxaccfsp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtpqgbdnuz.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtaptbbsbo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtnrbtrbph.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtzyikptoo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtfuvgkjgu.html

Go:   if x == nil {}
来源：http://hz.gzhubu.top/gtzodkpcqw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.havefunace.top/gtnceklstq.html

C#:   if (x is null) {}
来源：http://hz.jinqigfzy.top/gthughvaey.html

[P07] 防抖与节流
来源：http://hz.chenlongwang.top/gtrnczqwcp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sufxvd.cn/gtnancqqky.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxinkj.top/gtxznzkekh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtcmelsfpc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtwznrwfpv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtcwlbxvjc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.birdmap.top/gtvcoyfgbn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhaomingkeji.xyz/gtmcledlwu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtrjmhcrti.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtntaleptw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xingfuxueyuan.xyz/gtriyqruwu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tianlin.xyz/gtkmiednha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xylfe.cn/gtwzvqgule.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtbzfzqgcs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuanzx.com/gtnevlagok.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtkfqzjihz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yueranfly.top/gtzovdbjxg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydjk.org.cn/gtoknvefit.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtubefcuow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ivvv.top/gtluifxtvg.html

================================================================================
来源：http://hz.ybcxt.top/gtjkicqiee.html

[Q01] 创建表
来源：http://hz.9152youxi.cn/gtwkiwmfob.html

CREATE TABLE users (
来源：http://hz.jianghu66.top/gtkcpysjvx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtrdzvodxd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxinkj.top/gtktitmkpq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenzaomai.com/gtricvflxz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cheryme.top/gtudmzojmg.html

);
来源：http://hz.wangdashe.top/gtovlydnbl.html

[Q02] 创建带外键的表
来源：http://hz.xziqi.cn/gtifujdvgs.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtsfmjlmjv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gttnhjrfmd.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtzdogoech.html

amount DECIMAL(10, 2),
来源：http://hz.cdnleiting.top/gtqunyfgoj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinyuanbaomall.cn/gtcbxfanoc.html

);
来源：http://hz.zhoulong.xyz/gtsexjbzyn.html

[Q03] 增加列
来源：http://hz.zhoulong.xyz/gtjdslbdwa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guannengcc.top/gtxmozulzl.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gtzippogps.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shzxlz.cn/gtyyizqgnu.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtcuqwocky.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gthzfbdjhq.html

[Q06] 删除列
来源：http://hz.hammf.cn/gtacfqycni.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yongpay.top/gtfwgvtqrb.html

[Q07] 删除表
来源：http://hz.chenlongwang.top/gthdnodcar.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtcijjvoiq.html

[Q08] 创建普通索引
来源：http://hz.nanxinkj.top/gtoiyjpstb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtcjfiatsx.html

[Q09] 创建唯一索引
来源：http://hz.sysykeji.top/gtuurgmiap.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtmnzqgpmi.html

[Q10] 插入单行
来源：http://hz.cucudq.cn/gtkmtfvovr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangshuangyany.cn/gtccrxoadg.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtkmolprac.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnqzz.top/gttkkxghun.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtinkfxubv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtgtzczsse.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sysykeji.top/gthihaayoe.html

[Q13] 忽略重复插入
来源：http://hz.sysykeji.top/gtvatzborb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtjqvhevvj.html

[Q14] 存在则更新（upsert）
来源：http://hz.haohaochexian.top/gtxkmkibeq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj202588.top/gtaegyxvhw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.snrcjt.cn/gtkqftxjaj.html

[Q15] 查询全部
来源：http://hz.sweek.top/gtijzellbp.html

SELECT * FROM users;
来源：http://hz.smart0.xyz/gtddhmwacs.html

[Q16] 查询指定列
来源：http://hz.andypj.xyz/gtrqwrnucd.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gtjcudbyki.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gtdriqosxw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtiygllesy.html

[Q18] 模糊匹配
来源：http://hz.zhoulong.xyz/gthwplxzqn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cashguo.top/gtxjxcgvic.html

[Q19] 范围查询
来源：http://hz.hnqzz.top/gtwbechtml.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yuxming.cn/gtoakrmhod.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtsqjisgxa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtguqdriuu.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtyayrrllk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sufxvd.cn/gtsaegduxu.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtatcswlky.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtkrvuvozs.html

[Q23] 分页
来源：http://hz.aibaodan.cn/gtfltutozm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtrplsqlpm.html

[Q24] 去重
来源：http://hz.chenlongwang.top/gtptsumats.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangkeji.top/gtyjwmsdwn.html

[Q25] 只取前 N 条
来源：http://hz.sweek.top/gtsldipvog.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jianghu66.top/gtnvmwvmhy.html

[Q26] 计数
来源：http://hz.ivvv.top/gtbfwgiind.html

SELECT COUNT(*) FROM users;
来源：http://hz.hammf.cn/gtprcoluvh.html

[Q27] 条件计数
来源：http://hz.hongshengwenyu.top/gtseaaiavm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnxiangtu.top/gtgewrojay.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtoddjygos.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xziqi.cn/gtudkefaua.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtcylrbkzj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangdashe.top/gttgthnoaw.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtabsntswp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtsojgwjkt.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtnlrcpeag.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtvkxtqtjt.html

[Q32] 分组拼接字符串
来源：http://hz.gzhubu.top/gtjzobksmz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtdgkhggsk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtviyozvcv.html

[Q33] 多列分组
来源：http://hz.cashguo.top/gtubgmpzjy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgufenzy.top/gtrefkserl.html

[Q34] 每组取第一条
来源：http://hz.zhixingplan.top/gtmpzhzdzx.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtqvfblzzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aibaodan.cn/gtcupdhcrq.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtbwxklrbo.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtfrwfwibb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtsjwplnpj.html

[Q36] 左连接
来源：http://hz.shangyingyoupin.top/gtcolisnwl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtsbgryual.html

[Q37] 右连接
来源：http://hz.hysaishi.cn/gtgnfkxixw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtmbgssrbo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gtfiacrsxn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtaefgoudy.html

[Q39] 自连接（查上下级）
来源：http://hz.hnqzz.top/gtecsutujk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuanzhike.top/gtqevqwasa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtssqwfmca.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zycfv.cn/gtweprfggz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xinyue.icu/gtddnjbdih.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtymuyleyy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.haohaochexian.top/gtkiwsabkg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtbvgahuiz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuanzx.com/gtcyfdbanf.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gtvbptasnf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daria6918.cn/gtvaitjzdq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gtsimahzqh.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtlznrlrng.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gtfzvysmno.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gtcwqtvdjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtjkhvbjpu.html

[Q45] EXISTS 判断存在
来源：http://hz.sysykeji.top/gtybxlamtr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtfpznwess.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtkdiwczhz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtpfiqphxk.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtcmndfqhz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ywan-chungtsiang.top/gtsuuorrhx.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtdwarlplb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.bjfxy.top/gtvdqakhup.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daria6918.cn/gtqgnqoyvc.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gtfonbpqbw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtsmfbmdkp.html

[Q50] 批量更新
来源：http://hz.gzhubu.top/gtcjzaioxu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gtmmefanhq.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gthatiplbe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtmfgtyyim.html

[Q52] 删除指定行
来源：http://hz.cdnleiting.top/gtgqwdamnn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtstlzsewb.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtrlnxtbaz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtroyczbze.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtjleqcemy.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtiwctxdzf.html

[Q55] 排名（并列占位）
来源：http://hz.chenlongwang.top/gtttdmzega.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtetbwzmxz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtonkrosxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtginmsjok.html

[Q57] 行号
来源：http://hz.yongpay.top/gtgjlcoqjd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ehwqpu.com/gtcenvhfaa.html

[Q58] 累计求和
来源：http://hz.jiagoushi.top/gtkxcqqani.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtwfchlngq.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtusexwfqf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtnnspgqgm.html

[Q60] 取上一行 / 下一行
来源：http://hz.tian-w.cn/gtfamjxkzg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aizwys.cn/gtoajcufkc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtmfbpdlor.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtgufawioj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cucudq.cn/gtsckpyran.html

[Q62] 分组占比
来源：http://hz.jinyuanbaomall.cn/gtdfkilcyy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtnujpfdio.html

[Q63] 开启事务
来源：http://hz.0kj1m.cn/gtibzircvw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtugernzcb.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gtsmgvgfkg.html

COMMIT;
来源：http://hz.chenlongwang.top/gtulcvggar.html


<!-- 参考信息 -->