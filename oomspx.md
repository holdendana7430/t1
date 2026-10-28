代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgfzy.top/gtzradnulv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hongshengwenyu.top/gtccagegdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtavzaevjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtfyawgric.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtzxvinias.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtutfxysjy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gtlnlltndb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtwsgozigw.html

================================================================================
来源：http://hz.shuidangran.top/gtdmxafgml.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtliyxujlr.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxicimcix.html

[O01] 启动一个线程
来源：http://hz.gotoacloud.top/gtysbeaxgs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gthlmhpnyc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.0kj1m.cn/gtmqceivha.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtmbargrts.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtjsuzenhn.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtsfbhmrfs.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtbutrtvsz.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gttvrqftqi.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gthhyqldza.html

[O02] 使用线程池
来源：http://hz.zhixingplan.top/gtqytpgzji.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxinkj.top/gtytcffafg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtxzwmjnbd.html

JS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtdvyrkhas.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtfstnpxgo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gthgyfkbjq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtndyylksy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xingfuxueyuan.xyz/gthptgdczy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtgwgjynmf.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gtgvizmvar.html

Py:   with lock: shared += 1
来源：http://hz.redwolf501.top/gttwuqzbbk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gtvfjrjenp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gtlgyistja.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtcvpzddsj.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtmzgcsmyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnxiangtu.top/gtlwpmpvjk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtpeefsgeg.html

C#:   lock (gate) { shared++; }
来源：http://hz.dianchejie.cn/gtqfwhgmfh.html

[O04] 定义异步函数并等待
来源：http://hz.mhx1999.top/gtzpmfrxil.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtyrcvobol.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtkjduoppd.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtsgjnulsc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yonumen.top/gtuaacngmg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenjidiqi.icu/gtbbxhclzw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yonumen.top/gtymnlyggb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cqqwz.cn/gtavizsraq.html

C#:   async Task F() { await G(); }
来源：http://hz.yvedp.cn/gtpwxsabwq.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtwpkgyupe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtnhcrrims.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daria6918.cn/gtesoivymk.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtrzwaqiel.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtjwbzflsd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtthhpkraa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtmmiwubdp.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtehbsnjhp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtgzogomfc.html

[O06] 使用进程池
来源：http://hz.guannengcc.top/gtnoihlohy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtfsbrwoiz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtxjyydeoz.html

JS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtjzmibquj.html

TS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtpcdhueas.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj202588.top/gtlxabiepw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtnwvwwbqd.html

Ruby: // fork 块
来源：http://hz.tanke756.top/gtwvyiulff.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtzdwgxdov.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbqgzltlg.html

P. 常用工具函数
来源：http://hz.guannengcc.top/gtevuyfjiy.html

================================================================================
来源：http://hz.c1oappe.top/gtudhxcdxq.html

[P01] 生成 UUID
来源：http://hz.xziqi.cn/gtqpogotmj.html

Py:   str(uuid.uuid4())
来源：http://hz.yonumen.top/gtnqnyywpt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cdnleiting.top/gtbdivtmhd.html

JS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtshiexiuh.html

TS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtdepzqmin.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtcjlktjom.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtvtvgxuvf.html

Ruby: SecureRandom.uuid
来源：http://hz.shangyingyoupin.top/gtotmdtlmd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shzxlz.cn/gtecvcykxw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fzhhl.top/gtkcaeayax.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.kuanghao11.cn/gtehzirppk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fzhhl.top/gthyovxiln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zycfv.cn/gtihbgwuir.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gthxquyyjl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtjlckmzlw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtowbgqgmw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.meibo888.top/gtjdvokzjk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtgqwpnaeb.html

[P03] 生成短随机字符串
来源：http://hz.xylfe.cn/gthnwwbubh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtjjwlsvop.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gzhubu.top/gtbjcpnxrs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtibuimjmt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daxiang520.top/gtoypckjep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yueranfly.top/gtgprqetlb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yonumen.top/gtyzvctmny.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.c1oappe.top/gtpdjvnnss.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gtqyjibxsc.html

[P04] 求长度
来源：http://hz.hywenlv.cn/gtrwhvvkpp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.snrcjt.cn/gtngwnfnhq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gthhhkmfag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtuuclynkp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtrwkupgak.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtptxotjkf.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtsusyczcj.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtdfgqxsky.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangshuangyany.cn/gtlhkbcjuk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtkntvygte.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.meibo888.top/gtzrbmscsh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gttbhpgstf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtbrcxjech.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtbrdwzezr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenlongwang.top/gteiszcohj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtmwzoksix.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtzsaftzat.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtiseewfuv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinghuilouyu.cn/gteorwqevp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtelezmpqv.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258.top/gtzfhoociq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gtpdnepjdn.html

TS:   if (x == null) {}
来源：http://hz.hysaishi.cn/gtpojfmhvy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangdashe.top/gtwayzwkaq.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtbhnlwanb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yvedp.cn/gtbijuomzt.html

C#:   if (x is null) {}
来源：http://hz.zdqjudy.top/gtbzayzuiq.html

[P07] 防抖与节流
来源：http://hz.zhijiandao.cn/gtrpyytdwx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gtfjswuupx.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gtbodcfisn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gterhohzpy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtihlnubwz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtcktraalr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gthxpzifwf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.52xcode.cn/gtsqxhntfu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtcdqvpaqh.html

[P08] 处理浮点精度问题
来源：http://hz.cashguo.top/gtyrhkmrvc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtwihtrtmi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtmzkahexd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.birdmap.top/gtpxxkdold.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gtdcwdtwpv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shuidangran.top/gtrphxhfjc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ppjwa.cn/gtbgfctzfs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenjidiqi.icu/gtxtfffqjb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pycfn.com/gtemroyccf.html

================================================================================
来源：http://hz.mhx1999.top/gtkuifnhlx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.smart0.xyz/gteqwqabel.html

================================================================================
来源：http://hz.c1oappe.top/gtrnwdlkuw.html

[Q01] 创建表
来源：http://hz.ydjk.org.cn/gtaympanet.html

CREATE TABLE users (
来源：http://hz.zhengqikj.top/gtziaubexj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtlftsxksl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gtgtyoguem.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fengsongda.top/gtswwphgih.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangshuangyany.cn/gthrlxodsw.html

);
来源：http://hz.jinqigfzy.top/gtbhbwmzzu.html

[Q02] 创建带外键的表
来源：http://hz.mhx1999.top/gtdkljxnpj.html

CREATE TABLE orders (
来源：http://hz.jinyuanbaomall.cn/gtsgnyngjr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtrrdllryc.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtzivmkthb.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtlcpypvoh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnqzz.top/gthpvfvgwf.html

);
来源：http://hz.snrcjt.cn/gtwcmlaigl.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtifofmmho.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258888.top/gtgndavrxo.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtjckqrgtn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cqqwz.cn/gtcsbbypsd.html

[Q05] 重命名列
来源：http://hz.daria6918.cn/gtnyntzgbp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.redwolf501.top/gtdwwuchxa.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtdnqrdccp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtezdebabp.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtfslamynf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtbbzdmefu.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtgubmqfmx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gthsiebcdf.html

[Q09] 创建唯一索引
来源：http://hz.nanxinkj.top/gttcjdskkd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtuzsdovpu.html

[Q10] 插入单行
来源：http://hz.jiagoushi.top/gtlxhnpgdk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ehwqpu.com/gtbgdwkaku.html

[Q11] 一次插入多行
来源：http://hz.aizwys.cn/gtomwzycqr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtrztutpgs.html

[Q12] 插入后取自增 ID
来源：http://hz.pycfn.com/gtuwbwkrvx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigufen.top/gtvemcwarf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangtech.top/gtlcvhnasl.html

[Q13] 忽略重复插入
来源：http://hz.zhiwuduotai.top/gtlmgawmuk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.kuanghao11.cn/gtgfzxjbhu.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtlxptttxv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhengqikj.top/gtviqxycsh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gtqoffxtje.html

[Q15] 查询全部
来源：http://hz.gzhubu.top/gtzagudzfm.html

SELECT * FROM users;
来源：http://hz.yj202588.top/gtalhjqwig.html

[Q16] 查询指定列
来源：http://hz.jiagoushi.top/gthasnsmtz.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtovoukvuo.html

[Q17] 条件查询
来源：http://hz.fzhhl.top/gtdgjqimcl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.smart0.xyz/gtfgmdguyf.html

[Q18] 模糊匹配
来源：http://hz.yuxming.cn/gtrmearvcs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtxqyfcqdn.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gtkxfgunlv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtxgjdbkwd.html

[Q20] IN 列表
来源：http://hz.yuxming.cn/gtussmyirj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtccdfbkhx.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtrjntloid.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtyvnlcomp.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtxqizsqds.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtcoypjowm.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gthkoygpcc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtpguyycjs.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtzmzbwzjl.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtymetrzkb.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gtkiwohiyb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xingfuxueyuan.xyz/gthycrwgwg.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtcazyfkbh.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinqigufen.top/gtjiqhuwaw.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtnumsfvek.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhiwuduotai.top/gtffdzhtyd.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtzmhnpejx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtqomtdtwm.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gtrquvjlor.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtchfsarms.html

[Q30] 分组统计
来源：http://hz.ywan-chungtsiang.top/gthsstiwev.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtxggiitve.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtibubnrvv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gtxybpndut.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gtdeeurxys.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtuiipbicv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hongshengwenyu.top/gttculccof.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtujogasay.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtkawiwvbm.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangtech.top/gtsextkyhy.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtahvddpzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtaosibhid.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtqvilmreq.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtjokcbmji.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtocwiwgqm.html

[Q36] 左连接
来源：http://hz.yueranfly.top/gtotpppaeq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtismnshgr.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gthwmuitzb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtdcwozchr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtzzmgdaul.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gtrfsjnohi.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtvrhpizpu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtwfqkafar.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtlyywdldz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tian-w.cn/gtbooeexwb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gthswtmjgt.html

[Q41] 多表连接
来源：http://hz.guowangkeji.top/gtmuhqtvup.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.redwolf501.top/gtdhzcnpdn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gzhubu.top/gtwoimvhmi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxuanxn.top/gtdhshfckn.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtfgghcvyx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtlyeoonma.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtmdwqmhad.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtvplwmlft.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ivvv.top/gthkidgnkt.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtxuvmijvh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtdpyiteyw.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtwfvxmwsy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtbnlomqag.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxinkj.top/gtdlshhdbk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtobwosfvq.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtoxeqjnxn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtzdwqobzq.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxuanxn.top/gtjmhhkfid.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sweek.top/gtkzomcvzw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydjk.org.cn/gthdpntlhs.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gttjtuzvid.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgfzy.top/gtioldxpwo.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gteigiplju.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gthaeshoqy.html

[Q51] 用子查询更新
来源：http://hz.cqqwz.cn/gtdnvnncmn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cdnleiting.top/gtfqrrlkil.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtfzgjdzrr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sxryk.cn/gttnzjcoej.html

[Q53] 按条件删除
来源：http://hz.snrcjt.cn/gtsilsksvm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gttvcrnvat.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gtrnujjkpm.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtuwnyedqk.html

[Q55] 排名（并列占位）
来源：http://hz.zhoulong.xyz/gtqfoxmkql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtugpbqmnj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yanxiufei.cn/gtfaohqwvb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gtifgnceyn.html

[Q57] 行号
来源：http://hz.chenzaomai.com/gtqqvmzmcb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shangyingyoupin.top/gtxyejsqvv.html

[Q58] 累计求和
来源：http://hz.quarkkingdee.top/gtwxlwojmx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xziqi.cn/gtvohrtwti.html

[Q59] 分组内累计
来源：http://hz.xuetiantiany.cn/gtrwpvpynx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtguigbunk.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtlyjgzunn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenlongwang.top/gtnurtsmje.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gtjudxovvg.html

[Q61] 移动平均
来源：http://hz.ydzc1.top/gtgmobxbaw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jiagoushi.top/gtlguhgrro.html

[Q62] 分组占比
来源：http://hz.wangshuangyany.cn/gtapbhihtc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtqodgftzs.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtujyvyksa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgufenzy.top/gtvtrcfxox.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gthmanfmen.html

COMMIT;
来源：http://hz.hywenlv.cn/gtnupddhvo.html

[Q65] 回滚事务
来源：http://hz.aizwys.cn/gthewzrbsd.html

ROLLBACK;
来源：http://hz.jqgufenzy.top/gtsbhlihom.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtgbdhtbay.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtlyzfzfah.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtgsqrxoqc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtmpzgumty.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gtnanpypjm.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtqsrebwtx.html


<!-- 参考信息 -->