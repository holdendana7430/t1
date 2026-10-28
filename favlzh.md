代发 wailian999

[O02] 使用线程池
来源：http://hz.tian-w.cn/gtohtmsfha.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhiwuduotai.top/gtwafygpwp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.meibo888.top/gtduazmylp.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtetyxgugz.html

TS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtokgmbwpw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtugtdxnza.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.andypj.xyz/gtxnhdbasc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ybcxt.top/gtdhyqeqaq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtuyxhjszo.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtmoqpxnxv.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtmkesdtlm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtorezbtni.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtzcgkbxks.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtovahdprm.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtrmokuezk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jlsjyb.cn/gtyibgtfnp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenjidiqi.icu/gtjqqxuthp.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtozjliava.html

[O04] 定义异步函数并等待
来源：http://hz.hywenlv.cn/gtkaalwqyj.html

Py:   async def f():⏎    await g()
来源：http://hz.pengpengdd.cyou/gthdlducfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ivvv.top/gtlrztxkou.html

JS:   async function f() { await g(); }
来源：http://hz.zhixingplan.top/gtbibxcvrj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.kuanghao11.cn/gtscetsbgd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtbxavoswv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtgsqjzmsz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtrpawypfo.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtgqmaehqd.html

[O05] 并发执行并等待全部完成
来源：http://hz.9152youxi.cn/gtuprchjtl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtjqogeqyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj202588.top/gtexetsmdh.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtlptfzmzr.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtohyytiys.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gzhubu.top/gtbwkqjxvn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuanzx.com/gtaevqsqhg.html

Ruby: threads.map(&:join)
来源：http://hz.mhx1999.top/gtvfrxadeg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.9152youxi.cn/gtlgoaqqfh.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gtxovcqzhr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtcxutzzua.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jiagoushi.top/gtewbeaflv.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtdfbhgigy.html

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtgwcxmwel.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shuidangran.top/gtqlngegwv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtaafzrhsq.html

Ruby: // fork 块
来源：http://hz.yvedp.cn/gtthlnilsc.html

C#:   Parallel.For
来源：http://hz.xuanzx.com/gtfsfplxur.html

================================================================================
来源：http://hz.cheryme.top/gtvnmqjfpt.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtglnytfxd.html

================================================================================
来源：http://hz.cashguo.top/gtwmrkyeqx.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gttrtslpqa.html

Py:   str(uuid.uuid4())
来源：http://hz.ivvv.top/gtsomzygcl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtmpgxuzju.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtysajkeus.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtuqxgqlbr.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtoazsegml.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangshuangyany.cn/gtzzskvwlj.html

Ruby: SecureRandom.uuid
来源：http://hz.ydjk.org.cn/gtizxttvns.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sufxvd.cn/gtyndzffka.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgufenzy.top/gtpqvlowhx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtrbizjxed.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtpwmbhqve.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.havefunace.top/gtpypgpohp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtghoivrid.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shanyushiyangkeji.top/gtgufxibke.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sysykeji.top/gtyxojfqdl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtvvjbuuao.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhoulong.xyz/gtrvtvxkck.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gtgbaggkcn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtqzpbbzth.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.mhx1999.top/gtabfhiyaa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtmrxwelnj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gttrnuzxdi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtzxazpdwi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gteoxwipct.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtzkbzzhvh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ivvv.top/gtlnvnfdtg.html

[P04] 求长度
来源：http://hz.cdnleiting.top/gtxvbrlxqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yueranfly.top/gtmzbbygrm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtghfxmwim.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtqovyrigo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtanqqosgi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hywenlv.cn/gttuenprki.html

Go:   len(arr);  len(m)
来源：http://hz.cdnleiting.top/gtsgpfkhhj.html

Ruby: x.length;  x.size
来源：http://hz.kuanghao11.cn/gtmpdqniup.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtnzwrrylz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtnspqpvag.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dashuyun.cn/gtkkgpujnp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtlmvuihhi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yvedp.cn/gtofqxwoff.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gteprkbfeb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtctphsyox.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtybygiyob.html

Ruby: a == b
来源：http://hz.yangfankeji.com/gtrjdmbyhg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258888.top/gtdfcymmbi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gtocyeiqvi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtmzszooft.html

PHP:  if (empty($x)) {}
来源：http://hz.hongshengwenyu.top/gtejorpakf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtsslzbjyj.html

TS:   if (x == null) {}
来源：http://hz.tianlin.xyz/gtqwvornag.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtgvtdhrbe.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gtmjunkrjg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtgwphxzna.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gttbfgpouw.html

[P07] 防抖与节流
来源：http://hz.xziqi.cn/gtgvjjigcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yangfankeji.com/gtmsiktkov.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtwcrzqeia.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtbjxsiexw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtvekjdvyd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtafeckxjw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtajlddnpm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtpzvukvwl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gotoacloud.top/gtjzvivoma.html

[P08] 处理浮点精度问题
来源：http://hz.pycfn.com/gtbihoaiwa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hysaishi.cn/gtmhrjqriu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtrhbnrlui.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtfjbiatyw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tian-w.cn/gtysifafxi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtlpivirkl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yueranfly.top/gtfmguszxh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cdnleiting.top/gtpdouvspr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtdbvdrbzu.html

================================================================================
来源：http://hz.xuanzx.com/gtcuqajvgq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhiwuduotai.top/gtgonflnne.html

================================================================================
来源：http://hz.yj20258888.top/gtvosoqfiy.html

[Q01] 创建表
来源：http://hz.zhaomingkeji.xyz/gtmtcvcdix.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtyddthcbh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtbwxjemkd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtvsbfjqng.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gtaqxbldds.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yueranfly.top/gtawqidblv.html

);
来源：http://hz.pycfn.com/gtujpigoms.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gttmxcdwxq.html

CREATE TABLE orders (
来源：http://hz.gotoacloud.top/gtzcpmvjir.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtfbplhfvz.html

user_id INT NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtjlubkyzs.html

amount DECIMAL(10, 2),
来源：http://hz.jqgfzy.top/gtxirgsrrx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenzaomai.com/gtazjcbghf.html

);
来源：http://hz.sysykeji.top/gtfgbkgjas.html

[Q03] 增加列
来源：http://hz.ywan-chungtsiang.top/gtgehctdnw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gttpcftikt.html

[Q04] 修改列类型
来源：http://hz.mhx1999.top/gtzzdooijd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daxiang520.top/gtruwvmqpe.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtlziylrhd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.316326.xyz/gtyuprnksb.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtcmiokrws.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtbfijcabt.html

[Q07] 删除表
来源：http://hz.ppjwa.cn/gtmnzgglnp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtxjyczcyf.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtfmblelup.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtivlrflvc.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtqpxbeqsb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtdpotuoyb.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gtxtizyicq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxuanxn.top/gtztajvkmm.html

[Q11] 一次插入多行
来源：http://hz.c1oappe.top/gtkkeniamp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gtqosrqyrm.html

[Q12] 插入后取自增 ID
来源：http://hz.snrcjt.cn/gtzdwuetvt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yvedp.cn/gtydhnwzdh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gtbzvdxolt.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtbpemsqru.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gteqzwgkie.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtyhcrsrlf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sxryk.cn/gtbkxocazh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtskrbxqxe.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gtdbvsesre.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtppeadfko.html

[Q16] 查询指定列
来源：http://hz.sysykeji.top/gtnjhuhief.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtxlspnhux.html

[Q17] 条件查询
来源：http://hz.smart0.xyz/gtsmuugzgy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtibnjqcmd.html

[Q18] 模糊匹配
来源：http://hz.fengsongda.top/gtdujcqwba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtjmyscrqk.html

[Q19] 范围查询
来源：http://hz.xziqi.cn/gtcujjwqaj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nwbrower.top/gtktjlnzyv.html

[Q20] IN 列表
来源：http://hz.bjfxy.top/gtukthczzh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtvwbbokre.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtcctroktj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtprmmlrvl.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtsfbhnkfx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ywan-chungtsiang.top/gtipziijcj.html

[Q23] 分页
来源：http://hz.c1oappe.top/gthjgexazi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangtech.top/gtapqamufu.html

[Q24] 去重
来源：http://hz.sysykeji.top/gtsadjsjwh.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtrhhiqcvj.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtgtashbws.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yongpay.top/gtxgxqcsxd.html

[Q26] 计数
来源：http://hz.xinyue.icu/gtpytqatkv.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gttsybbszb.html

[Q27] 条件计数
来源：http://hz.ywan-chungtsiang.top/gtfeapquoy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yueranfly.top/gtrzsqmshp.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtibgpbbma.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtctstjqjr.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtchryaluf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydjk.org.cn/gtvmgjujcg.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtgzndwkgf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtfahvfivv.html

[Q31] 分组后过滤
来源：http://hz.yuanzhike.top/gtgibwnzwq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtbhrmzwjr.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtsyoaevqo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtqpmuasuw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.meibo888.top/gtiofknpsi.html

[Q33] 多列分组
来源：http://hz.yanxiufei.cn/gtrxrxdqqz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtyvquovsk.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtbsxtzfso.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gtgmlexofa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtienmwyfi.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtzlmctunn.html

[Q35] 内连接
来源：http://hz.jqgfzy.top/gtpshdtnvg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtmxsuvorg.html

[Q36] 左连接
来源：http://hz.gotoacloud.top/gtwscpmhoy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtzobkalrs.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtlqcckizv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtkyftvast.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtartqdbjs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ywan-chungtsiang.top/gthhrbrhcq.html

[Q39] 自连接（查上下级）
来源：http://hz.zhongyouzk.top/gtwepnzccj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gtskhgnreo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhongyouzk.top/gtdsfvtgzy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yanxiufei.cn/gtfctjtbcl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtlmvjfdwt.html

[Q41] 多表连接
来源：http://hz.feifeiyinyue.top/gtekvpjqam.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ehwqpu.com/gtopvfqavi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ppjwa.cn/gtwpgjiebw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jyoumei.cn/gtxovmyggj.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gtuvytfjli.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtluezmgec.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtdeiwcavt.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtyjkviojz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gzhubu.top/gtjfgzykza.html

[Q44] IN 子查询
来源：http://hz.ppjwa.cn/gtfvolfnve.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yvedp.cn/gtdesdgaoy.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtyzzosgus.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtpnfbyggk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtsrlrchta.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtfcenhzfj.html

[Q47] 与平均值比较
来源：http://hz.guannengcc.top/gtbvblvznr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtqotbvdlf.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gthfwtcuyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gtegmnzajx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daria6918.cn/gttildiyzw.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtrqyjcgif.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gttazzugjk.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtyvhgdavf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtdrpledhf.html

[Q51] 用子查询更新
来源：http://hz.yongpay.top/gtxuievzcu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.quarkkingdee.top/gtrnqvnmmp.html

[Q52] 删除指定行
来源：http://hz.hnxiangtu.top/gtxkxgugft.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtdnllktod.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gtsvzgysgh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtwgvyqubo.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtpvlezpxg.html

TRUNCATE TABLE logs;
来源：http://hz.ydjk.org.cn/gtbpguowel.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtjxlrluvb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nwbrower.top/gtfugzmsan.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gttsirxtlz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydzc1.top/gtdalijasv.html

[Q57] 行号
来源：http://hz.xziqi.cn/gthmskemaa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nwbrower.top/gtlaqkicnz.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtcxdnmodc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gthbssvzdt.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtbjasfjjk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtgmyjvotp.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gttjiuzgyj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fengsongda.top/gtvrouyvmn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gttngknzyt.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtzgwtpyua.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtvdxjblnq.html

[Q62] 分组占比
来源：http://hz.smart0.xyz/gtfzgnbtdn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gthaiimzgo.html

[Q63] 开启事务
来源：http://hz.nwbrower.top/gtbtazqjtf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhaomingkeji.xyz/gtbylphnzz.html

[Q64] 提交事务
来源：http://hz.nwbrower.top/gtqsczhefs.html

COMMIT;
来源：http://hz.yangfankeji.com/gtwphkhkxj.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtzzcrbjfz.html

ROLLBACK;
来源：http://hz.tanke756.top/gtedzhxjmu.html

[Q66] 行锁查询
来源：http://hz.aizwys.cn/gtndrglpmb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtemtfubqb.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gttgfarlmn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtyuldjduq.html

[Q68] 保存点
来源：http://hz.yongpay.top/gtifmrmrqx.html

SAVEPOINT sp1;
来源：http://hz.ywan-chungtsiang.top/gttztjjfqh.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtsxofosbo.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gtcohhlzuq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtgagzvvqn.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtoygoxiqn.html

ANALYZE TABLE users;
来源：http://hz.xuanzx.com/gtxgidjjzp.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtxswnafyn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtjcyzboop.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtgdpyoqrc.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtgedjdkeu.html

[Q73] 查看表状态
来源：http://hz.tanke756.top/gtzljsksrg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtymvknyan.html

[Q74] 强制使用索引
来源：http://hz.jinghuilouyu.cn/gtflegohbx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtaomnywhe.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gtobhkxfpf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.snrcjt.cn/gtrhxsjmug.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj202588.top/gtegqieuaw.html

[Q76] 按天统计
来源：http://hz.tian-w.cn/gtjmlzgcrf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gtxhmmrpyd.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtihajjofr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.andypj.xyz/gtxkrfqmxk.html


<!-- 参考信息 -->