代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gttrxoswkw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtkleoxhtv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gttpcmuzuz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtzdskrxsi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtgyzdfnwy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtefnipnny.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gthwbjehdp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtyboaqhxn.html

================================================================================
来源：http://hz.yvedp.cn/gtqtuonftq.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtgzzgwfgr.html

================================================================================
来源：http://hz.cheryme.top/gtryosfxjq.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtiyjpzvtz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258.top/gtjoehugsq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtpygpizwm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuetiantiany.cn/gtrgzwehyl.html

TS:   // 同 JS
来源：http://hz.jiagoushi.top/gtvsbnjlvt.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtspntpxym.html

Go:   go f()
来源：http://hz.guannengcc.top/gtjjaomsfm.html

Ruby: Thread.new { f }
来源：http://hz.chenlongwang.top/gtbzzsgrvm.html

C#:   Task.Run(() => F());
来源：http://hz.ybcxt.top/gthdmmbkhx.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtzhfedfgv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtcokkjlfu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtoydduzsi.html

JS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtipzstwvo.html

TS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtmiahrezu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gttlxiutjl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zdqjudy.top/gtvgkwgiex.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtbdfjkyqv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tanke756.top/gtemqftlcz.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtvqohknwi.html

Py:   with lock: shared += 1
来源：http://hz.zhiwuduotai.top/gtjeqvoitd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtbejzsdmw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.quarkkingdee.top/gtzutbohwo.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtaoglxbah.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtcjvvxtfh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shuidangran.top/gtxnzlyrzz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gtbaekfioe.html

C#:   lock (gate) { shared++; }
来源：http://hz.jlsjyb.cn/gthcloiqif.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtnlhvgiej.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtexkublap.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tian-w.cn/gtrdsxkssg.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtjafdyvvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigfzy.top/gtxzaslgcs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.haohaochexian.top/gtoviiriah.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guannengcc.top/gtqrnsjemy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtnlwxpstt.html

C#:   async Task F() { await G(); }
来源：http://hz.haohaochexian.top/gtrwdbdzfb.html

[O05] 并发执行并等待全部完成
来源：http://hz.yonumen.top/gtnjfigigj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtkctmeqjb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.fzhhl.top/gtycbkcvdb.html

JS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtpmatgzpc.html

TS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtpynwhtdz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtpgdbzovs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtykoakjte.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gtwhfvnzpc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yueranfly.top/gtwlptdjza.html

[O06] 使用进程池
来源：http://hz.tanke756.top/gtwvxnunif.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gtqhttqsxs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhongyouzk.top/gtgonisobj.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtdlkztafq.html

TS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtppwthwng.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtdmdpjahq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydjk.org.cn/gtsdaamcsp.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtkxuoajpf.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gttfjxrfnu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrjnaalvw.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtrphkvguy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxacyhydl.html

[P01] 生成 UUID
来源：http://hz.hnqzz.top/gtgquyxomp.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtfwxxgsug.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtedfdglfm.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtqhwuoazz.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtnqabmkkd.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangdashe.top/gtszzpzjmc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtldzuyznx.html

Ruby: SecureRandom.uuid
来源：http://hz.ppjwa.cn/gtudzqrvme.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtlljiahtx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtauypquab.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangdashe.top/gthjdhcfql.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gtcvjwcdjc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gtofnwdjjn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gtxnuuclln.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gtizywetie.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gtnwomuong.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtsvvruaas.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtdlgfglpu.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtdyfyhxyj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.0kj1m.cn/gtmiaxohtu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenjidiqi.icu/gtamzqeqqh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtafpdjvrd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtqsphoing.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gticgqhrda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnxiangtu.top/gtzhqqvgtx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtchrlijdy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hongshengwenyu.top/gtsnurtlmx.html

[P04] 求长度
来源：http://hz.yvedp.cn/gtiakndnbf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gthawkczce.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtpygqxcyt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtesuxeuwr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtsoxpevqt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hongshengwenyu.top/gtxtdayrda.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtueskhvwq.html

Ruby: x.length;  x.size
来源：http://hz.redwolf501.top/gtqfjvpkfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtggfydffp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shuidangran.top/gtcbmpvbfr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtjvlraham.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtyvafkfut.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gtpcclkurk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtuebpixwn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtcmcpjxjj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj202588.top/gtxhyzlavv.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtahasevrw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhengqikj.top/gtffivmtbc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtyszkdvda.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tianlin.xyz/gtexuxzuqt.html

PHP:  if (empty($x)) {}
来源：http://hz.aibaodan.cn/gtadbqmfoa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fengsongda.top/gtefeazavl.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtfuubjjlf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtiejwdima.html

Go:   if x == nil {}
来源：http://hz.sufxvd.cn/gtvvnuhxjb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtjwulebsh.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangkeji.top/gtkflxpjnu.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gtxubwtuyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtiimyznjb.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtsymsvuln.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtpshrslqd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtfkfcawpt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtwlcsmedz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtvdufdkov.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gaohongyu789.top/gthunnvphm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guowangkeji.top/gttvzrvdye.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtpblnktbw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gtzlzvjiuq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daxiang520.top/gtqlsubinz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtkssfmfaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxinkj.top/gtamdtjvor.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhongyouzk.top/gtbnjwqyhn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.snrcjt.cn/gtgkvhlolk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydzc1.top/gtdaqkxitt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtkmyejvdt.html

================================================================================
来源：http://hz.xylfe.cn/gtaihywtvi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sysykeji.top/gtftjkbgkr.html

================================================================================
来源：http://hz.cdnleiting.top/gtiaxcdwgq.html

[Q01] 创建表
来源：http://hz.aibaodan.cn/gtqzdxixhh.html

CREATE TABLE users (
来源：http://hz.feifeiyinyue.top/gtsxbpjunu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtbnultpwp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pengpengdd.cyou/gtlpdrwiix.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sweek.top/gtbtikcmph.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jlsjyb.cn/gtccaurvxz.html

);
来源：http://hz.gaohongyu789.top/gtceasoglt.html

[Q02] 创建带外键的表
来源：http://hz.jqgfzy.top/gttsfqpojr.html

CREATE TABLE orders (
来源：http://hz.xylfe.cn/gtjbblhqut.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtgtiwjfkg.html

user_id INT NOT NULL,
来源：http://hz.xziqi.cn/gtiednfznw.html

amount DECIMAL(10, 2),
来源：http://hz.hfpthk.cn/gtahogdcoj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtpzmkonfu.html

);
来源：http://hz.cashguo.top/gtvajqikab.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtmnspwzyx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258.top/gtncrowagw.html

[Q04] 修改列类型
来源：http://hz.zycfv.cn/gtzlajsieb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtruyjqqnd.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtbrfyuyvv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtjurqicbx.html

[Q06] 删除列
来源：http://hz.xingfuxueyuan.xyz/gtrdrcaqkp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.bjfxy.top/gtpcleltmo.html

[Q07] 删除表
来源：http://hz.sufxvd.cn/gtccbgscfk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gthxtetflv.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtvnqcotsn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtkmordxpu.html

[Q09] 创建唯一索引
来源：http://hz.ybcxt.top/gtnkyubmrx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtgbslztyw.html

[Q10] 插入单行
来源：http://hz.feifeiyinyue.top/gtnycifmkj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fengsongda.top/gtugqqzncf.html

[Q11] 一次插入多行
来源：http://hz.wangdashe.top/gttozohqkq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtjyjwylhz.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtczhjecpv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtenbrbmzh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtygfuyoig.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gtulhhtgyt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sweek.top/gthvsvjbob.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtknvkfssw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnqzz.top/gtzpnihgha.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtxmigqzwq.html

[Q15] 查询全部
来源：http://hz.zhoulong.xyz/gtrcofuecf.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtgornvjye.html

[Q16] 查询指定列
来源：http://hz.sufxvd.cn/gtzaufigpb.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtbmnrsufu.html

[Q17] 条件查询
来源：http://hz.chenjidiqi.icu/gtsdsuofou.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gttuolbzgx.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gttjgrgyjj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dashuyun.cn/gtawoldjsz.html

[Q19] 范围查询
来源：http://hz.gaohongyu789.top/gttjgorkgv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yangfankeji.com/gtohxwdrom.html

[Q20] IN 列表
来源：http://hz.yongpay.top/gthgvrgkhj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenzaomai.com/gtppksuepb.html

[Q21] 空值判断
来源：http://hz.xingfuxueyuan.xyz/gtrpwhqxbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgufenzy.top/gtjcyevzyt.html

[Q22] 排序
来源：http://hz.birdmap.top/gtyjhxuxxc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xingfuxueyuan.xyz/gtynnbohrf.html

[Q23] 分页
来源：http://hz.xingfuxueyuan.xyz/gtwjexhbkq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daria6918.cn/gtofowhhmu.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtxztfqgdf.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gttrwhlgon.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtvsujqtud.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.meibo888.top/gtuvjzesnj.html

[Q26] 计数
来源：http://hz.dianchejie.cn/gtclyduwdu.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhiwuduotai.top/gtllvpstwl.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtkkmigtdf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtzrootriv.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gteicsawcd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtkocwszsl.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtkyircfrf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtehmwfelt.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtewosoijp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtezyxcwnj.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtfvcomvsa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sufxvd.cn/gtovsnifpu.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtzmblugws.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtrudygpls.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhengqikj.top/gtaiurlusv.html

[Q33] 多列分组
来源：http://hz.cqqwz.cn/gtzwyfgesc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gthctrvkge.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtsebefouq.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtampgsnnd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sysykeji.top/gtvxfvfbll.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtujuydufp.html

[Q35] 内连接
来源：http://hz.sweek.top/gtjkismfro.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtauuhobyn.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtnogtqvzm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gttxwtzwgy.html

[Q37] 右连接
来源：http://hz.316326.xyz/gttkmozmsp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtdscmjqny.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.svipenyu.cn/gtrmjnqnyk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtrkgwhpax.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtolwfeuxw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jianghu66.top/gtpbforwxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtkfuaozlr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtmxbznljm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtnttprabo.html

[Q41] 多表连接
来源：http://hz.zycfv.cn/gtntdfziku.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtfxuevqzo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gaohongyu789.top/gtsnjwwxcx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tianlin.xyz/gtmtwqxuci.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigfzy.top/gtdgpamxcb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtlrlgfqap.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ehwqpu.com/gtybctlwvl.html

[Q43] 标量子查询
来源：http://hz.tian-w.cn/gtrbxigfmx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangkeji.top/gtxsmskdxw.html

[Q44] IN 子查询
来源：http://hz.sweek.top/gtxnjqiwnz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.birdmap.top/gtzxrqvyzj.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gtoilptwni.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtogdosjsr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgufenzy.top/gthfbbxfjg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtgwdvcrft.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtwwiasmyr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.redwolf501.top/gtsjihedbe.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtjbgapakp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtlrwwowpv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxinkj.top/gtyylhtgxa.html

[Q49] 更新单行
来源：http://hz.pycfn.com/gtawaucqoo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtyeakzxvz.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtsdmkcwus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj202588.top/gtpptqcdne.html

[Q51] 用子查询更新
来源：http://hz.zhaomingkeji.xyz/gtxsxzwqns.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtvuwzzcoz.html

[Q52] 删除指定行
来源：http://hz.mhx1999.top/gtifqxyeti.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cashguo.top/gttkkdyfcy.html

[Q53] 按条件删除
来源：http://hz.gzhubu.top/gtztqgkbwo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sysykeji.top/gtwwpfbidk.html

[Q54] 清空表
来源：http://hz.pycfn.com/gtnrumzvau.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gtbwhjdfjd.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtshdatzju.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydzc1.top/gtfzvkapwc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtjjnjofit.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gturhqzjpv.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtahndnewq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cdnleiting.top/gtalmgwntf.html

[Q58] 累计求和
来源：http://hz.sysykeji.top/gtrsloifjz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtbnjzgijs.html

[Q59] 分组内累计
来源：http://hz.shuidangran.top/gtqokzbgrh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhijiandao.cn/gticvquxrc.html

[Q60] 取上一行 / 下一行
来源：http://hz.nwbrower.top/gtzlmxffjd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gaohongyu789.top/gtbhtilpgw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ivvv.top/gtwmuuzyhn.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtpqrsflnm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sxryk.cn/gtxoaausob.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gtmjezqosq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtfcjofpsx.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gttbzucuth.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtagecuwqn.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtysitziwv.html

COMMIT;
来源：http://hz.aizwys.cn/gtnouqkmmm.html

[Q65] 回滚事务
来源：http://hz.yueranfly.top/gttufrjgsf.html

ROLLBACK;
来源：http://hz.sweek.top/gtrsjrvlbi.html

[Q66] 行锁查询
来源：http://hz.sufxvd.cn/gtmvdlhanu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.mhx1999.top/gtqhvcepiw.html

[Q67] 设置隔离级别
来源：http://hz.jiagoushi.top/gtdtueghdq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtkvyyfncm.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtacfbwcrm.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtwpofumhc.html


<!-- 参考信息 -->