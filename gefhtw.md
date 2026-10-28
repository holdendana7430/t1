代发 wailian999

================================================================================
来源：http://hz.andypj.xyz/gtsebtiksm.html

O. 并发与异步
来源：http://hz.shuidangran.top/gtfdthbryh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqelyhfos.html

[O01] 启动一个线程
来源：http://hz.zhoulong.xyz/gtwwnrzpvi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtcijuqsgm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtvhtgqplz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtrtonsoen.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtrpaxebgr.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtispzyutj.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtvstqgaed.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtlovtnmoc.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtuwvpevww.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gtdylhkwic.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gtaxunhvlp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtenshkfei.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtttkawcyt.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtidmffzea.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtxlkokwlc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hfpthk.cn/gtdimwovju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtqhptgiji.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtfjktjuxd.html

[O03] 加锁保护共享数据
来源：http://hz.redwolf501.top/gtjnuqzitm.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtgavyjshd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gteevpvjfa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gthwpazyck.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gthcbgdpbg.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtkhhrtgol.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cashguo.top/gtnkdptvrc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtjijpunfj.html

C#:   lock (gate) { shared++; }
来源：http://hz.9152youxi.cn/gthosgnznd.html

[O04] 定义异步函数并等待
来源：http://hz.shuidangran.top/gtpgdrfupw.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gtysznadmv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtcsbetnwi.html

JS:   async function f() { await g(); }
来源：http://hz.hnxiangtu.top/gtcjqqmzta.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtxxzwghiq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xingfuxueyuan.xyz/gtlifczzda.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtegyieneu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shzxlz.cn/gtvpohmvyv.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gtgefrtaag.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gttxqedmea.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gtcqaeisja.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtrkzrjxaz.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtbrgkqerw.html

TS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gtgwckgjjn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtuxekxkbh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gogol.net.cn/gtlwaxdofw.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtinbvhmjl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtxjdxtkyy.html

[O06] 使用进程池
来源：http://hz.jinqigfzy.top/gtebvnzzzk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtqgdhzsaq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtsfmuroca.html

JS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gttinelucp.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtovzmckpk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtowfvyewq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jlsjyb.cn/gtofurzprs.html

Ruby: // fork 块
来源：http://hz.wangdashe.top/gtvttxeilb.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtjiadvwwt.html

================================================================================
来源：http://hz.aizwys.cn/gtqflywqor.html

P. 常用工具函数
来源：http://hz.tanke756.top/gtdfhnqoaq.html

================================================================================
来源：http://hz.bjfxy.top/gtokjkxbfo.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtmvdhdism.html

Py:   str(uuid.uuid4())
来源：http://hz.zhongyouzk.top/gtuzpjjyyx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.snrcjt.cn/gtyfuugzms.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtjkjpvfka.html

TS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtppmsxqvk.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgfzy.top/gtqaigrlfv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtgwziqugh.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtuzectyuw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hfpthk.cn/gtjudwxjlm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtmhpaknlk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ehwqpu.com/gtvwxulhtf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtxnmkdgyr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gttfglryva.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.c1oappe.top/gtlrazbnaa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtbzicpbjt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.havefunace.top/gtfsqqcecl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtilgstjjt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtulhzesjv.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtbbxgqysu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xylfe.cn/gtbtfihzxx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuanzx.com/gtntnleqen.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtxujtlclm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gthkdvlbas.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangshuangyany.cn/gtdaiiomku.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hysaishi.cn/gtwoygziqv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtdtuvlaom.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhaomingkeji.xyz/gtfzuiugim.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtropjyoqg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtcsqgolei.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gthhirtrxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtsqkdjbih.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtxtrmvfrw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhijiandao.cn/gtmaxetomt.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtcvejylpn.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtaiphkdfb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tian-w.cn/gtxjuqpsyz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydzc1.top/gtacbvtuym.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aibaodan.cn/gtidilfleh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtxkdkavpd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtujdeblrs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gttyeiigol.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtqzkspxrw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gttptaypcm.html

Ruby: a == b
来源：http://hz.feifeiyinyue.top/gthqzolpjf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gthoogvlti.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtqxmwugrw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtidlimtoy.html

PHP:  if (empty($x)) {}
来源：http://hz.smart0.xyz/gtnqgdlabf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.mhx1999.top/gtqisimdbn.html

TS:   if (x == null) {}
来源：http://hz.nanxuanxn.top/gtvyfmlknw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtgjtzpxru.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtkfjcaqhv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tanke756.top/gtvkgskpco.html

C#:   if (x is null) {}
来源：http://hz.yj202588.top/gtyzujairl.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtzleuzvoy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangshuangyany.cn/gtxqayvpso.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtceuhpryi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gttmntjrxn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtbvspnwaa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gogol.net.cn/gtorytaiwc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hfpthk.cn/gteppafcyk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtfanvabvg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.feifeiyinyue.top/gtapwwldfs.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtssjocabk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhoulong.xyz/gtnmzvqhuv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtydswgjem.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtranrnnfb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daria6918.cn/gtagbvhngv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.vqdsnc.cn/gtlarnzwud.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtazmzlrrz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.bjfxy.top/gtfvwmjwto.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtgfbtfyvq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthsofdvgg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ywan-chungtsiang.top/gtzgvzfgcx.html

================================================================================
来源：http://hz.jinqigufen.top/gtqboschpg.html

[Q01] 创建表
来源：http://hz.xinyue.icu/gtstyhpsow.html

CREATE TABLE users (
来源：http://hz.sxryk.cn/gtilnolszp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtkcqwglit.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtmebywhnj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtvtjfcxem.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangshuangyany.cn/gtpryvyfyk.html

);
来源：http://hz.jlsjyb.cn/gtnugfbrud.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtjjmgthpr.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gtmzwgmkic.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtbhlmjlvq.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gtfejxxtnn.html

amount DECIMAL(10, 2),
来源：http://hz.hnqzz.top/gtgdpojdos.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtywlmajlk.html

);
来源：http://hz.svipenyu.cn/gtjgerjnws.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtsnehdnyt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtvpjfhdyv.html

[Q04] 修改列类型
来源：http://hz.nanxuanxn.top/gtmvsoqmbg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtodfjgscf.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtdwynxmja.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cheryme.top/gtoqkghpep.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtcprbqfxs.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gteqjorohw.html

[Q07] 删除表
来源：http://hz.hnxiangtu.top/gtojmjfdzs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuanzx.com/gtiqdslwkl.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtqodlklno.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtjxlxjqkf.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gtvtzskgou.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtigcriflm.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtzgyoilyj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gteyapoppt.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtbvvdnvlx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtqfeomaga.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gttadwhfpc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydjk.org.cn/gtfysoiiej.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtzogteiya.html

[Q13] 忽略重复插入
来源：http://hz.smart0.xyz/gtuatgulxw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnxiangtu.top/gtytiqbcsv.html

[Q14] 存在则更新（upsert）
来源：http://hz.daxiang520.top/gttnlvbjhv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtkpizytak.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aizwys.cn/gtulhzszzq.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtwjlwujts.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtihadxbzy.html

[Q16] 查询指定列
来源：http://hz.yj202588.top/gtuctaxyko.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gtxgxiirfr.html

[Q17] 条件查询
来源：http://hz.0kj1m.cn/gtedjvrate.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtofarfelq.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtkfwmreny.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gttlapfnvi.html

[Q19] 范围查询
来源：http://hz.jinghuilouyu.cn/gtvrkoxrug.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.quarkkingdee.top/gtajttfvbe.html

[Q20] IN 列表
来源：http://hz.yanxiufei.cn/gtqevapofl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtmooshwyb.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtpnitsktz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgfzy.top/gtkexwszat.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtcmnvknqb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yueranfly.top/gtmjaffess.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gtcvsyjvis.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gtksrdmycq.html

[Q24] 去重
来源：http://hz.wangdashe.top/gtnpkxyvyl.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtgxbcfahw.html

[Q25] 只取前 N 条
来源：http://hz.jinyuanbaomall.cn/gtxddiqnnl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nwbrower.top/gttwjqnlwo.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gthcxmkcij.html

SELECT COUNT(*) FROM users;
来源：http://hz.yueranfly.top/gtkninjemh.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtcdcxvxcm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gtbjqkcrjx.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtlhwyaubz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtjngyngcl.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtbhkjjytl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.0kj1m.cn/gtwtzphovb.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtrvdgjkca.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtuxbysuen.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gthdgoaceg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtttrnjlua.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtpvfysocg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gttdxauoek.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtxbacjdfx.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtwoyyguat.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenlongwang.top/gtqufbxtfa.html

[Q34] 每组取第一条
来源：http://hz.zhoulong.xyz/gtvbzzhcib.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtzvvjvssj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dashuyun.cn/gtbebpjgpi.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtjfirjwgb.html

[Q35] 内连接
来源：http://hz.guowangkeji.top/gtqzstlqdy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtxnbtezft.html

[Q36] 左连接
来源：http://hz.ydjk.org.cn/gthqwzlesx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtggcwchxf.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gtwoffashu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gzhubu.top/gtlivxfxxm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gtkfzehije.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tian-w.cn/gtinhjbqte.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtfrhwxrld.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangdashe.top/gtcfxflhey.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtqjcdltgx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.andypj.xyz/gtrxlevtdx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtwlimbeik.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtbqekhuox.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fzhhl.top/gtxzpobuji.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtvyqhpoky.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhiwuduotai.top/gtzyrjenyr.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gttqnsfggr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xingfuxueyuan.xyz/gtpgmwbqgv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gtgimxurvf.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtkiijzdxn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gtdgizieso.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtdirgohxt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.birdmap.top/gtermwiajm.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gthafvimxd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtordehbbr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gthtimjdvj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtggiunwps.html

[Q47] 与平均值比较
来源：http://hz.pycfn.com/gtuffnvmgs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangkeji.top/gtkjhejenz.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtcsnxkrhe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guowangkeji.top/gtlrilfmfq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shzxlz.cn/gteqawekba.html

[Q49] 更新单行
来源：http://hz.pengpengdd.cyou/gtvdwjkowe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtphbonmue.html

[Q50] 批量更新
来源：http://hz.52xcode.cn/gtmqllsuqg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yongpay.top/gtscmiebdm.html

[Q51] 用子查询更新
来源：http://hz.bjfxy.top/gtcqdxnern.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hysaishi.cn/gtzvtmrszf.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtjzvyclje.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtvgepyfar.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gticvpruli.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtmmofbxzt.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtwmugrpom.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtvcuomaix.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtgsvxveep.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtdedkdpbl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtutbihbca.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fzhhl.top/gtoostrqpp.html

[Q57] 行号
来源：http://hz.yongpay.top/gtyecxzpqw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xylfe.cn/gtnoqshtis.html

[Q58] 累计求和
来源：http://hz.zhaomingkeji.xyz/gtrougguor.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtmcstgbav.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtwnznmhpl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shzxlz.cn/gteoevfbgz.html

[Q60] 取上一行 / 下一行
来源：http://hz.jyoumei.cn/gtcagjhxma.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sysykeji.top/gtjanrvlek.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sxryk.cn/gtytsxqiae.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtsdktobye.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtqkyoofwn.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtmgcfzcfa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtlewzlrha.html

[Q63] 开启事务
来源：http://hz.yj20258.top/gtsaxiidfs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xinyue.icu/gtowddukwc.html

[Q64] 提交事务
来源：http://hz.daria6918.cn/gtfznkeegc.html

COMMIT;
来源：http://hz.gzhubu.top/gtfceshoom.html

[Q65] 回滚事务
来源：http://hz.yanxiufei.cn/gttlclfnik.html

ROLLBACK;
来源：http://hz.yuanzhike.top/gtmfsisysh.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtavdfjmhy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydzc1.top/gtajvtcjiw.html

[Q67] 设置隔离级别
来源：http://hz.chenjidiqi.icu/gtpimxmrka.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtdernatvb.html

[Q68] 保存点
来源：http://hz.yongpay.top/gtxpohcjbs.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtoomgiwct.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtzmqwfobl.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gttchxnzxf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtifgwxdke.html

[Q70] 更新统计信息
来源：http://hz.jianghu66.top/gtlajdbxqa.html

ANALYZE TABLE users;
来源：http://hz.zycfv.cn/gtqiflcfom.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gttlhltxwv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtfbkktxmc.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtdzhftpra.html


<!-- 参考信息 -->