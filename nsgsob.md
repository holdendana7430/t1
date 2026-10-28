代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zycfv.cn/gtxgecfmdg.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtgtkuhlqw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gtaxmtqekb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gtdyodwxpd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtyfhhjgkf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtqblayosi.html

C#:   async Task F() { await G(); }
来源：http://hz.shangyingyoupin.top/gtiautnbpa.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtjtbttqso.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtambbojkz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.fengsongda.top/gtnxklpntz.html

JS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtgjgxapar.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gttnkqlngh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj202588.top/gtwhyhmmys.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinghuilouyu.cn/gthbkoibqx.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtecsmmpfz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnqzz.top/gtjiaabtvh.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtfbxujqsl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtumbyiqts.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuxming.cn/gtifmxagdh.html

JS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtpnkplrfp.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtsmjtbnts.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jianghu66.top/gtyhiqpgof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yueranfly.top/gtukxpmcop.html

Ruby: // fork 块
来源：http://hz.pycfn.com/gtnemqsbey.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtbdrtbyys.html

================================================================================
来源：http://hz.cdnleiting.top/gtwxrubamh.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gteqnxqgvq.html

================================================================================
来源：http://hz.shuidangran.top/gtprycmita.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gthxhyowpb.html

Py:   str(uuid.uuid4())
来源：http://hz.aizwys.cn/gtehuuhhwa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daxiang520.top/gtpqkemcsn.html

JS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtgovmylpg.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtusobnnzd.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtuhcehelh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtyufvdidy.html

Ruby: SecureRandom.uuid
来源：http://hz.gzhubu.top/gtcslcurxe.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtammafntn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtwzrcxugv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aibaodan.cn/gtmbclepof.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtbikfdlje.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtqlrxrbwq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gthuusycgw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhixingplan.top/gtbxffbrnl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtgbrvtzbl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtzswrhxgs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtkndesewq.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtcwvochpm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxuanxn.top/gtrsljfdjx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtwtlvzwwp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtutnqmrlr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtmigpqbku.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ivvv.top/gtirctqser.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtoaolmuhn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ivvv.top/gtougzornv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gtbnxdycqe.html

[P04] 求长度
来源：http://hz.iojbl.cn/gtubdcwcqp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtavjzjvgf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtgxabgdik.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtfvvrzxqc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtybkdsevv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenzaomai.com/gtfgwencaw.html

Go:   len(arr);  len(m)
来源：http://hz.xinyue.icu/gtjgkvovwp.html

Ruby: x.length;  x.size
来源：http://hz.pycfn.com/gtgbdnrpdr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtcgisulut.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhijiandao.cn/gtzhanyuta.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gtdolumoap.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxinkj.top/gtlduovioe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cqqwz.cn/gttscxznfe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtmldtpozq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cheryme.top/gtbucjpyav.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtsyehzhpg.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtgdutbowk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gtmllxaaws.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtyiitsguq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhijiandao.cn/gtjhxmlfqv.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtcucnhjsb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gtucbhmjfa.html

TS:   if (x == null) {}
来源：http://hz.jlsjyb.cn/gtarcgspqu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtgwgfklpw.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtgvszcimv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ivvv.top/gtluuhdnjn.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtikqsqfvi.html

[P07] 防抖与节流
来源：http://hz.sufxvd.cn/gtngfmmatr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhoulong.xyz/gtntuxnffq.html

PHP:  // 手写时间戳比较
来源：http://hz.hnqzz.top/gtwvlhtnnq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtokcqjgxb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtklxyzamu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenzaomai.com/gtsuolqtig.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gtlxadprrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtvfcjxtla.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cucudq.cn/gtvsrjvyiy.html

[P08] 处理浮点精度问题
来源：http://hz.smart0.xyz/gtijrqofma.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtylciebtf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangtech.top/gtksaadpvm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtxzkycmot.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gtkmyybbjy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gteodprond.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.havefunace.top/gtqioiezat.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtwnrdymuf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gtwyfftxjz.html

================================================================================
来源：http://hz.pycfn.com/gtnahseazf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ywan-chungtsiang.top/gtimuilehl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwrrujkoj.html

[Q01] 创建表
来源：http://hz.jinyuanbaomall.cn/gtxamztgiy.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtgkedarly.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtslghuwxf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gtpobgqzkp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtgddctvdc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gtrwwnqygi.html

);
来源：http://hz.haohaochexian.top/gtuqazlhdw.html

[Q02] 创建带外键的表
来源：http://hz.smart0.xyz/gtdkczfawb.html

CREATE TABLE orders (
来源：http://hz.xylfe.cn/gtbujhddhz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtychacyqz.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtkdvzgfvs.html

amount DECIMAL(10, 2),
来源：http://hz.guannengcc.top/gtzrazogwk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnxiangtu.top/gtpwrxqzux.html

);
来源：http://hz.ivvv.top/gtmxysyugr.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gterdxchpe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtrbfnqpmt.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtmcjcmuor.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtpeiyrhcw.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtvxxfgpdj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangtech.top/gtliuoximc.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtadsuiibz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cheryme.top/gtwuiyakfe.html

[Q07] 删除表
来源：http://hz.vqdsnc.cn/gtsbhekfsq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xylfe.cn/gtnkohqgio.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtyolbwuzs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gtiwgchqwx.html

[Q09] 创建唯一索引
来源：http://hz.zdqjudy.top/gtszmyvdyt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.bjfxy.top/gtjlpdpxol.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtvzeozuxy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gtbvisiier.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtdccnuzzq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guannengcc.top/gteuuwjpfr.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gtfugiitrf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jlsjyb.cn/gtzbegoopn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenlongwang.top/gtzdymfjgv.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gteznjtyhp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtpmbyhcnw.html

[Q14] 存在则更新（upsert）
来源：http://hz.fengsongda.top/gtbmquydam.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgufenzy.top/gtmjrzqjdd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gthovczvvj.html

[Q15] 查询全部
来源：http://hz.sweek.top/gtispotonu.html

SELECT * FROM users;
来源：http://hz.shangyingyoupin.top/gtpyyvicjf.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtltxyhxpb.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtnkdmcivl.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtyijsdhry.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtvnhlvosa.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtfejdnwhm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtephcioow.html

[Q19] 范围查询
来源：http://hz.jinyuanbaomall.cn/gtwfybnjxp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtdrvnmhxw.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtlhxexwdf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.mhx1999.top/gtmxutbpbh.html

[Q21] 空值判断
来源：http://hz.hnqzz.top/gtridvtldg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtovuscfbn.html

[Q22] 排序
来源：http://hz.aizwys.cn/gtgjngmmpg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigufen.top/gtfljfpxne.html

[Q23] 分页
来源：http://hz.cucudq.cn/gtxrzwnpal.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gtblkskecu.html

[Q24] 去重
来源：http://hz.yanxiufei.cn/gtvxxdbfvo.html

SELECT DISTINCT city FROM users;
来源：http://hz.quarkkingdee.top/gtoipubibw.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gtowuseezo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxinkj.top/gtdovnyelx.html

[Q26] 计数
来源：http://hz.yj20258888.top/gtmhdybsoa.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtybwrbjte.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtzvwmagiw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sysykeji.top/gtgbgqplty.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtzyttvcgk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gthnrigwje.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtdgbznbpu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ivvv.top/gtbauofqev.html

[Q30] 分组统计
来源：http://hz.xziqi.cn/gtcilezsmz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtcnvwgvjs.html

[Q31] 分组后过滤
来源：http://hz.jqgufenzy.top/gtidvyvucb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aizwys.cn/gtadkbrqjb.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtkjzgcvvr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtsgftedok.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jiagoushi.top/gteqrvsmzu.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtjriuecas.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtdvqtbwtx.html

[Q34] 每组取第一条
来源：http://hz.meibo888.top/gtjedffdcd.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtsoqjjomr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtvrepcask.html

) t WHERE rn = 1;
来源：http://hz.guowangkeji.top/gtsltcpaxn.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtazcdhrpk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtdhqdjkpy.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtkexwoyqt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtxfrsshjp.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gtoitlgbia.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtujnndjtq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangtech.top/gtccwlgeli.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtsuymnbfq.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtqtxedzgd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtlzvnvqgt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yonumen.top/gtrojjwamx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtypwxrfcq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.snrcjt.cn/gtnpmkvagc.html

[Q41] 多表连接
来源：http://hz.daxiang520.top/gtwpogyhim.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtfgwxbyzz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nwbrower.top/gtznddhnlf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gtlvziwvqd.html

[Q42] 连接条件附加过滤
来源：http://hz.xuetiantiany.cn/gtgcbqquuz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtbixlusah.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtzfepoqyo.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtaltmilqz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtwnxmtlzc.html

[Q44] IN 子查询
来源：http://hz.52xcode.cn/gtfuygqwqq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gtsaskooui.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gtbtwuzdaf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtyzlffbfl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.0kj1m.cn/gtnchdvkou.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtkdvgknnp.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gtiswzbbjn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtmzmgpvyr.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gtxkziroff.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gtvfsydblt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtzvgcokia.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtiruqficn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtynpineaw.html

[Q50] 批量更新
来源：http://hz.shanyushiyangkeji.top/gtztfyyato.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sufxvd.cn/gthngcuvyi.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtaqxvlqnj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.quarkkingdee.top/gtxmvfjkil.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtgfsrsvtt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gtgbmrrbnr.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtgnakaeec.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtdsdkubhf.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtldufbgra.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtuajlarpv.html

[Q55] 排名（并列占位）
来源：http://hz.ppjwa.cn/gtlcogbyjp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtzoidfhge.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cdnleiting.top/gtipzxptyk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtlpafparw.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtbhdddklk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gttoqvximc.html

[Q58] 累计求和
来源：http://hz.cucudq.cn/gtidrkpamk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtppalwoby.html

[Q59] 分组内累计
来源：http://hz.zdqjudy.top/gtyojvcmot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jiagoushi.top/gtktmjcsxh.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gttqfjiieg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenzaomai.com/gtjwqjzbre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtzafpoxxt.html

[Q61] 移动平均
来源：http://hz.ivvv.top/gtsmajekeo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtvuyfdpnr.html

[Q62] 分组占比
来源：http://hz.wangshuangyany.cn/gtvluolsnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtdkdzbtia.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtgfszflgk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtvoonuvon.html

[Q64] 提交事务
来源：http://hz.hongshengwenyu.top/gtshaayuyb.html

COMMIT;
来源：http://hz.gzhubu.top/gthrgsbwpu.html

[Q65] 回滚事务
来源：http://hz.ehwqpu.com/gtriwtfnlc.html

ROLLBACK;
来源：http://hz.ywan-chungtsiang.top/gtaxfpexyu.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangkeji.top/gtttifzzvw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtpnmepcbe.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtgdhwkpcf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtskbyhmiz.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtcfouzwkk.html

SAVEPOINT sp1;
来源：http://hz.ybcxt.top/gtyjtneeko.html

ROLLBACK TO sp1;
来源：http://hz.sweek.top/gtoxqfbsqx.html

[Q69] 查看执行计划
来源：http://hz.guannengcc.top/gtqiuvofqb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258.top/gtglubwzpw.html

[Q70] 更新统计信息
来源：http://hz.dianchejie.cn/gtcggmtnmu.html

ANALYZE TABLE users;
来源：http://hz.ywan-chungtsiang.top/gtcmbeuuau.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtqnyfageg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtdufuhyvn.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gtxdzbzzhx.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gthbimtmnu.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gttzgfiqwx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.vqdsnc.cn/gtokrqlwtb.html

[Q74] 强制使用索引
来源：http://hz.guannengcc.top/gthmtswcoz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenlongwang.top/gtungtlwvs.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtigmtjujs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hongshengwenyu.top/gtladvydcv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gtmqafwsob.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtmkbsocgp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258.top/gtqkemsusd.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gtkljzdqvf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtegkfqodh.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtnxajfbhn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtbdmgqfms.html

[Q79] 字符串拼接
来源：http://hz.daria6918.cn/gtiumqfalu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shuidangran.top/gtbomcqgnw.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtiesgeszl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258888.top/gtonixfkxu.html

[Q81] 字符串替换
来源：http://hz.gaohongyu789.top/gthaglvqcl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtvmytbink.html

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtqzldmpss.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jyoumei.cn/gtfbxlmpto.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtpffnylxh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ppjwa.cn/gtrpudrgzh.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtylwhoayt.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gttmbgsdum.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtgralfirr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gtaliczjts.html

[Q86] 读取 JSON 字段
来源：http://hz.xingfuxueyuan.xyz/gtdrkylmya.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fengsongda.top/gtqdyuoudb.html

[Q87] JSON 字段做条件
来源：http://hz.zycfv.cn/gttnuopoeb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtlnayarzy.html


<!-- 参考信息 -->