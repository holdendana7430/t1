代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtcxmobjtg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtczqhbbga.html

[N11] 二叉树中序遍历
来源：http://hz.gaohongyu789.top/gtbyqlpbzf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xingfuxueyuan.xyz/gtwjxbtuyr.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtshfmzvbi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gttmwheosn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtxvofqecr.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtqdufccqu.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtvianlvxv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gogol.net.cn/gtweebtnzh.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtdiwjopdx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aizwys.cn/gthlmnqsxk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangshuangyany.cn/gtpnmrdcao.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtpcaffzrr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtptisncwt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gtwashnzdi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtqyrzjjrk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gthajmomck.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.bjfxy.top/gtmqnmbpsv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtxmioqsgk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqdllicsq.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtqvxvwson.html

================================================================================
来源：http://hz.zhongyouzk.top/gtljjwgbcl.html

[O01] 启动一个线程
来源：http://hz.jlsjyb.cn/gtoahegwax.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtihrngwzv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtrczijtvu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtppgnnipr.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gttifasafj.html

Java: new Thread(() -> f()).start()
来源：http://hz.pengpengdd.cyou/gtjqylhayn.html

Go:   go f()
来源：http://hz.yj202588.top/gtcofrjfyf.html

Ruby: Thread.new { f }
来源：http://hz.daxiang520.top/gtlckngsiy.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtzhxwefgp.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtfbqiyphs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zdqjudy.top/gtahexgidn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtrmkywirl.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtkhylswzs.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtvajarqff.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xuanzx.com/gtenbhzekw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtnmzlgyzy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gteycydnax.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gzhubu.top/gtsqgdacfy.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangtech.top/gtjkeducxf.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gttldzfjte.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.mhx1999.top/gtowyuwsab.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xingfuxueyuan.xyz/gtnsrelnzd.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtqhmpnosn.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtyrakhues.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigfzy.top/gthyfkozby.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtzuekkrxi.html

C#:   lock (gate) { shared++; }
来源：http://hz.yonumen.top/gtdjiehqse.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gtjghiyocy.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtlxwvwlfr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtytdjbymy.html

JS:   async function f() { await g(); }
来源：http://hz.yongpay.top/gtqtrkkixd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.smart0.xyz/gtmjuwhlwr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangkeji.top/gtkzqsjtiu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sxryk.cn/gtzwvpzydc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gtibkxvhvm.html

C#:   async Task F() { await G(); }
来源：http://hz.birdmap.top/gtviaxzxsv.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydjk.org.cn/gtmmhgxeck.html

Py:   asyncio.gather(*tasks)
来源：http://hz.havefunace.top/gtgrqsqxls.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnqzz.top/gtmuytfzzg.html

JS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtmfftsdfz.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtczxdcjmh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sweek.top/gtyeyyoncu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gthmbjttby.html

Ruby: threads.map(&:join)
来源：http://hz.xingfuxueyuan.xyz/gttnppxocp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.redwolf501.top/gtyiyjsmec.html

[O06] 使用进程池
来源：http://hz.yonumen.top/gtijwukkuj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenzaomai.com/gtmyjyambi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gtdsazakud.html

JS:   // child_process / cluster 模块
来源：http://hz.yongpay.top/gtjfwccimq.html

TS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtfsjwbeqp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangkeji.top/gtjxjdjcno.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gttfhszffh.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtwkdtidty.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtdlsirinb.html

================================================================================
来源：http://hz.jianghu66.top/gtiyfcydbt.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtcpnobefw.html

================================================================================
来源：http://hz.zycfv.cn/gtwajhltpo.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gtamfrsnwj.html

Py:   str(uuid.uuid4())
来源：http://hz.ppjwa.cn/gttifkfzjx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtjkrcevlx.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gteyhkimac.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtxkubgtiz.html

Java: UUID.randomUUID().toString()
来源：http://hz.daria6918.cn/gtbspycfki.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtzqysrdsv.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtofzaklag.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj202588.top/gtbobohgak.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yueranfly.top/gtbhacwpbx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtxrmvymnq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtsdpbigax.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtfitlpcih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangshuangyany.cn/gtuxgamkjy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtctswoisb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.quarkkingdee.top/gtznnqvwrs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenjidiqi.icu/gtvlmppwhi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtvrcqaayn.html

[P03] 生成短随机字符串
来源：http://hz.shzxlz.cn/gtdctyaxqx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.52xcode.cn/gtkxnvbbor.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.0kj1m.cn/gtlzbphhuj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtzpvztrkg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtcglxeaxu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtjwhxlmys.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtfikvqgng.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yonumen.top/gtnhycaqwv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydjk.org.cn/gtypwvhhwu.html

[P04] 求长度
来源：http://hz.shuidangran.top/gtooubprxa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tian-w.cn/gtdzubbokm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtgxtotghp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtkokuvpme.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtykcdlnwa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shzxlz.cn/gtzzqybpcq.html

Go:   len(arr);  len(m)
来源：http://hz.gzhubu.top/gtuxjmgdre.html

Ruby: x.length;  x.size
来源：http://hz.jinyuanbaomall.cn/gtqsrlrwze.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gtttkcacra.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtuydlowrg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtqsbblrax.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daria6918.cn/gtyiykkmtc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtsqnwnqbx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtbkqjjjwc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gtdbtfkxoa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dashuyun.cn/gtjpklnwgj.html

Ruby: a == b
来源：http://hz.yongpay.top/gtfnqvjlys.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xingfuxueyuan.xyz/gtozkiljzb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtwiffzevp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gtshojanga.html

PHP:  if (empty($x)) {}
来源：http://hz.yonumen.top/gtbbpsabnr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtytpkxnev.html

TS:   if (x == null) {}
来源：http://hz.xingfuxueyuan.xyz/gtvdlhxwan.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtceiueupy.html

Go:   if x == nil {}
来源：http://hz.yuxming.cn/gtgbumqtqe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fengsongda.top/gtargjdltm.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gtxogvcagv.html

[P07] 防抖与节流
来源：http://hz.xziqi.cn/gtmgtotaos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.316326.xyz/gtkcafhnow.html

PHP:  // 手写时间戳比较
来源：http://hz.xuetiantiany.cn/gtylibxupc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtyngqhdqo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtjxjnhzll.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtummkmrjc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtrpplefdw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ywan-chungtsiang.top/gtugggqtfm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258.top/gtebajzuwz.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gthziqxwbj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.svipenyu.cn/gtkhbwiemw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtzhcvukvd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtmhkylkug.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinyuanbaomall.cn/gtefgovcfg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangdashe.top/gtveozacax.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ppjwa.cn/gtubtgcyvs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.haohaochexian.top/gtcvpnmvck.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtemkelxzn.html

================================================================================
来源：http://hz.birdmap.top/gtqxtrthsd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhengqikj.top/gtjcvdywhu.html

================================================================================
来源：http://hz.chenzaomai.com/gtfjsmljfz.html

[Q01] 创建表
来源：http://hz.daxiang520.top/gtrcjqrdyd.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtrhhtizrv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gthpbigabj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.0kj1m.cn/gtgemrpcoe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgufenzy.top/gthcwjqwbx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtsomxkepa.html

);
来源：http://hz.jiagoushi.top/gtqwraisfo.html

[Q02] 创建带外键的表
来源：http://hz.shangyingyoupin.top/gtmpdockbm.html

CREATE TABLE orders (
来源：http://hz.gotoacloud.top/gtcmdgaelh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gteewbmcnu.html

user_id INT NOT NULL,
来源：http://hz.guannengcc.top/gtmfatgtzw.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtguthfvts.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtmrurgptc.html

);
来源：http://hz.tanke756.top/gtkacjsiya.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtkjgidldk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ywan-chungtsiang.top/gtikcgsies.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtkrjvttfq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtqnztdnal.html

[Q05] 重命名列
来源：http://hz.jinyuanbaomall.cn/gttsykwigb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtalzbwvaw.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtvjzmzonm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtoxcujgkl.html

[Q07] 删除表
来源：http://hz.sysykeji.top/gtosxcgaev.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenlongwang.top/gtvvrrqgrr.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gtejxokwrr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nwbrower.top/gtdgtldukg.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtfpbdxizn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtojfxanfy.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gthyksyhtn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenzaomai.com/gtgejsuqjn.html

[Q11] 一次插入多行
来源：http://hz.quarkkingdee.top/gtgfexruav.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtzyzixhjv.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangtech.top/gtfunpynnr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxinkj.top/gtpkyeaaep.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shangyingyoupin.top/gtwafmjozl.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtdcraealz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtyrzwlqsm.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtqgsecqep.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenjidiqi.icu/gtvnrrwutb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gtwuhkjlea.html

[Q15] 查询全部
来源：http://hz.zhoulong.xyz/gtznnyluza.html

SELECT * FROM users;
来源：http://hz.havefunace.top/gtyarzppio.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtguvmtokt.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtpqigkmrc.html

[Q17] 条件查询
来源：http://hz.shzxlz.cn/gtgwxoqwkt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgufenzy.top/gthhzorznb.html

[Q18] 模糊匹配
来源：http://hz.zycfv.cn/gtjwgwbvgi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xylfe.cn/gtwffdhrzl.html

[Q19] 范围查询
来源：http://hz.hnqzz.top/gttzjsaxhq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtiuncttty.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gtejzxzqwz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtidwrmrdl.html

[Q21] 空值判断
来源：http://hz.jyoumei.cn/gtxqdmvygk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dashuyun.cn/gtfeagjxuk.html

[Q22] 排序
来源：http://hz.sweek.top/gtyqoohcgi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.feifeiyinyue.top/gtxgkxrarn.html

[Q23] 分页
来源：http://hz.yonumen.top/gtjffbftde.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sysykeji.top/gtxyxptjud.html

[Q24] 去重
来源：http://hz.dashuyun.cn/gtumqqosbf.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gthzjwnrsa.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gtdywvpnqd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtkokzjjxy.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtvalipncz.html

SELECT COUNT(*) FROM users;
来源：http://hz.xylfe.cn/gtirdxrvvv.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtuvanimbb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigfzy.top/gtlpiijkgd.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtdbgyldzo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtwatshvya.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtcpwcwiqn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yanxiufei.cn/gtkwthdqng.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gthogdqhsx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtaxslxibg.html

[Q31] 分组后过滤
来源：http://hz.hongshengwenyu.top/gtmifnbaol.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuanzhike.top/gtugduuxyk.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtanxpuetv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtbttymvco.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.havefunace.top/gtutzcyzww.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gthaphdrqg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtorhapqcj.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtkyylrvey.html

SELECT * FROM (
来源：http://hz.cheryme.top/gtnpdlztdy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtrflfaugj.html

) t WHERE rn = 1;
来源：http://hz.svipenyu.cn/gtlkzwsrkz.html

[Q35] 内连接
来源：http://hz.xuetiantiany.cn/gtdbdwbxti.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtgqshzbkb.html

[Q36] 左连接
来源：http://hz.andypj.xyz/gtvbnglram.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtdfbjbfxw.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtmsbjsmev.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtttivzbin.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangtech.top/gtqxqrwzug.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtjfbpnjaw.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtnrxmisqc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.birdmap.top/gtafzofbbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cqqwz.cn/gtpnhqvqti.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gttchilabi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtsjfqjwgt.html

[Q41] 多表连接
来源：http://hz.vqdsnc.cn/gtfybjndfj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sufxvd.cn/gtcsowdrjp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtojxepeev.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gtjcmxbept.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtixcndapv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtqmcvmbsa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.0kj1m.cn/gtuhmiapzt.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtqmmofimb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jyoumei.cn/gtchblkygr.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtmgeoatmd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shangyingyoupin.top/gtnzeosqns.html

[Q45] EXISTS 判断存在
来源：http://hz.sweek.top/gtrpkrlzdi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtpcyzipnj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gtpcikiqzf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtpszhvmnu.html

[Q47] 与平均值比较
来源：http://hz.jlsjyb.cn/gtwjwfbxvw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gtrprxuahh.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtdjttbtya.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gtzihagzvs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shzxlz.cn/gtvarvshyu.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtxqwbbbwd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtxeoniscy.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtbanusnci.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xingfuxueyuan.xyz/gtgshwiume.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtrebqlizz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shzxlz.cn/gtjtzjqcyp.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtxqerwlxd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jiagoushi.top/gtbukuddwc.html

[Q53] 按条件删除
来源：http://hz.birdmap.top/gtsnxsttae.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtchhilxge.html

[Q54] 清空表
来源：http://hz.fengsongda.top/gtccbndbfe.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gteagsmhot.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtpytxpssz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxuanxn.top/gtvfwhwhys.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangdashe.top/gtqzhzyehp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtzslnhonm.html

[Q57] 行号
来源：http://hz.jinqigfzy.top/gtygjrlfbf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtrpnjmtzc.html

[Q58] 累计求和
来源：http://hz.dianchejie.cn/gtvzqkraox.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tanke756.top/gtbrjxhvws.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtjpqsvabv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.c1oappe.top/gtnszglcmg.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtylsyavly.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jiagoushi.top/gtzldzueop.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtrimiblya.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtmipxrfah.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtafyjcnqh.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtqrqnkocs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtrgzozoxr.html


<!-- 参考信息 -->