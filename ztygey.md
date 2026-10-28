代发 wailian999

Go:   // 手写递归
来源：http://hz.pycfn.com/gtkvjsnqkx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gtflkylada.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gtcqcxnsmf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtjzprikbk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenjidiqi.icu/gtlhmydwim.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtwvfhalra.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtmmuqzxjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtjqpjtjux.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtgsxlsogw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gturpluamz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cheryme.top/gtepehplcj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtofduhasa.html

================================================================================
来源：http://hz.yj20258888.top/gtznajeeyc.html

O. 并发与异步
来源：http://hz.sysykeji.top/gtcblnhbyg.html

================================================================================
来源：http://hz.cdnleiting.top/gtsqmhcagk.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtjknygajn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhongyouzk.top/gtbgpiyoze.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtdfhxqnhl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangshuangyany.cn/gtruzvbowz.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtrvhdpsww.html

Java: new Thread(() -> f()).start()
来源：http://hz.cqqwz.cn/gtvkzanhiy.html

Go:   go f()
来源：http://hz.jlsjyb.cn/gtgchohxqm.html

Ruby: Thread.new { f }
来源：http://hz.xingfuxueyuan.xyz/gtuqxlijtg.html

C#:   Task.Run(() => F());
来源：http://hz.hywenlv.cn/gtvsvqvsyh.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtgsmzbaoo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shzxlz.cn/gthmyjbqhr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtugrwiljl.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtlpebkxpy.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtloydlymw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtomwokbuw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gtchrhbvbj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gteovuiodu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuanzhike.top/gtyuqgwokq.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtexucrivd.html

Py:   with lock: shared += 1
来源：http://hz.meibo888.top/gtvvhclnrj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtvfbuqxdr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.svipenyu.cn/gtejnqejvm.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtiwywpynf.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gtztpsygbx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.feifeiyinyue.top/gtluvrhjlh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtwcjoviwj.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgufenzy.top/gtrsbrsovu.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gtxzrxnpxy.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtpzldrcni.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtvskyjopt.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtrpprttdb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtocsmucou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dashuyun.cn/gtzeclenig.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenlongwang.top/gtzrllzoyb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtfzsafhyc.html

C#:   async Task F() { await G(); }
来源：http://hz.yuanzhike.top/gtexnxjaay.html

[O05] 并发执行并等待全部完成
来源：http://hz.gotoacloud.top/gtrzzlylvu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zdqjudy.top/gtlvycqoqz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtnufzbugn.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtnubykzak.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtweymzodf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.iojbl.cn/gttejuuxzp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtftjkxheo.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtcbbsiwzs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtfcseanlr.html

[O06] 使用进程池
来源：http://hz.jlsjyb.cn/gtoqolegfw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.meibo888.top/gthgqcjfjr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtpyldnsns.html

JS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtxavnsgjj.html

TS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtciqigovf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtspvxykex.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtlqryebzw.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtrynukaqi.html

C#:   Parallel.For
来源：http://hz.hammf.cn/gtxzrvxmwm.html

================================================================================
来源：http://hz.chenzaomai.com/gtyxhjvxjz.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtdazufqqv.html

================================================================================
来源：http://hz.chenzaomai.com/gtblpwblxk.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gthwbcobpj.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangkeji.top/gtwlckdtca.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pycfn.com/gtodenjnau.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtxvthmlte.html

TS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtpktlvedt.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtyjbxwtac.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gzhubu.top/gtpeppjbyu.html

Ruby: SecureRandom.uuid
来源：http://hz.316326.xyz/gtrjfzcsvs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnxiangtu.top/gtpktrirug.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hfpthk.cn/gtmzsvkemy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cashguo.top/gtdywzpxlt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnxiangtu.top/gtkhuovltz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yvedp.cn/gtcnpqucdb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtzyafbwyf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtacagqnqd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.bjfxy.top/gtvvywmurk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtmgnkvybd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtxzsskyux.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtvvjmslem.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gtstzpqyhn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gtkyhnqbbk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtvqhllzbo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtwoyvfyif.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtwwxrbqsr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gtdmxgrjyj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtpjcdrbnq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtmgmbisqc.html

[P04] 求长度
来源：http://hz.wangdashe.top/gtblysgwrj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yonumen.top/gtgykswoeg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtqzbegwuf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gthjjzeypm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtfffjkevt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtsetghlou.html

Go:   len(arr);  len(m)
来源：http://hz.jianghu66.top/gtsnjbvhfb.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtezrkeyfi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtkstwjkjk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cashguo.top/gtxuzdnmwd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtkeprwatb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtydgqkiut.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sxryk.cn/gtjqzohexn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gthirawkdg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hfpthk.cn/gtoyphghzm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtwdllweoy.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtlqwtbicw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigfzy.top/gtjkfozbzc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ivvv.top/gtpxtnlogc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gaohongyu789.top/gtfyyvoptr.html

PHP:  if (empty($x)) {}
来源：http://hz.zhijiandao.cn/gtknvzihps.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gtafduadxk.html

TS:   if (x == null) {}
来源：http://hz.dianchejie.cn/gtyilnjjkl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtowjtqjxk.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtpqgikngd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ehwqpu.com/gtnjnisnky.html

C#:   if (x is null) {}
来源：http://hz.daxiang520.top/gtfdfmuofn.html

[P07] 防抖与节流
来源：http://hz.guannengcc.top/gtovrxulro.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtjeonjwpt.html

PHP:  // 手写时间戳比较
来源：http://hz.ydzc1.top/gtkocysoou.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtromdyrtb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtmnidwual.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtgslttvfq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtflwaskox.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtkumyrbyd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hammf.cn/gtepilzerv.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gtwyqijdjt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daria6918.cn/gtqycrfvpa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.0kj1m.cn/gtsnuqntqn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gtqguyemjd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtduamyadj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gthqvedvuq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtgrmhdoky.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtjquosqjo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtpznkgfik.html

================================================================================
来源：http://hz.iojbl.cn/gtdtewzjvy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ybcxt.top/gtkmnazfzc.html

================================================================================
来源：http://hz.cqqwz.cn/gtdqjxqnho.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtebkmwajy.html

CREATE TABLE users (
来源：http://hz.pycfn.com/gtkwqfylrc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtspgemsmm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuxming.cn/gtreloxjtz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cqqwz.cn/gtpcwzxnds.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dianchejie.cn/gturryllxe.html

);
来源：http://hz.zhengqikj.top/gtcbvpnhge.html

[Q02] 创建带外键的表
来源：http://hz.feifeiyinyue.top/gtlnfzpjis.html

CREATE TABLE orders (
来源：http://hz.wangshuangyany.cn/gtdfnecoax.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtdicvuvnk.html

user_id INT NOT NULL,
来源：http://hz.yj202588.top/gtfztojwas.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtenovwsyy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sweek.top/gtussusdpj.html

);
来源：http://hz.tian-w.cn/gthjnqrpfv.html

[Q03] 增加列
来源：http://hz.yvedp.cn/gtvocnjdyg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj202588.top/gtvfzvscko.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtxivgasab.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.52xcode.cn/gtjokleotb.html

[Q05] 重命名列
来源：http://hz.xylfe.cn/gtcotfmhtb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtcwiyapoi.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gthnuzitnx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigufen.top/gtruurvhfv.html

[Q07] 删除表
来源：http://hz.nwbrower.top/gtarpeqjrf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj202588.top/gtutkreleu.html

[Q08] 创建普通索引
来源：http://hz.yueranfly.top/gtualxelnf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtrrewwtth.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtpaceunoz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtbtpxvtsl.html

[Q10] 插入单行
来源：http://hz.gogol.net.cn/gtlebuseca.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cqqwz.cn/gtkqlikxcq.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtrdilpkgn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinyuanbaomall.cn/gtqupatnha.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gtyrrpnmtu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.havefunace.top/gtyqanfext.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tanke756.top/gtjpgcxven.html

[Q13] 忽略重复插入
来源：http://hz.gzhubu.top/gtxdypxdlh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuanzx.com/gtxerfjedz.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtsycwlqoj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtdihjfnui.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtrevfvrnr.html

[Q15] 查询全部
来源：http://hz.sxryk.cn/gtdwefkdef.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtzihyjeav.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gttudnausr.html

SELECT id, name FROM users;
来源：http://hz.sweek.top/gtombmbjvk.html

[Q17] 条件查询
来源：http://hz.hfpthk.cn/gtebpdlwfh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtzglvtliy.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gttbqetmla.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtiwneoiuv.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gthqihkseu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hywenlv.cn/gtrgubrogh.html

[Q20] IN 列表
来源：http://hz.shzxlz.cn/gtorkahogo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gtporhagan.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtnffzeihr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gtiegmbeem.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtnjncwxpv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtdyaxksev.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtxflheukh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gthnafjsbj.html

[Q24] 去重
来源：http://hz.sysykeji.top/gtxewwlefu.html

SELECT DISTINCT city FROM users;
来源：http://hz.vqdsnc.cn/gtjbezjqxl.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtgxlxxgrr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhiwuduotai.top/gtcjcepuot.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtiarmziyh.html

SELECT COUNT(*) FROM users;
来源：http://hz.cdnleiting.top/gtspzdwtad.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtxwxnmidm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gotoacloud.top/gtpapeebgz.html

[Q28] 求和与平均
来源：http://hz.guowangkeji.top/gthleuhqsp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtlrrllrjf.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtqshatpcg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnqzz.top/gtokclzbut.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gteyofqhlx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtwvhlamtz.html

[Q31] 分组后过滤
来源：http://hz.snrcjt.cn/gtycmbfbko.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxuanxn.top/gtuvalzucp.html

[Q32] 分组拼接字符串
来源：http://hz.bjfxy.top/gtmbzulatt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtkhucmtvq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtioxnaulx.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtkyxzuffh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtzsgybmzf.html

[Q34] 每组取第一条
来源：http://hz.cheryme.top/gtdwifnwjm.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtkyekafkc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tanke756.top/gtrgowksjk.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtpbxofaef.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtnjsowqam.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtdkijwdsn.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtjjwsmbhg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtbnjqjbge.html

[Q37] 右连接
来源：http://hz.zhaomingkeji.xyz/gtdkhzllee.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtpzegghdh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gtplvyzzoq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtnniylfyc.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gttfshyhgq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sweek.top/gtwnocjiew.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtoeugfkls.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jyoumei.cn/gtstvgtcff.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gthjzlownu.html

[Q41] 多表连接
来源：http://hz.zhengqikj.top/gtyefcjiih.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xingfuxueyuan.xyz/gtrlbwvnop.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zdqjudy.top/gtwgzdpesk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gteoickydx.html

[Q42] 连接条件附加过滤
来源：http://hz.andypj.xyz/gtrdnkwjgh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtsjykwfkl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gtzkrbupyh.html

[Q43] 标量子查询
来源：http://hz.quarkkingdee.top/gtzxzjigvb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtecsnjppt.html

[Q44] IN 子查询
来源：http://hz.ydzc1.top/gtsimwuxna.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangdashe.top/gttjkutoaq.html

[Q45] EXISTS 判断存在
来源：http://hz.sxryk.cn/gtuorroaxv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtdbvlcroc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gtbyuloecj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtpvecgksv.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtxmmoeymo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daria6918.cn/gtbxsmbzts.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gtjtqwxnmo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gttegygskl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtfbrsxfmo.html

[Q49] 更新单行
来源：http://hz.hongshengwenyu.top/gttgmnxbye.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gttrsyyonc.html

[Q50] 批量更新
来源：http://hz.cashguo.top/gtixahmiwl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shangyingyoupin.top/gtueyomxqq.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtgqsqemae.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtyaajpcmu.html

[Q52] 删除指定行
来源：http://hz.shzxlz.cn/gtzmajoxwn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.c1oappe.top/gtmnklkgcr.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtokzrgtlf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sweek.top/gtcqraxnri.html

[Q54] 清空表
来源：http://hz.guannengcc.top/gtfhipfkwv.html

TRUNCATE TABLE logs;
来源：http://hz.jlsjyb.cn/gtzopmefpm.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gthecbyzeh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gtnljhepfo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tian-w.cn/gtfjfavnpr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.smart0.xyz/gtujhdsicy.html

[Q57] 行号
来源：http://hz.haohaochexian.top/gtdggbvlqa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtcydsitdo.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtixhbnupe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tian-w.cn/gtntpadkxs.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtxgexdmgj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ehwqpu.com/gtymfwvxvl.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtsalizhpm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cheryme.top/gtvcxvxfzb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtymxfrbrx.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtgihdjhua.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtlejzkkhz.html

[Q62] 分组占比
来源：http://hz.yonumen.top/gtxxqtifms.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtczragrsw.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtubiqpwps.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jlsjyb.cn/gtliumtnqg.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtchwfnpfa.html

COMMIT;
来源：http://hz.yonumen.top/gtyldhwdvd.html

[Q65] 回滚事务
来源：http://hz.shangyingyoupin.top/gtkslusipl.html

ROLLBACK;
来源：http://hz.redwolf501.top/gtkjreomcm.html

[Q66] 行锁查询
来源：http://hz.hnxiangtu.top/gtromfzozr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtaqxfjles.html


<!-- 参考信息 -->