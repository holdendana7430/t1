代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gttelbtuxe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.snrcjt.cn/gtxfssvcbi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhijiandao.cn/gtrojkjaho.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtinlnxdro.html

================================================================================
来源：http://hz.yj202588.top/gtjxyzdfdv.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtxeidafdl.html

================================================================================
来源：http://hz.sysykeji.top/gtstyhicwm.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtbtxqbypw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtoggjsxhw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.andypj.xyz/gtenztlwqb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxuanxn.top/gtwlwohxkg.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtrmezworv.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtkbvhekao.html

Go:   go f()
来源：http://hz.yuanzhike.top/gthsqgwanx.html

Ruby: Thread.new { f }
来源：http://hz.nwbrower.top/gtottofack.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gthpfeuckm.html

[O02] 使用线程池
来源：http://hz.xuetiantiany.cn/gtohmlqrqh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.havefunace.top/gtysyylljy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtwwmohfqh.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtdhfordpp.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtouhxwbcd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtmjkhczmn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.meibo888.top/gtknibzdgu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtzrsboafn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtrudtxjlr.html

[O03] 加锁保护共享数据
来源：http://hz.redwolf501.top/gttevnosnk.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtgsojhouc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtwnhxhddj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtdrnjxynd.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtcoapmdmo.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gtvcuhfupd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.52xcode.cn/gtcemhiggy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxuanxn.top/gtajwkktkc.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnqzz.top/gtsuukkzxe.html

[O04] 定义异步函数并等待
来源：http://hz.yueranfly.top/gtdetjghqf.html

Py:   async def f():⏎    await g()
来源：http://hz.tanke756.top/gtwwgsekzn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hfpthk.cn/gtkhffgkax.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gtmjkcmhyz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sxryk.cn/gtfgiazmyi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.svipenyu.cn/gtpkcufgbg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ehwqpu.com/gtpjabmfbi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtwgsyzdzw.html

C#:   async Task F() { await G(); }
来源：http://hz.wangdashe.top/gtlmiefhbc.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtevcmbzgs.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigufen.top/gtdsedvomm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnqzz.top/gteibjffdt.html

JS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtmzpfubsv.html

TS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtsornxabo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gtgsnqqzcx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtvinruzle.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtbxeihlxd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gaohongyu789.top/gtzoixqkmy.html

[O06] 使用进程池
来源：http://hz.xinyue.icu/gtxcrphnnv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gtqgicqukv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangshuangyany.cn/gtnplzivyf.html

JS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtkgsaordp.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtxdihdmev.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhiwuduotai.top/gtebdpuwck.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yangfankeji.com/gtdaimlxvr.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtlxpxwbsb.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtprcmtonw.html

================================================================================
来源：http://hz.zdqjudy.top/gtujssvfuy.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtfzjzisfv.html

================================================================================
来源：http://hz.cashguo.top/gtbmlosrxr.html

[P01] 生成 UUID
来源：http://hz.hongshengwenyu.top/gtevmmiuqa.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtgjarfcgy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tianlin.xyz/gtlemckxok.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtgyhwfdvs.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtwcvoecxr.html

Java: UUID.randomUUID().toString()
来源：http://hz.jiagoushi.top/gtkwzkaznv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenzaomai.com/gtnsxludgz.html

Ruby: SecureRandom.uuid
来源：http://hz.c1oappe.top/gtfvlfixfv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guowangkeji.top/gtmcqmtudg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtkubinzgy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtfgijlvai.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtvyauxche.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtelsofekf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtivdumnjc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtujziotbk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtqlmlwadg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhoulong.xyz/gtutikilrr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.redwolf501.top/gtpgmnsjxd.html

[P03] 生成短随机字符串
来源：http://hz.xuetiantiany.cn/gtbejnqzrh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuetiantiany.cn/gtxknulthw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtxhseawjm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtprdfahsi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtyeothqyq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtsmoprrst.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtckwqnkjj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtybjwrdpz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtargvwafd.html

[P04] 求长度
来源：http://hz.chenjidiqi.icu/gtojgyqsqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhiwuduotai.top/gtygfbvbku.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtxvxbvdbl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtzmzbvhoa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtztjgwfms.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtkaadoaok.html

Go:   len(arr);  len(m)
来源：http://hz.tian-w.cn/gtalvuxspi.html

Ruby: x.length;  x.size
来源：http://hz.daria6918.cn/gtvgohnwmn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtjnsjovbk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gtazulkbwr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fengsongda.top/gtnmgfzroz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtyquyfxlf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hammf.cn/gtimayrzmc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtbabhcbxd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtpouicech.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nwbrower.top/gtshbikapj.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtputfwlpt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gtzdadgwnl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtudvvispa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guowangkeji.top/gtddxfbzti.html

PHP:  if (empty($x)) {}
来源：http://hz.mhx1999.top/gtptbcggia.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtfvxmaqhr.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtvbziyxkj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xziqi.cn/gtqubjvnud.html

Go:   if x == nil {}
来源：http://hz.nwbrower.top/gtvmhhrhbe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhengqikj.top/gtfyoovmei.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtjrnemsqk.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gtrpfzmzwa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtwdesejrq.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtotxskfrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtmcvwspwg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtryopildh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guowangkeji.top/gtyjcktqjo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtigiuirln.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yvedp.cn/gttqlybudg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtvgiexido.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gthibztyye.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gtzkvvouvi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangtech.top/gthsgliefb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xinyue.icu/gturerlygw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.snrcjt.cn/gtjstolabh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.meibo888.top/gtflvrwhxq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtxsqgrglg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtdgiuhfyp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuxming.cn/gtielgiwgb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtyclaqlei.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gtmvbwijpz.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjnlxqdwz.html

[Q01] 创建表
来源：http://hz.vqdsnc.cn/gtjanpuqua.html

CREATE TABLE users (
来源：http://hz.zhiwuduotai.top/gtgmzvpxyn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtfdqqnblu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gtyjwqklpx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gtshqrvpec.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gtwxyvjggh.html

);
来源：http://hz.yongpay.top/gtwvtubldu.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtqqwfdjxj.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtbirmhmoz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtamzygvul.html

user_id INT NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtfkyruvkz.html

amount DECIMAL(10, 2),
来源：http://hz.bjfxy.top/gtkhuebgkt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gthcfpmfhn.html

);
来源：http://hz.yangfankeji.com/gtubgxjzba.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gteqvezsjd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhaomingkeji.xyz/gtcewaoruz.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gthsukmwxw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnxiangtu.top/gtwqoonxep.html

[Q05] 重命名列
来源：http://hz.jinqigufen.top/gtqtasanbt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtyrdlacrs.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtxgbcijdd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgufenzy.top/gthkrzxbaz.html

[Q07] 删除表
来源：http://hz.tanke756.top/gtrxsggoqa.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtpypxncue.html

[Q08] 创建普通索引
来源：http://hz.jlsjyb.cn/gtdefgzuya.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daxiang520.top/gtaehpalkw.html

[Q09] 创建唯一索引
来源：http://hz.sysykeji.top/gthwjgnnfo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtwbuftntt.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtbnwpppat.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gthxcllutu.html

[Q11] 一次插入多行
来源：http://hz.cdnleiting.top/gtxysufnll.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxuanxn.top/gtbzulcrlz.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtexvuhzqe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtigudtwgh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtcabugzrp.html

[Q13] 忽略重复插入
来源：http://hz.zhixingplan.top/gtygpicfwl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtxamoohhx.html

[Q14] 存在则更新（upsert）
来源：http://hz.gogol.net.cn/gtowolsxin.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ybcxt.top/gtiukvyyth.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.52xcode.cn/gtdwrrmmkb.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gteqrlqcyb.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtsfmvccex.html

[Q16] 查询指定列
来源：http://hz.nanxuanxn.top/gtfylacdep.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gthvizzgzg.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtbgicubca.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gogol.net.cn/gtwmtfkdce.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtlbqzjjkg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.smart0.xyz/gtmrwhnpvf.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtelfqjscu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigfzy.top/gtalxlliql.html

[Q20] IN 列表
来源：http://hz.shzxlz.cn/gtveytvger.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtgbtnzuob.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtdpztdnvi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtgbcpesnz.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtbhauwjuo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haohaochexian.top/gtqmyridle.html

[Q23] 分页
来源：http://hz.yueranfly.top/gtfhbvbogt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gttpyvbgbk.html

[Q24] 去重
来源：http://hz.316326.xyz/gtzldmeehs.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtujxormoe.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtatyceucs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gtfnqxscbp.html

[Q26] 计数
来源：http://hz.pengpengdd.cyou/gtlfkucgio.html

SELECT COUNT(*) FROM users;
来源：http://hz.cheryme.top/gtkqlzykep.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtwyvlxdoy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgufenzy.top/gtfcjsulht.html

[Q28] 求和与平均
来源：http://hz.yuanzhike.top/gtjlsnhpdq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gttlzjrxnn.html

[Q29] 最大最小值
来源：http://hz.zhijiandao.cn/gtoisikfgy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtvmmdylrc.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtdqzuketu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtsurxnkgz.html

[Q31] 分组后过滤
来源：http://hz.hongshengwenyu.top/gtsernpkmm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtrhlzfhjx.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtuyazaqvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtmzbiwwcg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tianlin.xyz/gtjjjebmdp.html

[Q33] 多列分组
来源：http://hz.yueranfly.top/gticremkqb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtvtgtusgb.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtqhwmqncq.html

SELECT * FROM (
来源：http://hz.shzxlz.cn/gtidtzkrxf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yueranfly.top/gtdtqwaigb.html

) t WHERE rn = 1;
来源：http://hz.9152youxi.cn/gtbtrhwtdf.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gttkbozkij.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtobikcbdm.html

[Q36] 左连接
来源：http://hz.yvedp.cn/gtitipccbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtwnmhciad.html

[Q37] 右连接
来源：http://hz.hfpthk.cn/gtslmhnfhe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cdnleiting.top/gtaldytxcy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guannengcc.top/gtchqmhxzv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtoyglyuwn.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258888.top/gtcppzeopz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.feifeiyinyue.top/gtmsmitlin.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtkrgrrbjc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gthnnphcjo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtsnazcjtw.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtwywkjtmg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ppjwa.cn/gtjanlqvad.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtmdsvfmvo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yanxiufei.cn/gtwjfrrjsw.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtliojcqor.html

SELECT u.name, o.amount FROM users u
来源：http://hz.redwolf501.top/gtwpcthxfc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuanzhike.top/gteydilomx.html

[Q43] 标量子查询
来源：http://hz.zhaomingkeji.xyz/gttfclushw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtcnpkovcw.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtkgcljokx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gttwvcyxbd.html

[Q45] EXISTS 判断存在
来源：http://hz.svipenyu.cn/gtzbcpjsuz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtgkrjrzrl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pycfn.com/gtzvtpnjhl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtzlsfucas.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtltduhygr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtwiftzmmz.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtllfdykhv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gtcqfzfjqb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xinyue.icu/gtpwhfumxu.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtcagjkmtz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtmxvygxvr.html

[Q50] 批量更新
来源：http://hz.aizwys.cn/gtxpzmjxdz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtsvuwynyc.html

[Q51] 用子查询更新
来源：http://hz.zhongyouzk.top/gtejlncohw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.mhx1999.top/gtqlsigwfq.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtaixifvii.html

DELETE FROM users WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gttbeqhsbt.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtohhxvnsq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ehwqpu.com/gtxaczxnmz.html

[Q54] 清空表
来源：http://hz.yanxiufei.cn/gtbfpskjky.html

TRUNCATE TABLE logs;
来源：http://hz.sweek.top/gtzbvrvndq.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gttlvfkmts.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtlgoguiwt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtvdshcsgn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gtypngtucu.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtfsdgiftb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sufxvd.cn/gtqjlzwdpk.html

[Q58] 累计求和
来源：http://hz.smart0.xyz/gttcjeunkp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtrkrtqpqt.html

[Q59] 分组内累计
来源：http://hz.jinyuanbaomall.cn/gtfajcgequ.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sysykeji.top/gtcnjnusdx.html

[Q60] 取上一行 / 下一行
来源：http://hz.smart0.xyz/gttcbihamt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtgyttiwtp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gttjqmmqiu.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtfozuufah.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtngbgxfjt.html

[Q62] 分组占比
来源：http://hz.jinyuanbaomall.cn/gtkerakywc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtqndfbfwo.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtcmhicqda.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sweek.top/gtzirqscje.html

[Q64] 提交事务
来源：http://hz.yuxming.cn/gthslyclsz.html

COMMIT;
来源：http://hz.gogol.net.cn/gtvmvgrbfs.html

[Q65] 回滚事务
来源：http://hz.yangfankeji.com/gtyxsyszno.html

ROLLBACK;
来源：http://hz.c1oappe.top/gthtvtkqwu.html

[Q66] 行锁查询
来源：http://hz.nwbrower.top/gtofinmmid.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hammf.cn/gtboheckgq.html

[Q67] 设置隔离级别
来源：http://hz.hongshengwenyu.top/gtkcovsuys.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtfjjrrjgh.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtqavtzjah.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtlaxnkbgg.html

ROLLBACK TO sp1;
来源：http://hz.havefunace.top/gtioxuuowa.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangtech.top/gtcmvkllup.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtrtsrviyr.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtuqmebjpz.html


<!-- 参考信息 -->