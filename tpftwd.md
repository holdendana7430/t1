代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ybcxt.top/gtzxvgzqyl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtduqiawir.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sweek.top/gtojukoqin.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtxgiogkle.html

Java: new Thread(() -> f()).start()
来源：http://hz.jianghu66.top/gttsoeaoys.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtdyldrcys.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtoaceyxvh.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtybadzvli.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtnqewenpi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtdxvdxwos.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.kuanghao11.cn/gtpjxjadvy.html

JS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtnpwukqxa.html

TS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtrukxwexm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtevwubprw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtpiaddnrb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtxhiddurl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gtswnuvvpu.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangkeji.top/gtdifyeqzg.html

Py:   with lock: shared += 1
来源：http://hz.chenlongwang.top/gtekvvzytm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtoqrrkbux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtwerfcshj.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtumkfebbh.html

Java: synchronized (this) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtxjjatwaw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.316326.xyz/gtibkccjaa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gtsgmirwvo.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtidqgydwf.html

[O04] 定义异步函数并等待
来源：http://hz.andypj.xyz/gtbnouqbys.html

Py:   async def f():⏎    await g()
来源：http://hz.xuetiantiany.cn/gtntxunipd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtuybojvok.html

JS:   async function f() { await g(); }
来源：http://hz.cheryme.top/gtpzlfpohv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zdqjudy.top/gtqglhmmmg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gthcgrimxz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guowangkeji.top/gthvmnwosh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zdqjudy.top/gtcepgyygf.html

C#:   async Task F() { await G(); }
来源：http://hz.fzhhl.top/gtmeocgmsl.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtzcwkaznq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtljkxoamu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtljtijfhq.html

JS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gttvuugpul.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtvlsxutdk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtpqnzzwar.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtzblaedrz.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtsogzfbst.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dashuyun.cn/gtiyrvxxnn.html

[O06] 使用进程池
来源：http://hz.fengsongda.top/gtcquapxro.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtlkkdlwvr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhoulong.xyz/gtmrvoovyd.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtiwdxbqeq.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtljtfrsny.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtsxcwnfqi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.bjfxy.top/gteisddpfb.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtuisckckz.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtqyzdwcgq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtiptcurxt.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtcdmuqcwo.html

================================================================================
来源：http://hz.xuanzx.com/gtcsqjmmfa.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtidmgzimo.html

Py:   str(uuid.uuid4())
来源：http://hz.dashuyun.cn/gtrydteujk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtptkzrmts.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtyicfwqcc.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtgsyqkhxu.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtumbiifgu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtoaxqoyto.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtxrjugssa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtnubfthpx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gthztcvoqt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtgzccgjda.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtemozdryx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jiagoushi.top/gtixviqmpn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gteyrlmeze.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yangfankeji.com/gttysqdavj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtqkflxaox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtdemdajje.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shuidangran.top/gtlnvghnkw.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtwevsflll.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtsosljklq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ppjwa.cn/gtitginqec.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtormwtijt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtmexrgqti.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenzaomai.com/gtvcrjvlpo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.svipenyu.cn/gtznlsnzzx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtqkaruhum.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtiyuzclos.html

[P04] 求长度
来源：http://hz.gotoacloud.top/gtpdmahzid.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gtdengrtuz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtbsvpzcid.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gttdiqptft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtjvwwijsg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtytavqimk.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gtkgvryzsp.html

Ruby: x.length;  x.size
来源：http://hz.bjfxy.top/gtrqhvrcmy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhaomingkeji.xyz/gthbytcroj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jlsjyb.cn/gttqcusxun.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtdjxeccdl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgfzy.top/gtdeeidvhg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gotoacloud.top/gtkepzbkup.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtbowypcdg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtvichfmvp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydzc1.top/gtlagruamn.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtxajyqzec.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.havefunace.top/gtvbohugty.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guowangkeji.top/gtiowwkcba.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtpxghbarr.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtqdcwosek.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtckedolpx.html

TS:   if (x == null) {}
来源：http://hz.tianlin.xyz/gtrkstzabm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cucudq.cn/gtarlurlgq.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtieakdlet.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtifeerbbk.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtqqyzjhgj.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gtsqcfaepv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fzhhl.top/gtanugwgdh.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtfaxgnsqk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtqcmwmqux.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtjbtobwrr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.smart0.xyz/gtvyecgcdp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258888.top/gtrugzzzyu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gtxkyakfgj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtsbtosqmw.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtjcifcxwp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xziqi.cn/gtgweszknj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangtech.top/gtsqovgovy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtihlqipme.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dianchejie.cn/gtusemxvyy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtqbamaijh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhengqikj.top/gtdxzgpcul.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.snrcjt.cn/gtjzlfbwli.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.feifeiyinyue.top/gtwwuuikno.html

================================================================================
来源：http://hz.0kj1m.cn/gtiieulttw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yanxiufei.cn/gtlamlhjts.html

================================================================================
来源：http://hz.hfpthk.cn/gtuepnbqrt.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gtympuhazl.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtpokoygqc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtzzrheogy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtprbmoooa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xinyue.icu/gtsknfacxw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtgwgcldel.html

);
来源：http://hz.yj20258.top/gtjrdzxcfz.html

[Q02] 创建带外键的表
来源：http://hz.chenlongwang.top/gtqlzgsnte.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gtnjquzqul.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtwbxajxmo.html

user_id INT NOT NULL,
来源：http://hz.ydjk.org.cn/gtpuisrjcx.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtdvkccjmj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gtafhvklsf.html

);
来源：http://hz.gotoacloud.top/gtwdbrlwlg.html

[Q03] 增加列
来源：http://hz.andypj.xyz/gtgqavexuh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.0kj1m.cn/gtjqdviaqw.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gtgdsjhgbc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtsdkugjhc.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtbwuwrins.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigufen.top/gtrtkmhidk.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtzqgtrbad.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gttbmnjbzj.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtepscltej.html

DROP TABLE IF EXISTS orders;
来源：http://hz.quarkkingdee.top/gttqcfyolq.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtagvyhyip.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtgamqwfnh.html

[Q09] 创建唯一索引
来源：http://hz.yuanzhike.top/gtcoqlggbt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtsejnxtcx.html

[Q10] 插入单行
来源：http://hz.cdnleiting.top/gtkivfthfe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pengpengdd.cyou/gtkplyumxb.html

[Q11] 一次插入多行
来源：http://hz.52xcode.cn/gtpdleqixw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hfpthk.cn/gttlhhocju.html

[Q12] 插入后取自增 ID
来源：http://hz.pycfn.com/gtteblvekt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtxfrsexxs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gtwrwqwcyf.html

[Q13] 忽略重复插入
来源：http://hz.daria6918.cn/gtcnbvzlud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.c1oappe.top/gttzjvqwwo.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxinkj.top/gtukzlobuz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yangfankeji.com/gtnqpnpwed.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtcwyjkqaz.html

[Q15] 查询全部
来源：http://hz.zdqjudy.top/gtvtkaxdcr.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtytxmkdmi.html

[Q16] 查询指定列
来源：http://hz.ivvv.top/gteyqxjibn.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gthnzikqpn.html

[Q17] 条件查询
来源：http://hz.zhongyouzk.top/gtpglhxwet.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gtbzsowucq.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtelniaxnw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtuvcvjbnd.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtpqrtqbmy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tian-w.cn/gtahzzjiwo.html

[Q20] IN 列表
来源：http://hz.gotoacloud.top/gtwdioxtzm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.316326.xyz/gtleysjtlq.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtqfyelzej.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sxryk.cn/gtzynbwxfq.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtzmirflyq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtptwfhgkd.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtheziolxg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtugrcefxh.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtbtdxadqz.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gtsuttazey.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtzifkuaju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuanzx.com/gtojdphejy.html

[Q26] 计数
来源：http://hz.chenzaomai.com/gtdlczpoht.html

SELECT COUNT(*) FROM users;
来源：http://hz.fengsongda.top/gtmztscjjv.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtdghxadjr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtvghxhfsl.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtmekvhumo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhiwuduotai.top/gtjtjiynzh.html

[Q29] 最大最小值
来源：http://hz.guannengcc.top/gtdrshqvhx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yuxming.cn/gttvlapgno.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtzjrnjtss.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtnigohrfq.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtcfyglavm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yonumen.top/gtyjzomflx.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gturokuvnw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtkhlpayht.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.0kj1m.cn/gtpdeyttkk.html

[Q33] 多列分组
来源：http://hz.wangshuangyany.cn/gtezhzntnv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ppjwa.cn/gtxmpnmdup.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtvuvudteo.html

SELECT * FROM (
来源：http://hz.yonumen.top/gtwjwhltvr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtrafczdgd.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtkscenzql.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtsetntqoz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtodowtkbb.html

[Q36] 左连接
来源：http://hz.zhijiandao.cn/gtmtfcsvmp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gthcnomhon.html

[Q37] 右连接
来源：http://hz.nanxuanxn.top/gtuaknqtks.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sxryk.cn/gtoqiwyhwc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ybcxt.top/gtkfbyzdln.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtzxpldznh.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtklfhuytt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuanzhike.top/gtwfvuttjo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gtmxdxoyzj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.birdmap.top/gtcsaticnx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aibaodan.cn/gttgqkooyr.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtpnmijxmt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aizwys.cn/gtabjreewy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ppjwa.cn/gtmctuesif.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangkeji.top/gtzjfqpeny.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gteasqdwvn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtcyaaqiuw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pycfn.com/gtchkglcwj.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtyhelguxo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtzeusmhps.html

[Q44] IN 子查询
来源：http://hz.0kj1m.cn/gtpdndoybc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtlenqwyrs.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtefhnzcgr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtdtwumrhv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gtqbpovryo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtnsrghdoh.html

[Q47] 与平均值比较
来源：http://hz.hywenlv.cn/gthhkydulj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtrrsvpanz.html

[Q48] CTE 公用表表达式
来源：http://hz.wangdashe.top/gtavtszgiz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hysaishi.cn/gtupkribtz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtsysrzikd.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtopmjehbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.birdmap.top/gtorijstmt.html

[Q50] 批量更新
来源：http://hz.jqgfzy.top/gtcjacukqq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxuanxn.top/gtngaczpug.html

[Q51] 用子查询更新
来源：http://hz.hywenlv.cn/gturbuehzh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtmsgpwdkl.html

[Q52] 删除指定行
来源：http://hz.aibaodan.cn/gthkahywyl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnqzz.top/gtglpgxnhm.html

[Q53] 按条件删除
来源：http://hz.gzhubu.top/gtmijmbulg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sxryk.cn/gtthjwhutr.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtjzlblwye.html

TRUNCATE TABLE logs;
来源：http://hz.ppjwa.cn/gtahyhbgky.html

[Q55] 排名（并列占位）
来源：http://hz.hongshengwenyu.top/gtbqomnrxt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cheryme.top/gtyxjmgehd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258.top/gthvmtiwbs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtzznafcbp.html

[Q57] 行号
来源：http://hz.gzhubu.top/gtqvlulqqd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtqwlgxbdc.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gthldgytkz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtevjqduzr.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtbqbyggzz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gthhbzkuae.html

[Q60] 取上一行 / 下一行
来源：http://hz.ybcxt.top/gtzqriygtq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jiagoushi.top/gtdzopuevf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtmpuswkdd.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtkfyntzcg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtxpdwbbef.html

[Q62] 分组占比
来源：http://hz.zhengqikj.top/gtbfafyngk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtzyhwpifu.html

[Q63] 开启事务
来源：http://hz.shanyushiyangtech.top/gtmpswrfvk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtdmqfwmxc.html

[Q64] 提交事务
来源：http://hz.xylfe.cn/gthdlkmnul.html

COMMIT;
来源：http://hz.316326.xyz/gttboqdrkk.html

[Q65] 回滚事务
来源：http://hz.yueranfly.top/gtlocnptwv.html

ROLLBACK;
来源：http://hz.zhongyouzk.top/gtenitcuow.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtgtqobtrq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtpifhyemx.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtmagybwgv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtpcpiqlfk.html

[Q68] 保存点
来源：http://hz.jinqigfzy.top/gtlzyqgxif.html

SAVEPOINT sp1;
来源：http://hz.shanyushiyangkeji.top/gtglghpzpm.html

ROLLBACK TO sp1;
来源：http://hz.jyoumei.cn/gtgdxymsxw.html

[Q69] 查看执行计划
来源：http://hz.ivvv.top/gtyauaxfjk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.quarkkingdee.top/gtjaobbiin.html

[Q70] 更新统计信息
来源：http://hz.gzhubu.top/gtvjlpyzpm.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gtbaohgpki.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtlwnfggde.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yongpay.top/gtrzjvxeth.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtobkrflgn.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gthlzppdgf.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gtffbnpxqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fzhhl.top/gtbshwlfyr.html

[Q74] 强制使用索引
来源：http://hz.chenlongwang.top/gtfhzhqsxn.html


<!-- 参考信息 -->