代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtrwpfgyka.html

Go:   go f()
来源：http://hz.mhx1999.top/gtsutbeznz.html

Ruby: Thread.new { f }
来源：http://hz.feifeiyinyue.top/gtpsschvuv.html

C#:   Task.Run(() => F());
来源：http://hz.hnqzz.top/gtqfwpyocv.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gthsqesfks.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fengsongda.top/gttyddwaoa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.feifeiyinyue.top/gtwcilxuut.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtjpmzuafw.html

TS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtqgbnmsea.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxuanxn.top/gtuegxznhm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtgxxadwui.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guowangkeji.top/gtescsukyb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtmanvhkvi.html

[O03] 加锁保护共享数据
来源：http://hz.pycfn.com/gtfhisxwaz.html

Py:   with lock: shared += 1
来源：http://hz.quarkkingdee.top/gtwpmjtzep.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtskdkckvd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gtjyhgffjt.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtojeiciln.html

Java: synchronized (this) { shared++; }
来源：http://hz.xylfe.cn/gtrxwbfvjs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtfbjdyaih.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtyflukemz.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtpvnpnsut.html

[O04] 定义异步函数并等待
来源：http://hz.nanxinkj.top/gtheiljubv.html

Py:   async def f():⏎    await g()
来源：http://hz.0kj1m.cn/gtdxzfiowf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj202588.top/gtfempzbpz.html

JS:   async function f() { await g(); }
来源：http://hz.hysaishi.cn/gtnooohjyb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtlscehfwh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yangfankeji.com/gtpkfqdtws.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gttpmxrrbc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cqqwz.cn/gtjhviucas.html

C#:   async Task F() { await G(); }
来源：http://hz.snrcjt.cn/gtdmuksbwg.html

[O05] 并发执行并等待全部完成
来源：http://hz.yueranfly.top/gtlmvyhmdv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtjameprbc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aizwys.cn/gtwkqzydoc.html

JS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtqlyxhkju.html

TS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtzbltxpdh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtrdpqlqgv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtswezofug.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtpwdpdkox.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ehwqpu.com/gtidatttrv.html

[O06] 使用进程池
来源：http://hz.birdmap.top/gtoojjeeii.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtryfoxgba.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sysykeji.top/gtrmsolfzs.html

JS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gtjobbfmmd.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtzzzwbrrr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.vqdsnc.cn/gthsrdkteq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gtvcfeejmi.html

Ruby: // fork 块
来源：http://hz.zhongyouzk.top/gtzpzxdsjn.html

C#:   Parallel.For
来源：http://hz.cashguo.top/gtclphvedc.html

================================================================================
来源：http://hz.iojbl.cn/gtiarscsjs.html

P. 常用工具函数
来源：http://hz.zycfv.cn/gtmfogpxru.html

================================================================================
来源：http://hz.zycfv.cn/gtwvuzygww.html

[P01] 生成 UUID
来源：http://hz.52xcode.cn/gtwhycsdqh.html

Py:   str(uuid.uuid4())
来源：http://hz.zhaomingkeji.xyz/gtohxfhoek.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gtfoczxtsn.html

JS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtifunujxm.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtodpsiorg.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangkeji.top/gtaxpmfmaf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinghuilouyu.cn/gtuzliqzer.html

Ruby: SecureRandom.uuid
来源：http://hz.yangfankeji.com/gtjmswisdk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtwhruogoc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtiaenbbrr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgufenzy.top/gtdwulzbdj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tanke756.top/gtvnoiqvjv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shangyingyoupin.top/gthkafofzf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenjidiqi.icu/gtcjcrgfmk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtfhauijlq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gtenljuidt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtxszqufra.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtbrzixvhc.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gttdrxmuty.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daxiang520.top/gtwidjilxq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.bjfxy.top/gtazhoszdf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtnkoajrbh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtjqvyesgv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.birdmap.top/gtaykhuzqx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenlongwang.top/gtxuthvjas.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtkbloqpvj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtwzgxqafm.html

[P04] 求长度
来源：http://hz.fengsongda.top/gtafkodnex.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtarwfegrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtekrcztus.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtbrtzlqst.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtyabqqxqd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtqzcazzzj.html

Go:   len(arr);  len(m)
来源：http://hz.guannengcc.top/gtekcwvrsn.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gtxlckdmkr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigfzy.top/gtgedmthfx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yonumen.top/gthbfnlmmn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cqqwz.cn/gtximdhjsb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sysykeji.top/gtqjyajhqi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinyuanbaomall.cn/gtjtnjtgdz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtiiebsztu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cashguo.top/gtquywcyne.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aibaodan.cn/gtmspuicke.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtozqtojtj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuetiantiany.cn/gtqvnukkyw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hongshengwenyu.top/gtfevfhvog.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gtmuklfaen.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtgjscyhya.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtpnzpxfam.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gtfbpoitvi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtbesdigad.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangtech.top/gttjatmbbh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtwrxfecmo.html

C#:   if (x is null) {}
来源：http://hz.fzhhl.top/gtficogcbr.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtxgsklngx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtvqcjwlti.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtiursjrhc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtfmmtdare.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtsriulnyr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtbrgwtphe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.redwolf501.top/gtnbpstrjl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuxming.cn/gtpajqexhb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yvedp.cn/gthobgzesq.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtvejburjq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtbcakrczh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ywan-chungtsiang.top/gtacysgggm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhoulong.xyz/gtixnjwbbg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dashuyun.cn/gtaijhxfms.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtopjyrubm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtlwsxgptc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenjidiqi.icu/gteqbbaihm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gthuppvsdi.html

================================================================================
来源：http://hz.cqqwz.cn/gtsfdxgzbt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtihxnshxd.html

================================================================================
来源：http://hz.316326.xyz/gtzaaldmde.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtnclayrqv.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtofpyibbi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtjjzfrpnf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gtshbrjzrc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gtfvzblkyu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtkrolcoxa.html

);
来源：http://hz.shanyushiyangtech.top/gtvvrhxfbq.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtitrhceru.html

CREATE TABLE orders (
来源：http://hz.zhijiandao.cn/gtuxzwavwx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtxcomelho.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gteqdrezuj.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gttrjiluhj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhengqikj.top/gtsvnybfzh.html

);
来源：http://hz.zhijiandao.cn/gtypickctq.html

[Q03] 增加列
来源：http://hz.yvedp.cn/gtbdbvdenn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tianlin.xyz/gtzupautkc.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtdbqqvjmh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.iojbl.cn/gtzyydapnl.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtjxnmchje.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtpfkqliea.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtkozvrbyd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fzhhl.top/gtimqvsxgr.html

[Q07] 删除表
来源：http://hz.jyoumei.cn/gtdjxjaxbq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenzaomai.com/gtojgnnjly.html

[Q08] 创建普通索引
来源：http://hz.aizwys.cn/gtktljdlsg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.andypj.xyz/gtajeryjna.html

[Q09] 创建唯一索引
来源：http://hz.tian-w.cn/gtebnycajd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtkevjofmp.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gtpcoavhqn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gtbbntxwls.html

[Q11] 一次插入多行
来源：http://hz.daxiang520.top/gttknuumpv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cheryme.top/gttkiblmuo.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gtsazmukrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtcxevseqj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtlngqoipp.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gthldydqhu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gtgzlffrxe.html

[Q14] 存在则更新（upsert）
来源：http://hz.meibo888.top/gtjhmvqntp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtehgugzqj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shzxlz.cn/gtpjkpjeeb.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtccpkbsis.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gtuvknlblz.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtqraqfgqe.html

SELECT id, name FROM users;
来源：http://hz.yj202588.top/gtjjavtape.html

[Q17] 条件查询
来源：http://hz.chenjidiqi.icu/gtaaqulwfg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gtbalrphyr.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtxmdpjybn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.0kj1m.cn/gtthpjwuha.html

[Q19] 范围查询
来源：http://hz.hammf.cn/gtisnrlpom.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtpbivayxo.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gtidffrwje.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtcvhwrgcr.html

[Q21] 空值判断
来源：http://hz.yj202588.top/gtsygorkps.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hongshengwenyu.top/gtkkabnldt.html

[Q22] 排序
来源：http://hz.yj202588.top/gtddwtdvmt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gtbgxuagpw.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtjlsmlnwu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cqqwz.cn/gtpklfcasp.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtvvmgdqoh.html

SELECT DISTINCT city FROM users;
来源：http://hz.yangfankeji.com/gtwsqucojd.html

[Q25] 只取前 N 条
来源：http://hz.shangyingyoupin.top/gtnaseipms.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.snrcjt.cn/gtyclowryk.html

[Q26] 计数
来源：http://hz.jinqigfzy.top/gthgjogpeb.html

SELECT COUNT(*) FROM users;
来源：http://hz.vqdsnc.cn/gteialacbm.html

[Q27] 条件计数
来源：http://hz.316326.xyz/gtqlnhyrsk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gthvcuzpro.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtniyatpsq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenzaomai.com/gtwrkledvv.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gtlefthvou.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daria6918.cn/gtmlhhyrfr.html

[Q30] 分组统计
来源：http://hz.yj20258.top/gtafvanqco.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gttsbwqdeg.html

[Q31] 分组后过滤
来源：http://hz.hysaishi.cn/gtjulvvwld.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.haohaochexian.top/gtyzbbvlsw.html

[Q32] 分组拼接字符串
来源：http://hz.jyoumei.cn/gtqltdrwhp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtfiyycrxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtavvswrxl.html

[Q33] 多列分组
来源：http://hz.tianlin.xyz/gtmadnhzta.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gttwvnvfna.html

[Q34] 每组取第一条
来源：http://hz.hongshengwenyu.top/gtusejdwoy.html

SELECT * FROM (
来源：http://hz.zhaomingkeji.xyz/gtrxtxrkkn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtqrtcdvlj.html

) t WHERE rn = 1;
来源：http://hz.sweek.top/gtdytnypoo.html

[Q35] 内连接
来源：http://hz.hammf.cn/gtmplyvmag.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtjtharljq.html

[Q36] 左连接
来源：http://hz.iojbl.cn/gtxtpcwuyv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtvakgduou.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtlleshovn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtjetubwit.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guannengcc.top/gtefryizbr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtogrdhcxt.html

[Q39] 自连接（查上下级）
来源：http://hz.hnqzz.top/gtjvjtxshz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yonumen.top/gtohuqfxao.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigufen.top/gtvmidtdri.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtbjweqsta.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gaohongyu789.top/gtnicqlufn.html

[Q41] 多表连接
来源：http://hz.quarkkingdee.top/gtlutjwdnj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gtlnqxkaml.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtrhimxicb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtnisbpwun.html

[Q42] 连接条件附加过滤
来源：http://hz.xinyue.icu/gteswtdnyt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhaomingkeji.xyz/gtnwjlinab.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtmldshjfq.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtnmkztdai.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258.top/gtepkzvmci.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtehvtrnvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnxiangtu.top/gtlfjhvvin.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtmpelsgsv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtcznragxj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shuidangran.top/gtzgwvjexy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtfeosheok.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtqtiyfbmh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnxiangtu.top/gtcmkykmva.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gtxkbqzhvj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guowangkeji.top/gtygvkunuk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gtpqzkidrt.html

[Q49] 更新单行
来源：http://hz.tianlin.xyz/gtaekulitx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtzxlwmpbw.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtjicuznpi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daxiang520.top/gtmkhoawiw.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtakwnsfla.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtrphibnlv.html

[Q52] 删除指定行
来源：http://hz.c1oappe.top/gtshesuvgb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xziqi.cn/gtwveisthg.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtosvdjjma.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtuslebzta.html

[Q54] 清空表
来源：http://hz.gzhubu.top/gttpntmlvk.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gthljhmjhq.html

[Q55] 排名（并列占位）
来源：http://hz.meibo888.top/gtujsbaxio.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gtxvrhslac.html

[Q56] 密集排名（并列不占位）
来源：http://hz.andypj.xyz/gtjmnuogtf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jianghu66.top/gtqbmdceil.html

[Q57] 行号
来源：http://hz.pycfn.com/gtenfikhoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtwyqpmkog.html

[Q58] 累计求和
来源：http://hz.jinqigufen.top/gtebntfbib.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gttzrdlxwh.html

[Q59] 分组内累计
来源：http://hz.shangyingyoupin.top/gtiahhcgen.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtzfzxzhbo.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtjmoqnqfh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtvmkswjaj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigfzy.top/gtlqubezns.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtyuxnhzdk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.haohaochexian.top/gttwzlnlhx.html

[Q62] 分组占比
来源：http://hz.xingfuxueyuan.xyz/gtgdtlhtpg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtnyfqsdct.html

[Q63] 开启事务
来源：http://hz.yueranfly.top/gtfyzlkrmm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yangfankeji.com/gtrmiuvlkq.html

[Q64] 提交事务
来源：http://hz.dianchejie.cn/gtoahbjaqm.html

COMMIT;
来源：http://hz.wangdashe.top/gttcbrhdwo.html

[Q65] 回滚事务
来源：http://hz.ydjk.org.cn/gttxnwzmou.html

ROLLBACK;
来源：http://hz.ywan-chungtsiang.top/gtljmvzpld.html

[Q66] 行锁查询
来源：http://hz.redwolf501.top/gtmcrtqajy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gotoacloud.top/gtuveajlkm.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtyckwicjz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gttgriilfs.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtofgrunjo.html

SAVEPOINT sp1;
来源：http://hz.ivvv.top/gtqcznfgje.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gttzpwkxzl.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtysqcsgfu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtnhmrteoy.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtiavqlauh.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtrixbfmwj.html

[Q71] 查看建表语句
来源：http://hz.gotoacloud.top/gtimvzpqzw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cashguo.top/gtrwaxdeiv.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gtiembljod.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtsqbiytne.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtonhosdhb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aibaodan.cn/gtpirdmmzr.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtgpmtzzsk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtmrtafxts.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtvtgegngf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtiwsnisop.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtyzvblavj.html


<!-- 参考信息 -->