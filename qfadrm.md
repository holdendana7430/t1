代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtkcqqdrbf.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtssztkmfx.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gtgavmznjh.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtrnnpelln.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gtwweqylxl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtzoqnoqwp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yongpay.top/gtlmdxcpun.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtuijbnrgq.html

TS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtkzoizmne.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtasjjqrom.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtzyyzqaqd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cqqwz.cn/gttrmrqmuj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zdqjudy.top/gtypwjrmgx.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtziimceua.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtovyxwjay.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jyoumei.cn/gtpbyeiyzr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shangyingyoupin.top/gtvzbhuwft.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtjgdiuvfm.html

Java: synchronized (this) { shared++; }
来源：http://hz.quarkkingdee.top/gtxlpmixqn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgfzy.top/gtsixkpojf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtbdxcvnuu.html

C#:   lock (gate) { shared++; }
来源：http://hz.iojbl.cn/gttnactadx.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtexazlmhr.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtjnesdigk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtisrpofel.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtosawismh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinghuilouyu.cn/gtejtrxphm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtvfehdumn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sweek.top/gtbjurygyt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigufen.top/gtfbsnqzdi.html

C#:   async Task F() { await G(); }
来源：http://hz.xinyue.icu/gtvwzzwxct.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtbzbselwm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xziqi.cn/gtywrlmmck.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gttrsaqrgq.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtdcevgeun.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtvkryluzw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.quarkkingdee.top/gtnoujzspg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.andypj.xyz/gtjchmpxjp.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtqlreycrb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sxryk.cn/gtpbcxdgdc.html

[O06] 使用进程池
来源：http://hz.dianchejie.cn/gtjmsthtpa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtomosoynx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtpwssdqyw.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtiybqdwhg.html

TS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtdxupqptr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinyuanbaomall.cn/gtwchnctld.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtgsyrezcd.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gtxydjrafb.html

C#:   Parallel.For
来源：http://hz.yonumen.top/gtcsvmfdek.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnruwoozb.html

P. 常用工具函数
来源：http://hz.gzhubu.top/gtrnbortvs.html

================================================================================
来源：http://hz.cqqwz.cn/gtqtfzmdfv.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gtggiyfjxw.html

Py:   str(uuid.uuid4())
来源：http://hz.zhongyouzk.top/gtrqnoexyo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtjgnrxbzs.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtwgdpbbkg.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtylxzcurd.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gtsceedlxb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xziqi.cn/gtwbbdimxc.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gtaznwbqfl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pengpengdd.cyou/gtuppgbqhm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtquiwblms.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtlzefvpjp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.meibo888.top/gtjvvkgnhj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yangfankeji.com/gtohodrskb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gaohongyu789.top/gthfxlqrtr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shuidangran.top/gtgzalyacl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258888.top/gtutrusmqc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aibaodan.cn/gttvsdzmfj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.quarkkingdee.top/gtsdxxeazw.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtztjikply.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.andypj.xyz/gtmjgmucwl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuanzx.com/gtpbvgxwwd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtrrkgqyon.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cdnleiting.top/gteeyhxzvf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenzaomai.com/gtjzlrbqpl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gtxveetvmu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hammf.cn/gtljaqdxqe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtbtzornpt.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gtknkxvtbl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtslwkponz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtgcckcocw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtkbcvhilp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gthddhjzhs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtlqyezhzy.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtgtrfszvh.html

Ruby: x.length;  x.size
来源：http://hz.dashuyun.cn/gtdzckvgnm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydzc1.top/gtttzrwstq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gaohongyu789.top/gtsjtdfpyg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yongpay.top/gtndxzjyws.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtjbwnripw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258888.top/gtsacrungc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtrbnzrwlw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtkwiianok.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtmeqpugmu.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtfumaqhla.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtyjqfuiop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtztrrykzf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gtbgnzrzmr.html

PHP:  if (empty($x)) {}
来源：http://hz.ydzc1.top/gtdjvikkvv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtpfbnkmeu.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtxawojdel.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtlsjplshx.html

Go:   if x == nil {}
来源：http://hz.zhaomingkeji.xyz/gtwdzwpjla.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtynltbbkn.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gttykzlrzm.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gthtqjimmm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhiwuduotai.top/gtapqplkcs.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtydgyfbas.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtbsjvbfih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtjwlytpol.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xingfuxueyuan.xyz/gtbsugmwer.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtoqtifcnc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ivvv.top/gtbtyecadx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtehcmhjai.html

[P08] 处理浮点精度问题
来源：http://hz.bjfxy.top/gtsshcedph.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangshuangyany.cn/gtaitzfxjs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtdqhmpvob.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtdtgpswjl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jyoumei.cn/gtrndfizfd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.c1oappe.top/gtxzihndqe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtyqqxnhmq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.svipenyu.cn/gtqhbjvits.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guannengcc.top/gtjxwkwobb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtincxfcmh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hysaishi.cn/gtavdphdst.html

================================================================================
来源：http://hz.dashuyun.cn/gtciwisjfv.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtiyubydzh.html

CREATE TABLE users (
来源：http://hz.yuanzhike.top/gtfbgbrfdw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtiechvqvl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cucudq.cn/gthtyfksxo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.0kj1m.cn/gtskchnfba.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtdhxyhfee.html

);
来源：http://hz.sweek.top/gthdxfycks.html

[Q02] 创建带外键的表
来源：http://hz.ybcxt.top/gtywdgvmsu.html

CREATE TABLE orders (
来源：http://hz.bjfxy.top/gtteazvdhk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtribnhlys.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gtuwiongqv.html

amount DECIMAL(10, 2),
来源：http://hz.cdnleiting.top/gtrksvobeh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.redwolf501.top/gtidzdiqxs.html

);
来源：http://hz.yongpay.top/gtsrgxsxrr.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gticvxtxfw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hongshengwenyu.top/gtwsnykihq.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gteiaebvlm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtgtibjeon.html

[Q05] 重命名列
来源：http://hz.smart0.xyz/gtgcaviegu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangkeji.top/gtquksvkau.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gtdqsttkbv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtsoylmxci.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gthjizuwgr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtkmxqvwzr.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gthdpitmqy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gtahggnfzk.html

[Q09] 创建唯一索引
来源：http://hz.ybcxt.top/gtgsgadngq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtpefavrbe.html

[Q10] 插入单行
来源：http://hz.316326.xyz/gtorgonudl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtzjnomqop.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtkckfqjaw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtfhbyfrul.html

[Q12] 插入后取自增 ID
来源：http://hz.jinqigfzy.top/gtwndooock.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gtdehowvro.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtvhbqmnfg.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtpvuysjix.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.redwolf501.top/gtxpkkzhps.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gttqsogcdr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sweek.top/gttspgyzfh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guannengcc.top/gtwnaowfgu.html

[Q15] 查询全部
来源：http://hz.snrcjt.cn/gtnlgeybbt.html

SELECT * FROM users;
来源：http://hz.ehwqpu.com/gtvqlqiddr.html

[Q16] 查询指定列
来源：http://hz.dashuyun.cn/gtszfttgmg.html

SELECT id, name FROM users;
来源：http://hz.sysykeji.top/gtqioiuwiq.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtsxsryglc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuanzhike.top/gtofwoafkj.html

[Q18] 模糊匹配
来源：http://hz.hongshengwenyu.top/gtliftgjbe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtwzhpekqb.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtgbzfivan.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtrsvazxbn.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtcvokdjhc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtdxtrtczk.html

[Q21] 空值判断
来源：http://hz.sweek.top/gtpjunhtav.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gtcyutbyst.html

[Q22] 排序
来源：http://hz.dianchejie.cn/gteeorutzm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtbgvufxpp.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtbunsfswi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cashguo.top/gtegyhplsr.html

[Q24] 去重
来源：http://hz.guannengcc.top/gtxtbgcjrc.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxuanxn.top/gtvjstotrs.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtydqhiesh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gtblzdeygc.html

[Q26] 计数
来源：http://hz.xinyue.icu/gtakjbhjgo.html

SELECT COUNT(*) FROM users;
来源：http://hz.sysykeji.top/gttyaschmw.html

[Q27] 条件计数
来源：http://hz.snrcjt.cn/gtywuxampq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtbmtbotnl.html

[Q28] 求和与平均
来源：http://hz.yonumen.top/gtiygbyrkg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cucudq.cn/gteonqdnjn.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtpxzrjxqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenlongwang.top/gtulysisqw.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtxtwrnblr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtkpwhaimc.html

[Q31] 分组后过滤
来源：http://hz.yuanzhike.top/gtsdajszpc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtnpbfvasr.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtlioglyvi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtnyfsomiu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtnblzghrt.html

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gtpfxyjtit.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jlsjyb.cn/gthaqsvpnp.html

[Q34] 每组取第一条
来源：http://hz.52xcode.cn/gtyplzbetx.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtgudvqlqs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258888.top/gtlhatftkj.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtamhdswmb.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtgqahjgwn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtwlhpwtwa.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtxnwqryuj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtfeaocpmi.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gttalhvoxj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nwbrower.top/gtmmzhbfjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hongshengwenyu.top/gtvrqaipns.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtozdzntaj.html

[Q39] 自连接（查上下级）
来源：http://hz.cucudq.cn/gtjypawqux.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gteynifgoy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.0kj1m.cn/gtardoxfcj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yuanzhike.top/gtlzljhxbc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnqzz.top/gtqtfhnpoi.html

[Q41] 多表连接
来源：http://hz.sxryk.cn/gtxbfzcuqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtpraxasau.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtvttnhafv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zdqjudy.top/gtifujgigp.html

[Q42] 连接条件附加过滤
来源：http://hz.tian-w.cn/gttrxospzn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ybcxt.top/gtfhoopgtg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtmjqqbrmj.html

[Q43] 标量子查询
来源：http://hz.jiagoushi.top/gtqljiieyt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtwpkntqas.html

[Q44] IN 子查询
来源：http://hz.tanke756.top/gtbstfrzyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cqqwz.cn/gtbneamqaa.html

[Q45] EXISTS 判断存在
来源：http://hz.aibaodan.cn/gtgxhrbvdc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtprteugiu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydjk.org.cn/gtzdcokiok.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtdxglssla.html

[Q47] 与平均值比较
来源：http://hz.jlsjyb.cn/gtbquwmxbg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yangfankeji.com/gtwaouzaio.html

[Q48] CTE 公用表表达式
来源：http://hz.zhongyouzk.top/gtztktfvhz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.kuanghao11.cn/gtsislvhly.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dashuyun.cn/gtekqppacl.html

[Q49] 更新单行
来源：http://hz.cucudq.cn/gtvdjxvngb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gtnrdaftvg.html

[Q50] 批量更新
来源：http://hz.sweek.top/gtwgzvjwji.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtlxxzcqen.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtwknzzhie.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtatedqpbw.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gtgtggzhor.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jiagoushi.top/gtjwqzjinm.html

[Q53] 按条件删除
来源：http://hz.yuanzhike.top/gtbjvcdkil.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258888.top/gtellyihbx.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtcalmtcla.html

TRUNCATE TABLE logs;
来源：http://hz.xinyue.icu/gtiangkjkp.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gtqghwlfbg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtpymmypil.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daxiang520.top/gtkixdrquh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhixingplan.top/gtfxahftki.html

[Q57] 行号
来源：http://hz.havefunace.top/gtzbmlgjpf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtazzqompn.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtuyddmhdr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtgqbehjpt.html

[Q59] 分组内累计
来源：http://hz.xingfuxueyuan.xyz/gtpsfkgxsc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtrouaploi.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gteohphkwr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj202588.top/gtbtylkhwe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtevfxsciq.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gthzmyhicy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtlhugtxhw.html

[Q62] 分组占比
来源：http://hz.wangshuangyany.cn/gtrxmydwyx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtgnrokigo.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtbhzngkea.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtfxmreeud.html

[Q64] 提交事务
来源：http://hz.tianlin.xyz/gtvbzhemxf.html

COMMIT;
来源：http://hz.zdqjudy.top/gtxubqhubg.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtwronteej.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtclmnafkn.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtoehtcdfa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.bjfxy.top/gtcoupxsdd.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gtwnzknowk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtkbvhbshu.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gtetatboti.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtpywlslpr.html

ROLLBACK TO sp1;
来源：http://hz.xuetiantiany.cn/gtcyurfrev.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtufidbhxa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtpsarcqww.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gtdpwjtgcw.html

ANALYZE TABLE users;
来源：http://hz.jqgufenzy.top/gtqnghxnvn.html

[Q71] 查看建表语句
来源：http://hz.gotoacloud.top/gtizpjmrgf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnqzz.top/gteptgjoow.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gtnuhyrlda.html

SHOW INDEX FROM users;
来源：http://hz.redwolf501.top/gtdajkjbbe.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gttzikfvtz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtqaxvljos.html

[Q74] 强制使用索引
来源：http://hz.pengpengdd.cyou/gtbqtxljcm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nwbrower.top/gtmpaglemh.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gteinntvkn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtbcdtfsfb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtsnoiefix.html


<!-- 参考信息 -->