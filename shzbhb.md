代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtbmpaepzm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gtudneeqvj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gzhubu.top/gtpfrcdvzh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtjiggfjje.html

================================================================================
来源：http://hz.zdqjudy.top/gtnfvfwvpw.html

O. 并发与异步
来源：http://hz.gzhubu.top/gttwkjsktm.html

================================================================================
来源：http://hz.nwbrower.top/gtzifwogjc.html

[O01] 启动一个线程
来源：http://hz.quarkkingdee.top/gtwfhzqbaw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtwqmgeive.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtjvsppbkq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gtexcuzffx.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtnudmijmq.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtxyifskds.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtvpnuhuxs.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gtgmegqjdx.html

C#:   Task.Run(() => F());
来源：http://hz.xuanzx.com/gtxoimxagg.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtlorrlojy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtxzdffwph.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtmupngjwv.html

JS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtccyudvmn.html

TS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtsdhpfmbe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.birdmap.top/gtgbixkbbz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.havefunace.top/gthjugnaom.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.c1oappe.top/gtrpwzkhxm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258888.top/gtueyqvokx.html

[O03] 加锁保护共享数据
来源：http://hz.xylfe.cn/gtdfqxerxq.html

Py:   with lock: shared += 1
来源：http://hz.jyoumei.cn/gtcauwwotd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtketjdnvr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtiktzeagr.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtfkgpcxvw.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuetiantiany.cn/gtrtzegqgw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pengpengdd.cyou/gtjkyaflye.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.meibo888.top/gtczzkxuon.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtlkqgyguo.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gthfxgxhsw.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtejomclzf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pengpengdd.cyou/gtdvlsmldn.html

JS:   async function f() { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gtnclfgsap.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtydlnxzcq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gthfqpbufn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxinkj.top/gtmttkczox.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtstzemzuf.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtcyzohxsl.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigfzy.top/gtduraoust.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtlxbffhvn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gtqmeapnvb.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtkbeucnwk.html

TS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtvcqspoej.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangdashe.top/gtfzpcufoa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jyoumei.cn/gtlltsnmgs.html

Ruby: threads.map(&:join)
来源：http://hz.yj202588.top/gtoojjzqpb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtfpzsxovd.html

[O06] 使用进程池
来源：http://hz.shzxlz.cn/gtqajdiizg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhaomingkeji.xyz/gtfwgealpm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtxrddfipq.html

JS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtqequjkyn.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtimrlfhio.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dashuyun.cn/gtwmdsochn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydjk.org.cn/gtfwovflrq.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtgfhfempi.html

C#:   Parallel.For
来源：http://hz.feifeiyinyue.top/gtxemrwzrc.html

================================================================================
来源：http://hz.shzxlz.cn/gtdrknudxz.html

P. 常用工具函数
来源：http://hz.hnqzz.top/gthspubbyl.html

================================================================================
来源：http://hz.52xcode.cn/gtpwhenlug.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtzmscdaqs.html

Py:   str(uuid.uuid4())
来源：http://hz.bjfxy.top/gtaudkhhom.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gteflfkytu.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gthlguplkg.html

TS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtogigpmyk.html

Java: UUID.randomUUID().toString()
来源：http://hz.smart0.xyz/gtycihklcn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gthrpamzxk.html

Ruby: SecureRandom.uuid
来源：http://hz.yueranfly.top/gtunrqykly.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.snrcjt.cn/gtjutsgaxy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtovpylsez.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cashguo.top/gtjkfmcpzo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnqzz.top/gteokykdnl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gteezpcikz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtqxwumdqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtxjfmykae.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gtqfgsqsrx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgfzy.top/gtwggvvpsj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtjyyjcuid.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtvdzudmie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gteesjsoou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtmisosqyk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtrqxkcxzm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtibknhzqq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenjidiqi.icu/gtmtpntwms.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtazalhpus.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.vqdsnc.cn/gtdesjdxrs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtmeiqiliy.html

[P04] 求长度
来源：http://hz.cqqwz.cn/gtyqiqmupb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtpwzcntxh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtgccxpzmr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gttahykllw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gterwzlpfc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhiwuduotai.top/gtwiozfxwe.html

Go:   len(arr);  len(m)
来源：http://hz.yongpay.top/gthrvnoopq.html

Ruby: x.length;  x.size
来源：http://hz.cashguo.top/gtajjvsbrw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cashguo.top/gtccrhnrni.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ehwqpu.com/gtzgtqlzmo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtzkfmibec.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tianlin.xyz/gtflfgjgbg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtqesynphl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gthtbpdzlq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtqndqcoej.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtoylvaujo.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtbuecgdoq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtozpxmvxl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtafugmhil.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.52xcode.cn/gtveivwoym.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtnoqgfexc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangtech.top/gtsfhjibck.html

TS:   if (x == null) {}
来源：http://hz.vqdsnc.cn/gtmsdaheya.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtxdtldlgj.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtipllxnhp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cashguo.top/gtzpcpyhnz.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gttscwfpor.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangtech.top/gtukqytais.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guannengcc.top/gtxkafkegu.html

PHP:  // 手写时间戳比较
来源：http://hz.zdqjudy.top/gtmliocltb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtabzdpeqy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gthyxxiaoz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gturyvphav.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gaohongyu789.top/gtbtlhgcvk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuanzx.com/gtvbugcaoo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtzlfzzanr.html

[P08] 处理浮点精度问题
来源：http://hz.jqgfzy.top/gtporstsgk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tianlin.xyz/gtsdevfxzv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinghuilouyu.cn/gtptdxkghc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuxming.cn/gtrykhosim.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtwlmwdfhl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtivexqvxz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtzadlhnvn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtcgppbntq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jiagoushi.top/gtnmgztqgi.html

================================================================================
来源：http://hz.ivvv.top/gtebyvxydt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gtdhojyidd.html

================================================================================
来源：http://hz.gzhubu.top/gtsynjplse.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gtgbnhitkr.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtfiosokcp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gthsecruvv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtuenkijgu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuanzhike.top/gtpayyrlwc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.feifeiyinyue.top/gththsuebp.html

);
来源：http://hz.tanke756.top/gtzklcbhdz.html

[Q02] 创建带外键的表
来源：http://hz.gaohongyu789.top/gtludpkiqo.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtqeuudnjx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtoajdatms.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtfveaubsr.html

amount DECIMAL(10, 2),
来源：http://hz.kuanghao11.cn/gtbtqcvjwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gtqzvgtwbi.html

);
来源：http://hz.zycfv.cn/gtzhoisjzo.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtbozzktza.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtcemblvgx.html

[Q04] 修改列类型
来源：http://hz.yvedp.cn/gtmlcqweot.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtcssqnalz.html

[Q05] 重命名列
来源：http://hz.gogol.net.cn/gtilolrzsp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yonumen.top/gtqsawqmou.html

[Q06] 删除列
来源：http://hz.hfpthk.cn/gtgfukgoev.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtnebjndfw.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtwldtkoga.html

DROP TABLE IF EXISTS orders;
来源：http://hz.0kj1m.cn/gtkwbmnoxx.html

[Q08] 创建普通索引
来源：http://hz.hysaishi.cn/gtlphylxrq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtwbvjbvlm.html

[Q09] 创建唯一索引
来源：http://hz.havefunace.top/gtszzzctdn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtlaheoxoo.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtehebrhxr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydzc1.top/gtsnsxrbvy.html

[Q11] 一次插入多行
来源：http://hz.ywan-chungtsiang.top/gtefhgnidq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtiofwgqik.html

[Q12] 插入后取自增 ID
来源：http://hz.gogol.net.cn/gtyjzfnyom.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xylfe.cn/gttmolstha.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtcirejytx.html

[Q13] 忽略重复插入
来源：http://hz.gotoacloud.top/gtngfzvgdn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gtvihlmexu.html

[Q14] 存在则更新（upsert）
来源：http://hz.tanke756.top/gtdoiuhjqz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gtmgdtqiit.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtifihcjeu.html

[Q15] 查询全部
来源：http://hz.gotoacloud.top/gtgqyxvjsj.html

SELECT * FROM users;
来源：http://hz.xinyue.icu/gteqcvihtl.html

[Q16] 查询指定列
来源：http://hz.yj20258.top/gtkjvjbjtr.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtutbnvnpu.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gtwcspjaxw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtkxyzfofx.html

[Q18] 模糊匹配
来源：http://hz.sufxvd.cn/gtlgymyfxf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuetiantiany.cn/gtxzgnrltq.html

[Q19] 范围查询
来源：http://hz.cqqwz.cn/gtnxywhmhu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xylfe.cn/gtrxhgqmfl.html

[Q20] IN 列表
来源：http://hz.ydzc1.top/gtduawqioh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtpsmjakuq.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gtivqabitk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtolkmpwvb.html

[Q22] 排序
来源：http://hz.birdmap.top/gtznnjvynj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gzhubu.top/gtegnxyszn.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gtphtduwck.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gotoacloud.top/gtyseltpuf.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtwnlagghk.html

SELECT DISTINCT city FROM users;
来源：http://hz.gaohongyu789.top/gtqenwdxzw.html

[Q25] 只取前 N 条
来源：http://hz.jinqigfzy.top/gthtzmhngo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtroidhexg.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtkynaxozt.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtnambqseu.html

[Q27] 条件计数
来源：http://hz.jinqigfzy.top/gtthzdzlof.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnqzz.top/gtembozzlc.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtqpymbloj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtepiijpka.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gtgpwerchb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gtssevgvit.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtdptsxdzx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtqwvbzenz.html

[Q31] 分组后过滤
来源：http://hz.ivvv.top/gtwwxsqayg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtqsnzllka.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtuosmlqqs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gttlfhroyf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtntfbqslg.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gtkpqzweya.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuanzhike.top/gthdwrhnrc.html

[Q34] 每组取第一条
来源：http://hz.quarkkingdee.top/gtfjhfyfki.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtjfabllwc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtbzezipbe.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangtech.top/gtfybbgcyo.html

[Q35] 内连接
来源：http://hz.jinghuilouyu.cn/gtbmdyjpfo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtjmozfixl.html

[Q36] 左连接
来源：http://hz.meibo888.top/gtklgcjtwp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtcyzjehyr.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtmtblyahj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gtdjiontvj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gttswbagcp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tian-w.cn/gtkmcyzfqw.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtqdnywuci.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xziqi.cn/gtgewopbju.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.smart0.xyz/gtfcmdydqi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnxiangtu.top/gttlnghwcv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtyxoewety.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtbggfpzjb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtervwkiig.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinghuilouyu.cn/gtxxncqdzd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtkhgxvizg.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtzvdflxbp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtcqzlnmpe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xinyue.icu/gtfedwdugu.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtmaehklxr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gtdqviqipg.html

[Q44] IN 子查询
来源：http://hz.52xcode.cn/gtlsfwqhyo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtwwkvguuh.html

[Q45] EXISTS 判断存在
来源：http://hz.gzhubu.top/gtvfqodtsg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gthypwwvpp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sweek.top/gtruvombab.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtljxkkqmy.html

[Q47] 与平均值比较
来源：http://hz.yonumen.top/gtvjehpocu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtnwybxeat.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtfijxdwrb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guowangkeji.top/gtsbqdfxmp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtjvsgmiwc.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtxvdykkst.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtdefzyrcg.html

[Q50] 批量更新
来源：http://hz.52xcode.cn/gttntrtlol.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtsgieyylx.html

[Q51] 用子查询更新
来源：http://hz.zhijiandao.cn/gtypnvzcwj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.bjfxy.top/gtbsvgjplu.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtmtiejzqt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtjjhdewqu.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtrvylicgy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zdqjudy.top/gtaurgfxzd.html

[Q54] 清空表
来源：http://hz.316326.xyz/gtnpmyarzn.html

TRUNCATE TABLE logs;
来源：http://hz.yuxming.cn/gtfxcguoem.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gttoobeywx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenjidiqi.icu/gtrerbtfva.html

[Q56] 密集排名（并列不占位）
来源：http://hz.c1oappe.top/gthavhnhvx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhongyouzk.top/gtsqoxsqhi.html

[Q57] 行号
来源：http://hz.guannengcc.top/gtftzuzqjf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jlsjyb.cn/gtcpmprvpe.html

[Q58] 累计求和
来源：http://hz.cucudq.cn/gtgzistafe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtpqyollby.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gtkczbqvjg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtlzqmsuje.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinghuilouyu.cn/gtydmtqzus.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtytzyhkri.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtxbqdrtpf.html

[Q61] 移动平均
来源：http://hz.hongshengwenyu.top/gtxvvarfye.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtxbltezrc.html

[Q62] 分组占比
来源：http://hz.316326.xyz/gtdcxhvbga.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtvsxacusr.html

[Q63] 开启事务
来源：http://hz.ybcxt.top/gtzzwuwook.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtxptjmptk.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtpxunbmdy.html

COMMIT;
来源：http://hz.xziqi.cn/gtrzzzeeoq.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtcckftfbm.html

ROLLBACK;
来源：http://hz.wangshuangyany.cn/gtcokfumie.html

[Q66] 行锁查询
来源：http://hz.xziqi.cn/gtugmzpebh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shangyingyoupin.top/gtdcoczbju.html

[Q67] 设置隔离级别
来源：http://hz.jinyuanbaomall.cn/gtmmlpusbr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gzhubu.top/gtttattmcy.html

[Q68] 保存点
来源：http://hz.gaohongyu789.top/gtssvjjvsg.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtvwfydddu.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtkmwwyybn.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtnfoqhgmc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dianchejie.cn/gtglrvroyw.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtgxabvjch.html


<!-- 参考信息 -->