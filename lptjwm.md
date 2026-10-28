代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtslawjtkk.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtqrcehrip.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtrovaarni.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtqelkeyzk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gthnjhqubz.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtguyryoxx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtehpcyabg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangshuangyany.cn/gtjbowfpoc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gaohongyu789.top/gtgihtrahy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtjfivuazv.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgufenzy.top/gtuzwmlvgc.html

[O05] 并发执行并等待全部完成
来源：http://hz.gogol.net.cn/gttptxbcli.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtfirssfrw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtmxwvkvpa.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtaelrqepq.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtcbkafots.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hongshengwenyu.top/gtjieivwne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangkeji.top/gtfydwhtzf.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtrsfwytwx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gtkfpzoror.html

[O06] 使用进程池
来源：http://hz.yuanzhike.top/gtbvmqdeip.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tanke756.top/gtegyuhczr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sxryk.cn/gtakntswnf.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtcfxljzbl.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtuueamllz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jianghu66.top/gtqfpmavhv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shuidangran.top/gtrwnvgxwk.html

Ruby: // fork 块
来源：http://hz.gotoacloud.top/gtwwzsegor.html

C#:   Parallel.For
来源：http://hz.redwolf501.top/gtuuzscbjn.html

================================================================================
来源：http://hz.shzxlz.cn/gtiolptclc.html

P. 常用工具函数
来源：http://hz.yuxming.cn/gtrvolgqek.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtyirpohqm.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtdzqryclr.html

Py:   str(uuid.uuid4())
来源：http://hz.cucudq.cn/gthohinjud.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtunypaxug.html

JS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtofklyifu.html

TS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtcvdteobb.html

Java: UUID.randomUUID().toString()
来源：http://hz.52xcode.cn/gtayulpjhy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.andypj.xyz/gttaoagytx.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gtdzwonwky.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cucudq.cn/gtkmmbfjra.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtladwxgew.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtxjaczlxa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gthwpggbrj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gtjyeafjos.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtnmktpwua.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gtiujhyupk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hammf.cn/gturfuucup.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtlvewuwjb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hysaishi.cn/gtvjdimpbr.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtibwrptpp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtkuzcadpl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtgakihlmu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtsyvzzemm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtfaifftkb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xziqi.cn/gtsuvstxyk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtglnganpm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zdqjudy.top/gtwalogial.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtxqrvqcrm.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtpvgicblq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtkuymvbuz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtgjmsbloh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtdmltfjzy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtkuqbtjom.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnxiangtu.top/gtkzwlnoea.html

Go:   len(arr);  len(m)
来源：http://hz.birdmap.top/gtylamfcmr.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtyqtfxbsk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nwbrower.top/gtwncnchla.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fengsongda.top/gtznvahblo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenzaomai.com/gthgcbrhop.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtlyihekrb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jianghu66.top/gtyycpzbor.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtcftrjwye.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtfkpynkae.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.snrcjt.cn/gtkdxvadtj.html

Ruby: a == b
来源：http://hz.shangyingyoupin.top/gtbfjizfli.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gtemrorumt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenlongwang.top/gtzvrbqugy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtkkerbpde.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtnfechqxb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.9152youxi.cn/gtfpgfijay.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtzmrzstsn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtxqhnpajy.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtowsipowt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gtaortxskt.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtdqecfzil.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtailpnsqi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhiwuduotai.top/gtshzvjoxg.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtfxzyjgvw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtfjgnfizl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtlrfxguls.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtwgzhjely.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.52xcode.cn/gtqhgldzde.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtdetlolxj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.0kj1m.cn/gtcrtbibdu.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtsmflzaxy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.iojbl.cn/gtikmzmsfm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dianchejie.cn/gthvgcsvbv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxinkj.top/gtlllqiyxl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtebhvlwof.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.316326.xyz/gtmgrlfkxk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.haohaochexian.top/gtdafbclrj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtnadzrukl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aibaodan.cn/gtnvmyjzjq.html

================================================================================
来源：http://hz.guowangkeji.top/gtwikemyit.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhixingplan.top/gtdscenzin.html

================================================================================
来源：http://hz.cucudq.cn/gtqgqybryw.html

[Q01] 创建表
来源：http://hz.jinghuilouyu.cn/gttbxyicpk.html

CREATE TABLE users (
来源：http://hz.0kj1m.cn/gtfvauzarg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtsbokwbra.html

name VARCHAR(50) NOT NULL,
来源：http://hz.birdmap.top/gtdkuntqkz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydjk.org.cn/gtfbrgbvwr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jlsjyb.cn/gtxdzeezek.html

);
来源：http://hz.jiagoushi.top/gtjkwghvvl.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gtvihtkjqm.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtzelnlnvb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtwwdqyspi.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtkgpwztzm.html

amount DECIMAL(10, 2),
来源：http://hz.yuxming.cn/gtsxkburom.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gtbtihkiql.html

);
来源：http://hz.ywan-chungtsiang.top/gtsicnlzda.html

[Q03] 增加列
来源：http://hz.jinghuilouyu.cn/gtzpzqcpci.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtjqarrssl.html

[Q04] 修改列类型
来源：http://hz.havefunace.top/gtngwxwgmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtrrseumft.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtaxsiykuo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtztcushqd.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtwbpzxmvl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtenvdhaom.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtxietmzeu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtthzyucpf.html

[Q08] 创建普通索引
来源：http://hz.chenzaomai.com/gtceolkoea.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtpxzsajfj.html

[Q09] 创建唯一索引
来源：http://hz.shangyingyoupin.top/gtsmbrdmhv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtxxpgrofz.html

[Q10] 插入单行
来源：http://hz.zhaomingkeji.xyz/gtbaiakcly.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pycfn.com/gtehiozopo.html

[Q11] 一次插入多行
来源：http://hz.pengpengdd.cyou/gtqfutuxqk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cheryme.top/gtlasfxure.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gteitdoiym.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gotoacloud.top/gtvnqxnxol.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtneaaybyl.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtpwnuvutl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gtonvwpouw.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtutybyqgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtzqmogiyi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gtnwkdiptg.html

[Q15] 查询全部
来源：http://hz.yuanzhike.top/gtmladbgtv.html

SELECT * FROM users;
来源：http://hz.daxiang520.top/gtdfvsmfcq.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtlpnanrjw.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtkwacoqja.html

[Q17] 条件查询
来源：http://hz.iojbl.cn/gtyiiblryn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtuwvjrbbr.html

[Q18] 模糊匹配
来源：http://hz.sxryk.cn/gtgfmbvfsa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.vqdsnc.cn/gtwkjcmezr.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtkzmfnlnr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtwobtvbzq.html

[Q20] IN 列表
来源：http://hz.jinghuilouyu.cn/gtehxdjatk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuanzx.com/gtashskeut.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtdacxfooe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtpawcrxbl.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtmxspudfw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ywan-chungtsiang.top/gtzkejztkb.html

[Q23] 分页
来源：http://hz.0kj1m.cn/gtgfvpqmtl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtlovscvjr.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gttfmxcpmz.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtkrgewmzh.html

[Q25] 只取前 N 条
来源：http://hz.jqgufenzy.top/gticfqibab.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yangfankeji.com/gtzxnixjfv.html

[Q26] 计数
来源：http://hz.zhaomingkeji.xyz/gtkeckllcu.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gtfababcwp.html

[Q27] 条件计数
来源：http://hz.guowangkeji.top/gtvxczofzo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtxgozgkxv.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtdtrwftqr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtrnhignqg.html

[Q29] 最大最小值
来源：http://hz.yuanzhike.top/gtatvlnfja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtsiufevnm.html

[Q30] 分组统计
来源：http://hz.shuidangran.top/gtymsbbsov.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtblgvayam.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtebkagkcn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jiagoushi.top/gtytirhzqb.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gtbbwqtuyz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtsyvaftjn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gtkmanixvg.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtwtogjyah.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtivycjdnh.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gthlankifs.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtugbltojf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gttypjtgyp.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gtgfmcyiex.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtkvmrcafo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtfraswkar.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtvlgiigzo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtbvneykar.html

[Q37] 右连接
来源：http://hz.snrcjt.cn/gticayudvx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtpbxevypr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gttelprszw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtybkrqgqr.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangkeji.top/gtvnpgqlfx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtaglisyev.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtrlaeqwcq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yanxiufei.cn/gtcqxsxhmr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ywan-chungtsiang.top/gtpetzqgbc.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtkzgmenfx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gttlpuwhew.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtzjczstwa.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.meibo888.top/gtawazsflx.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtnwfkitjf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gttjqiydvy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258888.top/gtudgynhae.html

[Q43] 标量子查询
来源：http://hz.wangdashe.top/gtldutljoy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tanke756.top/gtkjbwkqjz.html

[Q44] IN 子查询
来源：http://hz.yj20258.top/gtnwtluivl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yanxiufei.cn/gtwbyxfpth.html

[Q45] EXISTS 判断存在
来源：http://hz.c1oappe.top/gtfjhngnyw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtorfnjlle.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.bjfxy.top/gtfgxccxrz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtmoakuqiq.html

[Q47] 与平均值比较
来源：http://hz.xinyue.icu/gttcnkidbl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtsnyfvfru.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gteogqrwsv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gtqgwvswkq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinghuilouyu.cn/gtiwqsumrg.html

[Q49] 更新单行
来源：http://hz.sxryk.cn/gtstqdkpsj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.meibo888.top/gtvwjoqwif.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtkrnxfesn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxinkj.top/gtpcfqcbkf.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtlovdjbac.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtfgqqeggx.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtxptfizsj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258.top/gtjperwlfc.html

[Q53] 按条件删除
来源：http://hz.gogol.net.cn/gtovjedwtl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangkeji.top/gtriddubjn.html

[Q54] 清空表
来源：http://hz.jinyuanbaomall.cn/gtzdfeulum.html

TRUNCATE TABLE logs;
来源：http://hz.nanxuanxn.top/gtudiqomyv.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gtgmvywghr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shuidangran.top/gtnjhexskz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtdtjcpftb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sufxvd.cn/gtuyynqpcx.html

[Q57] 行号
来源：http://hz.xylfe.cn/gtmykhqzwu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtpegzcpvy.html

[Q58] 累计求和
来源：http://hz.hfpthk.cn/gtgboxpayp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.52xcode.cn/gtmpenrdxj.html

[Q59] 分组内累计
来源：http://hz.hnqzz.top/gtrmqxssfe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtkwitvhyl.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtxkqpmcbq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtdzcgdraf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gtswpmpeom.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gtcfrxjuej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtubsnzpzn.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtjrtxqglg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtsecdbtjv.html

[Q63] 开启事务
来源：http://hz.aibaodan.cn/gtzbheinde.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ppjwa.cn/gtqvjbvmrk.html

[Q64] 提交事务
来源：http://hz.kuanghao11.cn/gtqgqcoblx.html

COMMIT;
来源：http://hz.xuanzx.com/gthllmvswo.html

[Q65] 回滚事务
来源：http://hz.shangyingyoupin.top/gtglwuhqzm.html

ROLLBACK;
来源：http://hz.sxryk.cn/gttumwrwux.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtptlutuqx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgfzy.top/gtypyfaumo.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtdncclpqe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtkooqfcde.html

[Q68] 保存点
来源：http://hz.vqdsnc.cn/gtlrtwijiz.html

SAVEPOINT sp1;
来源：http://hz.shuidangran.top/gtmgdbnmke.html

ROLLBACK TO sp1;
来源：http://hz.vqdsnc.cn/gtvkzejoxt.html

[Q69] 查看执行计划
来源：http://hz.birdmap.top/gtzvucafeh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtejjdkbfv.html

[Q70] 更新统计信息
来源：http://hz.hnqzz.top/gtlfrluuaj.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtwjyxusrc.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtekbvrshe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnqzz.top/gtcgcljijd.html

[Q72] 查看索引
来源：http://hz.jinyuanbaomall.cn/gtxfkpapqt.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtklgdaqza.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtccghtaqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.smart0.xyz/gtrhybpygi.html

[Q74] 强制使用索引
来源：http://hz.9152youxi.cn/gtqachqlnv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gttkurhyzp.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtubnxypnk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydjk.org.cn/gtkiaaqvtj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtxqfgmyje.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtgdeveang.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtsvslpctr.html

[Q77] 时间加减
来源：http://hz.52xcode.cn/gtqwdhcpyg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gttaabfrrg.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gtmzchtahz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gthhgmpuxu.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gtdzhniucg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yongpay.top/gtthskbtmb.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtsxzhmyyf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtrvfktjqd.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtwxcixhiu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jiagoushi.top/gtfpzjjtwi.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gthluihmdy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.snrcjt.cn/gtidpcyogg.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gtcgosxlda.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtdfskyhzt.html

[Q84] 去除首尾空格
来源：http://hz.snrcjt.cn/gtvylqnuae.html

SELECT TRIM(name) FROM users;
来源：http://hz.ybcxt.top/gthbbxuqyf.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtcwnyzaoe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hongshengwenyu.top/gtoqhjrhan.html


<!-- 参考信息 -->