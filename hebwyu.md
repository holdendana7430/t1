代发 wailian999

================================================================================
来源：http://hz.wangdashe.top/gtemzjqrst.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtggudjqgl.html

================================================================================
来源：http://hz.cucudq.cn/gtzxfgzjyc.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangkeji.top/gtbuglawpq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangshuangyany.cn/gtvvurcrbd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtxyrmfiar.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gtxpdlvwkd.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtdnqmqkpq.html

Java: new Thread(() -> f()).start()
来源：http://hz.gzhubu.top/gtpclpywbn.html

Go:   go f()
来源：http://hz.jinyuanbaomall.cn/gtflglgcav.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gthdxrxgey.html

C#:   Task.Run(() => F());
来源：http://hz.vqdsnc.cn/gtuknpwtgu.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtlhltyczr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtgjzdgpbt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gttxumgoqw.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtwomehtsg.html

TS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtiddsuxgr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtgpvghcfs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.52xcode.cn/gthhwjgqqm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj202588.top/gtqolgdixl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jlsjyb.cn/gtrtlliyaz.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gtfcoyusts.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gtnngtskmn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtpowfksye.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gtbskawoli.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtcjqfzick.html

Java: synchronized (this) { shared++; }
来源：http://hz.ehwqpu.com/gthomhudtp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtdplvpspu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hammf.cn/gttwvidxaa.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gtmufvaunw.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtacihptmj.html

Py:   async def f():⏎    await g()
来源：http://hz.mhx1999.top/gtzrszkcvj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xylfe.cn/gtdkgkuwrf.html

JS:   async function f() { await g(); }
来源：http://hz.chenzaomai.com/gtwhientpe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pengpengdd.cyou/gtuqlipkjd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nwbrower.top/gtldzdauyh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtrhgucggt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuxming.cn/gtssqsjzkf.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gthkjibotn.html

[O05] 并发执行并等待全部完成
来源：http://hz.xingfuxueyuan.xyz/gtxkcqeybi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhiwuduotai.top/gtxihitrvq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtffsmxhty.html

JS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtemmyvotv.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtsbmjllct.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhoulong.xyz/gthvmplohw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gogol.net.cn/gtwsltnsdo.html

Ruby: threads.map(&:join)
来源：http://hz.jiagoushi.top/gthyjoihys.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenzaomai.com/gtguftcqnf.html

[O06] 使用进程池
来源：http://hz.nwbrower.top/gtolhthhhl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.52xcode.cn/gtwffnnwck.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.haohaochexian.top/gtjybqkbsm.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtmmcpgfao.html

TS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtjpmnqoiq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangdashe.top/gtkubntghd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gtqkyphrhs.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtcwyguvxw.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtrpkirajs.html

================================================================================
来源：http://hz.jiagoushi.top/gtycjuquxi.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gttabctrza.html

================================================================================
来源：http://hz.smart0.xyz/gtvqiizngo.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtmxxkbejh.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtkdpgszko.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guowangkeji.top/gtntlbinjv.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gttyvbbtax.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtetijqelo.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gtrmzbjucw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.meibo888.top/gtdcescuds.html

Ruby: SecureRandom.uuid
来源：http://hz.jlsjyb.cn/gtxhakxtgn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtjhpkmnph.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgfzy.top/gtnkdxvunt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.havefunace.top/gtnprhklur.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shangyingyoupin.top/gtlttvstoj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtynpivyve.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangdashe.top/gtdsdytnmg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.andypj.xyz/gtqrajofti.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtvhcmapxl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtbhzfoufm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yueranfly.top/gtxbtzdlmo.html

[P03] 生成短随机字符串
来源：http://hz.xuanzx.com/gtdulnqyed.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zdqjudy.top/gtrgipwoqs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gzhubu.top/gtumlojrjj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtthnaibst.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ehwqpu.com/gtzylmktic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gtqhstgwyd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnqzz.top/gtnprvndsh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj202588.top/gtzoulbbvd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtovtovopl.html

[P04] 求长度
来源：http://hz.316326.xyz/gtltppncdd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhengqikj.top/gtqdzzbrcr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtjlivdile.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtgxdzqdfi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtxarcfrxx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtpcrgplei.html

Go:   len(arr);  len(m)
来源：http://hz.chenjidiqi.icu/gtvmecaels.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gtswibjssc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cashguo.top/gtbtovsdoo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gtexjwgpkd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtrtvlarfs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jianghu66.top/gttzeirhcl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gtxwvelbro.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuanzhike.top/gtcntzqtqh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangtech.top/gtihlslmav.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtqlpcongq.html

Ruby: a == b
来源：http://hz.svipenyu.cn/gtnheizqkm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgufenzy.top/gtwtatkyfg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtqynlujzy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtcmztnsgq.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gtxcwndlcb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gteoynvagl.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtomvhupxj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.havefunace.top/gtsyxznrui.html

Go:   if x == nil {}
来源：http://hz.bjfxy.top/gtzakzofyr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtvxbtwemm.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtnqmwukyk.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtytjkwucv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sxryk.cn/gtgkjrlkzp.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtyyfjetdy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtpxfbygjv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtjcseuapz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtamvmfpgb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shangyingyoupin.top/gtslsrklst.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gttvxkrdep.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guowangkeji.top/gttdosbciq.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtmrjqrpcq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jlsjyb.cn/gtqsarintp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.vqdsnc.cn/gtzwgbwuha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtfzocchue.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cdnleiting.top/gtjhpqluec.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnxiangtu.top/gtiswltvmh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cashguo.top/gtluldacvs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.vqdsnc.cn/gtpjuvumty.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtbxauolwq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwxwmpfvq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aibaodan.cn/gtjvrlbxqt.html

================================================================================
来源：http://hz.9152youxi.cn/gtgfsnmuwv.html

[Q01] 创建表
来源：http://hz.hywenlv.cn/gtedvugweh.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtmecapcvu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtodmgjcdf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gteheeamrn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.vqdsnc.cn/gtomvmvmpe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gtywxmhbqv.html

);
来源：http://hz.hammf.cn/gtspzafkeb.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtxwbyywab.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtvkujlhgy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtngpjklud.html

user_id INT NOT NULL,
来源：http://hz.haohaochexian.top/gtrfwjzydg.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtphmmsucq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtlbnohmyx.html

);
来源：http://hz.zdqjudy.top/gtamspxgep.html

[Q03] 增加列
来源：http://hz.aizwys.cn/gtqlwkpxzp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.feifeiyinyue.top/gtkimfalfq.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtohteyfqc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yvedp.cn/gtdfyqctdi.html

[Q05] 重命名列
来源：http://hz.guowangkeji.top/gtdjelnzsw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.52xcode.cn/gtokeuuier.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtywzjpzhz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.52xcode.cn/gtbvbjbond.html

[Q07] 删除表
来源：http://hz.hnxiangtu.top/gttjoovjpi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nwbrower.top/gtwqkfvzhv.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtjkzrueem.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtgvkomclp.html

[Q09] 创建唯一索引
来源：http://hz.smart0.xyz/gtamyvgihd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtjmszikzg.html

[Q10] 插入单行
来源：http://hz.c1oappe.top/gtpuwiysya.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtpzerwtop.html

[Q11] 一次插入多行
来源：http://hz.nanxuanxn.top/gtiwpnjqwo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtampwlcrc.html

[Q12] 插入后取自增 ID
来源：http://hz.fengsongda.top/gtcewltzye.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtfwprhgxr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtpyrfixjq.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gtnnixlopk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gtzsavurdt.html

[Q14] 存在则更新（upsert）
来源：http://hz.andypj.xyz/gtetimxozm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgufenzy.top/gtehuwhckz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sysykeji.top/gthpcpdifq.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gttefwzaqk.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gtucgndqkk.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtgjgypxmi.html

SELECT id, name FROM users;
来源：http://hz.sxryk.cn/gthfyrxxcz.html

[Q17] 条件查询
来源：http://hz.tianlin.xyz/gtwckzagcu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hysaishi.cn/gtchdnawkm.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gtxwuwskog.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.quarkkingdee.top/gtvolaulvc.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtxrpzubsm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtyrswncyz.html

[Q20] IN 列表
来源：http://hz.yvedp.cn/gtfhhofftf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gttpezfwct.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gtjuauvuac.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtahavooei.html

[Q22] 排序
来源：http://hz.jqgfzy.top/gtckpkciua.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuxming.cn/gtvnymfpmz.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtuoxcpgms.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jiagoushi.top/gtvojwkjeg.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtwjriccah.html

SELECT DISTINCT city FROM users;
来源：http://hz.tian-w.cn/gtpqvyrkhr.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtkgontpnu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yueranfly.top/gtgipvqavx.html

[Q26] 计数
来源：http://hz.yj20258.top/gtqlfycyvl.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtkfszcwek.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtilepsnbh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtxbgvwxuw.html

[Q28] 求和与平均
来源：http://hz.birdmap.top/gtolqtkdyt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtrwwisvlx.html

[Q29] 最大最小值
来源：http://hz.zycfv.cn/gtargjhici.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gotoacloud.top/gtlqadnast.html

[Q30] 分组统计
来源：http://hz.xingfuxueyuan.xyz/gtvyvtkrat.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtlnbcqqot.html

[Q31] 分组后过滤
来源：http://hz.xziqi.cn/gtjtkrgiqa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtmvruffbh.html

[Q32] 分组拼接字符串
来源：http://hz.birdmap.top/gtczilfvca.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtkwvnmtnm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtkoeprthb.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtpnkogeyh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ppjwa.cn/gttccwhefa.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtiwtffhog.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtpstevhlf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtmhotkgbk.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtcbxtfmmw.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtmdjfzdfo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtgogqzgji.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtdcmwnjee.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gttvgmetsl.html

[Q37] 右连接
来源：http://hz.sweek.top/gtvwzehgws.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtcyrvvlhu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtbvvwrklj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gttqilukhk.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gteelxudpt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sxryk.cn/gtjvsfmmof.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gthvfyslxy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shuidangran.top/gtxstjgeel.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtjsgdvrwb.html

[Q41] 多表连接
来源：http://hz.hnxiangtu.top/gtbsyztgmz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gogol.net.cn/gttpixysnv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gzhubu.top/gtihnodjph.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.52xcode.cn/gtpffuxism.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtfvpzljyk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuanzx.com/gtninijkvd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jyoumei.cn/gtmxudikvw.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtzkmooyqe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtawhlmiiu.html

[Q44] IN 子查询
来源：http://hz.sysykeji.top/gtbcnbyfla.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guannengcc.top/gtlsbybwvk.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtwncsgvwk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtuikecpyg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fengsongda.top/gtoukgzphm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtpctvleia.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gtavhqoynj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigfzy.top/gthvevneae.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgufenzy.top/gtaofbneva.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnqzz.top/gtnqivafuf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtnluzciuy.html

[Q49] 更新单行
来源：http://hz.xingfuxueyuan.xyz/gtiovqlulv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtfyjdwjve.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtgrjggcav.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxuanxn.top/gtnktkxmlh.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtulgimdif.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aibaodan.cn/gtzvdhpfjv.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtkhfwqucd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtrtspbwtg.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gtnflgddxz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pengpengdd.cyou/gtpyorqfqn.html

[Q54] 清空表
来源：http://hz.tanke756.top/gtofoiuori.html

TRUNCATE TABLE logs;
来源：http://hz.ehwqpu.com/gtkxtyrpiz.html

[Q55] 排名（并列占位）
来源：http://hz.jyoumei.cn/gtcyirthss.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tianlin.xyz/gtobsfdvgl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydzc1.top/gtdxrcwoqy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhengqikj.top/gtotijuswe.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtuhfbtmnu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuanzx.com/gtmfheyqbd.html

[Q58] 累计求和
来源：http://hz.sweek.top/gtmatdouzt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.bjfxy.top/gtmimnwyzp.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtsadljiry.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtxyrmotzt.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydjk.org.cn/gtdnpntjqr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtuvkogygc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtdygiijxp.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gtneuqhabm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtlupeptbu.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtvsbzyufz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gteuklxjur.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gttgjxeroa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtepjqiolr.html

[Q64] 提交事务
来源：http://hz.smart0.xyz/gtcvhssmun.html

COMMIT;
来源：http://hz.cucudq.cn/gtajbrwxzz.html

[Q65] 回滚事务
来源：http://hz.aizwys.cn/gthnvuulwf.html

ROLLBACK;
来源：http://hz.xuanzx.com/gtenvbmksq.html

[Q66] 行锁查询
来源：http://hz.gaohongyu789.top/gtttnlrvju.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxinkj.top/gtkaxpvbge.html

[Q67] 设置隔离级别
来源：http://hz.quarkkingdee.top/gtdqxmbvba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtoxbskzro.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtdmvkfhur.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gttrkfvchx.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gtzvsuwsef.html

[Q69] 查看执行计划
来源：http://hz.sweek.top/gtmjstrpvp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtlvxqbyat.html

[Q70] 更新统计信息
来源：http://hz.316326.xyz/gtxeamyuzc.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtfyygdxyw.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtykalnrey.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtwbrugyog.html

[Q72] 查看索引
来源：http://hz.iojbl.cn/gtgusxbxsq.html


<!-- 参考信息 -->