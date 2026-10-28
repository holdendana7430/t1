代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.birdmap.top/gtreebdvru.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtuzmjmhjs.html

C#:   async Task F() { await G(); }
来源：http://hz.yongpay.top/gtligfquig.html

[O05] 并发执行并等待全部完成
来源：http://hz.andypj.xyz/gtnypjaauv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtdchnjqpz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jyoumei.cn/gtgvjmcbkc.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtqnjozuer.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtzpuueyae.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yonumen.top/gthrryeuie.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nwbrower.top/gtrplnkrgp.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtdyyssndu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtaavxjphz.html

[O06] 使用进程池
来源：http://hz.yj20258.top/gtzvxrgeon.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gttxzusibo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtkcemxvis.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtlohjneck.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtxgtvkryn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtalaydqdb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.feifeiyinyue.top/gtnxusmqge.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtvrlbqjru.html

C#:   Parallel.For
来源：http://hz.jinqigfzy.top/gtixuduuut.html

================================================================================
来源：http://hz.daria6918.cn/gtkugbdztz.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtpbecgkxp.html

================================================================================
来源：http://hz.wangdashe.top/gtgdrtunzf.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtsezwjbcz.html

Py:   str(uuid.uuid4())
来源：http://hz.dashuyun.cn/gtatokgesl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtyyipgpnn.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtodzrbpln.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtxjrjiioq.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gtjvptdsle.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtidqzyuwn.html

Ruby: SecureRandom.uuid
来源：http://hz.shzxlz.cn/gthpxeywni.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtulpankrb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.redwolf501.top/gtgzalxwhm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtnhupderw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.smart0.xyz/gttkducqlj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhengqikj.top/gtzrpuzrpj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nwbrower.top/gtzziywaut.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenjidiqi.icu/gtfmetfpmp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tianlin.xyz/gtglsafhgk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtrayzyshh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xylfe.cn/gtmubmrvoc.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtepvkxslg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtspofohoe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.0kj1m.cn/gtsvflpaon.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtsvtnmbqt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtjrwzpebt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fengsongda.top/gtccpydxph.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinqigufen.top/gtmjlecvtr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daxiang520.top/gtpeoqxamf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hammf.cn/gtjhbxhaiq.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gttimgljnm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtkyzcqiab.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtmehzcuui.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtapnwngrm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtposepecj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtwkvhdlci.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtgrvrzbhj.html

Ruby: x.length;  x.size
来源：http://hz.sweek.top/gtpeujhiku.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gthidagsbp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtvpnskmdf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtcqxtbrhi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtrvfycxoz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gtikefjoeu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gtpskcwhwl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yvedp.cn/gtigbhqsmf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangshuangyany.cn/gtzlgjryti.html

Ruby: a == b
来源：http://hz.yj202588.top/gtjeeljqyr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xziqi.cn/gtpfrlkmrq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtslblahnd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.feifeiyinyue.top/gtjetedpro.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtarvbqrqf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtertujsmo.html

TS:   if (x == null) {}
来源：http://hz.zhongyouzk.top/gtptbnlbva.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtskieygbx.html

Go:   if x == nil {}
来源：http://hz.tanke756.top/gtvyadgrax.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuanzhike.top/gtcrovurbw.html

C#:   if (x is null) {}
来源：http://hz.fzhhl.top/gtjzqmwbdb.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtyphchnzt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgufenzy.top/gtbpftcozb.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gttdttwvch.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtnndccrva.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtwkmifjiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtaqmexooj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtefaxdaff.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtxwrvnabu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hfpthk.cn/gtczvatdfx.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtxjygvesu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.snrcjt.cn/gthulfscbj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtepyzsaqd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtyllddwbe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtzhhnabve.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gtkgopxvth.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydjk.org.cn/gtvwgkmnnx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yvedp.cn/gtmojcjqnq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtnnajceiy.html

================================================================================
来源：http://hz.jinqigufen.top/gtfnyhgxsa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gtcaeozwkc.html

================================================================================
来源：http://hz.yonumen.top/gtodihrqdd.html

[Q01] 创建表
来源：http://hz.jiagoushi.top/gtcifjzudl.html

CREATE TABLE users (
来源：http://hz.ivvv.top/gtjxsfittk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtuztslteo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yanxiufei.cn/gtilsvkitl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenzaomai.com/gtubrnzrpa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtlfktasil.html

);
来源：http://hz.316326.xyz/gtrrsyrbck.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtkwqgosgx.html

CREATE TABLE orders (
来源：http://hz.cheryme.top/gtgxmnhlwy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtbxgdqwdt.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtcdnuzhga.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtnlsikebq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj20258888.top/gtqavkuofq.html

);
来源：http://hz.nwbrower.top/gtdrjwqhkm.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtqrxjzmvp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtnorkxnkb.html

[Q04] 修改列类型
来源：http://hz.gotoacloud.top/gtoqtmhvkw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtyqtovqrf.html

[Q05] 重命名列
来源：http://hz.guowangkeji.top/gtpfbuhekv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yvedp.cn/gtdkzchmvy.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtldncjcpg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuxming.cn/gtfdrzntmj.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtpekjmvfe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yangfankeji.com/gthpsktjog.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtqdjyucvl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gttfsguhqv.html

[Q09] 创建唯一索引
来源：http://hz.gzhubu.top/gtxbulmyfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtoebektnp.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtszyjttya.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daxiang520.top/gtlbtyxzbe.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gttoddxhom.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gzhubu.top/gtfhozunus.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtektmxlzk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtnjkjehpu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxinkj.top/gtlgcvvcve.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtudmacctd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258888.top/gtwjwnedvr.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenlongwang.top/gtlwegsvld.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtsiijpryu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.daxiang520.top/gtiiaiehcu.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gtxgzgoszj.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtjlnxbrvt.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtyppqpccb.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtqirhbldc.html

[Q17] 条件查询
来源：http://hz.guannengcc.top/gthyaadqqn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtelxsjgkv.html

[Q18] 模糊匹配
来源：http://hz.nwbrower.top/gtpfztqjnv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cucudq.cn/gtyfzfmmuw.html

[Q19] 范围查询
来源：http://hz.jyoumei.cn/gtiswzsutu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.feifeiyinyue.top/gtbqfdaphi.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtpeyjjypr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtticapdqr.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtnpixkoeq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.mhx1999.top/gtoqhzasae.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtopbhocdg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtfddotbag.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtbtipgwse.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gtnkntvmho.html

[Q24] 去重
来源：http://hz.zhengqikj.top/gtfhvkitot.html

SELECT DISTINCT city FROM users;
来源：http://hz.sufxvd.cn/gtgitxrgzt.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtlhpkbtnb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gtaevmgufg.html

[Q26] 计数
来源：http://hz.smart0.xyz/gtrqzwrpsk.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtqgsxgwtq.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtnxbodxpu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtjelgkcmx.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtruwvitba.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtzvoeopkw.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtahkcqcgs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtmafojmoi.html

[Q30] 分组统计
来源：http://hz.dashuyun.cn/gttrelznga.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtqluxshcu.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtvtnqvryg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gtukazzqkw.html

[Q32] 分组拼接字符串
来源：http://hz.zycfv.cn/gtpqaxskbi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtwrmwxeru.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sysykeji.top/gtnomzkkdt.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gtljhmxjxt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtvrjveezb.html

[Q34] 每组取第一条
来源：http://hz.quarkkingdee.top/gtlncyuzlp.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtdixvpkrv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fzhhl.top/gtaetwpzuw.html

) t WHERE rn = 1;
来源：http://hz.hysaishi.cn/gtmjyuvvdw.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gtrwwltjrf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtkmvuxtnc.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtzcxlafok.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtzrpwscib.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtjwxdltjt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhijiandao.cn/gtpnfzotyy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtwnnvcssq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtgrbcveoi.html

[Q39] 自连接（查上下级）
来源：http://hz.jinyuanbaomall.cn/gtrvslajpe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtdtnsgnby.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtlmwzpusr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aibaodan.cn/gthzhvyiau.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gthxgfrfcq.html

[Q41] 多表连接
来源：http://hz.cheryme.top/gtfuamrfww.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtgbkmekjz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtivdhcqpx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sufxvd.cn/gthduuvndl.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtluaopouc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jlsjyb.cn/gtvegecedd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.haohaochexian.top/gtuvjzgwac.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtaazcnxhj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gteuufclcu.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtpsdxepqo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guannengcc.top/gtocwbzlzk.html

[Q45] EXISTS 判断存在
来源：http://hz.gzhubu.top/gtkwtxtckm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtvppvgzle.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.birdmap.top/gtsekafaui.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtjqxrkutn.html

[Q47] 与平均值比较
来源：http://hz.birdmap.top/gtpqrejwqd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.52xcode.cn/gtxiorrrhh.html

[Q48] CTE 公用表表达式
来源：http://hz.shzxlz.cn/gtscexurka.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtxxlfekcv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtrylsfwpl.html

[Q49] 更新单行
来源：http://hz.cucudq.cn/gtokbbzrse.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtukgddrvm.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gthdtusfns.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtfksokbky.html

[Q51] 用子查询更新
来源：http://hz.fengsongda.top/gtahwdrkxk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtkoumfgxa.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtqqnmkpup.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gthvjuxuue.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtwqtgbqpn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangdashe.top/gtutzzagyl.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtqcipijfp.html

TRUNCATE TABLE logs;
来源：http://hz.9152youxi.cn/gtducaihmt.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258.top/gtikkpoodv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gthixcjxou.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tianlin.xyz/gtjsxdqwos.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.feifeiyinyue.top/gtgqjvwvle.html

[Q57] 行号
来源：http://hz.nwbrower.top/gtldqibexi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuanzhike.top/gtntwmxnve.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gtcrcesjqj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fengsongda.top/gtuvwaqpcb.html

[Q59] 分组内累计
来源：http://hz.xziqi.cn/gtagfddcoe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hywenlv.cn/gtgkxrspyy.html

[Q60] 取上一行 / 下一行
来源：http://hz.cashguo.top/gtapeqzvak.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtssfyhlgb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hfpthk.cn/gtilkreqtb.html

[Q61] 移动平均
来源：http://hz.jinyuanbaomall.cn/gtdzqplnsn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtopjxrwsz.html

[Q62] 分组占比
来源：http://hz.c1oappe.top/gtpfetfipq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtjzqqslia.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtlnywrwxy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.9152youxi.cn/gtdrpxzogt.html

[Q64] 提交事务
来源：http://hz.nanxinkj.top/gtatmeotse.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtiukodhnz.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtjepgvokv.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtdazvtesz.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtfzgdgoks.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhongyouzk.top/gttdygiwzi.html

[Q67] 设置隔离级别
来源：http://hz.yuanzhike.top/gtgbxuijvm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtvxgptfon.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gtthgfjnjw.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtqcshweew.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtuzeihoos.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gtrmibjhez.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtxyvubebe.html

[Q70] 更新统计信息
来源：http://hz.dianchejie.cn/gtxzbbdjfo.html

ANALYZE TABLE users;
来源：http://hz.jqgfzy.top/gteabaemzv.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtekdgauhy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtqabkdlqh.html

[Q72] 查看索引
来源：http://hz.sysykeji.top/gtdlrxmcoq.html

SHOW INDEX FROM users;
来源：http://hz.ydzc1.top/gtivoyhgyj.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gtbjhqjtup.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtjxrbfwmb.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtpvooglzk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shuidangran.top/gttertfvpw.html

[Q75] 日期格式化
来源：http://hz.xuanzx.com/gtmrjbucra.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258.top/gtvxkzyuxx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtzoydusbm.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtblcpuzvx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fzhhl.top/gtldeyqjbi.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtvjubaywc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtuxoqkinh.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtftkhxwoh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.haohaochexian.top/gtywrfikyh.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtzkalzxzu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aibaodan.cn/gtnldzcqmg.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtyakotaag.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhixingplan.top/gtoqqczxtr.html

[Q81] 字符串替换
来源：http://hz.tanke756.top/gtynebgdfw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhengqikj.top/gtryzqxfqm.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtrtntfepp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtizjhalbo.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtqvbpgofn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gteblmdkid.html

[Q84] 去除首尾空格
来源：http://hz.yonumen.top/gtbvazoubk.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtqdeqiqys.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtfyklgwcy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258888.top/gtpxirjrnj.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtpkzrylou.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtmylbaord.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtzyoyskzs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtbxxfyydv.html

[Q88] 行转列（条件聚合）
来源：http://hz.jiagoushi.top/gtkgxdlgnz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jlsjyb.cn/gtjnzgnrrq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ppjwa.cn/gtaiqhxerx.html

[Q89] 判断表是否存在
来源：http://hz.zdqjudy.top/gtvkfycxnj.html


<!-- 参考信息 -->