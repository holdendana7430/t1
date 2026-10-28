代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtvccqnthn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtmtmytvea.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtzsugmevz.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtjopaprca.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtptagleuu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtqfkouypq.html

C#:   // 手写递归
来源：http://hz.andypj.xyz/gtynoszkdo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxuanxn.top/gtdytxlpjs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.svipenyu.cn/gtxzjbusrw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtidfenmbp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtsvxmbube.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtzgqazxim.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtkbtxnjnz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sxryk.cn/gthxpohhhx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.redwolf501.top/gtjhzoxtul.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtpngpubjn.html

================================================================================
来源：http://hz.bjfxy.top/gtvbotians.html

O. 并发与异步
来源：http://hz.yongpay.top/gtxckigtdz.html

================================================================================
来源：http://hz.ydzc1.top/gtrjevxlys.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtotiovdqd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gthujogwix.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtdxaafwrr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtufmiyfcm.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtxvtcfrnt.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgufenzy.top/gtudsfqduf.html

Go:   go f()
来源：http://hz.dashuyun.cn/gtwojmuiub.html

Ruby: Thread.new { f }
来源：http://hz.shuidangran.top/gtkupzpvqe.html

C#:   Task.Run(() => F());
来源：http://hz.jianghu66.top/gtjempsdlz.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtbapvudnh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cdnleiting.top/gtcmpyxvnq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtyqxvwpax.html

JS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtsqdchjcg.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtsynnaftm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jianghu66.top/gtpeubbvlt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ybcxt.top/gtklhobeqb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gtlzdzsrim.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cdnleiting.top/gthxknfvsm.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtoizbubof.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtupyepcrv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gtkqrieayu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtejtozwnj.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtoqanedns.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtudwiurce.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shangyingyoupin.top/gtlhlshfvy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gtwljexcaf.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtmexaaggb.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gthwwdicde.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtjfhklprh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtuvcbfnzc.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtqnnrlqig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jiagoushi.top/gtrzmrkcla.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.0kj1m.cn/gtsswrenom.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtztgikjlx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhengqikj.top/gtiupkxjgi.html

C#:   async Task F() { await G(); }
来源：http://hz.kuanghao11.cn/gtqrcgpsfg.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtgbngxiqj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtenmatufy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhaomingkeji.xyz/gtujougaxv.html

JS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtyaycfocb.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtcayflpib.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtzlpslddq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtzuvtjuma.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtdlscdpnd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtpbrowndl.html

[O06] 使用进程池
来源：http://hz.hammf.cn/gtyaaomxjg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtzlacpnnm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtwozkfwcl.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtjprgiuus.html

TS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtotwudyec.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gttacxhxkw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jyoumei.cn/gtyhrvzznt.html

Ruby: // fork 块
来源：http://hz.cucudq.cn/gtvthrkyoi.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtyodfyknl.html

================================================================================
来源：http://hz.xinyue.icu/gtzacsvkge.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gtycjdlfvh.html

================================================================================
来源：http://hz.jyoumei.cn/gtzkpvtymn.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtibfaduwm.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtigbdjocx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtwubalhbx.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtmcbnsfmh.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtxwsnlcme.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtgeithbjm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aizwys.cn/gtveruanhp.html

Ruby: SecureRandom.uuid
来源：http://hz.zhoulong.xyz/gtsetkzden.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtcprgepkx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ehwqpu.com/gtnmxykafy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cheryme.top/gtnzkdvlal.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtdjuehgcp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtpqakohwn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhongyouzk.top/gtyrcliyni.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtuushclaj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.andypj.xyz/gtcdjtiauy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sweek.top/gtlcsjpdkm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gttdlzqefk.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtuslvcoqv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtegesbmig.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ehwqpu.com/gtnkkfpeni.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtjxmnjuvj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtyeovhhps.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cheryme.top/gtvqfcxufn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtrudzddmj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pycfn.com/gtxhbwzsxv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.haohaochexian.top/gtuphroucn.html

[P04] 求长度
来源：http://hz.havefunace.top/gtcuqxttjm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cashguo.top/gthglxgbfz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.0kj1m.cn/gtexcbmzvx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.iojbl.cn/gtzckyqayb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtaeviwqux.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gtrjnrjird.html

Go:   len(arr);  len(m)
来源：http://hz.dashuyun.cn/gtdswmftco.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gtsjubqskv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtuaqwdfgt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtanftxvuc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtgflwxomo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtnorfdadn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtflvkztjx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtczzagwdw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtymhtffhs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtfqugijtj.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gtgmltqgzj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gthfcdkhim.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigufen.top/gtpyxxeqmj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xziqi.cn/gtoqaqhzmi.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigfzy.top/gtlmgagbvb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtutpspsah.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtmmiadams.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtxkudpavx.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtvndzvtri.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtkgpbunte.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtjwkbciob.html

[P07] 防抖与节流
来源：http://hz.cdnleiting.top/gtphinzojd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhiwuduotai.top/gtqodeqkpf.html

PHP:  // 手写时间戳比较
来源：http://hz.hysaishi.cn/gtspigcale.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtizsfbwoc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtxfplpjlp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gtpxacfiyb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.feifeiyinyue.top/gtqmnwviey.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xingfuxueyuan.xyz/gtwqwwiisq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtnjpbkcmo.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtnhcvxlaz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnqzz.top/gtuadlpxmz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.svipenyu.cn/gtzggeyqrc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtkmeoplzq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yvedp.cn/gtzritmiud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.snrcjt.cn/gtuamjnmbz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xingfuxueyuan.xyz/gtwawoqdlg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhixingplan.top/gtaphnwlhy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtepnupoej.html

================================================================================
来源：http://hz.yj20258888.top/gtdachbgqo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aizwys.cn/gtxkaiibsf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gteqccrvwl.html

[Q01] 创建表
来源：http://hz.xingfuxueyuan.xyz/gtspirmszw.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtsivwibhq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtoobrlpxr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtfpnfflrr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.0kj1m.cn/gtiiplrrrz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gteprwqvnm.html

);
来源：http://hz.mhx1999.top/gtokkhqkhl.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtyrdqwapc.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtnftbcnly.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gttflgmgga.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gtxaoxfush.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gthjbkxfql.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtompwvove.html

);
来源：http://hz.ivvv.top/gtqzjydflc.html

[Q03] 增加列
来源：http://hz.yueranfly.top/gttuxzfpve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtvyhkdiem.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtbkwidjmn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ydzc1.top/gtjpqpigof.html

[Q05] 重命名列
来源：http://hz.zhoulong.xyz/gtryxwzdfl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtdadonpyt.html

[Q06] 删除列
来源：http://hz.jlsjyb.cn/gteosvmxlu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtakznvpdt.html

[Q07] 删除表
来源：http://hz.dashuyun.cn/gtkdsgbwlp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxuanxn.top/gtwsnoyozf.html

[Q08] 创建普通索引
来源：http://hz.sxryk.cn/gtgemxaqwj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ivvv.top/gtuzoqpoui.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtejzsqojf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtosvkqwmx.html

[Q10] 插入单行
来源：http://hz.shuidangran.top/gtsvlgxvdz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhiwuduotai.top/gtlkbrznhh.html

[Q11] 一次插入多行
来源：http://hz.pengpengdd.cyou/gtkzeyfbmc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dashuyun.cn/gtlychsgns.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtgtoyuqqn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gttliuxccb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gtribqcpah.html

[Q13] 忽略重复插入
来源：http://hz.sysykeji.top/gtwxxsmudm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtxjkmtpdf.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgfzy.top/gthemidibt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtvjunxdyd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jlsjyb.cn/gteivzpavd.html

[Q15] 查询全部
来源：http://hz.tanke756.top/gtjvlyinll.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtijcxjoqy.html

[Q16] 查询指定列
来源：http://hz.haohaochexian.top/gtdyifowhw.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gturxdxqhn.html

[Q17] 条件查询
来源：http://hz.birdmap.top/gtstzizfgs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtnysywfag.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtvwykhwvl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtcynqqsqv.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtxesycgne.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.birdmap.top/gtuwcrxrqc.html

[Q20] IN 列表
来源：http://hz.guowangkeji.top/gtunilxzew.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.52xcode.cn/gtkroiknyk.html

[Q21] 空值判断
来源：http://hz.nanxinkj.top/gtcpkrdxum.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shzxlz.cn/gtmrdczcmp.html

[Q22] 排序
来源：http://hz.cashguo.top/gtssqezkxf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtihiwngtg.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtytcxuhnp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xziqi.cn/gtfbufgsrp.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtbhzpaejq.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtlwhykbdx.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtlhrddckz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ywan-chungtsiang.top/gtxoacmxaw.html

[Q26] 计数
来源：http://hz.hongshengwenyu.top/gtlrxcrtyr.html

SELECT COUNT(*) FROM users;
来源：http://hz.xylfe.cn/gtakehvuoj.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtnskxqpwr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtxtzztpnj.html

[Q28] 求和与平均
来源：http://hz.cucudq.cn/gtypoulica.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtrogbbbia.html

[Q29] 最大最小值
来源：http://hz.ehwqpu.com/gtgrvunbrc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gtrhruwyro.html

[Q30] 分组统计
来源：http://hz.mhx1999.top/gtcwcxssxk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtsglxhtgj.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtntloycbp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gteujqvvui.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtnfrgkrbw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtwfsnzyap.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gtspdkmwqa.html

[Q33] 多列分组
来源：http://hz.ppjwa.cn/gtbjvosdxn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yongpay.top/gtyvuyxnki.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtemrqouon.html

SELECT * FROM (
来源：http://hz.ppjwa.cn/gtglhbmrkh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtboxbiwdg.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gtvvtrxstu.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtlvkolpzk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtafqaqgtv.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtgaewbzwb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtomktrfbm.html

[Q37] 右连接
来源：http://hz.birdmap.top/gtzvehjqal.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ybcxt.top/gtedhcdioq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtqfucxjmb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtbvffahvu.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtfggawjny.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aizwys.cn/gtbwqgzahv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtizavcozq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shuidangran.top/gtaxovtjmh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fzhhl.top/gtibpnkdqy.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtdxcqrgmm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gthmbfxtmb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangdashe.top/gtxjafjlit.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtivtozcsc.html

[Q42] 连接条件附加过滤
来源：http://hz.tian-w.cn/gtnlvgbidd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtijposcnn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtrgyglqyt.html

[Q43] 标量子查询
来源：http://hz.zdqjudy.top/gtyorksfcx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtqoovnxvp.html

[Q44] IN 子查询
来源：http://hz.cashguo.top/gtbqldbxmf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtzaohdxjc.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtlursliuw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtqgpnqmrl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.svipenyu.cn/gtzramcxsk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtuajdghfx.html

[Q47] 与平均值比较
来源：http://hz.dianchejie.cn/gtbrpwuupf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtnydbfmmn.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtkgtvxheh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gtenajpbxr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtkpmefwsn.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtwenbcbsc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtgaznajlg.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gtnxhzuwfo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.mhx1999.top/gtikqjhbit.html

[Q51] 用子查询更新
来源：http://hz.gaohongyu789.top/gtvcidclmy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtgwnnnbks.html

[Q52] 删除指定行
来源：http://hz.gzhubu.top/gtlzdrjbnb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgfzy.top/gtwzhqdewt.html

[Q53] 按条件删除
来源：http://hz.sweek.top/gtdjncxezi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtydamtjft.html

[Q54] 清空表
来源：http://hz.chenlongwang.top/gtlxzyygqk.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtmbakmeia.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtkagcjyxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtldzbxdvc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtyfmgnyvt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yangfankeji.com/gtanaebvkz.html

[Q57] 行号
来源：http://hz.0kj1m.cn/gtjqkwqjcb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtdtqaafns.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gttwieigwn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhengqikj.top/gtrwtzryry.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtnxatxblk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tianlin.xyz/gtiirpxfqv.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtxonsymzb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gtwfhmfuxy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cashguo.top/gtnklgjmxz.html

[Q61] 移动平均
来源：http://hz.shuidangran.top/gtuwnorory.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gtjvnrwdwi.html

[Q62] 分组占比
来源：http://hz.cucudq.cn/gtvlmgquyb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gteuqflfop.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtqdkubdbl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtcklyxicp.html

[Q64] 提交事务
来源：http://hz.zhaomingkeji.xyz/gtfgbvvvdc.html

COMMIT;
来源：http://hz.hfpthk.cn/gtqcrwydqf.html


<!-- 参考信息 -->