代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtqvflwnqs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtxpkfouuq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gturhqhfzz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtjzeiyevu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtqqrsbtzt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtikfstcwz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gtpuplarld.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtgwmnvqtq.html

================================================================================
来源：http://hz.yj202588.top/gtgcwbrgsi.html

O. 并发与异步
来源：http://hz.gogol.net.cn/gtouojzmkv.html

================================================================================
来源：http://hz.redwolf501.top/gtpfyvnccq.html

[O01] 启动一个线程
来源：http://hz.nwbrower.top/gtebyhylkf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhongyouzk.top/gtrghiusiz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ppjwa.cn/gtazkszcmc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtudfetdsa.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtpdoqetjk.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtrciapzyy.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtlzmczmfb.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gthcigcrac.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigfzy.top/gtpzabtmcv.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtzkthtlsl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yongpay.top/gtcaipdbmp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtlrbhyigr.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtbgdqmuio.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtxfhwbkyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.iojbl.cn/gtccnzhvyu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtkovppsmi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtfasyazfg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gthfjcfmua.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gtcmdohfci.html

Py:   with lock: shared += 1
来源：http://hz.316326.xyz/gtxrtrvmin.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnxiangtu.top/gtsymrpcvx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nwbrower.top/gthuoehyfd.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtxgyyumwe.html

Java: synchronized (this) { shared++; }
来源：http://hz.hfpthk.cn/gtmgldqdpg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtxuourkbw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.haohaochexian.top/gtdiihgeuk.html

C#:   lock (gate) { shared++; }
来源：http://hz.feifeiyinyue.top/gtkpuopafm.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gteholvcrj.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtlntjqpss.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258.top/gtvlxcfsrt.html

JS:   async function f() { await g(); }
来源：http://hz.gaohongyu789.top/gtjkirpktp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtrwycwxeu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtexldvwkm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258.top/gtxyfyzzif.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtlwpejtrs.html

C#:   async Task F() { await G(); }
来源：http://hz.kuanghao11.cn/gtlijmbckf.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtxsnvbpee.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daxiang520.top/gtuardfebz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gogol.net.cn/gtrxnrtmvw.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtdldgzymh.html

TS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtrbphkrtu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtefwfjaqw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtbftymfls.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gtamepeema.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtgkvfpqng.html

[O06] 使用进程池
来源：http://hz.jqgufenzy.top/gtnwqjjytg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtzchvqqqq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtwcsduxxp.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtmgsaqtfm.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtrkjipqoc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nwbrower.top/gtiifrwrqg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtjvmqsjtb.html

Ruby: // fork 块
来源：http://hz.chenlongwang.top/gtvjovhnmf.html

C#:   Parallel.For
来源：http://hz.aizwys.cn/gtqmrhfjfq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwinnrvda.html

P. 常用工具函数
来源：http://hz.zycfv.cn/gtacfsztfw.html

================================================================================
来源：http://hz.yueranfly.top/gtnlgvphot.html

[P01] 生成 UUID
来源：http://hz.aibaodan.cn/gtzqxwtzor.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtkyrhkerc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pycfn.com/gtpdmzxxxs.html

JS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtcihgjqbh.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtxtwnnqyt.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtwtnqzmof.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gzhubu.top/gthzeuftyl.html

Ruby: SecureRandom.uuid
来源：http://hz.yvedp.cn/gtlmnchtph.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtvjozkxjb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtbzpavbkc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tanke756.top/gtkntgpubn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dianchejie.cn/gtayadhxwi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtmxegypcx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gtxkyydtym.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtpptikxha.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gthgctbqjd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gthmpwwhhv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.52xcode.cn/gtqmgdnwis.html

[P03] 生成短随机字符串
来源：http://hz.fengsongda.top/gtsaqcazwj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhongyouzk.top/gtfvtdvndq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenzaomai.com/gtawvjqgyq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtvjojfwdq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtanhhxytg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtjqwcmwmw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtcwxtzazm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pycfn.com/gtkyyspaiz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtonuqoxxl.html

[P04] 求长度
来源：http://hz.yonumen.top/gtnfxppmoi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gticmhfuht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtvpimdxyy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtcjhpnlbz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtvefcqtec.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtbpppcuwx.html

Go:   len(arr);  len(m)
来源：http://hz.yuanzhike.top/gtithchhth.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtmidwgsap.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shuidangran.top/gthdcbebff.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtwownyopu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtxczidddu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.haohaochexian.top/gtduyxwqco.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sxryk.cn/gtatymbnus.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtbgbfhjwx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhijiandao.cn/gtaqnkahzx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gaohongyu789.top/gtymuucndd.html

Ruby: a == b
来源：http://hz.daxiang520.top/gtrpbilllz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gticxmsiik.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nwbrower.top/gtutnkmcct.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtceyzwpui.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtocvnwavk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtkwekngxf.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gtwajmnuqa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gtadjhlwxq.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtezfxibak.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtnvykjnds.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtoktjulxb.html

[P07] 防抖与节流
来源：http://hz.wangshuangyany.cn/gtangvfdas.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtprmljtcr.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gtifjgtwcf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtjkhkrtfz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtuwedmmob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtsnkmjvdg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtxujhbdmn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtmwyefscx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtfakusdwm.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtxcpojmpg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtjvzicccw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gtndajyodl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gthtrdlhqr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtusjiqmul.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gtikkwnmkf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.birdmap.top/gttroxsepq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gtoyyarnys.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtxexxuupr.html

================================================================================
来源：http://hz.tian-w.cn/gtzxzmszrm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtspjodxpo.html

================================================================================
来源：http://hz.jinqigufen.top/gtdhittqny.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gtockywjhu.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtubmaplmf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtsglvncco.html

name VARCHAR(50) NOT NULL,
来源：http://hz.9152youxi.cn/gtwldwnonp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtgmdqjuch.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gtdjadqoci.html

);
来源：http://hz.tianlin.xyz/gtahoirfxi.html

[Q02] 创建带外键的表
来源：http://hz.yj20258.top/gtnlzmsfsa.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtxmunhsia.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtxmjbdwvi.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtfdcpmknf.html

amount DECIMAL(10, 2),
来源：http://hz.yonumen.top/gtyofcyimp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tianlin.xyz/gtbvpagwal.html

);
来源：http://hz.dashuyun.cn/gtiqqnthsr.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtnhtazbur.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhaomingkeji.xyz/gtlzjszstn.html

[Q04] 修改列类型
来源：http://hz.jinghuilouyu.cn/gtlcbwrpcw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhixingplan.top/gtvmtvuuem.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtabswiqlr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtfcgawatt.html

[Q06] 删除列
来源：http://hz.guowangkeji.top/gtsiqotpds.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gtpjaimnmn.html

[Q07] 删除表
来源：http://hz.ydzc1.top/gtgnbslgyu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtrtdckvjq.html

[Q08] 创建普通索引
来源：http://hz.jinqigfzy.top/gtgszjauaw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtpiyhydum.html

[Q09] 创建唯一索引
来源：http://hz.aibaodan.cn/gtzqrpqgli.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtqzbrccmb.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtuffnxzas.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenjidiqi.icu/gtkhvhysgv.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtjheynhte.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hysaishi.cn/gtxfcqssfd.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gtckbcvqgs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yangfankeji.com/gtpemqnaeu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtrsiuntkc.html

[Q13] 忽略重复插入
来源：http://hz.tianlin.xyz/gtlwdlulof.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gttrtvultp.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtprjbokmi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtqdidogkj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guannengcc.top/gteshenpjc.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gtqzmcauls.html

SELECT * FROM users;
来源：http://hz.yvedp.cn/gtchnhpxte.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtpvkqsikz.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtpeisundb.html

[Q17] 条件查询
来源：http://hz.chenjidiqi.icu/gtwmecbmqg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigfzy.top/gtuxiwmpsg.html

[Q18] 模糊匹配
来源：http://hz.xingfuxueyuan.xyz/gtkyxzkmae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sufxvd.cn/gtpwfuoxxq.html

[Q19] 范围查询
来源：http://hz.zhongyouzk.top/gtddijpahw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xingfuxueyuan.xyz/gttjwrcilf.html

[Q20] IN 列表
来源：http://hz.ivvv.top/gtjmaeaacb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtfwiardpz.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtviuijvip.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xylfe.cn/gtcakdvtmb.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtcrcoebjf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yvedp.cn/gtptflesgc.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gtstmoplnq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtqvqrsstf.html

[Q24] 去重
来源：http://hz.birdmap.top/gteypbqnyc.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtslfnidrx.html

[Q25] 只取前 N 条
来源：http://hz.shzxlz.cn/gtdkqtbdtd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.quarkkingdee.top/gtcscnvcye.html

[Q26] 计数
来源：http://hz.hammf.cn/gtaykhphto.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnxiangtu.top/gtbvxtervi.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gtilzibqie.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtlqtarrmk.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gttisvqapk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtogvjftcx.html

[Q29] 最大最小值
来源：http://hz.jinqigufen.top/gttqvrxjcs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gtgcybmkas.html

[Q30] 分组统计
来源：http://hz.zycfv.cn/gtzvummjbt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtmfewzgse.html

[Q31] 分组后过滤
来源：http://hz.hywenlv.cn/gtgfmhottv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangtech.top/gtnefmkpqn.html

[Q32] 分组拼接字符串
来源：http://hz.vqdsnc.cn/gtqiniacdf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtbozsvvho.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sysykeji.top/gtxnhnzczn.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtskqegpzk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtebbbqapd.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gtcnzxzafr.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtnlfjxjyj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtmpsoxzkt.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gthkmrejre.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtfxbmrnty.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtrbwaruhu.html

[Q36] 左连接
来源：http://hz.yonumen.top/gtytnmimtc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtewcedefg.html

[Q37] 右连接
来源：http://hz.yj20258888.top/gtjcbpdmlr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gteyxsvtvc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtipwcxlay.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tanke756.top/gtkoacejom.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtldrikkcb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtqrvnygyn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gtybkbnzze.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yangfankeji.com/gtsntvwnoc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gtjgzrjptt.html

[Q41] 多表连接
来源：http://hz.aibaodan.cn/gtxuuawwan.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daria6918.cn/gtsgnlgtzo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gtschuiwac.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.smart0.xyz/gtucllwmbm.html

[Q42] 连接条件附加过滤
来源：http://hz.hywenlv.cn/gthkojhlsy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtjnnhjbhc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aizwys.cn/gtbkrfsrqr.html

[Q43] 标量子查询
来源：http://hz.jinqigufen.top/gtmlejoeyt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigufen.top/gtzvtzgkco.html

[Q44] IN 子查询
来源：http://hz.jlsjyb.cn/gtptcydqrs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtuhnjeplb.html

[Q45] EXISTS 判断存在
来源：http://hz.zhoulong.xyz/gtimxqhyjw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtbzpjnfet.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtilhkweca.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtefvhconw.html

[Q47] 与平均值比较
来源：http://hz.feifeiyinyue.top/gtzmmyrixw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtpsubmzbt.html

[Q48] CTE 公用表表达式
来源：http://hz.jyoumei.cn/gtjlkkaggd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgufenzy.top/gtzgnyrwvc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydjk.org.cn/gtqxoqtokb.html

[Q49] 更新单行
来源：http://hz.sufxvd.cn/gtapyieelr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtsbtrmlyj.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtmueznmme.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tian-w.cn/gtvdvhruoe.html

[Q51] 用子查询更新
来源：http://hz.hongshengwenyu.top/gtgyhzbycx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.smart0.xyz/gtxyixplsm.html

[Q52] 删除指定行
来源：http://hz.hammf.cn/gtcggnpodn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtnnbjthsu.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtjgshrqjn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangdashe.top/gtgegjvuhw.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtilhilwjw.html

TRUNCATE TABLE logs;
来源：http://hz.guannengcc.top/gtgtuqwbth.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gttujneusl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtmvxtpjdg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtizdggeed.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daria6918.cn/gtxurapfyq.html

[Q57] 行号
来源：http://hz.redwolf501.top/gtnbpbuogl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtmtzwzlmf.html

[Q58] 累计求和
来源：http://hz.zdqjudy.top/gttwcfyhbz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.0kj1m.cn/gttkbhjgel.html

[Q59] 分组内累计
来源：http://hz.xylfe.cn/gtiodtowpy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.bjfxy.top/gtbigpaexr.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtytctwstf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ivvv.top/gtgzzdunqc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtthmfgeei.html

[Q61] 移动平均
来源：http://hz.daxiang520.top/gtisbheohd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtwgrwists.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtitzdfomi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtrshejxfw.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtzwfxxqck.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hnqzz.top/gtndqqgvcj.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtgvbtmzhk.html

COMMIT;
来源：http://hz.9152youxi.cn/gtvrileiuu.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtqaeczmle.html

ROLLBACK;
来源：http://hz.52xcode.cn/gtohzejtna.html

[Q66] 行锁查询
来源：http://hz.xuetiantiany.cn/gtsccmkfjh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yonumen.top/gtzwikhjzx.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtxchgjgrv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xylfe.cn/gthfkrlupw.html

[Q68] 保存点
来源：http://hz.gotoacloud.top/gtjirakcio.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtpzdkjvbi.html


<!-- 参考信息 -->