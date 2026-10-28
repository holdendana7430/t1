代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtsadambgx.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtjrpuhsaw.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gtxgymxsos.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtuiuijbzh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtwhreqfby.html

JS:   async function f() { await g(); }
来源：http://hz.c1oappe.top/gttoyumzno.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtagjpxxvr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.c1oappe.top/gtyeewscea.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenzaomai.com/gtvrzzeejw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinghuilouyu.cn/gtthzbztgz.html

C#:   async Task F() { await G(); }
来源：http://hz.xingfuxueyuan.xyz/gtmxcqfamw.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtvdotmgdz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhengqikj.top/gtkpdffcmx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhaomingkeji.xyz/gtrpqdhghv.html

JS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtrupaadyn.html

TS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtvswvhnks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtifbhpjcg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.feifeiyinyue.top/gtslnypzfz.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtxhvlksoz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtdwimteoy.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtqolthunz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sysykeji.top/gtyzhoegva.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgufenzy.top/gtculxdifz.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtswgnrdfq.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gteajenuwx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hywenlv.cn/gtksgteexq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aizwys.cn/gtmtjtfzqw.html

Ruby: // fork 块
来源：http://hz.kuanghao11.cn/gtdpvlrhyy.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gtmiygcurp.html

================================================================================
来源：http://hz.shzxlz.cn/gtmmzmtlvt.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gtogmhmupp.html

================================================================================
来源：http://hz.yuanzhike.top/gthbfpdvog.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gttksjchnu.html

Py:   str(uuid.uuid4())
来源：http://hz.redwolf501.top/gtwavqvfgh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtzlbdwrjy.html

JS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtjrwjvxlf.html

TS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtpwbajtli.html

Java: UUID.randomUUID().toString()
来源：http://hz.0kj1m.cn/gtzbsecioo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtjjqrbera.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtvfgjdtwg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.iojbl.cn/gtaicyltcj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.316326.xyz/gtmllxsebx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gtcyycjymp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gttmuoefkf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtnhxqfxnu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtqpgdqmgl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cucudq.cn/gtuzxyrnrn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hongshengwenyu.top/gtakpzizek.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtwjwiuluw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daxiang520.top/gtegjfdmez.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtlcaladlk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gtmnnyeqvh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xinyue.icu/gtddwxrztu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtptalcrrr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtgvoejdyl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuetiantiany.cn/gtbhkboala.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtnhnrzczg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tianlin.xyz/gthnduwetv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cdnleiting.top/gtckvvxfre.html

[P04] 求长度
来源：http://hz.316326.xyz/gtrlxkvfoi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gtoskhweys.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtjrqhhpxb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtzunifpwa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtpmnlkhwf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtyetlkddi.html

Go:   len(arr);  len(m)
来源：http://hz.aibaodan.cn/gtzjlymdee.html

Ruby: x.length;  x.size
来源：http://hz.shuidangran.top/gtxvmlshkk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydzc1.top/gtamdwfmes.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gtfehqdaci.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnxiangtu.top/gtpztferok.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.redwolf501.top/gthqjtkxhp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gtomsdzngn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtnkgywimv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gttqayhrxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtyzmmqhol.html

Ruby: a == b
来源：http://hz.zhiwuduotai.top/gthjrekbhj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtetxqipus.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cheryme.top/gtvtxwbdcw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigufen.top/gtjqtcoevp.html

PHP:  if (empty($x)) {}
来源：http://hz.andypj.xyz/gtsfnszulq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yanxiufei.cn/gtgcigwjvy.html

TS:   if (x == null) {}
来源：http://hz.jinqigfzy.top/gtuvwzgpxi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtlzhuodhf.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gttzmadbhr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuetiantiany.cn/gtukoxsmli.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtfhoieveh.html

[P07] 防抖与节流
来源：http://hz.0kj1m.cn/gtlitdntnf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtejjodmrw.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtshglncbc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtcqforbwu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtcrgegawo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnqzz.top/gtcnhtwyye.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gthtnvbsos.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtiokcmhac.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtnskegmnj.html

[P08] 处理浮点精度问题
来源：http://hz.yangfankeji.com/gtyzummjmh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yonumen.top/gtpimumfmg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guannengcc.top/gtavmcvhab.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gthjgzwttk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yonumen.top/gtsvkpgcte.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nanxinkj.top/gtfymxpdpb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtdnejnfbc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.vqdsnc.cn/gtttrwegvd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nwbrower.top/gtsbhlronj.html

================================================================================
来源：http://hz.gzhubu.top/gtlvmmseyb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtyzumlqit.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwhlznfwj.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gtntnmmnse.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtneupffcn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtyiscbdek.html

name VARCHAR(50) NOT NULL,
来源：http://hz.iojbl.cn/gtpeliuhlf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hongshengwenyu.top/gtwjaeizwv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gtbxbnkusj.html

);
来源：http://hz.zhongyouzk.top/gttcycdqdt.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtctsmkzlz.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtepefsohd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtyyrsuuol.html

user_id INT NOT NULL,
来源：http://hz.yongpay.top/gtkanwavmm.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtbfadetms.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhengqikj.top/gtuubmmqcp.html

);
来源：http://hz.jinqigufen.top/gtnjtjkkzu.html

[Q03] 增加列
来源：http://hz.hammf.cn/gtnnarpqxu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenjidiqi.icu/gtonxemrvm.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtsdwoqfgu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.svipenyu.cn/gtlxvppjvr.html

[Q05] 重命名列
来源：http://hz.dashuyun.cn/gtotnhyhdk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sweek.top/gtdbrwkisw.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtylbrvpnu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shuidangran.top/gtmpwrgtbh.html

[Q07] 删除表
来源：http://hz.hongshengwenyu.top/gtrigyxxih.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtelluzays.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtnvibsrjl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xylfe.cn/gtidhmtdmq.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtcguaadmk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.birdmap.top/gtomrguery.html

[Q10] 插入单行
来源：http://hz.ydzc1.top/gttdaddkcd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gogol.net.cn/gtbhowfzge.html

[Q11] 一次插入多行
来源：http://hz.sxryk.cn/gtmpdgiiba.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtxqzxudao.html

[Q12] 插入后取自增 ID
来源：http://hz.fengsongda.top/gttapaevbn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtpskhbfed.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangtech.top/gtqbqhzbfg.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtrbxwgvta.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtrlwdarek.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtwxzcykbc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtbfzfwvtk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gotoacloud.top/gtximwwtvt.html

[Q15] 查询全部
来源：http://hz.andypj.xyz/gtxtykjzgx.html

SELECT * FROM users;
来源：http://hz.52xcode.cn/gtshwhdjic.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gtyszlvood.html

SELECT id, name FROM users;
来源：http://hz.zdqjudy.top/gtkapaupbi.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtlogosnnk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gtoxpopnaj.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtcgupluyp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gtbiygxzgu.html

[Q19] 范围查询
来源：http://hz.havefunace.top/gtojqjtmas.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtmealjqsx.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gtqfinbkwa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sysykeji.top/gtxodwbtds.html

[Q21] 空值判断
来源：http://hz.ydjk.org.cn/gthkieuatd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtsrmnxman.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtiypvaamz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yongpay.top/gtfxendhyc.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtzhlkfdsn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtktotuebc.html

[Q24] 去重
来源：http://hz.xylfe.cn/gtpncdesiw.html

SELECT DISTINCT city FROM users;
来源：http://hz.cqqwz.cn/gtxewbkayr.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtnyxougqz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.meibo888.top/gtmshxlzco.html

[Q26] 计数
来源：http://hz.jyoumei.cn/gtirccnezg.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gtrqgcxgle.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gtvrsdurms.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xinyue.icu/gtsoiancpu.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtetyrqlua.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtqapclnko.html

[Q29] 最大最小值
来源：http://hz.meibo888.top/gtelzinrtv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtunsemvyb.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtjianiabq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtwiytmnsx.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtwmcxmylp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gtuxopjnpx.html

[Q32] 分组拼接字符串
来源：http://hz.yueranfly.top/gtourbnbmd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtbvuufqtl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigufen.top/gtynotzbex.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtktlmlixf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258.top/gtuilkorfs.html

[Q34] 每组取第一条
来源：http://hz.9152youxi.cn/gtkfkankeq.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gttozxzlqx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cheryme.top/gthjkeatre.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtquxtkvaw.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gtcnquaqxv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtneixefnz.html

[Q36] 左连接
来源：http://hz.jinqigfzy.top/gtigmixque.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtqxuigunj.html

[Q37] 右连接
来源：http://hz.nwbrower.top/gtpvvwkkzf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtfrtfcjji.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhiwuduotai.top/gtrbtujbhp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.feifeiyinyue.top/gtzgvemafy.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gthyhbsmvl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtwrkqlbsu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.52xcode.cn/gtdejfhrkr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtofzcdywg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.kuanghao11.cn/gtdymszskw.html

[Q41] 多表连接
来源：http://hz.sysykeji.top/gtoypbtwiq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jlsjyb.cn/gtpvfjkvtu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sweek.top/gthkasyxsq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtzsnecrnx.html

[Q42] 连接条件附加过滤
来源：http://hz.iojbl.cn/gtaufheetx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.andypj.xyz/gtvwizdaat.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ybcxt.top/gtlgnsdbzo.html

[Q43] 标量子查询
来源：http://hz.chenjidiqi.icu/gtmrfvbkjt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gteqnyqjim.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtklshjxaj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigfzy.top/gtydfedivc.html

[Q45] EXISTS 判断存在
来源：http://hz.c1oappe.top/gtrhwgkpaj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtbarsirfv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jiagoushi.top/gtlgsxkcst.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtvibdgjjo.html

[Q47] 与平均值比较
来源：http://hz.daxiang520.top/gtlbpcgpth.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtxjovejsz.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtesdhuibb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgufenzy.top/gtqkpedlmp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtloxtidui.html

[Q49] 更新单行
来源：http://hz.xingfuxueyuan.xyz/gtaalydsoe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtevxybmrm.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtddqfpnjx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtnhyiacjo.html

[Q51] 用子查询更新
来源：http://hz.zhongyouzk.top/gtyplnbhwt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yanxiufei.cn/gtvyjmtlqj.html

[Q52] 删除指定行
来源：http://hz.shangyingyoupin.top/gtlhhgyhsr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtuixvbvuw.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtrwjynzqb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgufenzy.top/gtaopojjxd.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gthqnmsrmg.html

TRUNCATE TABLE logs;
来源：http://hz.ehwqpu.com/gtcoxtvnnt.html

[Q55] 排名（并列占位）
来源：http://hz.ppjwa.cn/gtosfrvuvv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtwjnvcrkv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtplmabdui.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtbazsdjib.html

[Q57] 行号
来源：http://hz.yj202588.top/gtfkvrwcby.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtidzaqzbj.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtjvqrtkiw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtcmgxugfp.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gtknkjaojx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtmzirqitr.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenlongwang.top/gtwpgurqtb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.redwolf501.top/gtelzxmkcb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.svipenyu.cn/gtixxrcdmb.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gtmalcyqkw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtxzetkukk.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtgsskpurz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtrydzwgyk.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gtguzlwrtr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yangfankeji.com/gtuejrogjl.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gtvcuifqfe.html

COMMIT;
来源：http://hz.tian-w.cn/gtsuzloafu.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtdyibpssg.html

ROLLBACK;
来源：http://hz.zdqjudy.top/gtvzaacwyr.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gtmuocitpr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gthhnlaoba.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtthuqaimm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.meibo888.top/gtmbfwgfhd.html

[Q68] 保存点
来源：http://hz.shanyushiyangkeji.top/gtoaganzim.html

SAVEPOINT sp1;
来源：http://hz.shzxlz.cn/gtgzwfgzzu.html

ROLLBACK TO sp1;
来源：http://hz.jinyuanbaomall.cn/gtmpymqmgo.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtykqtuoim.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtvcxzgbaj.html

[Q70] 更新统计信息
来源：http://hz.hongshengwenyu.top/gtnlnscbwr.html

ANALYZE TABLE users;
来源：http://hz.xylfe.cn/gtpclhgxca.html

[Q71] 查看建表语句
来源：http://hz.jinyuanbaomall.cn/gtfyvminud.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xinyue.icu/gtnqjwfapf.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtphiiizep.html

SHOW INDEX FROM users;
来源：http://hz.cucudq.cn/gtbtdjdoew.html

[Q73] 查看表状态
来源：http://hz.guowangkeji.top/gtwstyyjro.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gtxbrnlukh.html

[Q74] 强制使用索引
来源：http://hz.guowangkeji.top/gtlaxbcobn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangkeji.top/gtespveaov.html

[Q75] 日期格式化
来源：http://hz.zhijiandao.cn/gtqxodaann.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gttstflfjd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtwaywszyj.html

[Q76] 按天统计
来源：http://hz.hammf.cn/gtaynragtr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj202588.top/gtwnrwmrfl.html

[Q77] 时间加减
来源：http://hz.yangfankeji.com/gthkycbrnv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xziqi.cn/gtzkgnlhem.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtmixnjyli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtfumzkwrv.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gtsszdfmmg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sxryk.cn/gtluvzfcjx.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtpirvoiwm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenzaomai.com/gtuunkskto.html

[Q81] 字符串替换
来源：http://hz.aibaodan.cn/gtpcspnjia.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gtfxhznjrk.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtgbnvzlmd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtrhjfesci.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtxmiqrgku.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtoylrysls.html

[Q84] 去除首尾空格
来源：http://hz.ppjwa.cn/gtmadrlxju.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtdccujckw.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtjxxjqmjf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtdedcsfgt.html


<!-- 参考信息 -->