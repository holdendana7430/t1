代发 wailian999

================================================================================
来源：http://hz.yanxiufei.cn/gtpwvncxjn.html

O. 并发与异步
来源：http://hz.pengpengdd.cyou/gthlvpfuhc.html

================================================================================
来源：http://hz.yongpay.top/gtihxeesua.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtqeagydng.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258888.top/gtjcrvtvha.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gthjurpjqm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtwuctzpef.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtyedwfpgb.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtbetzcrnr.html

Go:   go f()
来源：http://hz.sysykeji.top/gtgbmgdfhh.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtxysgkqry.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtdtbrtive.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtmryfpruu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtxhypmuur.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtbgivkfgp.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtiizvflqs.html

TS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gthbdwijtp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtkclaglgr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.birdmap.top/gtdlnzkicr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtefosnyek.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.mhx1999.top/gtqsbvizzo.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gtfoyxpqmz.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtfgccwlgx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.c1oappe.top/gtgqiyltcm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtlqkeunjp.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtednqdxse.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtoyfozmjz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.redwolf501.top/gtagnpqygf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtrxjotkdo.html

C#:   lock (gate) { shared++; }
来源：http://hz.shangyingyoupin.top/gtbtaaxxed.html

[O04] 定义异步函数并等待
来源：http://hz.xuanzx.com/gtaidxzvru.html

Py:   async def f():⏎    await g()
来源：http://hz.daxiang520.top/gtdrulcjtg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gthvlciiyi.html

JS:   async function f() { await g(); }
来源：http://hz.yueranfly.top/gtsqyuhawc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gzhubu.top/gtfqfexbkv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxuanxn.top/gtseiffxwy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ivvv.top/gtozhlivak.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtoukhuehs.html

C#:   async Task F() { await G(); }
来源：http://hz.tian-w.cn/gtmgjzfjas.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gtorxwvonn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hammf.cn/gtutoxqwuo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtlwifbzmf.html

JS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtzmwtiegv.html

TS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gtzrbtgjtl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtpcwmeely.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.birdmap.top/gtwldrjnni.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtydetyqvc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnxiangtu.top/gtcjdtzchd.html

[O06] 使用进程池
来源：http://hz.jqgufenzy.top/gtdgmzehqy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tianlin.xyz/gtjqpcwwob.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtkjbdjtru.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtwqkzemdl.html

TS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtxoepenok.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtzbwfchyj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangkeji.top/gtfeedlzzb.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtrstcqlmw.html

C#:   Parallel.For
来源：http://hz.zhixingplan.top/gtsgcftjyg.html

================================================================================
来源：http://hz.hammf.cn/gtjxowjrzk.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtzmjuvmnv.html

================================================================================
来源：http://hz.fengsongda.top/gtbmkgdhps.html

[P01] 生成 UUID
来源：http://hz.gotoacloud.top/gtelrpteru.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgfzy.top/gtneomygep.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shzxlz.cn/gtzovtddod.html

JS:   crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtsqzzeafa.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtwyjwigkm.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtbhabpwjv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtndjbcsxz.html

Ruby: SecureRandom.uuid
来源：http://hz.iojbl.cn/gtpoindkcu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtcdeorqkj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtqkrxrhbs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhengqikj.top/gtsygpzyyb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gtynsrppze.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ehwqpu.com/gtxyfpllnt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tianlin.xyz/gtsgeciwts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhengqikj.top/gtvdpxojmy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhiwuduotai.top/gtmqolsgcc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gotoacloud.top/gtwvnynjhn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yvedp.cn/gtvqwfqjvv.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtmczfpsix.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gotoacloud.top/gtuhrdusvg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtaejixcpq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtjsabkilg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtcjvhbywq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ybcxt.top/gtnpiiefsk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jlsjyb.cn/gtonioprtq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangkeji.top/gtghzozovb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtbbgfgslk.html

[P04] 求长度
来源：http://hz.ybcxt.top/gtgnjkrymf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtcycxpxke.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtnnubzvcd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtrkmjlqzy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtzkxujhzt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ivvv.top/gtxvuvbert.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtofmsmmkt.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtvtoyyhui.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtvkxgdgtn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yanxiufei.cn/gtffrratkt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtozrxktkt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtgcmefnob.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cdnleiting.top/gtosasumvm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtemqdfhcb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gttxbiwxlc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gtfasbujhs.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtsqysbzch.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhoulong.xyz/gtxcwxjgqu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.feifeiyinyue.top/gtheazxkfw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtxxdtlycd.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtowdlbidv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hywenlv.cn/gtxsmmwfwa.html

TS:   if (x == null) {}
来源：http://hz.jqgufenzy.top/gtlescgkny.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtovxfqelt.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtcamgdpon.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pycfn.com/gtbqkqwbkp.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtllxhdkci.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtrterlckn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cucudq.cn/gtcuqwnsov.html

PHP:  // 手写时间戳比较
来源：http://hz.xingfuxueyuan.xyz/gtqhpkmjns.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtteklugkq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtycmndpdv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yangfankeji.com/gtlkrvqiua.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtcbfqrbgk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtyxwwugjw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtjveyrrks.html

[P08] 处理浮点精度问题
来源：http://hz.c1oappe.top/gtbfyutwhg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhoulong.xyz/gtxcsvgdje.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gtutmpubdr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtccrguyjr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sxryk.cn/gtyglxobiu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtelvwjvgq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gteuhkijot.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtzhsmsnfp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gtapxlfmgf.html

================================================================================
来源：http://hz.jianghu66.top/gtfsjyabtr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gtvzlvnudy.html

================================================================================
来源：http://hz.tanke756.top/gtyvjucftk.html

[Q01] 创建表
来源：http://hz.chenlongwang.top/gtkuywuivt.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtrxoezino.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtdidmmjqj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.quarkkingdee.top/gtdsdxlaog.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtxfsywacv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtbfwxsbov.html

);
来源：http://hz.jinqigfzy.top/gtpmwsovoh.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gtdbcslsmr.html

CREATE TABLE orders (
来源：http://hz.sxryk.cn/gtssmsiiov.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtiozbcaqu.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gtsvexkwjb.html

amount DECIMAL(10, 2),
来源：http://hz.hongshengwenyu.top/gtjgvnluwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daria6918.cn/gtvbkzgprp.html

);
来源：http://hz.kuanghao11.cn/gtlvmhdnmy.html

[Q03] 增加列
来源：http://hz.jqgufenzy.top/gtofygvjas.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.andypj.xyz/gtzyoebios.html

[Q04] 修改列类型
来源：http://hz.guannengcc.top/gtmdlvcwio.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gthurxyggr.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtlnxzrbby.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.bjfxy.top/gtbprbtaet.html

[Q06] 删除列
来源：http://hz.hywenlv.cn/gtekfdfxug.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dianchejie.cn/gtltzedjck.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtnqnizosi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtbvqmosts.html

[Q08] 创建普通索引
来源：http://hz.zdqjudy.top/gtiecfiwuy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtdzzqwcqv.html

[Q09] 创建唯一索引
来源：http://hz.ppjwa.cn/gtiywlaawq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtngrhwblc.html

[Q10] 插入单行
来源：http://hz.dashuyun.cn/gttezpxftr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gaohongyu789.top/gtsffkfjdz.html

[Q11] 一次插入多行
来源：http://hz.wangdashe.top/gtqlrvusak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtulubjakh.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtmxzphqvw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yangfankeji.com/gtzxkxtzoj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtepdenbjj.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtwcqbdxgu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guannengcc.top/gtefjqided.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gtfwgumsyf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hfpthk.cn/gtagzbcxhd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.smart0.xyz/gtdevoqlzw.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtxdsnuhly.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gtqesifclq.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtguiteoxn.html

SELECT id, name FROM users;
来源：http://hz.zhengqikj.top/gtryslwhpd.html

[Q17] 条件查询
来源：http://hz.yanxiufei.cn/gtjckaxxjc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtuxibpggq.html

[Q18] 模糊匹配
来源：http://hz.fengsongda.top/gtmmmpnduj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenlongwang.top/gtjtxoxjtz.html

[Q19] 范围查询
来源：http://hz.xinyue.icu/gtlusbllfr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gotoacloud.top/gtnvqoxood.html

[Q20] IN 列表
来源：http://hz.yuanzhike.top/gthedvdjla.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangshuangyany.cn/gtipvdvrve.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gtnuuwgdru.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gthhgauzca.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtoaiseedl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtxyolmgrh.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtvwhhaeyl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtxhsjbray.html

[Q24] 去重
来源：http://hz.chenjidiqi.icu/gtcaynpkxh.html

SELECT DISTINCT city FROM users;
来源：http://hz.feifeiyinyue.top/gtcttyyftp.html

[Q25] 只取前 N 条
来源：http://hz.sysykeji.top/gttprftttq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhiwuduotai.top/gtzwtcnfxf.html

[Q26] 计数
来源：http://hz.meibo888.top/gtpjrtewgv.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtovyxpfci.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtsqxfiqmz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.feifeiyinyue.top/gtaeohtofj.html

[Q28] 求和与平均
来源：http://hz.ywan-chungtsiang.top/gtpfmosmxj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtespittmg.html

[Q29] 最大最小值
来源：http://hz.ivvv.top/gtjglbopmu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtyvxwccjx.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtfbqqbpsa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtjvxvjzms.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gtudtmtwak.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhiwuduotai.top/gtbjmjdnjk.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtcniatrxu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtrdhoosqt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtfbvhryft.html

[Q33] 多列分组
来源：http://hz.hywenlv.cn/gtayzdhuvd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtikctvwsg.html

[Q34] 每组取第一条
来源：http://hz.wangdashe.top/gtdvzrbfus.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtwgdswarz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yvedp.cn/gtkblyiine.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtrnnujfur.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtygfectwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtsgyfhivv.html

[Q36] 左连接
来源：http://hz.shangyingyoupin.top/gtjowqgisk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtpgrzlavn.html

[Q37] 右连接
来源：http://hz.zhaomingkeji.xyz/gtxllbcnct.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtpzfjyibh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtwlozuqaz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtzeyjipwf.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtulfuncux.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtypgphbrp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgfzy.top/gtbelmoryb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtmzigpdry.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtalxqledk.html

[Q41] 多表连接
来源：http://hz.cheryme.top/gtthqlabjx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtqszfgiwh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gtjeaxqrww.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxuanxn.top/gtmiifjxhc.html

[Q42] 连接条件附加过滤
来源：http://hz.birdmap.top/gtraskckwf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtdjljorwr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtmilowlmd.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtriryksyl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtjtcbarpd.html

[Q44] IN 子查询
来源：http://hz.hammf.cn/gtclznwzhz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtrlfftllo.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtgrcetjkr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtmfrilnbb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gaohongyu789.top/gtssbtkzyj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtglhiljkj.html

[Q47] 与平均值比较
来源：http://hz.xinyue.icu/gtoyeottbv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtycbomiyw.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtwgposaog.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtthjhdcxd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dashuyun.cn/gtqiaqllxh.html

[Q49] 更新单行
来源：http://hz.nanxinkj.top/gtzgnefgwz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtcjthuyuc.html

[Q50] 批量更新
来源：http://hz.hywenlv.cn/gtcjsptpwb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtrdfrisuc.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtqgmfovoy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtbncqhmeh.html

[Q52] 删除指定行
来源：http://hz.cucudq.cn/gthuksintu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtbvitmgja.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtcznvjifw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtjqdxndyr.html

[Q54] 清空表
来源：http://hz.cqqwz.cn/gtbgozlymf.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gtcgsmjnkl.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gtmywsrhvd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtgbewsvyr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gteifcfyge.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtbjbhmfig.html

[Q57] 行号
来源：http://hz.nanxuanxn.top/gtiskimdqm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cdnleiting.top/gttjyaglwr.html

[Q58] 累计求和
来源：http://hz.feifeiyinyue.top/gtnchqlryx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnqzz.top/gtzodpyoyq.html

[Q59] 分组内累计
来源：http://hz.hongshengwenyu.top/gtiycjzzub.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gtpoksmixw.html

[Q60] 取上一行 / 下一行
来源：http://hz.xingfuxueyuan.xyz/gttykefkri.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gaohongyu789.top/gtwwsjfntq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gtvzacodyb.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gthehyacuk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.redwolf501.top/gtqclavkao.html

[Q62] 分组占比
来源：http://hz.meibo888.top/gtsdonbajy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gthslnhtut.html

[Q63] 开启事务
来源：http://hz.redwolf501.top/gtwseupxrg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ehwqpu.com/gtieclqtiy.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtyoxibbba.html

COMMIT;
来源：http://hz.wangshuangyany.cn/gtgvmfqoae.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtrlxgfhlp.html

ROLLBACK;
来源：http://hz.yanxiufei.cn/gtbiwgdloq.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtivzvtmlx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gtwgshvtpr.html

[Q67] 设置隔离级别
来源：http://hz.fzhhl.top/gtydvmfhba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtnhyusbvz.html

[Q68] 保存点
来源：http://hz.vqdsnc.cn/gtlmvievso.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtxinnvkzc.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtnthuajxu.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gtehjybqgh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gtebpwchmo.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtdvrkwjaj.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtjgxacynz.html

[Q71] 查看建表语句
来源：http://hz.9152youxi.cn/gtbjbakvoh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtyjedsvvq.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gtctxieifu.html


<!-- 参考信息 -->