代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ywan-chungtsiang.top/gtwxnwajbm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtskqejumu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jiagoushi.top/gteyjbjfsn.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtwlnwshgp.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtnmrpbdoi.html

Go:   go f()
来源：http://hz.shangyingyoupin.top/gthijwpger.html

Ruby: Thread.new { f }
来源：http://hz.shzxlz.cn/gttjwvfiyw.html

C#:   Task.Run(() => F());
来源：http://hz.guannengcc.top/gtlbarmkxb.html

[O02] 使用线程池
来源：http://hz.meibo888.top/gtiqtbpqpf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtwidrhbnf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pycfn.com/gtmojyljsg.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtfbfjhzfk.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtqacjunla.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtnoidnqey.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gthyhtazeq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtqwtfcvte.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtimkwcbbn.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtfschivde.html

Py:   with lock: shared += 1
来源：http://hz.chenjidiqi.icu/gtizdcxwlo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtuhrtzmpp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtcsiozlkx.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtorzkzevb.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtmjgwivqr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtnvglsjmb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtturkfsgi.html

C#:   lock (gate) { shared++; }
来源：http://hz.nwbrower.top/gtahkkfick.html

[O04] 定义异步函数并等待
来源：http://hz.chenjidiqi.icu/gtozxlpjer.html

Py:   async def f():⏎    await g()
来源：http://hz.yonumen.top/gtwogjeuiy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtvfqtwvgs.html

JS:   async function f() { await g(); }
来源：http://hz.redwolf501.top/gtwttfhvzd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtawglcwfv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yongpay.top/gtsxfxbsta.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gtlczklfab.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangkeji.top/gtmylzqyok.html

C#:   async Task F() { await G(); }
来源：http://hz.dashuyun.cn/gtknerurhm.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gttwjgriaq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtydoyfbap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pycfn.com/gtqjyvqovg.html

JS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtqjvqfuyg.html

TS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gthturnpdw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gtrgvphavr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gtlopvboik.html

Ruby: threads.map(&:join)
来源：http://hz.aizwys.cn/gtqdxwbibi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aizwys.cn/gtbyywhvvf.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtpspioxqc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.vqdsnc.cn/gtpgdixfah.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtvovlaaql.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtzluyqtsn.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtwwpxgfoq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuetiantiany.cn/gtibbyqlrw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtzcvnnypc.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtvegeyxsn.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtsrajdmuu.html

================================================================================
来源：http://hz.mhx1999.top/gtdtwxosju.html

P. 常用工具函数
来源：http://hz.birdmap.top/gtnkrzaenq.html

================================================================================
来源：http://hz.gotoacloud.top/gtwzildsdo.html

[P01] 生成 UUID
来源：http://hz.hfpthk.cn/gtqlnufdee.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtovjdlvsl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtgvxkiqnt.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtxqjcsdrx.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtexjcubbp.html

Java: UUID.randomUUID().toString()
来源：http://hz.guowangkeji.top/gtlqdinnwj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gthuabtgfg.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtueaebmem.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtiydrsmgk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtqqfhrkuk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gteybuxyoc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yongpay.top/gtmyhexzqq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cqqwz.cn/gtynukgaug.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gttfazqbqg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gthzddpfhn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hysaishi.cn/gtzslyxtoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gtxthwpyxe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yonumen.top/gtgrbgufxv.html

[P03] 生成短随机字符串
来源：http://hz.ivvv.top/gtcemjnbuz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gtzxjqddfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtokfyvaqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtezrkbrtl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tian-w.cn/gtjghjhpau.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aizwys.cn/gtbxupwnjq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jiagoushi.top/gtuoxsrptw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtnpehbjla.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhixingplan.top/gtwcbmdunq.html

[P04] 求长度
来源：http://hz.mhx1999.top/gtmzfwqbth.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yongpay.top/gtdeswhnnk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtoijounom.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtxwzjnduz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtiznndvvk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtxulpaxxz.html

Go:   len(arr);  len(m)
来源：http://hz.chenjidiqi.icu/gtqyozahdl.html

Ruby: x.length;  x.size
来源：http://hz.ehwqpu.com/gtekyvsdgo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ybcxt.top/gtvrlkvaqp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gtmvzsolqe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinghuilouyu.cn/gtvdnegweq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydjk.org.cn/gtijiiswkn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gtcieshvuw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtcdittnpq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gtvxxhhrfj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ppjwa.cn/gtbdpmoqyj.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtrzvkhprj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtdfssrrja.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtkrvjqwar.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtntsgwfze.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtawhdxecl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gtdiwujgmj.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtierbstln.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtdsmqucuv.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtavklsuty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangdashe.top/gtbxlxuwwb.html

C#:   if (x is null) {}
来源：http://hz.jinqigfzy.top/gtbeexuqww.html

[P07] 防抖与节流
来源：http://hz.ydzc1.top/gtcjspsmmm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtcvhvqfgv.html

PHP:  // 手写时间戳比较
来源：http://hz.sufxvd.cn/gtwdcqivqz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtjmbztocf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtcjnsnxro.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtjnspcyyd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gttozexsfa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtadulznur.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhijiandao.cn/gtiejmmctf.html

[P08] 处理浮点精度问题
来源：http://hz.quarkkingdee.top/gttbyfppmc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ppjwa.cn/gtbuagtrib.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtluszdlyk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jyoumei.cn/gtfmoztnjf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shangyingyoupin.top/gtbafpsdqn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guowangkeji.top/gtdthwknjv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cashguo.top/gtulapxbgx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtlxafqlpi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuanzx.com/gtakueouyx.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlfavggqd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangkeji.top/gtmyuexvry.html

================================================================================
来源：http://hz.zhoulong.xyz/gtusrvesld.html

[Q01] 创建表
来源：http://hz.meibo888.top/gtncpcentn.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtvzclesek.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtvhyklfyx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gtrzetqpbl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtjxalxtzr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtkvtlegpc.html

);
来源：http://hz.xuetiantiany.cn/gtweeihoqs.html

[Q02] 创建带外键的表
来源：http://hz.jqgfzy.top/gtnuwryclg.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gthpunuiym.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtputoudvw.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtztbriniu.html

amount DECIMAL(10, 2),
来源：http://hz.dianchejie.cn/gtqanvlezf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gogol.net.cn/gtozstzumv.html

);
来源：http://hz.wangshuangyany.cn/gtzqvahbvl.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtnhbrhlox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtvdfknjtt.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtlrarklmq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhoulong.xyz/gtykbjjktv.html

[Q05] 重命名列
来源：http://hz.shuidangran.top/gtibcfozck.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zdqjudy.top/gthjdwqvne.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtknmwqwix.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenzaomai.com/gtvkkveeth.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtynwrjazh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hysaishi.cn/gtmhlyatkz.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtoxvrlqrz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtfbevksls.html

[Q09] 创建唯一索引
来源：http://hz.ppjwa.cn/gtmdhjxzmv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aizwys.cn/gteqpbbymt.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtqjfilmiv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ywan-chungtsiang.top/gtkgfpbuyu.html

[Q11] 一次插入多行
来源：http://hz.yongpay.top/gtvydldago.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.c1oappe.top/gturzhsdar.html

[Q12] 插入后取自增 ID
来源：http://hz.zdqjudy.top/gtqmffwmdf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guowangkeji.top/gthvanrwnv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtzyueqkxs.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtxbavusxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.vqdsnc.cn/gtnqwqisyx.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhaomingkeji.xyz/gtrrdyhkga.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtqzvanpww.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gthytjdnfr.html

[Q15] 查询全部
来源：http://hz.ybcxt.top/gtnydufuhv.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtffikgmyo.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtobrptyks.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtpqdgshgn.html

[Q17] 条件查询
来源：http://hz.0kj1m.cn/gtmnvyfagh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.feifeiyinyue.top/gttmvxwqbt.html

[Q18] 模糊匹配
来源：http://hz.jinqigfzy.top/gtgbbsiido.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tanke756.top/gtpyolarbh.html

[Q19] 范围查询
来源：http://hz.chenjidiqi.icu/gtgwtksaqn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hammf.cn/gtvgmrsopq.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtcgqrawfp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gtwajnbgrm.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gttapfpfab.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydzc1.top/gtxhxirdma.html

[Q22] 排序
来源：http://hz.ywan-chungtsiang.top/gtiytxnzgg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnxiangtu.top/gtzlfputpa.html

[Q23] 分页
来源：http://hz.yvedp.cn/gtaxnjlvlv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xylfe.cn/gtfizxsooi.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtcfhrxibi.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gttkbnlaew.html

[Q25] 只取前 N 条
来源：http://hz.c1oappe.top/gtmuxpcmvj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.kuanghao11.cn/gtegtesmmq.html

[Q26] 计数
来源：http://hz.xuetiantiany.cn/gthumwfvjt.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gteockmgey.html

[Q27] 条件计数
来源：http://hz.yonumen.top/gtrtqwnhiw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gttrlgzfaq.html

[Q28] 求和与平均
来源：http://hz.fzhhl.top/gtphgcikgz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nwbrower.top/gtpcpjtebr.html

[Q29] 最大最小值
来源：http://hz.9152youxi.cn/gtfmgiggjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bjfxy.top/gtaplcnonz.html

[Q30] 分组统计
来源：http://hz.ppjwa.cn/gttiwhtrxa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gthlumjnxx.html

[Q31] 分组后过滤
来源：http://hz.316326.xyz/gtbwutuqvz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtgppswpnu.html

[Q32] 分组拼接字符串
来源：http://hz.chenzaomai.com/gtgmrgjafm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtafngigya.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtfowmvfpw.html

[Q33] 多列分组
来源：http://hz.hysaishi.cn/gtokxzwldm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtffnsztit.html

[Q34] 每组取第一条
来源：http://hz.dianchejie.cn/gtffoenurh.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gthmqnbwdg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtzosmwkhl.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtqahcbiax.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtqfnbghlv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtdyngmzkg.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtvtyhyccq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtxbpyvuur.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtdlhxodbo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gaohongyu789.top/gtpcewxjnp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258.top/gtbtwerawt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtzgonvnuw.html

[Q39] 自连接（查上下级）
来源：http://hz.0kj1m.cn/gtowwupkqf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gotoacloud.top/gtbwdzqaay.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fengsongda.top/gticwrxrqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtslqryrxp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gtxbaezaqw.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtnunaufee.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gogol.net.cn/gtwlzpireo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yanxiufei.cn/gtofanolbf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gtcpqplynp.html

[Q42] 连接条件附加过滤
来源：http://hz.sufxvd.cn/gtiecnsqys.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cheryme.top/gtqhvgldnz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtrorqbfdh.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtuorqwbok.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuanzx.com/gtibvpbvwb.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtoliiqrak.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jianghu66.top/gtrypfgedv.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gthpbkmzkb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtvpbbkdej.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangdashe.top/gtgkrrjgiu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtennkoqzb.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtofrelxcr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenzaomai.com/gthbbhlxfn.html

[Q48] CTE 公用表表达式
来源：http://hz.havefunace.top/gthtkstryf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhixingplan.top/gtqcliucnk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tianlin.xyz/gtpxzhbkhp.html

[Q49] 更新单行
来源：http://hz.zhengqikj.top/gtirmlfrgs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtvlscessz.html

[Q50] 批量更新
来源：http://hz.yuanzhike.top/gtmfaglbrh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtwojuisyn.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtevoiibpc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cdnleiting.top/gtwgdymyhd.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gtbdphtfsy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gtvoenuake.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtkpszctgb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtpcmhukdy.html

[Q54] 清空表
来源：http://hz.zhixingplan.top/gtzzjkwxmd.html

TRUNCATE TABLE logs;
来源：http://hz.yonumen.top/gtnszkwklb.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtztcepnwb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.vqdsnc.cn/gtbkhxxcun.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tanke756.top/gtvkhftmtx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtdtghmypr.html

[Q57] 行号
来源：http://hz.shzxlz.cn/gtyflbsnjj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gtxioregts.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtifaxvtjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtuyfmpyzr.html

[Q59] 分组内累计
来源：http://hz.havefunace.top/gtezdltqrg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxinkj.top/gtwxzabbsp.html

[Q60] 取上一行 / 下一行
来源：http://hz.zycfv.cn/gtlcjfvlih.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtgaygmdan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.svipenyu.cn/gtkrbrmrea.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtaaipmqdm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtknqtfvzj.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gteegapgee.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gttvihjwaw.html

[Q63] 开启事务
来源：http://hz.tanke756.top/gtzpykgket.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangshuangyany.cn/gtzrmalakb.html

[Q64] 提交事务
来源：http://hz.jqgufenzy.top/gtdpqudpmw.html

COMMIT;
来源：http://hz.fzhhl.top/gtuarxvrzs.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtglcuhfhk.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtqfhczdka.html

[Q66] 行锁查询
来源：http://hz.ywan-chungtsiang.top/gtkasevldz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gtlqgmpojg.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtyzmauwyz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gogol.net.cn/gtvielbhuj.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtjwymdpes.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gtgqpdpyrs.html

ROLLBACK TO sp1;
来源：http://hz.feifeiyinyue.top/gtoliavvkh.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtjvsxgfgx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jyoumei.cn/gtzrofytle.html

[Q70] 更新统计信息
来源：http://hz.ybcxt.top/gtjhwymwbm.html

ANALYZE TABLE users;
来源：http://hz.tian-w.cn/gtwmulfisa.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtnrrqsmqt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtwrbzapnf.html

[Q72] 查看索引
来源：http://hz.cucudq.cn/gtwcalizfi.html

SHOW INDEX FROM users;
来源：http://hz.jqgfzy.top/gtntsxccbb.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gtjpepmxml.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.redwolf501.top/gtwbmwzrli.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtnwlfjxxi.html


<!-- 参考信息 -->