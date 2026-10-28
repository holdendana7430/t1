代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtxrndgiui.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtgbepcuoy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtecrknpvj.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtmtjaetea.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtpgpwtguc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gaohongyu789.top/gtguoqjnzx.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtfjgkhcwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gthtyyuhcd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtchardbhs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtsleenkwt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gthqhpbpha.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtekqevezd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtunyijaox.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtlcmoisgm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydjk.org.cn/gtwikrgamk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtqjulfvno.html

================================================================================
来源：http://hz.xuanzx.com/gtwioibnpq.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtemhmhvcx.html

================================================================================
来源：http://hz.dianchejie.cn/gtrqmpouew.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtrapvhbpi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtoqgaojtm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtzhukpdbb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhongyouzk.top/gtvpcbzpby.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtrwznpebo.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtbwnxeshu.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtpvblcucx.html

Ruby: Thread.new { f }
来源：http://hz.hfpthk.cn/gtclngrvrq.html

C#:   Task.Run(() => F());
来源：http://hz.fzhhl.top/gtkezdeyqs.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtefcxowpx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtdmfylcsj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yonumen.top/gtmnjxydgw.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtbqlguvgf.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtzfxzyqlm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtdmncyzne.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.snrcjt.cn/gtdobntmtn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenzaomai.com/gtfngpuoyj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhoulong.xyz/gtambrdtrw.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtsknpytme.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtofmhgnsb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtnybhpwbt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtzzutiltt.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtemyetvcd.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtgzgshndp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.redwolf501.top/gtcuzkgrzq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.52xcode.cn/gtdrfmplxk.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gtzgrfsllb.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtguhvousr.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtbqekfdqg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gtohzogkjf.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtmpuvsenq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.9152youxi.cn/gtlywtgubr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtcokmmyza.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gzhubu.top/gtbcmerera.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xziqi.cn/gtrdfsybvn.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtjxecenab.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtvtmoxrja.html

Py:   asyncio.gather(*tasks)
来源：http://hz.316326.xyz/gtpflnbrhc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtrjvlxyxw.html

JS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtjburazfb.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtmxgavaua.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gtseuleouu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhaomingkeji.xyz/gtngeueuhi.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gtmxzqvxxq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ppjwa.cn/gtnlwxugcq.html

[O06] 使用进程池
来源：http://hz.sufxvd.cn/gtkqfejcas.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtwcbgzihj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tianlin.xyz/gtjoghznsj.html

JS:   // child_process / cluster 模块
来源：http://hz.yj202588.top/gtkktytxln.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtezyqxrht.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtlwtewfmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gthxzwosad.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtxwplvxkh.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtxyypfkpy.html

================================================================================
来源：http://hz.xylfe.cn/gtqsvvkrjs.html

P. 常用工具函数
来源：http://hz.pengpengdd.cyou/gtwyzugrij.html

================================================================================
来源：http://hz.zhengqikj.top/gtvbnqqbaf.html

[P01] 生成 UUID
来源：http://hz.daxiang520.top/gtrnanlwnn.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gtvxqnueqw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtfxqdarsl.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtyrytmvtl.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtafkgbjin.html

Java: UUID.randomUUID().toString()
来源：http://hz.iojbl.cn/gtfmiitlrg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtgxctdowl.html

Ruby: SecureRandom.uuid
来源：http://hz.ppjwa.cn/gtswldfzwl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtcwwxiwqh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtzbsmkpok.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gtwgjvnvfo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hysaishi.cn/gtwsxbxlnh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guannengcc.top/gtjublshya.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cqqwz.cn/gtfqgfqxve.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhengqikj.top/gtynsmqaai.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xziqi.cn/gtozaeince.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gteyxefiyl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhijiandao.cn/gtvlzbftdy.html

[P03] 生成短随机字符串
来源：http://hz.jianghu66.top/gtxynjhgza.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.andypj.xyz/gthwnfuozp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gtqvpcekdr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daxiang520.top/gtfqhdaczh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sysykeji.top/gtdcpbkssg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xziqi.cn/gtrhcoafvr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gtmejdtmse.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.snrcjt.cn/gtkluishmg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.snrcjt.cn/gtwgxrykhb.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtyhwcyngn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hysaishi.cn/gtcfczslpl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gthutsejlu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtxkbtrppo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtygpdpncs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shuidangran.top/gtcoefmxyn.html

Go:   len(arr);  len(m)
来源：http://hz.jiagoushi.top/gtrgxmjhyb.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtsqdibefz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtyvxdhkdy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hongshengwenyu.top/gtgyhmsskw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gteocwluky.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtgeysacgr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtlzwjfgzc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtupwcxunr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenjidiqi.icu/gtaqhmwphk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj20258.top/gthfwljtin.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtjdlheaon.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hysaishi.cn/gtvrrmkbmn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cheryme.top/gtbzeztugi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtlswxzspz.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtfjcdarzv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hongshengwenyu.top/gtkrkccirh.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtfgwysobo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtgxkhrgbo.html

Go:   if x == nil {}
来源：http://hz.quarkkingdee.top/gtzrnbfiui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtkxrwmtis.html

C#:   if (x is null) {}
来源：http://hz.gotoacloud.top/gtpqnhzqee.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtstkuoghe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgfzy.top/gtcjeajqoz.html

PHP:  // 手写时间戳比较
来源：http://hz.sxryk.cn/gtnddruyst.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtecymqktk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtnwxlesio.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtyyqodxga.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jianghu66.top/gtzfhvsjkh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtcqbqacti.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtyhodcnin.html

[P08] 处理浮点精度问题
来源：http://hz.yanxiufei.cn/gtdysmojis.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.smart0.xyz/gtrjiiawir.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ywan-chungtsiang.top/gtprjqjgtu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtyprnpciu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtqllrcwid.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gthdgxtmef.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gthkuzxxmi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtqehxwrmr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtgglhzcea.html

================================================================================
来源：http://hz.zdqjudy.top/gtkxloetyg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gtqxdfllus.html

================================================================================
来源：http://hz.316326.xyz/gtiojpbqea.html

[Q01] 创建表
来源：http://hz.haohaochexian.top/gtcvtzyzkw.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtholwohcx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtxylkqnan.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shangyingyoupin.top/gtljscxwcm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gthtuaewzw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.0kj1m.cn/gtjzteeczg.html

);
来源：http://hz.ydzc1.top/gtktsunlbi.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtbnjcdoww.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gttmrnotvf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtgjtnztsq.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtcwnlfdkq.html

amount DECIMAL(10, 2),
来源：http://hz.wangdashe.top/gtadjwvfdm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuanzx.com/gttwrcggvx.html

);
来源：http://hz.zdqjudy.top/gtksehlacf.html

[Q03] 增加列
来源：http://hz.zhongyouzk.top/gtpqqmoprp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtstpogtom.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtvhbblsdy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxinkj.top/gtxrhazzyz.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtbwoafpov.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gthzlsxhte.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtpihwlrza.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gttbevhtsl.html

[Q07] 删除表
来源：http://hz.sufxvd.cn/gtsuivangl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shangyingyoupin.top/gtiapsrfny.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gtouklimhy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtzhgfpgod.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtvqekjyvm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtbufrlvnf.html

[Q10] 插入单行
来源：http://hz.yangfankeji.com/gtltquxlmk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yonumen.top/gtxticsgto.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtpluusuhr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtzgitbwql.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangtech.top/gtfxalzkxc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtgjqvnuhl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtxlvoxbec.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtscherdtj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtialthbrs.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtamdmzsgx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gtxtwehkfq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydzc1.top/gtypdjlwzm.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtbiuhtdgz.html

SELECT * FROM users;
来源：http://hz.feifeiyinyue.top/gtqvosdxas.html

[Q16] 查询指定列
来源：http://hz.gotoacloud.top/gtumdhtgjv.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtaidwbehx.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gtduvdxkhn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.havefunace.top/gtjlhxwgmy.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtguzrudnv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gtywcuqcfp.html

[Q19] 范围查询
来源：http://hz.ehwqpu.com/gtayqvaoid.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtwslkmfsl.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gtelokekia.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtfqqwuaqs.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtkazzlamg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xylfe.cn/gtmjddardm.html

[Q22] 排序
来源：http://hz.zhongyouzk.top/gthicnoerr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.kuanghao11.cn/gtesuoudzq.html

[Q23] 分页
来源：http://hz.tanke756.top/gtgkrgtteu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gteatjvjys.html

[Q24] 去重
来源：http://hz.cucudq.cn/gtfyusdmum.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtxmiquxtc.html

[Q25] 只取前 N 条
来源：http://hz.jinqigufen.top/gtxyhidziq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gtgjdsihch.html

[Q26] 计数
来源：http://hz.shuidangran.top/gttqfmzefj.html

SELECT COUNT(*) FROM users;
来源：http://hz.aizwys.cn/gtbahloxsu.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtuqhvunjt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuanzx.com/gtwbpuqdbu.html

[Q28] 求和与平均
来源：http://hz.nanxinkj.top/gtidjrwkko.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtufdzhhrh.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtygzhgyka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gticvapqju.html

[Q30] 分组统计
来源：http://hz.zdqjudy.top/gtulrvoepm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtldrlefel.html

[Q31] 分组后过滤
来源：http://hz.0kj1m.cn/gtdkxfdlse.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.andypj.xyz/gtsygovlip.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtnonrhkoh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtpexeyydc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xziqi.cn/gttcidbsan.html

[Q33] 多列分组
来源：http://hz.cucudq.cn/gtzjrtlyle.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtsgveylnj.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtrqqlfdcr.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gttausgoxz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gtbmxilyad.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtodaczupc.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtlsktqwvb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtgjlgezgq.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtgkurxioq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtdpyklxrr.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtrbwznpxn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenlongwang.top/gtoncuwtqu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtalrymcki.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gthyegbwpb.html

[Q39] 自连接（查上下级）
来源：http://hz.cqqwz.cn/gtstjahkis.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtepzgymim.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtvdsarvid.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.mhx1999.top/gtbjumwvps.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sufxvd.cn/gtzmphmrrx.html

[Q41] 多表连接
来源：http://hz.fengsongda.top/gtztwvqpgs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cashguo.top/gtihrurrpd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhoulong.xyz/gtsdizwtvu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xylfe.cn/gtiuasftdu.html

[Q42] 连接条件附加过滤
来源：http://hz.vqdsnc.cn/gtmrvtoyli.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtuasyhxqj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtulhptoju.html

[Q43] 标量子查询
来源：http://hz.tian-w.cn/gtnqyfjesz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtxtashwfp.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtydzfbmnq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtiyrcgyoc.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtdshnymrq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtqzgtfvyk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dashuyun.cn/gtptqobpuz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtefokhlva.html

[Q47] 与平均值比较
来源：http://hz.hysaishi.cn/gtwwioatou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhengqikj.top/gtbnqajtkx.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258888.top/gtufriwrfh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtiambpbib.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.52xcode.cn/gtvgwbpskl.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtwqofdioc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.9152youxi.cn/gtjzieleha.html

[Q50] 批量更新
来源：http://hz.yuxming.cn/gtoaukgbld.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtqsrngrjm.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtjdiriais.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtwuwhgoie.html

[Q52] 删除指定行
来源：http://hz.wangdashe.top/gtfclkyoui.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daria6918.cn/gtcjlrlazj.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtytkdclyn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.vqdsnc.cn/gtnlsdcevj.html

[Q54] 清空表
来源：http://hz.chenlongwang.top/gtdbeomugz.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gthctcgqid.html

[Q55] 排名（并列占位）
来源：http://hz.316326.xyz/gtwxoipeoh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtynvqtqwa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aibaodan.cn/gtuawqzndo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgfzy.top/gtcoilxcxt.html

[Q57] 行号
来源：http://hz.shanyushiyangtech.top/gtbwzgibqd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xinyue.icu/gtysierssz.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtgvyrwmri.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtejcgdcfj.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtwbdttcxf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xylfe.cn/gturtdwhvn.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtbudhcswd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhengqikj.top/gtvenfzcyq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sufxvd.cn/gtpjegpxzn.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gtpoibpzrn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.0kj1m.cn/gtfcmeaouz.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gtpowhdsij.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtfdfhtovz.html

[Q63] 开启事务
来源：http://hz.dianchejie.cn/gtafxvqmcs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hnqzz.top/gtqydhmaqn.html

[Q64] 提交事务
来源：http://hz.zycfv.cn/gtfflzvnef.html

COMMIT;
来源：http://hz.316326.xyz/gttfyayffe.html


<!-- 参考信息 -->