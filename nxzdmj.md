代发 wailian999

================================================================================
来源：http://hz.zhoulong.xyz/gtcnjyhqii.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gtidopjkpz.html

================================================================================
来源：http://hz.zhengqikj.top/gthsawsxnc.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtengztwzt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigufen.top/gtthrzwimj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtisshqrmc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtiwgvcbfl.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtlqwfgtrl.html

Java: new Thread(() -> f()).start()
来源：http://hz.tanke756.top/gtlrctzaju.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtclftsxid.html

Ruby: Thread.new { f }
来源：http://hz.ppjwa.cn/gtoccenqff.html

C#:   Task.Run(() => F());
来源：http://hz.ybcxt.top/gtrltdnkdu.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtzbokaikc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sufxvd.cn/gtgtihdhxi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuanzhike.top/gtgxemtqyp.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtcdmiemgq.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtfnnpfqiz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj202588.top/gtekrjbxck.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtjahijbja.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtekqfmpqq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtzwvvhogw.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtmdjpscol.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtcuvsyxcb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtnhpiuumb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gtqzuokstq.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtlnxeuows.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gthxlmhlky.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtgyamahpk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.haohaochexian.top/gtjgjtpcgm.html

C#:   lock (gate) { shared++; }
来源：http://hz.svipenyu.cn/gtosqpgokg.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258888.top/gtoodwflsb.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtpwideiyh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hammf.cn/gtytrjnvhc.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtyuaaunat.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gtjydcvgdm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtodemlvov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hfpthk.cn/gtjxihwgyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtrtewqacj.html

C#:   async Task F() { await G(); }
来源：http://hz.xuetiantiany.cn/gtdknpicls.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gttotcwdmp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtaunaqqly.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigufen.top/gtiqufixut.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtpkqwknlo.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtuwrtgnke.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258888.top/gtghexvegw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gtawgniwnf.html

Ruby: threads.map(&:join)
来源：http://hz.yangfankeji.com/gtputoedtm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gtuxddecsu.html

[O06] 使用进程池
来源：http://hz.cdnleiting.top/gtkupxcowl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtclqlxjbo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hammf.cn/gtcnunubno.html

JS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gttxsbrztx.html

TS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtjmnkwjjo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zdqjudy.top/gtlafwahtf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ivvv.top/gtuyezwufi.html

Ruby: // fork 块
来源：http://hz.cucudq.cn/gtzcviymes.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtwxlolofb.html

================================================================================
来源：http://hz.zhengqikj.top/gtkzqfkuxi.html

P. 常用工具函数
来源：http://hz.haohaochexian.top/gtlsnsuicy.html

================================================================================
来源：http://hz.xylfe.cn/gtuppsmfud.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gtnxwpeibm.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gtesijzmfa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pycfn.com/gtxrpsuzgi.html

JS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtsomxodqx.html

TS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtlngjqhys.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtbmnlpnqt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtugiwoeta.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtpmodmxzw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ppjwa.cn/gtvnuevspa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.havefunace.top/gtuaemjqfj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gttbpfowbr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtkkzozhfo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ywan-chungtsiang.top/gtlrhohiod.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangshuangyany.cn/gtesxwlhum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtofdygtbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuanzhike.top/gtovejwjfe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtdijtlpyl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtnsrgnjyj.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gtffthpzmu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xingfuxueyuan.xyz/gtthazrfuv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtzgnynmnt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtjaqskxtj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtpdwbujyi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtbyuoibig.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gthwfjxfyp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtkydeqkjb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xingfuxueyuan.xyz/gtotpifmqm.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtjcxevzjh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtmertfuid.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gteeukzeom.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtzjdaaueu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtmypnrqzh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cqqwz.cn/gtfvqnwcat.html

Go:   len(arr);  len(m)
来源：http://hz.nwbrower.top/gtzbomyibq.html

Ruby: x.length;  x.size
来源：http://hz.daxiang520.top/gtuzgzatsn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangkeji.top/gtehmfgwpe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtamtpyvus.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinghuilouyu.cn/gtxnqvnmcj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fengsongda.top/gtooravipu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtxblzujmw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gtyuwsmedv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aizwys.cn/gtypbouzzr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgfzy.top/gtgnlobvak.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtrajelsoo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtxzozkear.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtawhtoivn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jianghu66.top/gtxmptgkmb.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gthpdeumbs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenlongwang.top/gtbkzptgvq.html

TS:   if (x == null) {}
来源：http://hz.zhongyouzk.top/gthgnjhkgy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuanzx.com/gtffdfcicu.html

Go:   if x == nil {}
来源：http://hz.quarkkingdee.top/gtpilarbcx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtepwrgvxd.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gtwqtkfkfu.html

[P07] 防抖与节流
来源：http://hz.sxryk.cn/gtzjwitqxb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgfzy.top/gttqgdddqa.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtkyxmswkq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtiqprfews.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtlwjyxpyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cucudq.cn/gtytihdrna.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cucudq.cn/gtjfdetqqw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sysykeji.top/gtbthvmtui.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtsiphvqll.html

[P08] 处理浮点精度问题
来源：http://hz.nanxuanxn.top/gtkvahorsl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtqibvyhrq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guowangkeji.top/gtlpjryuyo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xingfuxueyuan.xyz/gtozvfwqpx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cdnleiting.top/gtarrhhxua.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gteoeliafl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuetiantiany.cn/gtbeilzdmq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtghbslksv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gtxvfhzapv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpwfzgsbr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.iojbl.cn/gtahbukufj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtiffufyfr.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gttsfeulul.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtovxctmue.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtqaqhenlq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtexfqfynt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtncnbdrci.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtnuttbgtq.html

);
来源：http://hz.svipenyu.cn/gtigqeffix.html

[Q02] 创建带外键的表
来源：http://hz.fengsongda.top/gtouktckdb.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtsxdwavna.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gtxrhxdali.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtevcrxhoo.html

amount DECIMAL(10, 2),
来源：http://hz.pengpengdd.cyou/gtwbhixwfr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtvapjcrky.html

);
来源：http://hz.cashguo.top/gtkndgfnpg.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtjfwovyoi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xingfuxueyuan.xyz/gtuhaawpqm.html

[Q04] 修改列类型
来源：http://hz.pycfn.com/gthysaqsoz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtrhctyfvv.html

[Q05] 重命名列
来源：http://hz.meibo888.top/gtwofvfpzb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtzhejjjeq.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtorkdugux.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cashguo.top/gtghfvvdvo.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtjcbvywup.html

DROP TABLE IF EXISTS orders;
来源：http://hz.0kj1m.cn/gtqtslsknh.html

[Q08] 创建普通索引
来源：http://hz.cucudq.cn/gtmpxcdaab.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtltaehgxc.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gtaxxiqoeb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtpetivdwl.html

[Q10] 插入单行
来源：http://hz.ppjwa.cn/gthihbgdkn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtwaawtmrc.html

[Q11] 一次插入多行
来源：http://hz.daxiang520.top/gtbtfmmblj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtblrimgtf.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gtbefyodzg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daxiang520.top/gtqmurzxgr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtjdzchpep.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gtlrawfmfz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zycfv.cn/gtplbubaue.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gthadluusc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gtyiftbxet.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gthqwzycgm.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gtaztcmxww.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gthahvgkij.html

[Q16] 查询指定列
来源：http://hz.redwolf501.top/gthgawykpk.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangtech.top/gtycpfoghk.html

[Q17] 条件查询
来源：http://hz.shanyushiyangtech.top/gtjtackdfc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gaohongyu789.top/gtcyxtoezt.html

[Q18] 模糊匹配
来源：http://hz.pengpengdd.cyou/gtqbjpfhtl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtrkifnbkm.html

[Q19] 范围查询
来源：http://hz.tian-w.cn/gtfilbsojm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtymboohhh.html

[Q20] IN 列表
来源：http://hz.cucudq.cn/gtidvpdjvy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gotoacloud.top/gtohznovfb.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtbrdwfdus.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtiyjxcmfs.html

[Q22] 排序
来源：http://hz.aizwys.cn/gtoqgmqhjz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigfzy.top/gtxkxbbzje.html

[Q23] 分页
来源：http://hz.yj20258888.top/gtfgzpdbad.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gttvucwwwc.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtzobinxcu.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtdbulyigd.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtocpngpck.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangtech.top/gtrcabmmbg.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtteizkkor.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnqzz.top/gtthchduyj.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtuocyhxxf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtnoxullur.html

[Q28] 求和与平均
来源：http://hz.yongpay.top/gttgfaccsx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.feifeiyinyue.top/gtcbeobsfv.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtffwzcmgv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gtnlqabelw.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtyizfmecg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtizelydfh.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gtwtfqtwha.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jianghu66.top/gtyrucldar.html

[Q32] 分组拼接字符串
来源：http://hz.feifeiyinyue.top/gtbnuilojf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtkvbsxdmb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aizwys.cn/gtkprqxbmx.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtrrzuuiev.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtshoolvfp.html

[Q34] 每组取第一条
来源：http://hz.jinghuilouyu.cn/gtmtqbljgn.html

SELECT * FROM (
来源：http://hz.birdmap.top/gtqaphhgoz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtjohbltqa.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtnlbcrjmu.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtvwwivfah.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtxphixlwg.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtsvaefnqt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtpisfbnrf.html

[Q37] 右连接
来源：http://hz.zhaomingkeji.xyz/gtktrkjbsv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinyuanbaomall.cn/gtieomxjlu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtrlqmvfal.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtvdsunohl.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtvffibhez.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhoulong.xyz/gtvdofnhry.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fengsongda.top/gtcvedhjdj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tanke756.top/gttoekikbn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgfzy.top/gtylqgnjxf.html

[Q41] 多表连接
来源：http://hz.yuanzhike.top/gtafzchjtt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtasgrmhaz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ppjwa.cn/gtruxawlho.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtrbdykwup.html

[Q42] 连接条件附加过滤
来源：http://hz.52xcode.cn/gtvdvuubqh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtjdrwzhgd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtwgkshahv.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gtpigxmvvh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigufen.top/gtlwjfgczw.html

[Q44] IN 子查询
来源：http://hz.dashuyun.cn/gtofgoouwi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtmsfpvjws.html

[Q45] EXISTS 判断存在
来源：http://hz.sweek.top/gtzwbsmzvd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtuujahpkz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yongpay.top/gtoadoizsy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtczblsyto.html

[Q47] 与平均值比较
来源：http://hz.yueranfly.top/gtbulpjznh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtsxoluaeu.html

[Q48] CTE 公用表表达式
来源：http://hz.ehwqpu.com/gtjcvyueus.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shuidangran.top/gtheyreukm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.quarkkingdee.top/gtpyrefzqv.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtugwojkwx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.svipenyu.cn/gtampphvrm.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtxtvdwbyk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnqzz.top/gtppihyihs.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gtarwunshv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtfhraonxb.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtrvchsqmh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hywenlv.cn/gtzeywzujj.html

[Q53] 按条件删除
来源：http://hz.ybcxt.top/gtuajraqkz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtrmsfboey.html

[Q54] 清空表
来源：http://hz.birdmap.top/gtlxyehqic.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtzigmrweu.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtlitmtpua.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daxiang520.top/gtjfxforeh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuanzhike.top/gtblidfxjh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtlwcsnavm.html

[Q57] 行号
来源：http://hz.hammf.cn/gtabtiwrkr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtrcexpabn.html

[Q58] 累计求和
来源：http://hz.yj202588.top/gtxpdvmugq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtgmehuauf.html

[Q59] 分组内累计
来源：http://hz.tanke756.top/gtzqgmwicm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ehwqpu.com/gtmabtqffh.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtfsnjbavf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtxqpfihnc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtfdyrnlgu.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtpinjpkws.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtqvlifgex.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtbvgivkym.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtkakxxgby.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtncflryjx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgfzy.top/gtewvvcexy.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtwfyttwsp.html

COMMIT;
来源：http://hz.pycfn.com/gtcxegbgwd.html

[Q65] 回滚事务
来源：http://hz.yj20258888.top/gtjklcaaon.html

ROLLBACK;
来源：http://hz.hysaishi.cn/gtdgatrbig.html

[Q66] 行锁查询
来源：http://hz.andypj.xyz/gtbmxmdopp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtgpagwfkh.html

[Q67] 设置隔离级别
来源：http://hz.snrcjt.cn/gtzixhyjvr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhaomingkeji.xyz/gtoxfouxas.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtadlntffa.html

SAVEPOINT sp1;
来源：http://hz.yvedp.cn/gthjbaqnxe.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtkcedptmf.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtfelneyit.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtfkzlonla.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtkrngqhue.html

ANALYZE TABLE users;
来源：http://hz.jqgfzy.top/gtfrpgzgie.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtexcsbkae.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gtrpkgcrio.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtmhggnbsm.html


<!-- 参考信息 -->