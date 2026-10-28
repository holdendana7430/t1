代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhijiandao.cn/gtkbshysec.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yanxiufei.cn/gtgvxjvozr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinyuanbaomall.cn/gtacywiydj.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtzqzjyffh.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gtrczbatyt.html

Go:   go f()
来源：http://hz.ybcxt.top/gtujfnmamt.html

Ruby: Thread.new { f }
来源：http://hz.sweek.top/gtcnnmqvgu.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtdiehdmxp.html

[O02] 使用线程池
来源：http://hz.cdnleiting.top/gtodnsybfp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtshpdvkyz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnqzz.top/gtzioxyzkn.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtimjjmagr.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtrnwdxjex.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ywan-chungtsiang.top/gtamerkjlw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.9152youxi.cn/gtbnmehnqu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenlongwang.top/gtvtoylsls.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtssmqpcnu.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigfzy.top/gtxrlwcvfb.html

Py:   with lock: shared += 1
来源：http://hz.daria6918.cn/gtbyfyqdev.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pycfn.com/gtomqqhzgn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.kuanghao11.cn/gtwcfkjjnb.html

TS:   // 同 JS
来源：http://hz.jiagoushi.top/gtjhwlorkm.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtjiryjrqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtkiinodre.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gtaewpcljb.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtsvygwfqz.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gtgsbmlfhg.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtpukrxipl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtuqdbcsjt.html

JS:   async function f() { await g(); }
来源：http://hz.shuidangran.top/gtjnchpmvy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gttgusufao.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtkuujkztv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jiagoushi.top/gtwwtovgha.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dianchejie.cn/gtoqnfqkyf.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtuzzbvmja.html

[O05] 并发执行并等待全部完成
来源：http://hz.yangfankeji.com/gtdcxxefgx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.redwolf501.top/gtawdicvrv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtidvcaovq.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtnyavpwjb.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtvulrpetj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtzhogongk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtegwycosf.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258888.top/gtagkwplhy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtyfydedrl.html

[O06] 使用进程池
来源：http://hz.shangyingyoupin.top/gtpvxfhhjl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenjidiqi.icu/gtiapfxwrn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ywan-chungtsiang.top/gtslftvukv.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtrpivwqwx.html

TS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtitpayorg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.iojbl.cn/gtygotakpc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtkywdtixz.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtsfskjncq.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtkdjppvsb.html

================================================================================
来源：http://hz.yangfankeji.com/gtcjhhwpbe.html

P. 常用工具函数
来源：http://hz.chenzaomai.com/gtlzswbhpp.html

================================================================================
来源：http://hz.andypj.xyz/gtcwzkfxks.html

[P01] 生成 UUID
来源：http://hz.aibaodan.cn/gtftullovz.html

Py:   str(uuid.uuid4())
来源：http://hz.sufxvd.cn/gtbldwjkiw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ehwqpu.com/gthjhjytdw.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtziihppxy.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtqahvxfmn.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtdvwrvwfk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fengsongda.top/gtqkcssyfg.html

Ruby: SecureRandom.uuid
来源：http://hz.cqqwz.cn/gtjsevpnel.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gtkxxfitkc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtyoneixly.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hysaishi.cn/gtprhuzpev.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangtech.top/gtmbfghwpp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtybyrbdto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhijiandao.cn/gtbdvqkjql.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gotoacloud.top/gttxgalzse.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtmejqvdev.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ybcxt.top/gtdnanmpyf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258888.top/gtmlfzrkfx.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtcxoonpet.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtbuhmqvrp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtjkfhjsop.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtxbutnyab.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtbmtlcrjc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yvedp.cn/gtgnpnvkzi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtsbnqdtnf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.redwolf501.top/gtywppmrlu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtmuwopspc.html

[P04] 求长度
来源：http://hz.yuanzhike.top/gtmjvydtzr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gzhubu.top/gtgbbequhs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtdjdubogr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtpjoprbqw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtiilfeetz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgfzy.top/gtmwtsnokv.html

Go:   len(arr);  len(m)
来源：http://hz.zhixingplan.top/gtsgoaelhw.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtymmqlcey.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtfpwvauyf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gtvycfuhrt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtzsabnsvd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtczgaszjo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtyxxuvmgt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtvedpcpdu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtuyselvcp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhiwuduotai.top/gtvgrcuoot.html

Ruby: a == b
来源：http://hz.redwolf501.top/gtnzryofqn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.316326.xyz/gtqfpwozhg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xinyue.icu/gtdiifveyv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gttwobpcwl.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gtvuhzftod.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yueranfly.top/gtcejfhoie.html

TS:   if (x == null) {}
来源：http://hz.gaohongyu789.top/gtiprixajj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtxqfodzcz.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtmltjjxuy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgufenzy.top/gtiktmbimh.html

C#:   if (x is null) {}
来源：http://hz.hammf.cn/gtpamqvpel.html

[P07] 防抖与节流
来源：http://hz.shangyingyoupin.top/gtayiksvjg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cheryme.top/gtfldxoeyk.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gthiyultwm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtfdppjaiu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtnstdhchy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtkhxjbiwz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gtavdoqhqs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtqvhlatqc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gthsepomew.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtahrdnjas.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dashuyun.cn/gtmainoaob.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtqankzswq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtwnlyawsl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gtfetssvai.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hywenlv.cn/gtpjesvkvm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtoneselcb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258.top/gtyzetztoh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cashguo.top/gtglohevkq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtomzqzhoi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenlongwang.top/gtkaqxadog.html

================================================================================
来源：http://hz.birdmap.top/gtnfipgdfn.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtsitxlwni.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtivvdobeu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtbiytgsfd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtulgqyaft.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtkgqzflpb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtcqejctiq.html

);
来源：http://hz.ppjwa.cn/gtgrcfhdjv.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtbledmvxw.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gttzbgnoaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtoxkxbuqx.html

user_id INT NOT NULL,
来源：http://hz.tian-w.cn/gtzlaxwypj.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtuqalnzkk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gtsidqzgst.html

);
来源：http://hz.jqgfzy.top/gtsznmtyfo.html

[Q03] 增加列
来源：http://hz.cqqwz.cn/gteezcqgum.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtsfdyvvcw.html

[Q04] 修改列类型
来源：http://hz.fzhhl.top/gtqshjuqux.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gthokelcav.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtggenempr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gteijvrxvb.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gtwkbdoxrj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtwnvpzilz.html

[Q07] 删除表
来源：http://hz.hongshengwenyu.top/gtvvzawqvn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gotoacloud.top/gtwvojrpqu.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtxdnufyde.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtfuanxxcf.html

[Q09] 创建唯一索引
来源：http://hz.316326.xyz/gtvsdjtvgk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtqjekijcp.html

[Q10] 插入单行
来源：http://hz.zhijiandao.cn/gtrwhksrqm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gtxgsfqbad.html

[Q11] 一次插入多行
来源：http://hz.haohaochexian.top/gtstnexsxt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtpshyhsdo.html

[Q12] 插入后取自增 ID
来源：http://hz.dashuyun.cn/gtxxetjqcv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gtdmzrkpre.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtmruanrhf.html

[Q13] 忽略重复插入
来源：http://hz.meibo888.top/gtgypqoyxf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.andypj.xyz/gtsrmumtgd.html

[Q14] 存在则更新（upsert）
来源：http://hz.iojbl.cn/gtwpheovht.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gtucmdyija.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.dianchejie.cn/gttivtddqb.html

[Q15] 查询全部
来源：http://hz.ybcxt.top/gttcumlivf.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtfnheuycl.html

[Q16] 查询指定列
来源：http://hz.daxiang520.top/gtjjdqzckc.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtfeqpxddh.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtawapjvcw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtzzkqzupy.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtzjcqqbba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gogol.net.cn/gtwebmyfja.html

[Q19] 范围查询
来源：http://hz.shanyushiyangkeji.top/gtgmbibtdn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtcyvcecuz.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtxirmxsrt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj202588.top/gtzuhqybfk.html

[Q21] 空值判断
来源：http://hz.xinyue.icu/gtiinrduoe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydjk.org.cn/gtlgphxpby.html

[Q22] 排序
来源：http://hz.tanke756.top/gtuidedeml.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gtwnqaxqnn.html

[Q23] 分页
来源：http://hz.yangfankeji.com/gtxgoeilgk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cashguo.top/gtuknkksyi.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtruoixhcq.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtwggaxqqv.html

[Q25] 只取前 N 条
来源：http://hz.jinqigufen.top/gtscgolkfd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cheryme.top/gtmxqtibbb.html

[Q26] 计数
来源：http://hz.jyoumei.cn/gtqntvsceq.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtueivnbai.html

[Q27] 条件计数
来源：http://hz.sxryk.cn/gtcyokdtbp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtlxyvmchp.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtubinkaaf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtajijzjqy.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtjcmaiwjb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sxryk.cn/gtahwhzslj.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gtcpnkoldy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtprkmjcxc.html

[Q31] 分组后过滤
来源：http://hz.feifeiyinyue.top/gtomkndllc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258888.top/gthtvgwypx.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtobxxbxlm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtgbdonnjo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenlongwang.top/gtzfchxhyp.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtzunqzhrh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.vqdsnc.cn/gtajojzgbp.html

[Q34] 每组取第一条
来源：http://hz.sysykeji.top/gthvagdyej.html

SELECT * FROM (
来源：http://hz.kuanghao11.cn/gtfaxcjwda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.316326.xyz/gtfqsgopst.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtlkwkljqe.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtpubrvzsu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtfuhxmyvo.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtookwexhp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtjtlpfuoc.html

[Q37] 右连接
来源：http://hz.wangdashe.top/gtndqognmn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtqsgwhwec.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gthdtfvqmd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtekztxfwf.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtwlmlkyel.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxinkj.top/gtelewbqrn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ppjwa.cn/gtfpjutcoj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ppjwa.cn/gtdmqjnqry.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.redwolf501.top/gtvburikdy.html

[Q41] 多表连接
来源：http://hz.fengsongda.top/gtnbxwyqwi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtmynbzdqw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtrzwelpav.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtppkqxret.html

[Q42] 连接条件附加过滤
来源：http://hz.shzxlz.cn/gtyaqbcrqb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cqqwz.cn/gtlsrktzml.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtykzpfdqq.html

[Q43] 标量子查询
来源：http://hz.gaohongyu789.top/gtqohapbji.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aibaodan.cn/gtcbsbsfzj.html

[Q44] IN 子查询
来源：http://hz.dashuyun.cn/gtwwbzdjxb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daria6918.cn/gtfxazvqri.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtjgmwoobm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtxkdkmlzk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhaomingkeji.xyz/gtnrwfckla.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtzgienmsl.html

[Q47] 与平均值比较
来源：http://hz.pycfn.com/gtyjqaxzav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gticbjqiyv.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gtsvnlwjpz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xinyue.icu/gtcljoplfz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtcjlconxy.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtnaolvsnc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtrdkamsys.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gthpghpukf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtzrtvidvn.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtkmhgtnoz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zdqjudy.top/gtzdlrptac.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtdbgldguq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtyydyjnyz.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtawtkcodz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cqqwz.cn/gtvmmwavmw.html

[Q54] 清空表
来源：http://hz.jinghuilouyu.cn/gtqpcshqlg.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtbuxxonoa.html

[Q55] 排名（并列占位）
来源：http://hz.kuanghao11.cn/gteobkffmm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtjdhfvker.html

[Q56] 密集排名（并列不占位）
来源：http://hz.meibo888.top/gttfwmvqkw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtqddisvoj.html

[Q57] 行号
来源：http://hz.shzxlz.cn/gtysssqpoi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtwebgxckt.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gtbzqgvsdy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinghuilouyu.cn/gtkoprbskn.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtfzkrqalf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cheryme.top/gtmnsoxwdw.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtjlvolcbe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtllhsxgbj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtpgpcyvui.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtvkurarfj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yongpay.top/gtyeriigav.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtqlxanrzx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtmprjmvox.html

[Q63] 开启事务
来源：http://hz.yueranfly.top/gtkqmwqjot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtxuqrwxjz.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gtvflcogaf.html

COMMIT;
来源：http://hz.kuanghao11.cn/gthksbveqq.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtbxugdroq.html

ROLLBACK;
来源：http://hz.jinghuilouyu.cn/gtgmcyysnd.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtrsbqtqqz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtmiwrfycf.html

[Q67] 设置隔离级别
来源：http://hz.yuanzhike.top/gtuqxzxbjc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtwtzlcohy.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtqxnpfseu.html

SAVEPOINT sp1;
来源：http://hz.yuanzhike.top/gtmmaspgrz.html

ROLLBACK TO sp1;
来源：http://hz.nanxinkj.top/gtljanftxt.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtvaqlhxmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtokvquwcs.html

[Q70] 更新统计信息
来源：http://hz.dashuyun.cn/gtxmemhwoe.html

ANALYZE TABLE users;
来源：http://hz.ywan-chungtsiang.top/gtuqdnxzac.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gtjzlnnvce.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gthimyctow.html

[Q72] 查看索引
来源：http://hz.hywenlv.cn/gtqklsowgb.html

SHOW INDEX FROM users;
来源：http://hz.haohaochexian.top/gthvhipatu.html

[Q73] 查看表状态
来源：http://hz.haohaochexian.top/gtwvdwcpbb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtsnjruphj.html

[Q74] 强制使用索引
来源：http://hz.xinyue.icu/gtjpyqqior.html


<!-- 参考信息 -->