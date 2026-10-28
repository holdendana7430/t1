代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gzhubu.top/gtzbyvilnj.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtikvrifxp.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtpurywhut.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtrtgnfadf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhengqikj.top/gthxreerfr.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtchjuokax.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtyiooljgf.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtnmapwctg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhengqikj.top/gtulvblama.html

JS:   async function f() { await g(); }
来源：http://hz.zhongyouzk.top/gtudhsfcel.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuanzhike.top/gtxrdcgzfu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gttgsrtxgq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258.top/gtbutgqzwi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.9152youxi.cn/gtdnjgaspu.html

C#:   async Task F() { await G(); }
来源：http://hz.yvedp.cn/gtjeuymjfz.html

[O05] 并发执行并等待全部完成
来源：http://hz.cqqwz.cn/gtlifmtena.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtlntyxpgu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxuanxn.top/gtlzmwbcqi.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtqvswdlsz.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtrcwqappf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhaomingkeji.xyz/gtphnkpcqi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tian-w.cn/gtaaferdad.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtjocmamzy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtltrbeupt.html

[O06] 使用进程池
来源：http://hz.ydjk.org.cn/gtmbnpsaad.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenjidiqi.icu/gtyduvvhxf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtflunvgax.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtwupjhqrm.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtmcfuadjp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gtpwecafeo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.316326.xyz/gtsambzmxu.html

Ruby: // fork 块
来源：http://hz.yongpay.top/gtkuhjkldp.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtavkvqttt.html

================================================================================
来源：http://hz.jqgfzy.top/gtegyyilqe.html

P. 常用工具函数
来源：http://hz.hongshengwenyu.top/gtqqjvorda.html

================================================================================
来源：http://hz.sxryk.cn/gtdeclqcbd.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtgqevvdyj.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtqfwneseu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtecoaiubw.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtrdwlkmxg.html

TS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gthwccsrxh.html

Java: UUID.randomUUID().toString()
来源：http://hz.yueranfly.top/gtbeyqkuph.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydzc1.top/gtlizeiegx.html

Ruby: SecureRandom.uuid
来源：http://hz.xziqi.cn/gtswncmnzk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigufen.top/gtkuyipmmg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtxnannfnr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gtzhdyxzyz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hongshengwenyu.top/gtlsssausd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgufenzy.top/gtikldnpbb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sxryk.cn/gtuytusclc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtmiopzfmk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtdqwlevox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtelruijvb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gtvlbsieht.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtcmqthrfp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtspieclbu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shuidangran.top/gtggrzrlbs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ehwqpu.com/gtjwyztxwp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtkwrksayf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuetiantiany.cn/gtmvvtkcqo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gtdzpibulh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gzhubu.top/gtaycldspx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnqzz.top/gtorzhkpfr.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gtnlvztdld.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtmuuhimak.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtytoqzffp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtfrkjeiuk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtqbmokbye.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangdashe.top/gthocmspan.html

Go:   len(arr);  len(m)
来源：http://hz.jinyuanbaomall.cn/gtddiedfnk.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gtunomdkaf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gogol.net.cn/gtnivpsxmw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtgavzqbjm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtaedhvevr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtpuoyvivj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtmhlfhxet.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtcsckfluv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.316326.xyz/gtglnczwcs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xziqi.cn/gtnqkzncss.html

Ruby: a == b
来源：http://hz.yuxming.cn/gtdduhhfcy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtrrljhcbf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtlwhxazyo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtreokodiw.html

PHP:  if (empty($x)) {}
来源：http://hz.havefunace.top/gtnhxvdhkr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtthzvbtyr.html

TS:   if (x == null) {}
来源：http://hz.kuanghao11.cn/gtixxlidsd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gtiwjfqahu.html

Go:   if x == nil {}
来源：http://hz.bjfxy.top/gttxpvuozq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.9152youxi.cn/gtmhfhudeg.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtqtnmhzdk.html

[P07] 防抖与节流
来源：http://hz.gzhubu.top/gtissfuzdl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shuidangran.top/gtvtxwogxl.html

PHP:  // 手写时间戳比较
来源：http://hz.bjfxy.top/gtyeqnxxph.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtpmbpgwrb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtqwftwurh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.vqdsnc.cn/gtlkbdpmkm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtqztxxwot.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtzvlufcmf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cqqwz.cn/gtxbkfgqty.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtkguwtvxr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhongyouzk.top/gtjmutbugv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yonumen.top/gtibfyuwyr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtlmuyxemj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sweek.top/gtoccwlhlg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guannengcc.top/gtsiefkapd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.havefunace.top/gtnlaimojq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sweek.top/gtuqmtnyfy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj202588.top/gtmgptnmsm.html

================================================================================
来源：http://hz.yongpay.top/gttgohnoov.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daxiang520.top/gtnfybwguy.html

================================================================================
来源：http://hz.c1oappe.top/gtxlrawonu.html

[Q01] 创建表
来源：http://hz.c1oappe.top/gtjkgbrxne.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtzgdaqwbj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtohavidrj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gotoacloud.top/gtbhonywzr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258888.top/gtilfaxqyx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtoqbcgfvb.html

);
来源：http://hz.dashuyun.cn/gtdkfgeqhh.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtkedwyrwv.html

CREATE TABLE orders (
来源：http://hz.yueranfly.top/gteaftnxtd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtrnjdmolt.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtclmcwtzo.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtjhbbtwsw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenlongwang.top/gtoyzfxewl.html

);
来源：http://hz.birdmap.top/gtsfclbttg.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gthebezhxg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gttzkcqwtp.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtxnqjqmus.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxinkj.top/gtckejizyi.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gthnuoqvir.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sxryk.cn/gthtvqxefq.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtdrwqbmet.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gthirewjzi.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gtmgiqwzus.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtigmwbagq.html

[Q08] 创建普通索引
来源：http://hz.smart0.xyz/gtkiibeibs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sxryk.cn/gtcimeknnf.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtaflgasno.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtpfbhflnd.html

[Q10] 插入单行
来源：http://hz.cdnleiting.top/gtnajazspr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj202588.top/gtayztpchw.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtvobhfhic.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtkmqrcuky.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtwjxnyvqu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhongyouzk.top/gtyjqekfhv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gtuwxjmzyx.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtibwkizsb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tanke756.top/gtmlnvjdhr.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtzrljuhae.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtwjbbgxti.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gtwjkcpepm.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gtrrlvivkq.html

SELECT * FROM users;
来源：http://hz.yuxming.cn/gtervkhjtx.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtupzjjnmi.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtsatqovfp.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtgckyvmgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuanzx.com/gtaohencfv.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtwzolrefi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cheryme.top/gtylldunxk.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtmjsvqjsi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.kuanghao11.cn/gtyehsakjy.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtulibhjky.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtnzxczozm.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtozdwekbk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.9152youxi.cn/gtrcgqaboe.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtlsmaapea.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtauzyjzvj.html

[Q23] 分页
来源：http://hz.meibo888.top/gtpnzchwvg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtprcwomke.html

[Q24] 去重
来源：http://hz.cheryme.top/gtwcjtsmxy.html

SELECT DISTINCT city FROM users;
来源：http://hz.shzxlz.cn/gtijwxfwjh.html

[Q25] 只取前 N 条
来源：http://hz.birdmap.top/gtwskzvqor.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shuidangran.top/gthlhfzimy.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtjzljakym.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtngfmnsuq.html

[Q27] 条件计数
来源：http://hz.gogol.net.cn/gtxysnrwbm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yangfankeji.com/gtsvmuzyav.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtknbvodyb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ybcxt.top/gtaowhmshd.html

[Q29] 最大最小值
来源：http://hz.cheryme.top/gtlspvnfmm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hysaishi.cn/gtpysqwnmt.html

[Q30] 分组统计
来源：http://hz.sysykeji.top/gtpjnziyuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtzfhrhvgj.html

[Q31] 分组后过滤
来源：http://hz.tian-w.cn/gtrahugxpp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hammf.cn/gtjiykboet.html

[Q32] 分组拼接字符串
来源：http://hz.xuetiantiany.cn/gtoavqfvkc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtckrbvcmh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zdqjudy.top/gtqdwgybti.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gttebleboc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtgvefyojk.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtbxjvzdqe.html

SELECT * FROM (
来源：http://hz.andypj.xyz/gtturtrhkf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gteryrbjdv.html

) t WHERE rn = 1;
来源：http://hz.hfpthk.cn/gtcxawjmqf.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtmmapelol.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtmcusqnek.html

[Q36] 左连接
来源：http://hz.zhixingplan.top/gtuxgtlfcn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtuxjeknob.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtrgihrtwz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtvicndnjj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xingfuxueyuan.xyz/gtpfshjyqo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.birdmap.top/gtvvexejxj.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtchitquie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtgswovsbv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.havefunace.top/gtlvxegayd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtljlgslly.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtgwjueiss.html

[Q41] 多表连接
来源：http://hz.jianghu66.top/gteekruvey.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dashuyun.cn/gtnagprivw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.mhx1999.top/gtvyrpeykl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ywan-chungtsiang.top/gtyzulkpll.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gtuknqgrdc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shangyingyoupin.top/gtrpcdinhd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuanzx.com/gtjdbdjlvs.html

[Q43] 标量子查询
来源：http://hz.pycfn.com/gtdmyasjld.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tianlin.xyz/gtazqxoxts.html

[Q44] IN 子查询
来源：http://hz.ppjwa.cn/gteskzjrlu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guowangkeji.top/gtlnmvthyj.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtxlhjvzbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gttikpgxgv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtkwrujudl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtsnpdvtqz.html

[Q47] 与平均值比较
来源：http://hz.havefunace.top/gtwnehgfpx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtgejclcmw.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtzolkjgvk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gtzagxbutl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtbnpetxnc.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtxjifrspt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gtjhixlzmu.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gttnschhdn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtkpgibndl.html

[Q51] 用子查询更新
来源：http://hz.dianchejie.cn/gtzqhhwivh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtkzswxntf.html

[Q52] 删除指定行
来源：http://hz.yanxiufei.cn/gtycilzwwc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gttzdwahtf.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtxybkzimb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tanke756.top/gtvhgocqsv.html

[Q54] 清空表
来源：http://hz.nwbrower.top/gtvbijwgff.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtflbydokl.html

[Q55] 排名（并列占位）
来源：http://hz.yvedp.cn/gtwgmejoug.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gthajnpxcn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtlztzoygz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.quarkkingdee.top/gtoiounfng.html

[Q57] 行号
来源：http://hz.xinyue.icu/gtddndlmjb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hongshengwenyu.top/gtdphfkcnb.html

[Q58] 累计求和
来源：http://hz.chenlongwang.top/gtevfjloep.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtcbljjsfs.html

[Q59] 分组内累计
来源：http://hz.cucudq.cn/gtnzqgogdf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtypuezljq.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj202588.top/gtunanniob.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtnzvvrmao.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.9152youxi.cn/gtydxvbxns.html

[Q61] 移动平均
来源：http://hz.haohaochexian.top/gtrjjmxkaa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtfsxopbej.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtoflopenw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtqvfhclye.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtdqpxbqrh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aibaodan.cn/gtaolzupil.html

[Q64] 提交事务
来源：http://hz.wangdashe.top/gtpxzxdtri.html

COMMIT;
来源：http://hz.sufxvd.cn/gtsmhbegup.html

[Q65] 回滚事务
来源：http://hz.nanxinkj.top/gtscxmwrsj.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtjnmomeew.html

[Q66] 行锁查询
来源：http://hz.zhaomingkeji.xyz/gtmzowwtlw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtphcwwxpx.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gteczzvoqk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yangfankeji.com/gtygpcrfsg.html

[Q68] 保存点
来源：http://hz.gzhubu.top/gtmfbxzody.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtrwmikqko.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gthjpnykig.html

[Q69] 查看执行计划
来源：http://hz.aizwys.cn/gteqhxekyq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtfqruqrqy.html

[Q70] 更新统计信息
来源：http://hz.xziqi.cn/gtzxfkjnhv.html

ANALYZE TABLE users;
来源：http://hz.jinqigfzy.top/gtphchttzd.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtgkrmdiyt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258.top/gtzsqbrkcb.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtwmpprykr.html

SHOW INDEX FROM users;
来源：http://hz.hfpthk.cn/gtepvhusdq.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtowfxvbhy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gteihxolcb.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtersgeyaq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sweek.top/gtksmhgefl.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtezptclli.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gtmaeeczyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtryweazff.html

[Q76] 按天统计
来源：http://hz.cdnleiting.top/gtluzzuaea.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtdaxwuzkl.html

[Q77] 时间加减
来源：http://hz.aizwys.cn/gtxnqcyxsc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtugfmxcxc.html

[Q78] 当前时间
来源：http://hz.gzhubu.top/gtorfhdixo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aibaodan.cn/gtmssjvnrr.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtnjrotaod.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gtnhyjgdnn.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gttbiahdhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.iojbl.cn/gtyjkgavdq.html

[Q81] 字符串替换
来源：http://hz.jinqigufen.top/gtxmrvwsix.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtlwukdfzx.html

[Q82] 字符长度与字节长度
来源：http://hz.zdqjudy.top/gtiptxobkn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtrzvkiubq.html

[Q83] 大小写转换
来源：http://hz.haohaochexian.top/gtdjdqsjvt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydjk.org.cn/gtzauyrwcg.html


<!-- 参考信息 -->