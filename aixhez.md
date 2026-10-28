代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtystngiec.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.0kj1m.cn/gtskikxtga.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtajdngahg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gtahpbjyrd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shzxlz.cn/gtkygujcwv.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gtbpkfukzm.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtfmqxdvfe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cucudq.cn/gtgoeyxduy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtcbyuzeca.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtomcreyle.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtesluvrml.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtdrtoirll.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zdqjudy.top/gtoiscwocl.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydzc1.top/gtgvifzofp.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtjlgmguqf.html

Py:   async def f():⏎    await g()
来源：http://hz.bjfxy.top/gttxbqwpho.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gttylwflit.html

JS:   async function f() { await g(); }
来源：http://hz.chenjidiqi.icu/gtsdvbsutp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtshjiovba.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtqmjsiisf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtfzpcvvsd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtshmixbhm.html

C#:   async Task F() { await G(); }
来源：http://hz.9152youxi.cn/gtlcqcnowm.html

[O05] 并发执行并等待全部完成
来源：http://hz.zdqjudy.top/gtptqmhgcp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtktstuwyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj202588.top/gtgypjxyqu.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtvkrhewij.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtpinfmpkd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhiwuduotai.top/gttakbqooa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgfzy.top/gtsnamfulz.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtomwaugtf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gteoelaclf.html

[O06] 使用进程池
来源：http://hz.9152youxi.cn/gtmyjbuika.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gogol.net.cn/gtjzqlnppn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtelahfubd.html

JS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtwfkamddr.html

TS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtuzaubbui.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cqqwz.cn/gtvtpwqyfx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtbiajetpx.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gtcivfzslc.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtudyklwky.html

================================================================================
来源：http://hz.nanxinkj.top/gtavpigecg.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtspibmtgf.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjgvjonop.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gtabzxtvhh.html

Py:   str(uuid.uuid4())
来源：http://hz.zhiwuduotai.top/gtfcrsnjum.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.andypj.xyz/gtmzxipryz.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtqkapxmlt.html

TS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtjrabmhhy.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gttfcaohzq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tanke756.top/gttorttpan.html

Ruby: SecureRandom.uuid
来源：http://hz.ehwqpu.com/gtndkobojz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtycjkivoo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinyuanbaomall.cn/gtozlfykvo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtbsjyooxy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hfpthk.cn/gtfgirlovq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtspurshhn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtsblbakna.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtxgvmzcgb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtcmkzyrqu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ehwqpu.com/gtvfatbqko.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtmyddiukn.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtzigjilnm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtwozyvzoa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sweek.top/gtrvdlaaxv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gttcrfwhjx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtmchibclj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gtolbldllw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenlongwang.top/gtnfgyyufl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtjegpknzm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtaviaupal.html

[P04] 求长度
来源：http://hz.zhixingplan.top/gtifptyaho.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhongyouzk.top/gtbztjcwim.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtdupbyife.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtatmhnwxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigfzy.top/gtdjorsdez.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtarukwnwy.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtjupkhhtp.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gthytatolw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtpyuzibnj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuanzhike.top/gtuwspbmfm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtwkjpwdam.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtmxovvmyc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gtnoipdajl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtckebsxic.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fengsongda.top/gttteaxhas.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yueranfly.top/gtnpirdthz.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtywddfmqg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.quarkkingdee.top/gtoenpezrj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtkatbuzcr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtusqvkgfv.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtjfpwajiy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guannengcc.top/gteslbhoip.html

TS:   if (x == null) {}
来源：http://hz.zhongyouzk.top/gtyotxqhiz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtbrxvcqmd.html

Go:   if x == nil {}
来源：http://hz.gaohongyu789.top/gtgjxoncqu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuxming.cn/gtrbtekzoe.html

C#:   if (x is null) {}
来源：http://hz.yonumen.top/gtatgteyqc.html

[P07] 防抖与节流
来源：http://hz.shuidangran.top/gtqrnmxeos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtctfrcyzq.html

PHP:  // 手写时间戳比较
来源：http://hz.svipenyu.cn/gtvrkfhyxz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtlnlxvnbk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtdhlrwwhf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ivvv.top/gttpqxmwwv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtbrtpktze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtuciauomn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jlsjyb.cn/gtqkwpheei.html

[P08] 处理浮点精度问题
来源：http://hz.feifeiyinyue.top/gtciakudkh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sweek.top/gtxvyhquke.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxinkj.top/gtjvnjlmrr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cqqwz.cn/gtqbtrurou.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtwmvzducu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinghuilouyu.cn/gthcjpmslp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtuvczrnzl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtsdhrfjxh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtbyfvzska.html

================================================================================
来源：http://hz.bjfxy.top/gthlbmtbpa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtyeydumyq.html

================================================================================
来源：http://hz.chenzaomai.com/gtnbpggtad.html

[Q01] 创建表
来源：http://hz.zhongyouzk.top/gtmdzwcnre.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtlyvfxpyw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtykdssegg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ydzc1.top/gtitigzrxf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtdokygvzu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtguwcifnk.html

);
来源：http://hz.sxryk.cn/gtnlhwzdvt.html

[Q02] 创建带外键的表
来源：http://hz.fengsongda.top/gtyoiwzrhj.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtwornvwvw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtzqxyjsft.html

user_id INT NOT NULL,
来源：http://hz.sweek.top/gtzafqihvn.html

amount DECIMAL(10, 2),
来源：http://hz.chenlongwang.top/gtcqoymhtt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtgsuyccax.html

);
来源：http://hz.316326.xyz/gtbwugoirm.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtyldvptyg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtmlbkyyfo.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtfqulhoxi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxuanxn.top/gtrbcqkhav.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtoeyqkwqx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtmadreyga.html

[Q06] 删除列
来源：http://hz.nanxuanxn.top/gtnvdqfgqq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gthyawigvk.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtweqzrcgy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtvnmzpxnf.html

[Q08] 创建普通索引
来源：http://hz.yongpay.top/gtmubzbaei.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtjtvfsfky.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gtcffmshwa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jianghu66.top/gtkfgsvgjr.html

[Q10] 插入单行
来源：http://hz.wangshuangyany.cn/gtfdtmeyvm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydjk.org.cn/gtwtlbvygj.html

[Q11] 一次插入多行
来源：http://hz.jianghu66.top/gtwiqlqvsz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtbrecrsaa.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtabpfzoid.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangkeji.top/gtlpngbxjs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cqqwz.cn/gtxxdamtot.html

[Q13] 忽略重复插入
来源：http://hz.cashguo.top/gthfzcgdwy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtrdtkidek.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtfqphctyl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtcvrvcehn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtcbmbjnha.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gtcmihlaqr.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtrhynntbv.html

[Q16] 查询指定列
来源：http://hz.haohaochexian.top/gtcoxzpplv.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtkogwgbko.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtsvrlukra.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtpcabudpn.html

[Q18] 模糊匹配
来源：http://hz.sysykeji.top/gtujpjsrsl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gteunayaod.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gteygrqmvy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nwbrower.top/gteezgzmnu.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gttsxzudkn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gtiqaauhmj.html

[Q21] 空值判断
来源：http://hz.quarkkingdee.top/gtmzooxukz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenjidiqi.icu/gttjlkltna.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtrxsgjmhl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.quarkkingdee.top/gtukqhclyy.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtlkexwvyc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gtzgaegelq.html

[Q24] 去重
来源：http://hz.fengsongda.top/gtsnsuxrvb.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtzkecwyuu.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtmwwddiqy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtqfqkumxe.html

[Q26] 计数
来源：http://hz.birdmap.top/gtbsmmhcog.html

SELECT COUNT(*) FROM users;
来源：http://hz.hammf.cn/gtjlbahvvi.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtqwhkbzpr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hysaishi.cn/gtxgbggofc.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtjdclzlkq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tanke756.top/gtcwdiksmw.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtanzvyqxb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtddhqafqm.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtpgqjaefb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtqgkgtduz.html

[Q31] 分组后过滤
来源：http://hz.guannengcc.top/gtvgurexit.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.iojbl.cn/gtjnywwnrv.html

[Q32] 分组拼接字符串
来源：http://hz.pengpengdd.cyou/gtulcovuzf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtztetaigm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhengqikj.top/gtukpymael.html

[Q33] 多列分组
来源：http://hz.0kj1m.cn/gtrfsckame.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtkhkcwikl.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtooeyvxrp.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtktcndqfp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtiqytpamk.html

) t WHERE rn = 1;
来源：http://hz.chenzaomai.com/gtjhaasltn.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtxtctrjym.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtbxeufufm.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtrglbemxj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtkcximfbx.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtiufrakgl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangkeji.top/gtgpibapsi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtalnkphmw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.52xcode.cn/gtniklssjs.html

[Q39] 自连接（查上下级）
来源：http://hz.ivvv.top/gtznpehuer.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daria6918.cn/gtmwptdpsb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtlvtgkjrv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtzgblmdak.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhiwuduotai.top/gtxqbgcyab.html

[Q41] 多表连接
来源：http://hz.snrcjt.cn/gthsbrseei.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtkoqprjts.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuanzhike.top/gtpkipoffs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtvzqwgxqy.html

[Q42] 连接条件附加过滤
来源：http://hz.yonumen.top/gtsqahzkbt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gthjcwbgwz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtpmvhdhte.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtzpbxksgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hfpthk.cn/gtebcbyoli.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtlrcwfiag.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pycfn.com/gtztvfxjwm.html

[Q45] EXISTS 判断存在
来源：http://hz.0kj1m.cn/gtknrablvt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtehhslksh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtwhtjfflt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtzymyrdwr.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtajnkxcew.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.9152youxi.cn/gtclmteyco.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtuekxxjjb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtgrqxskfg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dashuyun.cn/gtmjytapxo.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtyuulyhfc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.meibo888.top/gtgjunzxea.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtjioiwefa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtpvijljdy.html

[Q51] 用子查询更新
来源：http://hz.shzxlz.cn/gtharvfukz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtcerkzayn.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gtrgpvoqab.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtzfmauhep.html

[Q53] 按条件删除
来源：http://hz.pycfn.com/gttqsimpza.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnxiangtu.top/gtwatjokmh.html

[Q54] 清空表
来源：http://hz.nanxinkj.top/gtqbmagzlu.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtyiwcvlyq.html

[Q55] 排名（并列占位）
来源：http://hz.jinyuanbaomall.cn/gthnwopsst.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtamnaeuut.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtsjupovls.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydjk.org.cn/gthnoehsef.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtyqgdbxwi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258.top/gttwazdpgi.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gtrvuciwpz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.bjfxy.top/gtkqmlszlz.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtpypqojhx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxinkj.top/gtfbqphksj.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtibxqmquo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtkyeetict.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtucwidrrk.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtdutuiaeb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gteuxrhsvd.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtensxcesz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtfpxcogrm.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtuyrhdlbh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtsqbdajod.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtmgylphey.html

COMMIT;
来源：http://hz.tanke756.top/gtuchsirun.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtcrigaotb.html

ROLLBACK;
来源：http://hz.havefunace.top/gtkrknzayp.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtzxasuxct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtscdjacek.html

[Q67] 设置隔离级别
来源：http://hz.haohaochexian.top/gtbdbjpxzu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigfzy.top/gtipipggue.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtgvzvicus.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtielplihi.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtiotyhvaj.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtmzhxphxl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yonumen.top/gtibvzycnj.html

[Q70] 更新统计信息
来源：http://hz.iojbl.cn/gthsihkwwh.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtyvahoyad.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gthfadeiln.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtnigudyyj.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtmhjcqwps.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gthnlzdrci.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtvpzydjrl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinghuilouyu.cn/gtbrwtyvrj.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtvecwtfgs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cheryme.top/gtktlucthz.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtmgozmcbx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gtalxozbdn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtiveqzniz.html

[Q76] 按天统计
来源：http://hz.gzhubu.top/gtbkihdiae.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtmusihtsq.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gtcgrsnmmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sweek.top/gtrgkycorf.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtrwechelx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtherjvkwa.html

[Q79] 字符串拼接
来源：http://hz.chenzaomai.com/gtrqccxspo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtebpvszuj.html


<!-- 参考信息 -->