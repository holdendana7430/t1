代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gttegymgpk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gthmffcosj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtlzjbcwpn.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtwwimsnxy.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtellzumgn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtvuayprbf.html

C#:   // 手写递归
来源：http://hz.aibaodan.cn/gtppqorxkc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sweek.top/gthpntzanp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ehwqpu.com/gtzgiqqopy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtupkgoxkd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtqquruwdf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtqcezuyec.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtruhnjgxs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtynkmgbfm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenzaomai.com/gtmldwqcrh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtzmtimwni.html

================================================================================
来源：http://hz.dianchejie.cn/gtqmlbxaea.html

O. 并发与异步
来源：http://hz.xingfuxueyuan.xyz/gtamsnlroz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtijcchbsm.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtprnjrewx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cdnleiting.top/gtclqnhfcb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtzruwrfwc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinyuanbaomall.cn/gtrdxpktbj.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtzeloqrjh.html

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtaakjieoe.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtsbkkmorc.html

Ruby: Thread.new { f }
来源：http://hz.jqgfzy.top/gtuedyyadn.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gtdarzlehd.html

[O02] 使用线程池
来源：http://hz.tanke756.top/gtzjxeufwt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtxziamzxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtfhptnxzh.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gthgwysgfa.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtjlamdsoj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtfzeunkmp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gtcymogjwe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fzhhl.top/gtjmvhwetv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jianghu66.top/gtdcmghcjo.html

[O03] 加锁保护共享数据
来源：http://hz.yuanzhike.top/gtbgcrkzwz.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtaisiwhco.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtjqqwxasv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtshufhvub.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtjzmzueps.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gthuzmyxsj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtoyrdmmya.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xziqi.cn/gtsxnbbrgt.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtvlgkrkar.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtbxxaoogj.html

Py:   async def f():⏎    await g()
来源：http://hz.snrcjt.cn/gtuyvfrhbx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtmaypxyot.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtwkgsuzgg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gttnoseisk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cheryme.top/gtbpovacjn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gtybwuxzoo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ehwqpu.com/gthjaxaxnf.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gtnygtopde.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtpptglmqi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtdbiiveha.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigfzy.top/gtfovlkclv.html

JS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtdhazizoz.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtujhmkkdn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtavrzeriu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtrguuarof.html

Ruby: threads.map(&:join)
来源：http://hz.yj202588.top/gthkldawqc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtumouxikb.html

[O06] 使用进程池
来源：http://hz.hfpthk.cn/gtgiutmmty.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtlvxknnst.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtspadhkhx.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtciigyjix.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtxsgamkvr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gotoacloud.top/gtjvsifati.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xuetiantiany.cn/gtgxjkeqxp.html

Ruby: // fork 块
来源：http://hz.hongshengwenyu.top/gtztnbebcy.html

C#:   Parallel.For
来源：http://hz.9152youxi.cn/gtdxgqvnol.html

================================================================================
来源：http://hz.fengsongda.top/gtqsdyoulu.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtiuplrkrn.html

================================================================================
来源：http://hz.sxryk.cn/gtdnfpkaiv.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtptnhpfco.html

Py:   str(uuid.uuid4())
来源：http://hz.jianghu66.top/gtejcajxmk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258888.top/gtnfezkjif.html

JS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtvscizmut.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtpjxctbms.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtnvmfielc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtgxxowfzr.html

Ruby: SecureRandom.uuid
来源：http://hz.xuanzx.com/gtkoetjsrc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guannengcc.top/gtoqbuiiac.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtzqbgnfpl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gttervkhux.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtpajmjttt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhoulong.xyz/gtutrzfjeg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gtakkcyupr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.svipenyu.cn/gtyydberqx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtptlxcyku.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cashguo.top/gtdpovdryf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jyoumei.cn/gtmnuhjokz.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gtlodylajo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.mhx1999.top/gtkxdyzfyy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtkiershdn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtwkmfvyrh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtvyaazpca.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yueranfly.top/gttemrvjdu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sysykeji.top/gtwtxlkdwk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tianlin.xyz/gtzuzehnpl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtuxuaeblk.html

[P04] 求长度
来源：http://hz.daria6918.cn/gtzkurhmwu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtvndumimi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtacxkyfex.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtoziillqt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtnkmoaigx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtuzflryns.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtqjsdoaed.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtqsugwejl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtkjilwhmb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtslewpwjs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtzomvclyy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gthdgnfzhf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gttkcmpolq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtigisddgz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aizwys.cn/gtcervvhor.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtbkrsuyux.html

Ruby: a == b
来源：http://hz.fengsongda.top/gteflysyax.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtvyhaapar.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.bjfxy.top/gtevjuydsr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sxryk.cn/gtkdcpzhrp.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gttkfhupji.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtrhcipjnz.html

TS:   if (x == null) {}
来源：http://hz.iojbl.cn/gtpngycbzx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtzufpzhlj.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtknhfrjvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtvhjyewyk.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtqeughcec.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gtszvkoehu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtosnoabiq.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtygzekxrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtnqyvnqkz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtfdssxqzj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gtaolbqtmb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gthqbqeymh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtpyyxvirv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtllaodgfo.html

[P08] 处理浮点精度问题
来源：http://hz.zhaomingkeji.xyz/gtvkazdpmz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxinkj.top/gtfmmdeuxs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtlgubfzqi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gthmgnuold.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtvfdqvtwt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtayjiccdo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtckzpalzh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gtnfkclpha.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtzhfzhefl.html

================================================================================
来源：http://hz.ppjwa.cn/gtiaifkkur.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.52xcode.cn/gtpdeqnrff.html

================================================================================
来源：http://hz.chenlongwang.top/gtnyvwejyx.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtreypvlde.html

CREATE TABLE users (
来源：http://hz.nanxuanxn.top/gtekaziycb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtxbrzkudi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guannengcc.top/gtbdksntml.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtnwsdtbtt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nwbrower.top/gtrqjdtbps.html

);
来源：http://hz.cucudq.cn/gtkxlvompv.html

[Q02] 创建带外键的表
来源：http://hz.ivvv.top/gtqmznobhp.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtffbiuxxz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtusfqbqvj.html

user_id INT NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtevkdewsh.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtythzygny.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtneouwlid.html

);
来源：http://hz.feifeiyinyue.top/gtwqziabid.html

[Q03] 增加列
来源：http://hz.jianghu66.top/gtltcxgmwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hongshengwenyu.top/gttdctovlg.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gtqlgoylld.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtwzatlqme.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtzuvtejsv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtazfbhbre.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtaiguzedl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fengsongda.top/gtyoaafzpm.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtkhfidkyo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ywan-chungtsiang.top/gtwjncbglx.html

[Q08] 创建普通索引
来源：http://hz.jlsjyb.cn/gtsokcqvfq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guannengcc.top/gtiwmnnpyc.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtnvqzlgvv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtpssrpbuk.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtcpdsjvji.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtwvpslrgc.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gthviqvujl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtrvjjgwqw.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtubckpsyu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtpuwegwkc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shuidangran.top/gtrbczicjb.html

[Q13] 忽略重复插入
来源：http://hz.c1oappe.top/gtrdncspei.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hfpthk.cn/gtmqvsznwo.html

[Q14] 存在则更新（upsert）
来源：http://hz.gotoacloud.top/gtgmitytsy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtqvaygqkb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ybcxt.top/gttzmpuygs.html

[Q15] 查询全部
来源：http://hz.tanke756.top/gtzshnribb.html

SELECT * FROM users;
来源：http://hz.sweek.top/gtqoquxqir.html

[Q16] 查询指定列
来源：http://hz.gaohongyu789.top/gtsusaphwj.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtphlbfuxq.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gtshujciyf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhixingplan.top/gtatknzylr.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gtpixgybht.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yonumen.top/gtxcrequli.html

[Q19] 范围查询
来源：http://hz.shzxlz.cn/gtkwudodpe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jiagoushi.top/gteyejzztp.html

[Q20] IN 列表
来源：http://hz.birdmap.top/gtwloojqrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtcczjirlc.html

[Q21] 空值判断
来源：http://hz.hysaishi.cn/gtjdgjiyhn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.c1oappe.top/gtmhklkmuj.html

[Q22] 排序
来源：http://hz.nwbrower.top/gtzlzmtfdy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtkhjwylgk.html

[Q23] 分页
来源：http://hz.ydzc1.top/gtfptuhpkp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gaohongyu789.top/gtirfictqd.html

[Q24] 去重
来源：http://hz.zhixingplan.top/gtzjoejvok.html

SELECT DISTINCT city FROM users;
来源：http://hz.cheryme.top/gtzmnbnodq.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtohoojoaa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhoulong.xyz/gtetfexpgp.html

[Q26] 计数
来源：http://hz.yj20258888.top/gtzyecvhqc.html

SELECT COUNT(*) FROM users;
来源：http://hz.gzhubu.top/gttsdyhncc.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtieddauod.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gtwspesbrt.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtdwzihtgh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnxiangtu.top/gtkuoshixh.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gtedqgwdvb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.vqdsnc.cn/gtkcmozehy.html

[Q30] 分组统计
来源：http://hz.svipenyu.cn/gtbahrqlqj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtqllfjjqd.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtqmittzdn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guannengcc.top/gtafskbudj.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtpfhjuovg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtpbenmcqq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigfzy.top/gtdsxqtktp.html

[Q33] 多列分组
来源：http://hz.yj20258.top/gtlawgahpr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hywenlv.cn/gtwmnerxvm.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtzrjhtmui.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtxvouopqq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zycfv.cn/gtjonievct.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtrmnykpyj.html

[Q35] 内连接
来源：http://hz.pengpengdd.cyou/gtfcnmxxts.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtswlztvpv.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtgsfqovcz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtqtkkkpcj.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtmscgspoc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fzhhl.top/gtfxaegibq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuxming.cn/gtadccyevq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtdjtvusfx.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtmjvsowuc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gteovkrngz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtfirfrzps.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtieyzvxxp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtxygxljsg.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gttxugcmww.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtyccmbmpr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jyoumei.cn/gtthbyhsur.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ppjwa.cn/gtyextarql.html

[Q42] 连接条件附加过滤
来源：http://hz.hfpthk.cn/gtyycbboei.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtvuspsrop.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtguiyiugw.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtpdemspgx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.birdmap.top/gtbqzshzcm.html

[Q44] IN 子查询
来源：http://hz.yueranfly.top/gtaohfeloe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtnejybkvg.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtigxsmtjn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtkekoaeqy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ywan-chungtsiang.top/gtjdvltjwv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gthtqqipua.html

[Q47] 与平均值比较
来源：http://hz.yangfankeji.com/gtnyhqkyed.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tianlin.xyz/gteyoyuqqr.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gtpdcermfn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtygmtapsn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtnwlfdlyp.html

[Q49] 更新单行
来源：http://hz.feifeiyinyue.top/gtghndinvk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtqwuxfqey.html

[Q50] 批量更新
来源：http://hz.birdmap.top/gtbvhmldrf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtofwnrtts.html

[Q51] 用子查询更新
来源：http://hz.aibaodan.cn/gtkglqgxkv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gtozqntgys.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtwwdcftxc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuanzhike.top/gtmfaetmvx.html

[Q53] 按条件删除
来源：http://hz.gaohongyu789.top/gtuodzzuii.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xinyue.icu/gtabpxyrgz.html

[Q54] 清空表
来源：http://hz.yvedp.cn/gtmfzezyks.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gtwakercuq.html

[Q55] 排名（并列占位）
来源：http://hz.tianlin.xyz/gtmulzncmb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gteqbvltwk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hammf.cn/gtmlvzchmh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.snrcjt.cn/gttarsbcil.html

[Q57] 行号
来源：http://hz.tanke756.top/gtowttzghn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhaomingkeji.xyz/gteqkfhuvq.html

[Q58] 累计求和
来源：http://hz.jinyuanbaomall.cn/gtcoltgtbv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangshuangyany.cn/gtammwaoqs.html

[Q59] 分组内累计
来源：http://hz.yvedp.cn/gtaxpqubdv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhoulong.xyz/gtvbpnfpis.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gtapfhogho.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xylfe.cn/gthdprgxpd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtokydzkda.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gtahontafu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtveembxyg.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtldzeiwce.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtiiwtnvmg.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gthnytayrh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtgiegppip.html

[Q64] 提交事务
来源：http://hz.ybcxt.top/gtfckfyawm.html

COMMIT;
来源：http://hz.ydjk.org.cn/gthknmledk.html


<!-- 参考信息 -->