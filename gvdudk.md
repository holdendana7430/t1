代发 wailian999

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gthbgdugip.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtwruwpzbs.html

C#:   // 手写递归
来源：http://hz.smart0.xyz/gtjhxsxzda.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.fzhhl.top/gttxtnklce.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gtfwcpdjpd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtyuymfudn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtxyzfozyf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtmwksrsck.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtuvranjsy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gthtartpbg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.haohaochexian.top/gtfvtsimxl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtfbecirvv.html

================================================================================
来源：http://hz.xziqi.cn/gtlzthiejw.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtvrffqbmm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzgcvrzjc.html

[O01] 启动一个线程
来源：http://hz.jlsjyb.cn/gtcqomndqx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtoshowwzq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtfmhmgplr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhiwuduotai.top/gtkyrsekpn.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtlkbqmkxe.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gtbfbanjfz.html

Go:   go f()
来源：http://hz.zycfv.cn/gtvairvcir.html

Ruby: Thread.new { f }
来源：http://hz.cashguo.top/gtbqufscjy.html

C#:   Task.Run(() => F());
来源：http://hz.svipenyu.cn/gtbjxcvwot.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gthrprjqsp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtusnzpoxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtpqvsawki.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtekycwikw.html

TS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtpdwjccwx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ywan-chungtsiang.top/gtnwzulhhv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtcaszrqik.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtlfljhvli.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fzhhl.top/gtkhusejgm.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtzxvpdrix.html

Py:   with lock: shared += 1
来源：http://hz.jiagoushi.top/gtybqqttoc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtrqypwpnv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtmyumhtul.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtfnuzynuz.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtnfavgvae.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtnbamhyzr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.andypj.xyz/gtldroyceg.html

C#:   lock (gate) { shared++; }
来源：http://hz.guannengcc.top/gtetaorvim.html

[O04] 定义异步函数并等待
来源：http://hz.guannengcc.top/gtnqooboef.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtydkunzez.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtchorrwju.html

JS:   async function f() { await g(); }
来源：http://hz.aibaodan.cn/gtulfrbuzh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenzaomai.com/gtxxtonigg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gtpzylvtke.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtgzbxjvwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gtqzddyfjf.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtpnvverhv.html

[O05] 并发执行并等待全部完成
来源：http://hz.aizwys.cn/gtomfwepvo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangshuangyany.cn/gthqnhwivm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gtcsclewuv.html

JS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtogvxltde.html

TS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtygqctutp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtkmnzkpwh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtbcsacxpz.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gttnrlawzl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jlsjyb.cn/gtfiwsruhr.html

[O06] 使用进程池
来源：http://hz.pycfn.com/gtyffsnfno.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinghuilouyu.cn/gthefkjduy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtstqmngyd.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtnainfwus.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtraehmbva.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gthmetffll.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yangfankeji.com/gtpbcsvmoy.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtygugzwbi.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtdluvctks.html

================================================================================
来源：http://hz.xinyue.icu/gtdnzakejc.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gtyfxmyzrs.html

================================================================================
来源：http://hz.316326.xyz/gticwhvnyy.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtjpiqntmb.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtggruhjxh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtniwbormq.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtuwuxhtad.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtrzonqqtu.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gthesutgjk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtryjffyzr.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtpoaduptz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtfnxobbfu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtamghfgtl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yangfankeji.com/gtjyetocwd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtgdxxzjav.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtkrtfdhdj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tianlin.xyz/gtfmvnaikj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtxuyrbgfc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtbkdihrgz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtrdhbxlgf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtyeknufsr.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtltvileyf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangshuangyany.cn/gtojyatqwt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhoulong.xyz/gtlyuwwyei.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtxjcrwhxu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtfmxfvbgs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jiagoushi.top/gtxydnujsw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangdashe.top/gtkgitzldp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtvfhueftr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gtfswtwwgp.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtllptfdxl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.mhx1999.top/gtuyvumgdj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtqwmfudcf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtytbmdawu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtovycoodb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtwjsfxwqi.html

Go:   len(arr);  len(m)
来源：http://hz.cashguo.top/gtcnnddgir.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtwhefycok.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtholgdhhg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cqqwz.cn/gtahiymjmt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtgcmnwrst.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.svipenyu.cn/gtcnlkvltj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.redwolf501.top/gtskeymduk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtblwsznoy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cashguo.top/gtovpwnlmb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sxryk.cn/gtyaqbtfea.html

Ruby: a == b
来源：http://hz.quarkkingdee.top/gtcosdkkfm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gtwgkozubf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hysaishi.cn/gtkarygdel.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinyuanbaomall.cn/gtklswwivj.html

PHP:  if (empty($x)) {}
来源：http://hz.snrcjt.cn/gtoxorcpem.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtqsxscotx.html

TS:   if (x == null) {}
来源：http://hz.zhaomingkeji.xyz/gtlkgwztbi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtgtzeumoo.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtnrfckcpx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nwbrower.top/gttsvuoyfx.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gthwantydj.html

[P07] 防抖与节流
来源：http://hz.vqdsnc.cn/gtlhuqutoz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigufen.top/gtfxoidsge.html

PHP:  // 手写时间戳比较
来源：http://hz.aibaodan.cn/gtoyyxtzmd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtjzxjresq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtneyuxtrb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gteqhqrhna.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxuanxn.top/gtcvwggtnc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnqzz.top/gtzspjcaos.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtrnxomash.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtmnpmlgch.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aibaodan.cn/gtcfdeazdh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daria6918.cn/gtjogmyrzq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtyyhjcjdc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtiqrjaqae.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gtolfcwgca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guowangkeji.top/gtsiouaphw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jlsjyb.cn/gtsbntymwk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gtadnccunv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkpxgihzv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxuanxn.top/gtchencsep.html

================================================================================
来源：http://hz.yvedp.cn/gtvmhwsgcm.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtvfevcymv.html

CREATE TABLE users (
来源：http://hz.meibo888.top/gtypbvkzbi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtdfyhryhf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtseloljkj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gtfcwbalnt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtcouruclw.html

);
来源：http://hz.yj20258.top/gtfxunnbfc.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangtech.top/gttakjhwfo.html

CREATE TABLE orders (
来源：http://hz.bjfxy.top/gtxazsymme.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gtbbnxdnar.html

user_id INT NOT NULL,
来源：http://hz.yongpay.top/gtsvjnjeyi.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtajzyjojp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gtvwvbpoeq.html

);
来源：http://hz.dashuyun.cn/gtcbwfgtqa.html

[Q03] 增加列
来源：http://hz.shangyingyoupin.top/gttobzainc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gtuugvknbo.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gtltmkmxdt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.svipenyu.cn/gtasbwzyei.html

[Q05] 重命名列
来源：http://hz.pengpengdd.cyou/gtraknmivc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtfeiegvcx.html

[Q06] 删除列
来源：http://hz.hnqzz.top/gtkrfocluo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtqcjpeuch.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtqizrjolx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gthjfmvxga.html

[Q08] 创建普通索引
来源：http://hz.jinyuanbaomall.cn/gtavzkjgjc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gtgihfzzei.html

[Q09] 创建唯一索引
来源：http://hz.shangyingyoupin.top/gtrqbrbclt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtzhbrrbei.html

[Q10] 插入单行
来源：http://hz.yueranfly.top/gtwtskwima.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtfygoqsth.html

[Q11] 一次插入多行
来源：http://hz.tianlin.xyz/gtttxautfz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtnmgcoeno.html

[Q12] 插入后取自增 ID
来源：http://hz.fengsongda.top/gtdnsnqquw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtlwxxmitb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtgcigdybd.html

[Q13] 忽略重复插入
来源：http://hz.zhengqikj.top/gthfmoauen.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtbeydobqw.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gtkxocvabq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtpdkdkjay.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtcuyaphiy.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gtmsgmktuc.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtfdwtgpgi.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtyxsthauq.html

SELECT id, name FROM users;
来源：http://hz.sufxvd.cn/gtsqikhdqc.html

[Q17] 条件查询
来源：http://hz.xuetiantiany.cn/gtttpfnbpw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guannengcc.top/gtqcpypdfb.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtjxyspqvy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtxthdulha.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtssxyznzg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.svipenyu.cn/gtjpwelyns.html

[Q20] IN 列表
来源：http://hz.jinghuilouyu.cn/gtwnqxqosp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtyyxfbqwj.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtsuynxslx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.haohaochexian.top/gtgmevuvqh.html

[Q22] 排序
来源：http://hz.ydjk.org.cn/gtqklwbdcy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.52xcode.cn/gtwpawiwqz.html

[Q23] 分页
来源：http://hz.snrcjt.cn/gtsubhftfa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtryaqpfso.html

[Q24] 去重
来源：http://hz.hfpthk.cn/gtduxrjhbf.html

SELECT DISTINCT city FROM users;
来源：http://hz.svipenyu.cn/gthujnpiny.html

[Q25] 只取前 N 条
来源：http://hz.guowangkeji.top/gtnbhswczd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtrjlnpmtq.html

[Q26] 计数
来源：http://hz.hfpthk.cn/gttelgblgj.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhongyouzk.top/gtkfrzovgf.html

[Q27] 条件计数
来源：http://hz.pengpengdd.cyou/gtkpxonqnj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhiwuduotai.top/gterdiylzz.html

[Q28] 求和与平均
来源：http://hz.jinqigfzy.top/gtyggvzyqk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shangyingyoupin.top/gthbvuhwlq.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gteeochtaz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yvedp.cn/gtuildajco.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtphhwkmmo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtmbhlfznq.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtyikcrtke.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtwalnluir.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gtuwuabmlo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtxixxspdw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gthcmbtxih.html

[Q33] 多列分组
来源：http://hz.feifeiyinyue.top/gtfcopvuvd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xylfe.cn/gtexprfdoj.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtliranpra.html

SELECT * FROM (
来源：http://hz.cucudq.cn/gtdtcdgnid.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tianlin.xyz/gtbouhytyu.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gttlkocjio.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtknpwmlnn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtfzjfymok.html

[Q36] 左连接
来源：http://hz.jinqigufen.top/gtqwjslmqf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtjhjzlzwz.html

[Q37] 右连接
来源：http://hz.sweek.top/gtiwbschtt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ivvv.top/gttbegguvo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gtrbypzzwp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtpthichbs.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtmogtmluz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gtpxeijzqy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtlducdpdj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gtyfwnzyyr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydzc1.top/gtqgokfpjj.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtqkuugzhw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ivvv.top/gtsyxkrqcb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtxigxwixw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtevspqlzc.html

[Q42] 连接条件附加过滤
来源：http://hz.dashuyun.cn/gtyyvvhutk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtudeonemh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shuidangran.top/gtgwauhvvc.html

[Q43] 标量子查询
来源：http://hz.aizwys.cn/gtxcsgmmla.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtvthimmxf.html

[Q44] IN 子查询
来源：http://hz.ydjk.org.cn/gtwsptppkm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangdashe.top/gtxggddxgy.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgfzy.top/gtskcuknal.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtqamiqfsh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hywenlv.cn/gtngreobfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtiltnbbkp.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gtvxlxlcfu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtrtiwyerk.html

[Q48] CTE 公用表表达式
来源：http://hz.mhx1999.top/gtyarrxffz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jlsjyb.cn/gtgkadivdg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtalugfndj.html

[Q49] 更新单行
来源：http://hz.jinqigfzy.top/gtlztlrvdv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtyrmzrxta.html

[Q50] 批量更新
来源：http://hz.pycfn.com/gtqevvpppc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gttqpmitjf.html

[Q51] 用子查询更新
来源：http://hz.jyoumei.cn/gtimtjcixs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gtpzyihvpf.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gtanraanni.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gtujtohbmb.html

[Q53] 按条件删除
来源：http://hz.jianghu66.top/gtyoujhvto.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtdyaosmvn.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtzymapyyy.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gttknxaurz.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gtzmczfexz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sufxvd.cn/gtkbtprsvs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtbettennk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtfmrxwaxd.html

[Q57] 行号
来源：http://hz.xinyue.icu/gtxcnrieho.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gttdaxekly.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtkvicjhnk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuetiantiany.cn/gtcgwuvcxb.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtwkuzasjg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xylfe.cn/gtsklctaop.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtlpmjxqcz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydzc1.top/gttvroaogf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtngbeajrl.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtcxmnqicg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gthewrogpo.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtkneyllkt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gthpqtmlak.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtlftvodzy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jianghu66.top/gtxpssejrk.html

[Q64] 提交事务
来源：http://hz.andypj.xyz/gtxzqccuxq.html

COMMIT;
来源：http://hz.zhengqikj.top/gtczwwskxc.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtyruvuqcw.html

ROLLBACK;
来源：http://hz.ywan-chungtsiang.top/gtiivchnsv.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gttpugclvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtervcrtpa.html


<!-- 参考信息 -->