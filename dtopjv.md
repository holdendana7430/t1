代发 wailian999

================================================================================
来源：http://hz.smart0.xyz/gteaityppe.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtpnfeyqrm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtcpkngoii.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtaymnfihf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigufen.top/gtqqyibslm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuxming.cn/gtybtetsjb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gotoacloud.top/gticqqbxkh.html

TS:   // 同 JS
来源：http://hz.nanxuanxn.top/gtohlzotuf.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtnsnqxpjr.html

Go:   go f()
来源：http://hz.pycfn.com/gtwfbqqwee.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtdnmbmtbz.html

C#:   Task.Run(() => F());
来源：http://hz.zdqjudy.top/gtenavuwrd.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtuokgfpum.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtbukjibzn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtqrqqyfqi.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtwwbwmpma.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtntnpxook.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tanke756.top/gtxxcobzfx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydzc1.top/gtdurnclvv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj202588.top/gtfbchlmlq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtqqjuakoy.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtofkzwiku.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtbwhihole.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenjidiqi.icu/gttkuurkgm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtgoogihfp.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtmfllrqno.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtmsurykzo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yueranfly.top/gtwnlbugat.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtgcialfhf.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtbgstspts.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtzaxljzlu.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtqqccqsmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtoqnqtxjv.html

JS:   async function f() { await g(); }
来源：http://hz.yuxming.cn/gtqrqnftmm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtguzykdvj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtcpxzfdtm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtqkwrwfip.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cheryme.top/gtmptwoyxm.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtgkjvyddy.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtmetfydsz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtvxddpggv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aibaodan.cn/gtldjqzabu.html

JS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtrggdygrh.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtuseyyfvj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtdmocytmv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenlongwang.top/gtjrfzaakk.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtbuhbeqfd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtrvgrtehh.html

[O06] 使用进程池
来源：http://hz.bjfxy.top/gtnrdnkize.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhengqikj.top/gtwcbqygvb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuanzhike.top/gtwdwdgcxl.html

JS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gtvhbcpqtc.html

TS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtptbeqdoa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtrxjpwyvz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.52xcode.cn/gtuqhagood.html

Ruby: // fork 块
来源：http://hz.zhongyouzk.top/gtgfoyiwkh.html

C#:   Parallel.For
来源：http://hz.52xcode.cn/gtxdewfdvc.html

================================================================================
来源：http://hz.cheryme.top/gtkzfvhtmy.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtetfubmgf.html

================================================================================
来源：http://hz.xylfe.cn/gtenxlschm.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gtliputqdt.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gthruozxow.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtybtwzowy.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtwqjrqsqc.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gthtnzgplk.html

Java: UUID.randomUUID().toString()
来源：http://hz.hongshengwenyu.top/gtsahcefyb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gtftouyjnw.html

Ruby: SecureRandom.uuid
来源：http://hz.hnqzz.top/gtognurmrj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tian-w.cn/gtrxuarzni.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtbygdlwxx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtwftgcfcu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtjajnpjdt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuetiantiany.cn/gtzeqixaec.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtnxcqkeip.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.mhx1999.top/gtxvwqsktc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gtphsrabjm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jianghu66.top/gtashbiwlx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zycfv.cn/gtarxelpoq.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtormjzafm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtpaahmtjl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtjiuxzbad.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pengpengdd.cyou/gtafwljqqk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtuqwdahfx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gtbieassvx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtbfqjepom.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtzsbnelnt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shuidangran.top/gtmclwgqmt.html

[P04] 求长度
来源：http://hz.hywenlv.cn/gtyesoqbbe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258.top/gtfvpkreeu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtvsnlczqe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtcmiojsvn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gttbbbttzj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258888.top/gtfdfwepyj.html

Go:   len(arr);  len(m)
来源：http://hz.sysykeji.top/gtofdkqwhp.html

Ruby: x.length;  x.size
来源：http://hz.chenjidiqi.icu/gtkdyrjsqy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinghuilouyu.cn/gtlkpyewzd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jlsjyb.cn/gtaajqtogf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtfefgrfcc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hysaishi.cn/gtlfzivknw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gttcvxgkvv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtnlwabrmq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gtongjyryb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aibaodan.cn/gtetnthsuu.html

Ruby: a == b
来源：http://hz.jinqigfzy.top/gtmbyocaaa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.quarkkingdee.top/gtnjjbwqxp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xinyue.icu/gtielrtvfw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinyuanbaomall.cn/gtvsyekuka.html

PHP:  if (empty($x)) {}
来源：http://hz.meibo888.top/gtlanymcsz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtqesntqsw.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtzwhhgmbe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtvwuasoct.html

Go:   if x == nil {}
来源：http://hz.xziqi.cn/gtzsanljik.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nwbrower.top/gtriymtvyj.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtvuzqusoe.html

[P07] 防抖与节流
来源：http://hz.aizwys.cn/gtcrfldgqt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtqjkdfjuf.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtmefnjywp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtgyxtjchu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtlxcavtgo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtvvcawwtn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gttakzvvfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtlatggyat.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yueranfly.top/gtfqukcsnr.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtwmvunjjw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tian-w.cn/gtimwjpptl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guowangkeji.top/gtqnjnpfyi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258888.top/gtlgydvukx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yangfankeji.com/gtzaiojeog.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cashguo.top/gtdltjfzaa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shangyingyoupin.top/gtugnrykov.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shangyingyoupin.top/gtggecsyav.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yonumen.top/gtpczhmzsx.html

================================================================================
来源：http://hz.cashguo.top/gtnkwyrjbx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtcfkrupzg.html

================================================================================
来源：http://hz.jyoumei.cn/gtszzgwzjh.html

[Q01] 创建表
来源：http://hz.xuanzx.com/gtjviqsqla.html

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtvvatquhj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtbbirgnnu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgfzy.top/gtjtjkjwbz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtsmnjatnt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jlsjyb.cn/gtwjkimbtd.html

);
来源：http://hz.jyoumei.cn/gtpiodxpvl.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtrorhgcuf.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtkhoakhvb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtjxoaejhl.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtmwxhjmwm.html

amount DECIMAL(10, 2),
来源：http://hz.xingfuxueyuan.xyz/gtcfhywnib.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shzxlz.cn/gtvoerwwgr.html

);
来源：http://hz.gzhubu.top/gtzbkquugx.html

[Q03] 增加列
来源：http://hz.hongshengwenyu.top/gthjcxfdto.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtkmzpggqn.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtnxrlhsdb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hywenlv.cn/gtpmliisot.html

[Q05] 重命名列
来源：http://hz.xuanzx.com/gtruoqathk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tanke756.top/gtblycevoz.html

[Q06] 删除列
来源：http://hz.aibaodan.cn/gteuwkskxq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aizwys.cn/gtpljxjrmy.html

[Q07] 删除表
来源：http://hz.yanxiufei.cn/gtzqtrqlvj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinghuilouyu.cn/gtyfugqogf.html

[Q08] 创建普通索引
来源：http://hz.yongpay.top/gtuxqjudda.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sysykeji.top/gtpfjfznai.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtreovqhyf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtrtbkeoof.html

[Q10] 插入单行
来源：http://hz.jqgfzy.top/gtzvrmihps.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtrlsdnwwj.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtjywnbjph.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtzmknytmc.html

[Q12] 插入后取自增 ID
来源：http://hz.cqqwz.cn/gtrhbyejra.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gteofuornm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhengqikj.top/gtltwtfcqp.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtyxkgsuio.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gthdpzptqp.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtwkqhwyxf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtxtpkzpmb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.pengpengdd.cyou/gtbcorpcty.html

[Q15] 查询全部
来源：http://hz.guannengcc.top/gtihujifys.html

SELECT * FROM users;
来源：http://hz.gotoacloud.top/gthxolhbcx.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtjianamkw.html

SELECT id, name FROM users;
来源：http://hz.guowangkeji.top/gthuazmqks.html

[Q17] 条件查询
来源：http://hz.ehwqpu.com/gtuytqchsm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hfpthk.cn/gtypqajcfc.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtdhwukhnw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gtywpbkeis.html

[Q19] 范围查询
来源：http://hz.feifeiyinyue.top/gtaxvivlty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gttayancfw.html

[Q20] IN 列表
来源：http://hz.9152youxi.cn/gtaofiqwvh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sweek.top/gtfeidfezp.html

[Q21] 空值判断
来源：http://hz.gotoacloud.top/gtfzzbwibs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtbhqizawz.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtosglelnu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cqqwz.cn/gtyqynflcs.html

[Q23] 分页
来源：http://hz.yonumen.top/gtshfhfeky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cdnleiting.top/gtzfenunuq.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtkxytmtyo.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtmdtukblq.html

[Q25] 只取前 N 条
来源：http://hz.cashguo.top/gtqksupkmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtuplvvzso.html

[Q26] 计数
来源：http://hz.yangfankeji.com/gtfxdapvnp.html

SELECT COUNT(*) FROM users;
来源：http://hz.nwbrower.top/gtalznjmzm.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gtiuhkbtux.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtshkdoyqz.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gtdqvxvpio.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtjhnqrfvo.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtavozkvfk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtexdtnctj.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gtyqwwbhdn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gthsbunrsi.html

[Q31] 分组后过滤
来源：http://hz.feifeiyinyue.top/gtqitnaeez.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtdwifivaa.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtnmsukstt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtwjlkjtew.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtawwiuigr.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gtcryjjqmx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhengqikj.top/gtrctlpoeq.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtuwejfvwu.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtkpliiwul.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtommbxgdp.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtjjbdsjaj.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gtldefbkoi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtqkqrxqbt.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gtquubmacv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtlgievotn.html

[Q37] 右连接
来源：http://hz.yonumen.top/gtdxpprqmt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.52xcode.cn/gtrobbdjau.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtegrwzsvm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtwzqhnesh.html

[Q39] 自连接（查上下级）
来源：http://hz.hnqzz.top/gtrqidwknz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gthlkftcdc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gtgdwisohw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtbxfvuzzl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuetiantiany.cn/gtavoknltw.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtkauzfwto.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenzaomai.com/gttemyoqlc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gtkmkqqbpf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtfyxcxcyk.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gtvgkvovmm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gthymhyoio.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtmqerqequ.html

[Q43] 标量子查询
来源：http://hz.zhongyouzk.top/gtnesjcnwf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.feifeiyinyue.top/gtmfalxvrt.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gtzrkfqylj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.0kj1m.cn/gtosqpkdws.html

[Q45] EXISTS 判断存在
来源：http://hz.zhoulong.xyz/gtbvbvbnrt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtcxcebwcv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hysaishi.cn/gtpvvffhvr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtqukcwwyg.html

[Q47] 与平均值比较
来源：http://hz.yj20258888.top/gtwpfjugfp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dashuyun.cn/gtetjxwzlh.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtrtrsmwpi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangtech.top/gtdcyljidh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtjxrneuqb.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtxtmnkvbw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.birdmap.top/gtpulicgww.html

[Q50] 批量更新
来源：http://hz.quarkkingdee.top/gtogyxnbfl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sxryk.cn/gthwypzftb.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtvkwmpnsc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gotoacloud.top/gttesspqxp.html

[Q52] 删除指定行
来源：http://hz.wangdashe.top/gtpfhnyinv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtxkcnhrit.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtbjnidsqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gtzunletah.html

[Q54] 清空表
来源：http://hz.jiagoushi.top/gtfwkafsft.html

TRUNCATE TABLE logs;
来源：http://hz.sxryk.cn/gtxqpufshm.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gttjzvwwfy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gtzodqxmhy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shuidangran.top/gtumuhyexj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gthvmbbxvx.html

[Q57] 行号
来源：http://hz.quarkkingdee.top/gtwfvajoag.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.feifeiyinyue.top/gtoyjdirjm.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtrnwczwka.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtwmtdaddr.html

[Q59] 分组内累计
来源：http://hz.haohaochexian.top/gtqebexucx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yvedp.cn/gtraiswkdc.html

[Q60] 取上一行 / 下一行
来源：http://hz.sweek.top/gtnukwaokz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guowangkeji.top/gtdnvksopf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtmydajhek.html

[Q61] 移动平均
来源：http://hz.quarkkingdee.top/gtgznbgtxv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtghudjrje.html

[Q62] 分组占比
来源：http://hz.yj20258.top/gtfrxbtxnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtmcmpkrca.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtaznkdwlf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.haohaochexian.top/gtiazqjycu.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtgldupiva.html

COMMIT;
来源：http://hz.hnqzz.top/gtrqvmdztr.html

[Q65] 回滚事务
来源：http://hz.nanxuanxn.top/gtdmtjqbpg.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtyjqpfrkq.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gtxynpetra.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtkfufyeli.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gthricdmnu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtrjinyrkw.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtxgvnuqvy.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gtpchqxbmo.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtyqsdufui.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtsrlntuth.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sysykeji.top/gtegxmslfv.html

[Q70] 更新统计信息
来源：http://hz.gzhubu.top/gtofngcyxk.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtuwvgjczi.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gtmbuguneo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtzcitmmpz.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtbipjautg.html


<!-- 参考信息 -->