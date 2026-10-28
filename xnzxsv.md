代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenzaomai.com/gtpsynezfe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuxming.cn/gtvgkvkvdt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtikrlhbev.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtajrmcern.html

Java: new Thread(() -> f()).start()
来源：http://hz.gaohongyu789.top/gtwmpychww.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtjoeaytuw.html

Ruby: Thread.new { f }
来源：http://hz.zhijiandao.cn/gthkpuutxb.html

C#:   Task.Run(() => F());
来源：http://hz.fengsongda.top/gtvycofbxq.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtzysdtzed.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.iojbl.cn/gtertritgj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ybcxt.top/gtvwhueqta.html

JS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtusjqqzco.html

TS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtsfnjhpbo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinyuanbaomall.cn/gtipzydlbk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtzphiwajh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gticejjpvp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtcwedxhqf.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtabbvxyit.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtxfqidswz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtxuuufgcg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xinyue.icu/gtfxbvijaa.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtalzofhrj.html

Java: synchronized (this) { shared++; }
来源：http://hz.aizwys.cn/gtfsyaaved.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtyrkrtami.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cqqwz.cn/gtdalwpice.html

C#:   lock (gate) { shared++; }
来源：http://hz.svipenyu.cn/gtmreebwnf.html

[O04] 定义异步函数并等待
来源：http://hz.yangfankeji.com/gtloorduyo.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtbqnnvhnv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.vqdsnc.cn/gtvluhpyrn.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtyncnjrjv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.52xcode.cn/gttrsokxxx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zdqjudy.top/gtwmlovmjm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.redwolf501.top/gtgyeebwcx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj202588.top/gtwrczdjdd.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtpiqogddu.html

[O05] 并发执行并等待全部完成
来源：http://hz.yangfankeji.com/gtczllrslf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtzwdqtnnq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sufxvd.cn/gtjcnognjb.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtyaaalubd.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gthjqbafrj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtpdgbcdsu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sufxvd.cn/gtetffzabg.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtakyqatwe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cqqwz.cn/gtdjdivhwl.html

[O06] 使用进程池
来源：http://hz.wangdashe.top/gtswbgoejr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tian-w.cn/gtqhdcflpc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tian-w.cn/gtjntjjoyt.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtwgmvzoeu.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtnvaygzsx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtmkaltyze.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xinyue.icu/gttowkemre.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtdmurjqbi.html

C#:   Parallel.For
来源：http://hz.sxryk.cn/gtydxudinj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcesmgfjs.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtkwapcytx.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrggapxmn.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtlrtuxnof.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtjfondqlj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtfguximjo.html

JS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtodvciitn.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtxlujcpze.html

Java: UUID.randomUUID().toString()
来源：http://hz.sxryk.cn/gtptdfonwn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tanke756.top/gtmzhljpar.html

Ruby: SecureRandom.uuid
来源：http://hz.xziqi.cn/gtejpyiqzb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.iojbl.cn/gtvzoidljx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnxiangtu.top/gtbetibszx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtssxjoiwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gtddbxtjcf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtaujminnh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.smart0.xyz/gtlbnkxjkn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gtrtvhgcnr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenjidiqi.icu/gtxdgsjvxi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtlbkinpvd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gtlygyfurh.html

[P03] 生成短随机字符串
来源：http://hz.jiagoushi.top/gtnzeokuyr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtqowyzfot.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.svipenyu.cn/gtczjgakvn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtpomulsmq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtsyerfvqt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtiphgbbsu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gthhmzvwam.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258888.top/gtkflhcaos.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhengqikj.top/gtrlqlswhj.html

[P04] 求长度
来源：http://hz.gzhubu.top/gtdwxucrmk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yonumen.top/gtvzwnmmkb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtntodyoed.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtqhvtmhqo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtmoucjhrv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtioombzxl.html

Go:   len(arr);  len(m)
来源：http://hz.tian-w.cn/gtloqpkxdn.html

Ruby: x.length;  x.size
来源：http://hz.yvedp.cn/gtigwyetul.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuanzx.com/gtmpeojdxh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.smart0.xyz/gtnwpkuqmq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtjeruqxny.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.snrcjt.cn/gtalachjnx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cashguo.top/gtrlogqvkz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtddzjhjxk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tian-w.cn/gtessywhia.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhijiandao.cn/gtputruuqd.html

Ruby: a == b
来源：http://hz.snrcjt.cn/gtjdpvoanm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtqcdzpkan.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtusmgzpgl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gtscrqisol.html

PHP:  if (empty($x)) {}
来源：http://hz.jinyuanbaomall.cn/gtyxmmalhp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sufxvd.cn/gtsfbcpbml.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gtrwuojkka.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtdfflktwy.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtqmdcvkks.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtoemoheth.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtmlcpysgk.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangtech.top/gtvfnoywnw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtdcuknmov.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtcckbiuop.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtldvloqyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtxvplqkac.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtoxvqscdg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhaomingkeji.xyz/gtnlkeeooo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtbybqbhob.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.9152youxi.cn/gtdzonteii.html

[P08] 处理浮点精度问题
来源：http://hz.yongpay.top/gtvbqdrfam.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daria6918.cn/gtzewuiett.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gthpozbyff.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtrucswwcn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.svipenyu.cn/gtukhpvcud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtoncnlxxe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shzxlz.cn/gtylbbvhxv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnqzz.top/gtmclmaafz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtccjgmtgm.html

================================================================================
来源：http://hz.shzxlz.cn/gtminspqqj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.c1oappe.top/gtndbgczfj.html

================================================================================
来源：http://hz.sxryk.cn/gtbcskccqg.html

[Q01] 创建表
来源：http://hz.cdnleiting.top/gtsoqboxdb.html

CREATE TABLE users (
来源：http://hz.gzhubu.top/gtriuurfrl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtgiyxklmt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ybcxt.top/gtivxxyalh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinyuanbaomall.cn/gtsdmowhqn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenzaomai.com/gteqqxmthj.html

);
来源：http://hz.ivvv.top/gtdvnxsmiv.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtreyscqbs.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gthsmeehiv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtclqndrkb.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gtoztcvdwg.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtsmyfcaae.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtaojyuzom.html

);
来源：http://hz.9152youxi.cn/gtgporqhrl.html

[Q03] 增加列
来源：http://hz.fzhhl.top/gtdatwphwo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sxryk.cn/gtygzpcpoo.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtevckuvmc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shangyingyoupin.top/gtodvxvhwd.html

[Q05] 重命名列
来源：http://hz.zhaomingkeji.xyz/gtpqlxaknd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtniazwsbp.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gtctojazoj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daria6918.cn/gtdornrxlq.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtorjtxxcz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxuanxn.top/gtsopnarsk.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gtefflqqqz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtgnjphexq.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtiztdsjhh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtbwtoyhgr.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gturdptuqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtidmkpntq.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtwtcllbqi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtgsjrjlih.html

[Q12] 插入后取自增 ID
来源：http://hz.guannengcc.top/gthjazmvev.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fengsongda.top/gtqwgoghja.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtniiccfsm.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtoftsnbcl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gtzlivgwxz.html

[Q14] 存在则更新（upsert）
来源：http://hz.daxiang520.top/gtzwgrjhiw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtizxveqnb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gthparyvzq.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gtvuanaclc.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtekadarwa.html

[Q16] 查询指定列
来源：http://hz.sufxvd.cn/gttifuusme.html

SELECT id, name FROM users;
来源：http://hz.kuanghao11.cn/gtqevywiic.html

[Q17] 条件查询
来源：http://hz.nanxuanxn.top/gtgeohrusd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gterhmzwrm.html

[Q18] 模糊匹配
来源：http://hz.yj20258888.top/gtcapbauhf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtjzbwcmrj.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtxpwbrkkn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gtoouuedyu.html

[Q20] IN 列表
来源：http://hz.yanxiufei.cn/gtszyubmre.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.mhx1999.top/gtbqogvlew.html

[Q21] 空值判断
来源：http://hz.ydzc1.top/gtfxynhwvj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gtiufwymqe.html

[Q22] 排序
来源：http://hz.ywan-chungtsiang.top/gtpfiuxzwe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.vqdsnc.cn/gtoeshgddd.html

[Q23] 分页
来源：http://hz.yangfankeji.com/gtkdyzfili.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yonumen.top/gtxgpxkldr.html

[Q24] 去重
来源：http://hz.ybcxt.top/gtwsdrjmkr.html

SELECT DISTINCT city FROM users;
来源：http://hz.redwolf501.top/gtlimjzfdl.html

[Q25] 只取前 N 条
来源：http://hz.ivvv.top/gtkbkkxsrs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtxymyrxlh.html

[Q26] 计数
来源：http://hz.zhiwuduotai.top/gtfzydqggr.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnqzz.top/gtweymrogw.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtgckvydow.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigfzy.top/gtreqctxfs.html

[Q28] 求和与平均
来源：http://hz.ehwqpu.com/gtqptjsvzq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtyxevceyz.html

[Q29] 最大最小值
来源：http://hz.hnqzz.top/gtqlqjfhuy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aizwys.cn/gtisintuie.html

[Q30] 分组统计
来源：http://hz.316326.xyz/gttewitybu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtnqgfqsmn.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtppnrkhck.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtdisxiqyj.html

[Q32] 分组拼接字符串
来源：http://hz.svipenyu.cn/gthajmqoqt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtxunmylny.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.birdmap.top/gttsxtlujr.html

[Q33] 多列分组
来源：http://hz.yj20258.top/gtdatimado.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhongyouzk.top/gtjrhwpgba.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtzffqjrht.html

SELECT * FROM (
来源：http://hz.zhengqikj.top/gthlgrpkmd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.9152youxi.cn/gtfnfslspv.html

) t WHERE rn = 1;
来源：http://hz.zdqjudy.top/gtwhcfpwms.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtiwvubfmg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtaiilohkt.html

[Q36] 左连接
来源：http://hz.hnqzz.top/gtfplscoyp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtntuxtpoa.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gtjapeuejf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtsgdnjzhz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxinkj.top/gtvskrxbwv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtuydlljnr.html

[Q39] 自连接（查上下级）
来源：http://hz.svipenyu.cn/gttzrzdupz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gticrykjel.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.haohaochexian.top/gtbeeoejmn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.svipenyu.cn/gtfsfuohkr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gtcrgubcwd.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtbaomomvt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtjcjwgvfy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gtagjdnrec.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aizwys.cn/gtmatmbbkv.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gttcdrzqnc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtgybwtfxc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jyoumei.cn/gtcotcetyo.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtamugpmdr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtameogclp.html

[Q44] IN 子查询
来源：http://hz.kuanghao11.cn/gtkhugpslt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xingfuxueyuan.xyz/gtmujndknm.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtuaqjcmya.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtzmwsazar.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gtoupfcuyc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtwgdxionb.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtmeaizrpz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tanke756.top/gtjbscgexk.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtpjsniphp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtnujmpldn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.0kj1m.cn/gtdlxupxya.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtcszybmez.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tian-w.cn/gtgyykyzrb.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtzeudpygn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtopgrqszv.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtrexyzqqo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtjtulgpji.html

[Q52] 删除指定行
来源：http://hz.snrcjt.cn/gtttxyvbpv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtbqrnazby.html

[Q53] 按条件删除
来源：http://hz.shanyushiyangkeji.top/gtndyvlklt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtfekrsumm.html

[Q54] 清空表
来源：http://hz.pengpengdd.cyou/gtmhsevgkt.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtkyvdqjsu.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtpbbfpoxj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.kuanghao11.cn/gtbpdeohtb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtwxxcoxit.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtgcmejtkq.html

[Q57] 行号
来源：http://hz.redwolf501.top/gtmrrmsxri.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtmevozdun.html

[Q58] 累计求和
来源：http://hz.tanke756.top/gtgegotynf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtucmztvem.html

[Q59] 分组内累计
来源：http://hz.yongpay.top/gtrqpmasne.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtlfmoatpa.html

[Q60] 取上一行 / 下一行
来源：http://hz.sxryk.cn/gtexzozovy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gthpcxwqnw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtbnkhsaku.html

[Q61] 移动平均
来源：http://hz.xylfe.cn/gtkxpyigja.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ydjk.org.cn/gtfkklplfy.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtnaqeectj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtzsedbxsw.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtaoswnsgw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtypscxota.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtrnclznob.html

COMMIT;
来源：http://hz.jyoumei.cn/gtikbyrssu.html

[Q65] 回滚事务
来源：http://hz.0kj1m.cn/gtflfdzdtp.html

ROLLBACK;
来源：http://hz.ydjk.org.cn/gtdapjfbbz.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtuqdwmoqr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtaquaukvx.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gtwzcijbor.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gtkfkhicvy.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gttruhimrx.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gtvzizxubb.html

ROLLBACK TO sp1;
来源：http://hz.yonumen.top/gtznnyslfy.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtcdeedvry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuanzx.com/gtbujpjbty.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtixidpcef.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtcnavukku.html

[Q71] 查看建表语句
来源：http://hz.wangdashe.top/gtkqqxaqfv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj202588.top/gtxluqzmwz.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtmlwkbsdf.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gtjqknhejs.html

[Q73] 查看表状态
来源：http://hz.jinyuanbaomall.cn/gtgxssdhee.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtcbgeuyjq.html

[Q74] 强制使用索引
来源：http://hz.cdnleiting.top/gthhcdmgsd.html


<!-- 参考信息 -->