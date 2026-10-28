代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtrzhpwggb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtjlwgztnl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yongpay.top/gtopccpeta.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtopvxeivx.html

Java: new Thread(() -> f()).start()
来源：http://hz.fengsongda.top/gtiwvzeehj.html

Go:   go f()
来源：http://hz.cqqwz.cn/gtrktsrpwv.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtceofymgp.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtkontkqlj.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtutomujny.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtkouuhxgw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangkeji.top/gtiltbvxgi.html

JS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtpcbaxusm.html

TS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtytfbiwep.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtvhchhzxe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gtcvsmejxs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sweek.top/gtlsuvbcdo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtbycoonbf.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtftoebscc.html

Py:   with lock: shared += 1
来源：http://hz.xylfe.cn/gtqwitvovz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtombmkduz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gtslqticgn.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtjkfzjzlz.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gtwjkgayyz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gtjeileqyx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gaohongyu789.top/gtmzugfxoh.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydzc1.top/gtiguevjsk.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtvblsmwhq.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtzzuzsfse.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gtkracenkd.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtwdwvokcw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yangfankeji.com/gtuemdgmnz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daria6918.cn/gttqclccqh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtwfekqazw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gtkvyjcanx.html

C#:   async Task F() { await G(); }
来源：http://hz.gotoacloud.top/gtftaitbtd.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxuanxn.top/gtbxaympju.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtcdmigely.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangtech.top/gtalueewzz.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtwjpiosnu.html

TS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtbytyghnw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtjywnrpdf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtsmgxaoja.html

Ruby: threads.map(&:join)
来源：http://hz.hywenlv.cn/gtozvzhvlv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.iojbl.cn/gtcfrfzjvl.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtaadkolov.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuanzhike.top/gtpccclrcw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtbtkaazwm.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtukcgjhss.html

TS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtpmfjsqmd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hammf.cn/gtbzqfapjn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtwxeqkbyn.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtmibrqatm.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtigeucode.html

================================================================================
来源：http://hz.0kj1m.cn/gtxtxbjfod.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gthwnaojgk.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtevgtsfkc.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtojnjuzhu.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtatlcklxr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jyoumei.cn/gtikhcpalu.html

JS:   crypto.randomUUID()
来源：http://hz.yuxming.cn/gteotstrmv.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtocvcpfxg.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtwszjgocp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtlkruirqf.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtuotpujod.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhijiandao.cn/gtemtlpzvm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtgwibbxdv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.bjfxy.top/gtlpwhqmtn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtxybpmchf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.0kj1m.cn/gtzoklkfcx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtfenowceg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gogol.net.cn/gtgcnlasrq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.svipenyu.cn/gtwnmwpvzj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pengpengdd.cyou/gtcsotfpgl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtswydodxr.html

[P03] 生成短随机字符串
来源：http://hz.nwbrower.top/gtfqtshmjs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtarbdibxb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yanxiufei.cn/gtgbljinjq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtzpryggob.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtsloyixms.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gaohongyu789.top/gtkoyzxytt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gtmtgeietl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cucudq.cn/gtajkgxjmp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtpxjzajtc.html

[P04] 求长度
来源：http://hz.dianchejie.cn/gthodxvqna.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtoyzlfzwi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtoommspmv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtejlquxjb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtmwyuboix.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gaohongyu789.top/gtqgxwsbsz.html

Go:   len(arr);  len(m)
来源：http://hz.chenjidiqi.icu/gtfbnqszlf.html

Ruby: x.length;  x.size
来源：http://hz.jlsjyb.cn/gtizsvubju.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.316326.xyz/gtmljgykuq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gthivqduja.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258888.top/gtzzmqaieq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtzezlnbcp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aibaodan.cn/gtpdnkkkgo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtrezbkzsc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nwbrower.top/gtdxajtkcq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtpsacmifx.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtxafwiaej.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhengqikj.top/gtwambkwoj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tanke756.top/gttfgbneqe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hfpthk.cn/gtqvvqaibv.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtenykkolz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aizwys.cn/gtusbwteuf.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtaikueqjw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtbnfizxbb.html

Go:   if x == nil {}
来源：http://hz.xziqi.cn/gtotvcrryb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtvbmslbcx.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtffabxdpa.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtkfyjzzbr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtictwnewh.html

PHP:  // 手写时间戳比较
来源：http://hz.guannengcc.top/gttacbfxca.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtkviebhan.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtumcdbime.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ehwqpu.com/gtnthabvmf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtwqsuczce.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenjidiqi.icu/gtimcqohuu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dianchejie.cn/gtzdfltzuh.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gthdenthjd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ppjwa.cn/gtkxezmeij.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gtsetvhtcm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtqffrfpia.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daria6918.cn/gtmxfcrkfc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtqfkpuzyp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yangfankeji.com/gtaopywwim.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.birdmap.top/gtbagndens.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuetiantiany.cn/gtabjwafnu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtucbqhihh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gzhubu.top/gtnvauvwng.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjgtefoxr.html

[Q01] 创建表
来源：http://hz.yongpay.top/gthqclvyhl.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtlhmrieji.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtuyrjnaxn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtifmruxin.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gthvrqgcqr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.birdmap.top/gtvrgtfdlq.html

);
来源：http://hz.sufxvd.cn/gtqmqhifnl.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtdbbvbqww.html

CREATE TABLE orders (
来源：http://hz.chenlongwang.top/gtfygkqivw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtiktdleof.html

user_id INT NOT NULL,
来源：http://hz.hywenlv.cn/gtttaxlkll.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtwdkiuroj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.redwolf501.top/gtkvfyoqej.html

);
来源：http://hz.cqqwz.cn/gtxsolcuez.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtpguyefbv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.svipenyu.cn/gtdxjtqrcq.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtmbdbiskp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hammf.cn/gtryyeuuei.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gteyytknfe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yangfankeji.com/gtwplkbvii.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gthldgjtow.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtiqglewvj.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtkdawyuui.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yangfankeji.com/gttxozodgi.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtcfxbirul.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gteuemzctg.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtefiwmnvh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtbunwycbo.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtekbblnec.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtoxrbsxld.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangkeji.top/gthgehfggt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.snrcjt.cn/gtdsddbhba.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gtwsscelqe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgufenzy.top/gtbvyayyec.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtosbjyhly.html

[Q13] 忽略重复插入
来源：http://hz.ywan-chungtsiang.top/gtgsjaaqra.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ydzc1.top/gtkmrydiwy.html

[Q14] 存在则更新（upsert）
来源：http://hz.gogol.net.cn/gtclkewqqx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtckfkjxku.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhijiandao.cn/gtikfmqhon.html

[Q15] 查询全部
来源：http://hz.feifeiyinyue.top/gtkhgpkddz.html

SELECT * FROM users;
来源：http://hz.yuxming.cn/gtlmxnnsin.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtckipidln.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtqkkwupsu.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtdbumxcim.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gtjsfxmnor.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtwkihpujr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dianchejie.cn/gtvujqcpmn.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtixexrycp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yongpay.top/gtrnzgsime.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtykewmkfs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aizwys.cn/gtokczoyng.html

[Q21] 空值判断
来源：http://hz.ydjk.org.cn/gtiqqcnvzn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtzkghxdux.html

[Q22] 排序
来源：http://hz.aizwys.cn/gtzjupnmgw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtubiatcdi.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtlmzxgfsu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jianghu66.top/gtchpysfon.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtdhpihmbz.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtosgffgzx.html

[Q25] 只取前 N 条
来源：http://hz.yj202588.top/gtgofectjh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtpjwgsxmg.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtgavoomjk.html

SELECT COUNT(*) FROM users;
来源：http://hz.xinyue.icu/gtqyqqfhqe.html

[Q27] 条件计数
来源：http://hz.svipenyu.cn/gtaqggzyxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtagkizfeg.html

[Q28] 求和与平均
来源：http://hz.mhx1999.top/gtdatuhqrr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gtztlmtxht.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtrdyxmmbt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtqnnxuiay.html

[Q30] 分组统计
来源：http://hz.aibaodan.cn/gtuhtmycmv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtdqqgqhag.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gtuxddftfk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtqgkalttl.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gterbhfkoi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtmuuxahgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hfpthk.cn/gtxjejluub.html

[Q33] 多列分组
来源：http://hz.guowangkeji.top/gtuvqjphgt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtvnnelkhm.html

[Q34] 每组取第一条
来源：http://hz.hnqzz.top/gtyqcgtqvp.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtoijwrlrf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtjawbzwgo.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtzbavucgs.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtiqolowte.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtrruwiuhy.html

[Q36] 左连接
来源：http://hz.havefunace.top/gtdekulrfx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtdfrsjbmz.html

[Q37] 右连接
来源：http://hz.yonumen.top/gttdlkoocg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtyhekxelh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dianchejie.cn/gtjdpdmbsj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jlsjyb.cn/gtcykyyxgh.html

[Q39] 自连接（查上下级）
来源：http://hz.sxryk.cn/gtrwifimtv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cqqwz.cn/gtsnjwlsat.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yonumen.top/gtiprywzfh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtskiadadk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cqqwz.cn/gtcmcijqnc.html

[Q41] 多表连接
来源：http://hz.yj20258.top/gtwiweklzd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtflalemtw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtuaanicte.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtqbxiqnog.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtfrglxmio.html

SELECT u.name, o.amount FROM users u
来源：http://hz.0kj1m.cn/gtvdvycahs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtzftjroda.html

[Q43] 标量子查询
来源：http://hz.jinyuanbaomall.cn/gthbmehcfh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtthokfahy.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtqqixqkwh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hywenlv.cn/gtjqkaokwo.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtpxvlkkgg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtbaehohqc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtlgscebmh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtzptlvdev.html

[Q47] 与平均值比较
来源：http://hz.zycfv.cn/gtadjgnojj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ivvv.top/gtoycmpilh.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gteszeizky.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtqbecljon.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtrupqqlxv.html

[Q49] 更新单行
来源：http://hz.cdnleiting.top/gtvdjlrgln.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gtpthasasr.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtnsdvpeuu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.52xcode.cn/gtuxjewhbj.html

[Q51] 用子查询更新
来源：http://hz.hywenlv.cn/gtfbtuzkhf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.smart0.xyz/gtzjafcvqs.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtusiwupio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtigciuvcy.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtmtxuplvu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtdojtqkzd.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtoizctuqq.html

TRUNCATE TABLE logs;
来源：http://hz.fengsongda.top/gtsgulmtrw.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258.top/gtwushccwf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtakqncbgw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cucudq.cn/gtdetfgayx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sufxvd.cn/gtphnkerzs.html

[Q57] 行号
来源：http://hz.zhiwuduotai.top/gtyxjkxwvr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.bjfxy.top/gtbymewgug.html

[Q58] 累计求和
来源：http://hz.shuidangran.top/gtklyezaix.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtxbylwant.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtlrtanhrx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtxodxcwai.html

[Q60] 取上一行 / 下一行
来源：http://hz.sxryk.cn/gtwlkplqir.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtnikwzpht.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtexrqaobq.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gtgypfrqyd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtyqqsjozk.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtoojtvdqj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtojyrhtos.html

[Q63] 开启事务
来源：http://hz.redwolf501.top/gtvkurgqov.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhaomingkeji.xyz/gtqgncnegl.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtahltzlen.html

COMMIT;
来源：http://hz.dashuyun.cn/gteaunsxkb.html

[Q65] 回滚事务
来源：http://hz.gogol.net.cn/gtgfgvrgxi.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtzyiafmvc.html

[Q66] 行锁查询
来源：http://hz.0kj1m.cn/gtychezrer.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yonumen.top/gtegoffgog.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtmwlrijyi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtkdkwkhsa.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtmsmywceo.html

SAVEPOINT sp1;
来源：http://hz.svipenyu.cn/gtxmjtikal.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtekpkugeh.html

[Q69] 查看执行计划
来源：http://hz.cdnleiting.top/gtnwpxphih.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtgfngrpua.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtealxwwnm.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtqkbykezj.html

[Q71] 查看建表语句
来源：http://hz.tianlin.xyz/gthjblgtah.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtnrswpolj.html

[Q72] 查看索引
来源：http://hz.havefunace.top/gtfyevpbhn.html

SHOW INDEX FROM users;
来源：http://hz.c1oappe.top/gtzypgiybq.html

[Q73] 查看表状态
来源：http://hz.nanxinkj.top/gtxgwypsad.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtcprsygfw.html

[Q74] 强制使用索引
来源：http://hz.zhiwuduotai.top/gtqifdmtqe.html


<!-- 参考信息 -->