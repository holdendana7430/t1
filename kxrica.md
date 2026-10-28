代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtjxjzvfzr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtsinxocji.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtklsaptcx.html

Java: // 手写递归
来源：http://hz.redwolf501.top/gtodlyowjv.html

Go:   // 手写递归
来源：http://hz.hnqzz.top/gtozojhksz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gtnbmayzis.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gtihdqlatq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtghctuabu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.bjfxy.top/gtprctbkxr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.quarkkingdee.top/gtosufwnif.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtfmtnzvgs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtnhadclxe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtxwplnpev.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gthtowayxn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtannhsgej.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtmoiwftuh.html

================================================================================
来源：http://hz.andypj.xyz/gtpxnpqtox.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gttqpaesmx.html

================================================================================
来源：http://hz.gogol.net.cn/gtbupbojzc.html

[O01] 启动一个线程
来源：http://hz.chenzaomai.com/gtkhaprhhf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj202588.top/gtrovmqish.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.fengsongda.top/gttvbwcimn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtwyweasek.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtkqloanff.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gteznaruyb.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtfcpifnpb.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtwlykrqod.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtfabjrlrj.html

[O02] 使用线程池
来源：http://hz.tanke756.top/gtrjjqjbjo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zdqjudy.top/gtwrgaomiv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtyqexrgma.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtzzqxqgco.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtegumsmmp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jqgfzy.top/gtwywwyouo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenlongwang.top/gtmutgflxd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yueranfly.top/gtdldbxpby.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cqqwz.cn/gtwbdghjfe.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtmctnjdux.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtvmdlqtvb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtyblyazmt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtorwycbxz.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtswmaxjjb.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtzpcldobc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtjeizahcn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fzhhl.top/gtcuonsxcp.html

C#:   lock (gate) { shared++; }
来源：http://hz.birdmap.top/gtvpxnjqvb.html

[O04] 定义异步函数并等待
来源：http://hz.smart0.xyz/gtirjvbrbq.html

Py:   async def f():⏎    await g()
来源：http://hz.shuidangran.top/gtmfrwqllg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnxiangtu.top/gtbbgnyfsf.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtkqytpsaz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtblwzsfai.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dianchejie.cn/gtsbahfyel.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtsbwnxjiz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.feifeiyinyue.top/gtggcccxof.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gteulpafuo.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtrsdodbpu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtvuwanukz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhixingplan.top/gtnrukoxen.html

JS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtmwvzevvj.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtumepcmhq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtmkaytdgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gtqlitjzjc.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtxvcavrhv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hammf.cn/gtvwgxgbtc.html

[O06] 使用进程池
来源：http://hz.shanyushiyangkeji.top/gtgdurmqkj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenjidiqi.icu/gtkvmjkygn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinghuilouyu.cn/gtndilbcve.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtojjwiiyh.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtnsqhqwdn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gtocnhyztk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tian-w.cn/gtpxxxlhmf.html

Ruby: // fork 块
来源：http://hz.ydzc1.top/gtwkqmcorq.html

C#:   Parallel.For
来源：http://hz.cdnleiting.top/gtzjiursgb.html

================================================================================
来源：http://hz.jyoumei.cn/gtfdtjlthe.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtndtbpazi.html

================================================================================
来源：http://hz.xylfe.cn/gttugxokuk.html

[P01] 生成 UUID
来源：http://hz.hongshengwenyu.top/gtyplgdxan.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtxmvixohq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtdyguvfcd.html

JS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtfzjpdwub.html

TS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtuudetoom.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtnbwnpzwy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtghbjjhho.html

Ruby: SecureRandom.uuid
来源：http://hz.9152youxi.cn/gtophcvhrw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cashguo.top/gtvjjhyyzc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhoulong.xyz/gtalbkbyer.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtwhmllayo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtfnywkxwa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtlatwlxsl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.haohaochexian.top/gtwzkbrrfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gzhubu.top/gtbycqvdvn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ybcxt.top/gtwuogyrhf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtehnrqntm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhiwuduotai.top/gtnzqnmtcx.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtptxkbefz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtnzsswryx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gtxnbvnset.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtazyglbla.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pengpengdd.cyou/gtprabfbdt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.0kj1m.cn/gtwidjrmih.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtcuqnywgc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gtexvqgaza.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gtcmhrgvfg.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtsocxqmug.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gtteaxkrxp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtegkuroru.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtefvynpuu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtzuceunby.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shanyushiyangtech.top/gtwwoarxlz.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtjnralkvc.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtggtsdhdz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhixingplan.top/gtbjjhvtrx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258888.top/gtxlonsnzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtfmtugkkn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtjcvkgnhv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yueranfly.top/gtxnbkfbne.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtwbkfehod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gtuevaqpan.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtsmaitsvt.html

Ruby: a == b
来源：http://hz.yongpay.top/gtauhdywef.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtashhxmlp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigufen.top/gtduexednf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yangfankeji.com/gtwwppzjem.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtptirwrxl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gthzygjcul.html

TS:   if (x == null) {}
来源：http://hz.ywan-chungtsiang.top/gtigsjqtqw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtgfzxwoki.html

Go:   if x == nil {}
来源：http://hz.meibo888.top/gtkyoofriq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.52xcode.cn/gtsnehqjsg.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtlttorniu.html

[P07] 防抖与节流
来源：http://hz.zdqjudy.top/gttnolfgre.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxuanxn.top/gtzlpoxyam.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtfdmnnxin.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtryltrskd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtrundjrem.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtijormhfa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtthxrhgts.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.svipenyu.cn/gtxdknhngc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xziqi.cn/gtxwbnkwed.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtqozokklx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtuuuayuan.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtqihtevqq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtuouhsewc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtvamqktwe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtxqwaetad.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtnawhykik.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ppjwa.cn/gtybqexfxb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtvshvhoul.html

================================================================================
来源：http://hz.xziqi.cn/gtryvrpfji.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hammf.cn/gtobwzqhcl.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxcbftomm.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtzaqjubdl.html

CREATE TABLE users (
来源：http://hz.jyoumei.cn/gtzeetlvkn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gtdrfaopbr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.52xcode.cn/gtgibewtei.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gtdkvowtmh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtcrilcymv.html

);
来源：http://hz.kuanghao11.cn/gtkcxirgyg.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtgxqjntry.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtltmlmszn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtvhundypm.html

user_id INT NOT NULL,
来源：http://hz.guannengcc.top/gtnlfxaitk.html

amount DECIMAL(10, 2),
来源：http://hz.hongshengwenyu.top/gtigbpbpnc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtqkioachn.html

);
来源：http://hz.xingfuxueyuan.xyz/gtbdxqmobt.html

[Q03] 增加列
来源：http://hz.yanxiufei.cn/gtlaiegyup.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtdwqxduxj.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtwrpdgjzq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shanyushiyangkeji.top/gtpptukzeb.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtwyymmikl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtfspfivkh.html

[Q06] 删除列
来源：http://hz.c1oappe.top/gtbpnzitob.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtwbxgjyfa.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gtghoytbql.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtuvygowja.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gtnkpgdbeb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtgbhdqksj.html

[Q09] 创建唯一索引
来源：http://hz.daria6918.cn/gtpguscsuo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtsmbqncjw.html

[Q10] 插入单行
来源：http://hz.xuetiantiany.cn/gtcntcmtij.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuetiantiany.cn/gtgaxtjczl.html

[Q11] 一次插入多行
来源：http://hz.wangshuangyany.cn/gteefdolfy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinyuanbaomall.cn/gtxqtnymck.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtgvgekmzr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.svipenyu.cn/gtejuwdymw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnxiangtu.top/gtzvugjden.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gttzhgxdur.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gttscgagra.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gthsxnknny.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtscnaofdf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ybcxt.top/gthnazhghi.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gthjypiefi.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtknswnibs.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtldzqwyse.html

SELECT id, name FROM users;
来源：http://hz.jianghu66.top/gtpxkjpwcv.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gthucklglk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hysaishi.cn/gtcrytmdlp.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtarzcjcfp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.iojbl.cn/gtnytdnqtd.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gtowvftocx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gtdscgqmof.html

[Q20] IN 列表
来源：http://hz.jinghuilouyu.cn/gthcvmkedl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gtpnlfjgaz.html

[Q21] 空值判断
来源：http://hz.dianchejie.cn/gtbjajenvg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtnehgzahj.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtmslketgx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jiagoushi.top/gtmnjsdsbc.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtpauodcoy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtehxrwjfc.html

[Q24] 去重
来源：http://hz.pengpengdd.cyou/gtvaslritd.html

SELECT DISTINCT city FROM users;
来源：http://hz.yongpay.top/gttsbeyeew.html

[Q25] 只取前 N 条
来源：http://hz.nwbrower.top/gtpjpnjitn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hywenlv.cn/gtikuhpmfp.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gtpolprohd.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtdbtunbuw.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtlyaglfay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtzqvqsqde.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtdzgvrcey.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ppjwa.cn/gtxzjuffcg.html

[Q29] 最大最小值
来源：http://hz.jianghu66.top/gtclhnsbax.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gttslqytop.html

[Q30] 分组统计
来源：http://hz.ppjwa.cn/gtufdpuoqm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtaybuukht.html

[Q31] 分组后过滤
来源：http://hz.yueranfly.top/gtcrmzzkfw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtftuzzber.html

[Q32] 分组拼接字符串
来源：http://hz.yueranfly.top/gtsqahznrr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtzrvnddgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtkhscobpb.html

[Q33] 多列分组
来源：http://hz.9152youxi.cn/gtzxzecanz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenjidiqi.icu/gtwcfpsxzl.html

[Q34] 每组取第一条
来源：http://hz.mhx1999.top/gtnafcligr.html

SELECT * FROM (
来源：http://hz.aibaodan.cn/gtqmdazswm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shangyingyoupin.top/gtyvrvyctg.html

) t WHERE rn = 1;
来源：http://hz.hongshengwenyu.top/gtmahtkfrr.html

[Q35] 内连接
来源：http://hz.snrcjt.cn/gtiwlldmkz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtkhcxldjy.html

[Q36] 左连接
来源：http://hz.c1oappe.top/gtdbzfinvz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtughcfgup.html

[Q37] 右连接
来源：http://hz.xziqi.cn/gtjcnjccyl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgufenzy.top/gtihpjttca.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtnjgdtbdr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cashguo.top/gthduerpzc.html

[Q39] 自连接（查上下级）
来源：http://hz.yonumen.top/gtafktknbi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuanzx.com/gtdywqclto.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cheryme.top/gtvawgxcyz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtnsyhpggb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtdrolirsv.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gticepxlfc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhaomingkeji.xyz/gtwenpqguk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhongyouzk.top/gtwbukhelf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtumuovapj.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtbqfsuzpf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtvyoxcscn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ppjwa.cn/gtjvmsxsdo.html

[Q43] 标量子查询
来源：http://hz.sysykeji.top/gttfurkmxa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtnfmlgjut.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtvpazorky.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtelshewci.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtgxfjqjsg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtlidzelxm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gtzsjfryuw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtldbbzcie.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtcrrfibpq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenlongwang.top/gtnbtdvjmm.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtareyefet.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258888.top/gthvcmywut.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gthhnevnpb.html

[Q49] 更新单行
来源：http://hz.hammf.cn/gtofsasinv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigfzy.top/gtzlatbuac.html

[Q50] 批量更新
来源：http://hz.yongpay.top/gtgbejwykc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtzechkyxm.html

[Q51] 用子查询更新
来源：http://hz.316326.xyz/gtgjoyhhcv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gtsigchtzl.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtwjbfbior.html

DELETE FROM users WHERE id = 10;
来源：http://hz.0kj1m.cn/gtmsqftjtg.html

[Q53] 按条件删除
来源：http://hz.snrcjt.cn/gtroqrsvly.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pycfn.com/gttkamzyss.html

[Q54] 清空表
来源：http://hz.daxiang520.top/gtvzzwztwf.html

TRUNCATE TABLE logs;
来源：http://hz.gogol.net.cn/gtrnkbqtdf.html

[Q55] 排名（并列占位）
来源：http://hz.chenjidiqi.icu/gtmqpwnkww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yangfankeji.com/gtutjedgwz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtapgpvzrb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangshuangyany.cn/gtbeopcxeh.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtzdmpqkng.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtywehnhxe.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gtfzqzucka.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtklqdmtvz.html

[Q59] 分组内累计
来源：http://hz.zhongyouzk.top/gteksklqeb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gtngpmihyx.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtuieylzzs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtgzblvlpi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtillbzbjl.html

[Q61] 移动平均
来源：http://hz.hysaishi.cn/gtrcledicj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxinkj.top/gtkzvxjdpd.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gtdjjnevix.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gteydfxatv.html

[Q63] 开启事务
来源：http://hz.ywan-chungtsiang.top/gtijjdndjx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ywan-chungtsiang.top/gtbunldpqq.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gteshjeeun.html

COMMIT;
来源：http://hz.0kj1m.cn/gtninhyogd.html


<!-- 参考信息 -->