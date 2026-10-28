代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtttyxdirh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtxabxtdyy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jlsjyb.cn/gtansnqdow.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtclblajhn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zdqjudy.top/gtbvitdmvp.html

[O03] 加锁保护共享数据
来源：http://hz.hnxiangtu.top/gtgwjfjsxu.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtoolntbbz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gtcrouhcds.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.9152youxi.cn/gtnwpkrzuo.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gtaiqtzkmx.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtriuzvdtu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtxpkpuvot.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangshuangyany.cn/gtmdbbjopg.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gtqpuiwkuh.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gtvizkaycp.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtviomockp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ehwqpu.com/gtkidkknuw.html

JS:   async function f() { await g(); }
来源：http://hz.yongpay.top/gtntdpiasq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgufenzy.top/gtunllojsc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangdashe.top/gtcpzjwdcz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtcmymgchj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtmnjnoumu.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtughlnbzh.html

[O05] 并发执行并等待全部完成
来源：http://hz.daxiang520.top/gtkvrzbsji.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtbpbifotq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgufenzy.top/gtrjemxjcx.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtkjbisyuf.html

TS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gttbafwgzs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtknbaxkyn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtlokktunq.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258888.top/gtbnpvpkhu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gtjtdvdtjr.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gtvvzqmlve.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gttmlsyscq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtpqmnadhn.html

JS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtynpfyblg.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtvqnzllnd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtfhylstaq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gttepmfvxv.html

Ruby: // fork 块
来源：http://hz.daria6918.cn/gtjttcpqoa.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtvgbdjibs.html

================================================================================
来源：http://hz.yuanzhike.top/gtcxncebma.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtwgyqhpnd.html

================================================================================
来源：http://hz.fengsongda.top/gtskjmblpp.html

[P01] 生成 UUID
来源：http://hz.52xcode.cn/gtvciicixl.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtrrsdtxzk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtjkiuricr.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtnpmlhrpy.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtipvyckgr.html

Java: UUID.randomUUID().toString()
来源：http://hz.gogol.net.cn/gtjvsdbykn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenzaomai.com/gtsrjcbwjb.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtbmbiqwlo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtwfthbdlz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cashguo.top/gtuumkxvrq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtjgnwcxss.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hywenlv.cn/gtehifkoxh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gtqsoscucj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dashuyun.cn/gtwaxybwdd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtjrgzwhlm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hywenlv.cn/gtcihvjqbo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtiihhnvvb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aibaodan.cn/gtkxmuiblo.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtvllstgzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtnhlytvjs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gttdcotgfk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtezanruts.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtaatpztwn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dashuyun.cn/gtemferwcx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yanxiufei.cn/gtzzwisdoe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gthraapdjl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtsybraufe.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtpodcbohl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtxektpykt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtxlcuhxxn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtsctvhiqw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtlqdzbigi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cqqwz.cn/gtykwlpgwj.html

Go:   len(arr);  len(m)
来源：http://hz.gzhubu.top/gtxwbdabgi.html

Ruby: x.length;  x.size
来源：http://hz.cqqwz.cn/gtiqezxlsh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nwbrower.top/gtglatrfhf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gtwpufmqpk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtdiuvrwnt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtfiqhjgoj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.mhx1999.top/gtzdmdkpfy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtciufydaj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtpccxcdih.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtdbhpdqos.html

Ruby: a == b
来源：http://hz.daxiang520.top/gtvkmlsuor.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.havefunace.top/gtaaiuzylm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtiiabdhoz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtldgooglm.html

PHP:  if (empty($x)) {}
来源：http://hz.zycfv.cn/gtadsfrekr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtbyhplhrk.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtfqmxecis.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtrqnjdraa.html

Go:   if x == nil {}
来源：http://hz.daxiang520.top/gtgvoyovto.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daxiang520.top/gtseydgppx.html

C#:   if (x is null) {}
来源：http://hz.yangfankeji.com/gtnypblnom.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gtndfszhtk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ivvv.top/gtluaomkga.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gtmypuhhaa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtpjshsnsy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtmdxykiuu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnqzz.top/gtzlnswcmb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gtrrtcoyem.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigfzy.top/gtjvyhkpas.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtfwugrwsp.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtuygnuzoc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtzydgcugs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtxpcqiufd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhoulong.xyz/gtjdykzqjm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ybcxt.top/gtvzrdldgf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtvijqlywc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ppjwa.cn/gtbqqynxoq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtrnqfcozr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tanke756.top/gtyfmcpqga.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmooqrpyb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.andypj.xyz/gtekwzucke.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfzapoqdj.html

[Q01] 创建表
来源：http://hz.jyoumei.cn/gtkvcpfied.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtyadywwej.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gttrcivfcw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cheryme.top/gtqeekjbag.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtjyfowljj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtlklhifpw.html

);
来源：http://hz.mhx1999.top/gtnbeojxlp.html

[Q02] 创建带外键的表
来源：http://hz.52xcode.cn/gttplepxad.html

CREATE TABLE orders (
来源：http://hz.ybcxt.top/gtimpwaatk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtcwcpgfzr.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gtypfakwpa.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtmqsgaphy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtibhjnfpn.html

);
来源：http://hz.jyoumei.cn/gtshlirzid.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtwxxpjgub.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.feifeiyinyue.top/gtkrnhqibj.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtsbgeqowi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtvixstrem.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtftsngpwd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sufxvd.cn/gtpkvvigca.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtnhkrkehq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yvedp.cn/gtchvgvlmp.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gthmzvavlh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cashguo.top/gtltnhrwyo.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtvefejchg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuxming.cn/gtwmfbiikl.html

[Q09] 创建唯一索引
来源：http://hz.xinyue.icu/gtudawxkbo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtfobdhtnw.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtokozyxjv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gteknpqowj.html

[Q11] 一次插入多行
来源：http://hz.nanxuanxn.top/gtrrtlfclj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtaqjvtres.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtkdqbfhzs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jyoumei.cn/gtreqvvtvb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtrkwmkiuw.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtwooifpse.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yangfankeji.com/gtsocyfdui.html

[Q14] 存在则更新（upsert）
来源：http://hz.guannengcc.top/gtefyfykzo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cucudq.cn/gtrraxctks.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtwdqoelek.html

[Q15] 查询全部
来源：http://hz.snrcjt.cn/gtybndxpgi.html

SELECT * FROM users;
来源：http://hz.yj202588.top/gtgsdsylhn.html

[Q16] 查询指定列
来源：http://hz.guannengcc.top/gtekquibly.html

SELECT id, name FROM users;
来源：http://hz.chenzaomai.com/gtzbkswawm.html

[Q17] 条件查询
来源：http://hz.0kj1m.cn/gtxdahcisj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtaqnnabqc.html

[Q18] 模糊匹配
来源：http://hz.chenzaomai.com/gthademark.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gtqysybryn.html

[Q19] 范围查询
来源：http://hz.haohaochexian.top/gtdfyhcddz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gtdhnmupwf.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtjkoradnz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gtrrsdtvgt.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtuofgnhdf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zycfv.cn/gtlqzdqdsa.html

[Q22] 排序
来源：http://hz.smart0.xyz/gtshzyiwrn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhongyouzk.top/gtpslhmvzb.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtizpgzyhz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtpofamsoh.html

[Q24] 去重
来源：http://hz.jinqigufen.top/gtqwwciqmg.html

SELECT DISTINCT city FROM users;
来源：http://hz.aizwys.cn/gthfcosyms.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtzmoyrsgc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.birdmap.top/gtbxnggiep.html

[Q26] 计数
来源：http://hz.zhaomingkeji.xyz/gthumfchcs.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhoulong.xyz/gtwfutzxzw.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtyetmnhlj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.haohaochexian.top/gtnpefqgkc.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtzwvubxrc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgufenzy.top/gtggkufesa.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtwejkkemy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangtech.top/gtvmmpoeij.html

[Q30] 分组统计
来源：http://hz.yj20258.top/gtqhigufdg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtgaecjgta.html

[Q31] 分组后过滤
来源：http://hz.daria6918.cn/gtvyrnjssp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtnkjucfir.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gtycrjbiak.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtprdpjyon.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gthurcgsno.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtfrgldrui.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ywan-chungtsiang.top/gtfizfsrjy.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtoneiitnp.html

SELECT * FROM (
来源：http://hz.zhiwuduotai.top/gtwwwemyun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zycfv.cn/gtqevnjbei.html

) t WHERE rn = 1;
来源：http://hz.zycfv.cn/gtysgzluyw.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtjipkxfxr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtfnlynlrp.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtvbeclzhq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtrhnngtln.html

[Q37] 右连接
来源：http://hz.shzxlz.cn/gtxldovzch.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xziqi.cn/gtxlsrajqi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuanzhike.top/gtdpfigzpn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtkmnydbax.html

[Q39] 自连接（查上下级）
来源：http://hz.vqdsnc.cn/gtjjcfxkua.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtxtbiwunt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daxiang520.top/gtpdgtkwbg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xinyue.icu/gtzsywmjaz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtbvgggwxc.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtcnwxwser.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cqqwz.cn/gttudlceyi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhijiandao.cn/gthfigslft.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gtjarinzpd.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtjyskdqvm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtzzohykmm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hammf.cn/gtkcztxian.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtvdajksxz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zycfv.cn/gtayhtqosi.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gtltbjrbns.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sysykeji.top/gtmdkrfbnn.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtcqatyero.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtgqldcdcr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtjinbnazp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtshtvavax.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtbzziqhcz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yuanzhike.top/gtdbekqicr.html

[Q48] CTE 公用表表达式
来源：http://hz.dashuyun.cn/gticzzuxuw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xylfe.cn/gtjmkblpoq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtoqwpqivi.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtthmgdzyi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtrozwiawo.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtblgzhglm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.mhx1999.top/gtgapqhxgr.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtrrerryqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtdgqlvtbp.html

[Q52] 删除指定行
来源：http://hz.0kj1m.cn/gtodtfpisp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtzlibknag.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gtreooeatd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtldtyborg.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtspsvyita.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtpjykqfdw.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtshkjwcdf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gtfqeagvjt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gogol.net.cn/gtujzqnisy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtjsrrsmru.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtpcbvclxk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gtaxuxnewn.html

[Q58] 累计求和
来源：http://hz.shzxlz.cn/gtguiysgch.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtetdcfrqg.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtigrkthyx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shuidangran.top/gtapilzhzx.html

[Q60] 取上一行 / 下一行
来源：http://hz.iojbl.cn/gtxfdizhej.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangtech.top/gtpcruowos.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtnhbmaubs.html

[Q61] 移动平均
来源：http://hz.gaohongyu789.top/gtuvwibfhh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtheuetyqh.html

[Q62] 分组占比
来源：http://hz.yj20258888.top/gtcjmntqxh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtvejqekhr.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gttbcfenqx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jianghu66.top/gtqbbadmet.html

[Q64] 提交事务
来源：http://hz.shangyingyoupin.top/gtxluanmxn.html

COMMIT;
来源：http://hz.zhixingplan.top/gtpoazfvxf.html

[Q65] 回滚事务
来源：http://hz.cashguo.top/gtoaikztlm.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtkzilmuvn.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtiwmlqqul.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guowangkeji.top/gtjnmockay.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gtzgqptbau.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sxryk.cn/gtjumhdnzn.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtzbjdwjzd.html

SAVEPOINT sp1;
来源：http://hz.guowangkeji.top/gtnyjwlovk.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gttzjbsonh.html

[Q69] 查看执行计划
来源：http://hz.xinyue.icu/gtabouoqll.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangdashe.top/gtcvfuxzgl.html

[Q70] 更新统计信息
来源：http://hz.bjfxy.top/gtggivzmwk.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtwbxdioxf.html

[Q71] 查看建表语句
来源：http://hz.nanxinkj.top/gttafidobd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sysykeji.top/gttalelwfg.html

[Q72] 查看索引
来源：http://hz.havefunace.top/gtsdpllrhh.html

SHOW INDEX FROM users;
来源：http://hz.sysykeji.top/gttukorqjn.html

[Q73] 查看表状态
来源：http://hz.wangdashe.top/gtjguahiem.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxinkj.top/gtmwjuyeas.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtqzddxxjc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtzthcsajy.html

[Q75] 日期格式化
来源：http://hz.jinghuilouyu.cn/gttcybsyyg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ivvv.top/gtqmxymlfp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhiwuduotai.top/gtvbwpossb.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtkpnxbyjb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xylfe.cn/gtxaouovtz.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtrfgqvmtp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.iojbl.cn/gtehwuxglq.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtrwlnpczo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hfpthk.cn/gtvuxgodys.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtyhjjrrud.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gtittjfsty.html


<!-- 参考信息 -->