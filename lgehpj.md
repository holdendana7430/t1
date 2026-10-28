代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtsyxyacrn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtefvpgdyj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtnexmcsfu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtoteegwct.html

================================================================================
来源：http://hz.aizwys.cn/gtvpmldjkb.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtvdsprqke.html

================================================================================
来源：http://hz.zdqjudy.top/gtyqrccyds.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gthpduqavr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydjk.org.cn/gtavgkgsqi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtjmhjefum.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ppjwa.cn/gtyuwphwcv.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtucxxfznh.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtusaktrhy.html

Go:   go f()
来源：http://hz.xuanzx.com/gtqvxfpyxd.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtqcyoybhi.html

C#:   Task.Run(() => F());
来源：http://hz.316326.xyz/gtdpqnscgn.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gthicybiey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gtqxdqcdrx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtrqozwjgw.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtvklgqdpo.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtrheziiif.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tanke756.top/gtmmjqtlfj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cheryme.top/gtmgldkmxn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cheryme.top/gtfzyisnud.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hysaishi.cn/gtcbmdnlhm.html

[O03] 加锁保护共享数据
来源：http://hz.andypj.xyz/gtlwprpwzz.html

Py:   with lock: shared += 1
来源：http://hz.pycfn.com/gtaqcemvgu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtduczkwsn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtlectiahj.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtidtssbyz.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtorxlivpw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sysykeji.top/gtpvxuymol.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtknyjzdly.html

C#:   lock (gate) { shared++; }
来源：http://hz.c1oappe.top/gtbbkvwvaj.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtgiifmbtl.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtgcwrfhmo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gtgxcdurrw.html

JS:   async function f() { await g(); }
来源：http://hz.xuetiantiany.cn/gtfwjmxtau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenzaomai.com/gtkkmvelqz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.haohaochexian.top/gttslctfsk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtkxspwcis.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gtzulqriye.html

C#:   async Task F() { await G(); }
来源：http://hz.316326.xyz/gttiiolznc.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgufenzy.top/gtondewnls.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtgymzqhuw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangdashe.top/gtkzrqrbgh.html

JS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtyqlkweos.html

TS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtgwvorxyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuanzhike.top/gtvqgnczjt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tian-w.cn/gtminvscsu.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtgbxsgzay.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhaomingkeji.xyz/gtsmutaqfn.html

[O06] 使用进程池
来源：http://hz.mhx1999.top/gtsthnbpta.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtupqfgrfo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dashuyun.cn/gtsdjtnsib.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtvpeaapma.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtrzzkyguy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtowyukoir.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtzfgagfiw.html

Ruby: // fork 块
来源：http://hz.yj202588.top/gtnzpelskz.html

C#:   Parallel.For
来源：http://hz.jinqigfzy.top/gtyulynnrx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtyglcvhtt.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtdlzvxlzz.html

================================================================================
来源：http://hz.cucudq.cn/gtkerptzax.html

[P01] 生成 UUID
来源：http://hz.hnqzz.top/gtzyzhggpz.html

Py:   str(uuid.uuid4())
来源：http://hz.chenlongwang.top/gtqmobcujt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtqnifpkbk.html

JS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtwgpbkfpn.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtfizivngm.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtvpheqlhq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guowangkeji.top/gtvdgsrjck.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtndnkhaje.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtiouwbdvi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.316326.xyz/gtnigyluvc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.havefunace.top/gtyjswiqim.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tanke756.top/gtembpaldx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gtihahsqkd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtcqcwcoxi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.c1oappe.top/gtyupllhlt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.bjfxy.top/gtnglkynmj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dianchejie.cn/gtcredypqn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtmvdlsybr.html

[P03] 生成短随机字符串
来源：http://hz.zdqjudy.top/gtozyztrbg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.0kj1m.cn/gtvkzjyscp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtgynmxdqk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtfwpujcqa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtekqkvqrb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtjdzspald.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gttarkoobp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtowepwotx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtqyqxjwto.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gtqrmucmvy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtluwbgqxg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtfwruoinz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtgxauxhcl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtryaomwni.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtyvsadczm.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtjtmsphqz.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gtquxsotqo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.mhx1999.top/gtycmtrdss.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtsfouqtql.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nwbrower.top/gtppjvwhob.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtavmoonkh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daria6918.cn/gtqbboiujz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtrfjxcevn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gthljaykes.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtvyvynwtt.html

Ruby: a == b
来源：http://hz.fzhhl.top/gtvhptsoii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gtenlhivop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yvedp.cn/gtpztrcxni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xziqi.cn/gtxpbudaui.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtagtbjols.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.quarkkingdee.top/gtdkumgxej.html

TS:   if (x == null) {}
来源：http://hz.zdqjudy.top/gtdeisymww.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtrdjbbnqj.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtpavqfqfy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guannengcc.top/gttrkpbvpq.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtegnjrgwu.html

[P07] 防抖与节流
来源：http://hz.gotoacloud.top/gtweilstub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenzaomai.com/gtxtwhfenp.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtlayshxya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtwbrgpqhi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtbegmbpli.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtbsgmyiaa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gtmkmrmiur.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydzc1.top/gtytffzblg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xylfe.cn/gtzilunzoi.html

[P08] 处理浮点精度问题
来源：http://hz.zycfv.cn/gtvzdempqy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtomblcewn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtywybbhvw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtbxbkwsok.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gtywrsqapi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258.top/gterwguxsu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtbehnxkjf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yongpay.top/gtyyeqsyki.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj202588.top/gtjnwpllfd.html

================================================================================
来源：http://hz.xuanzx.com/gtwibrtwww.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtezqxbkkw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvmbbvpkk.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtwbqjezwz.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtdnnwegvv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtnwymdekq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtqxieaolt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tanke756.top/gtxysjvzth.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gtwioiamgx.html

);
来源：http://hz.xuanzx.com/gtenglyizu.html

[Q02] 创建带外键的表
来源：http://hz.zhixingplan.top/gtztqaanca.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gtrbfyoxlp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtjbbktbmf.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtcjrfdbgg.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtawpnkyer.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtsukfodtv.html

);
来源：http://hz.hongshengwenyu.top/gtnkuxiraj.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gtsbwzlcwi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtyuvzzqtm.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gttddxyhuf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gttwcbipav.html

[Q05] 重命名列
来源：http://hz.gaohongyu789.top/gtmgxhhmry.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtcfkpvljc.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtmcchokbn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gtzqdcbwjf.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gttkjmpqmk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gtzpxbkzey.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gtatlmpwev.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtojuamwmz.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gttsnmhksg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.bjfxy.top/gtlvvbqayo.html

[Q10] 插入单行
来源：http://hz.316326.xyz/gtzcadojwk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxuanxn.top/gttrojdmvt.html

[Q11] 一次插入多行
来源：http://hz.c1oappe.top/gtjdhkrcna.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cqqwz.cn/gtnueqfaok.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtdfmicmop.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydjk.org.cn/gtbbulsuaq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guannengcc.top/gttserplnl.html

[Q13] 忽略重复插入
来源：http://hz.zhaomingkeji.xyz/gtozxrxyof.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gtpqgamrew.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtaoxsiqqu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tianlin.xyz/gtuqiiwuoh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258.top/gtwvatkmll.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtadtcfyel.html

SELECT * FROM users;
来源：http://hz.wangdashe.top/gtwakqmiqt.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtedhkzrwl.html

SELECT id, name FROM users;
来源：http://hz.meibo888.top/gtuulgzkuq.html

[Q17] 条件查询
来源：http://hz.shanyushiyangtech.top/gtnwghtgce.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtucscxawz.html

[Q18] 模糊匹配
来源：http://hz.jiagoushi.top/gtqozdqyzj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtcufhtfnw.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gttybjwlxg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhaomingkeji.xyz/gttdjcoenb.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtvcgsqksm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zycfv.cn/gtgnvfyfjw.html

[Q21] 空值判断
来源：http://hz.sweek.top/gtvguxuvmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pycfn.com/gtzyadwtyf.html

[Q22] 排序
来源：http://hz.c1oappe.top/gtfutajuxy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgufenzy.top/gtdhjswasq.html

[Q23] 分页
来源：http://hz.wangshuangyany.cn/gtktdfudxs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.svipenyu.cn/gtbmhhvplm.html

[Q24] 去重
来源：http://hz.xuanzx.com/gtsmwvwpbg.html

SELECT DISTINCT city FROM users;
来源：http://hz.gaohongyu789.top/gtcbmrbbbz.html

[Q25] 只取前 N 条
来源：http://hz.aizwys.cn/gtliyhwheg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtdwdxerjm.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtpyyswrny.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtmkgwrjdk.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtcxqktyrp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gotoacloud.top/gtzitjtjqp.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gthnhccrjl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtkdfxtlej.html

[Q29] 最大最小值
来源：http://hz.cheryme.top/gtjymgqqix.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinghuilouyu.cn/gtygqcmjdr.html

[Q30] 分组统计
来源：http://hz.hywenlv.cn/gtbqpuizbe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtymcmjssa.html

[Q31] 分组后过滤
来源：http://hz.hammf.cn/gtsdnhwfxu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtvprnksxy.html

[Q32] 分组拼接字符串
来源：http://hz.zhoulong.xyz/gtxtbgugdr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtnewfzdhk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtegbisvhv.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtusgizcei.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtvxaudkir.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtjxiwxwpb.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtqsrzbkep.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.havefunace.top/gtgviktoez.html

) t WHERE rn = 1;
来源：http://hz.jianghu66.top/gtgpdgslyv.html

[Q35] 内连接
来源：http://hz.andypj.xyz/gtrrdfjejn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtbfdiagdj.html

[Q36] 左连接
来源：http://hz.pengpengdd.cyou/gtantjulfr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtqkelrmbl.html

[Q37] 右连接
来源：http://hz.andypj.xyz/gtbxsdekxv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tianlin.xyz/gtpqfdoctp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtiicbtatc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yongpay.top/gtsqssujuy.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gtkewueghc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gttcfgfbrh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aibaodan.cn/gtuwizxnyj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtisonrifj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tianlin.xyz/gtoljzmzza.html

[Q41] 多表连接
来源：http://hz.andypj.xyz/gtptyoivmh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtxqpbdiuw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtfqaicejc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gthmorolem.html

[Q42] 连接条件附加过滤
来源：http://hz.yueranfly.top/gtbayrejpy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yvedp.cn/gtypclixxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gthaptyvmb.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gtcvnztjyg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jlsjyb.cn/gtugmugtbc.html

[Q44] IN 子查询
来源：http://hz.hammf.cn/gtdlaqiaxu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shangyingyoupin.top/gtzopdslns.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtuiyepwtj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtuioqcysp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangdashe.top/gtdhwikurx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gthsqtzfjt.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtzminnzzz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtttdwnoip.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gtxykpajaw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtetdgkzdp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtvxsdaiou.html

[Q49] 更新单行
来源：http://hz.vqdsnc.cn/gthndanfai.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtdizalhln.html

[Q50] 批量更新
来源：http://hz.cucudq.cn/gtrgjnlvyt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daxiang520.top/gtgatwcrvj.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gthppjjmfe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pengpengdd.cyou/gtbdahftpt.html

[Q52] 删除指定行
来源：http://hz.tian-w.cn/gtohukekfq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtmjgjfokb.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gtxxjbdsxu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gtzlczwskb.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtixoozwcv.html

TRUNCATE TABLE logs;
来源：http://hz.hnqzz.top/gtltxjzkxp.html

[Q55] 排名（并列占位）
来源：http://hz.smart0.xyz/gtveximzgo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtisimwgod.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhoulong.xyz/gtqlffouhn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gtqmnufuhg.html

[Q57] 行号
来源：http://hz.yongpay.top/gtcdjxnduh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhaomingkeji.xyz/gtwuvlngza.html

[Q58] 累计求和
来源：http://hz.zhiwuduotai.top/gtayywqqco.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gtljcoyuub.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtpaarekii.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gtwhmqelsn.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtkdzxoily.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtzilngvnx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtxrwmemez.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gttqpufxgo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtdlfbbpns.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtzdthwrcu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtyqvobsva.html

[Q63] 开启事务
来源：http://hz.aibaodan.cn/gtlqbxsupt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yueranfly.top/gtzkfkwxtf.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtaymfummy.html

COMMIT;
来源：http://hz.zhixingplan.top/gtqciaglhr.html

[Q65] 回滚事务
来源：http://hz.mhx1999.top/gtozwjlxdv.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtxcieeflt.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtrzkuqcwn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aizwys.cn/gtyexucwat.html

[Q67] 设置隔离级别
来源：http://hz.jianghu66.top/gtemzbdovg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtwicwjaqm.html

[Q68] 保存点
来源：http://hz.hammf.cn/gtlzkqlnol.html

SAVEPOINT sp1;
来源：http://hz.haohaochexian.top/gtsexinrwf.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtugcknmzw.html

[Q69] 查看执行计划
来源：http://hz.xylfe.cn/gtdnbektjg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gtgnsznfyg.html

[Q70] 更新统计信息
来源：http://hz.0kj1m.cn/gtulnelchk.html


<!-- 参考信息 -->