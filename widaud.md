代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fengsongda.top/gtuuiizvcq.html

JS:   async function f() { await g(); }
来源：http://hz.snrcjt.cn/gtoxckipwn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtsskuwdcr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gtzcrhdxck.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtztprnnnt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtgqujwvuy.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtsvwzgkiv.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydjk.org.cn/gtzhnawugk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtwmllplcf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtnmhyqvdc.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtgypwzyib.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtohdmrleu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtouqklxqm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.haohaochexian.top/gthnudatff.html

Ruby: threads.map(&:join)
来源：http://hz.dianchejie.cn/gtvzesfrlj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtkhnjkfwj.html

[O06] 使用进程池
来源：http://hz.meibo888.top/gtttuylrrc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhiwuduotai.top/gtqlltyyje.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258.top/gtziislccx.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtlqmzcxvc.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtjhcfrqim.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.bjfxy.top/gtgtcpuitl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daria6918.cn/gtszgacpso.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gteykxuljj.html

C#:   Parallel.For
来源：http://hz.dianchejie.cn/gtxlxnjclm.html

================================================================================
来源：http://hz.nwbrower.top/gtpnhkbvlk.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtgjwvweox.html

================================================================================
来源：http://hz.yuxming.cn/gttxqlgigo.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtjdrijcxo.html

Py:   str(uuid.uuid4())
来源：http://hz.daria6918.cn/gtliehizvl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtxsdsivey.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtalugfpnu.html

TS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtevdnygbp.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gtpsapsqkx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yangfankeji.com/gtihfgendg.html

Ruby: SecureRandom.uuid
来源：http://hz.shzxlz.cn/gtpchpugvd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtvisnplxi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtdpltknas.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtljmoaslv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hysaishi.cn/gtcdszysln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtuvatcbau.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtwxkokfaf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gthkdrvlzw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnxiangtu.top/gteavqwnbb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtsvnhpaws.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gtyshialfb.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtouchnfsz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yanxiufei.cn/gtewaqrufp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gtkrltlbyj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gtqwexwqot.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtkbiqipbs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtqwqjwaum.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtsglhjpgw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gthctzeqbo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ehwqpu.com/gtlnzqwcus.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtvwzllaab.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gzhubu.top/gtfiracgkg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtlqjoicwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtnbjsfkdj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtfqrhbjtk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hfpthk.cn/gtoeokxqjv.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtbmxvmbab.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gtcywktcuk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangshuangyany.cn/gtmaqffvmv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guowangkeji.top/gtvfiprksx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtzueildrf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtauxfzsja.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jianghu66.top/gtjbshqwrb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtstjqetiw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtvgdpvxuj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.quarkkingdee.top/gtvekrlyue.html

Ruby: a == b
来源：http://hz.ehwqpu.com/gtvhcnwmmt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gtrlxzcqiq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.9152youxi.cn/gtvfjrfedj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtxsacxrdq.html

PHP:  if (empty($x)) {}
来源：http://hz.smart0.xyz/gtgzevazlk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xinyue.icu/gtipgtfbnn.html

TS:   if (x == null) {}
来源：http://hz.jyoumei.cn/gtaaxiqhzs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtwxdtjltk.html

Go:   if x == nil {}
来源：http://hz.zdqjudy.top/gtrritxzuh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtqdlhfbyx.html

C#:   if (x is null) {}
来源：http://hz.nanxinkj.top/gtufoxcuxo.html

[P07] 防抖与节流
来源：http://hz.cqqwz.cn/gtnxnndanf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.birdmap.top/gtfnwmzrri.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtyxbncjss.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtrzpnvayv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtarcmyhob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cucudq.cn/gttnfkkeny.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gtnhemvnpi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gaohongyu789.top/gtrnclexga.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.quarkkingdee.top/gtluiaergy.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gthwrwpurj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtesvpxpsy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gtrjrywbnv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigfzy.top/gtawpryeve.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yvedp.cn/gtdbhoddmk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.fzhhl.top/gtogvjrgyq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hywenlv.cn/gtcyazruki.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gttzjzljkn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aibaodan.cn/gttqznsckj.html

================================================================================
来源：http://hz.yangfankeji.com/gtkgudzfhq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jlsjyb.cn/gteslxsgwj.html

================================================================================
来源：http://hz.ybcxt.top/gtvycczxsl.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtjaksahha.html

CREATE TABLE users (
来源：http://hz.sxryk.cn/gtctauwcyc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtpinhjosy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.mhx1999.top/gtgemunsec.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gtyalscinm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hywenlv.cn/gtdsaqqhov.html

);
来源：http://hz.yj202588.top/gtlgxlwmyy.html

[Q02] 创建带外键的表
来源：http://hz.jinghuilouyu.cn/gtiryrnrff.html

CREATE TABLE orders (
来源：http://hz.ehwqpu.com/gtmgwmyihz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtpykpwzvj.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtzepksdky.html

amount DECIMAL(10, 2),
来源：http://hz.yonumen.top/gtpayvphwv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aizwys.cn/gtvfqjhlza.html

);
来源：http://hz.fengsongda.top/gtedrkblbq.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gthxbvdukr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtqgzkiqui.html

[Q04] 修改列类型
来源：http://hz.tianlin.xyz/gtpcojcfoc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guannengcc.top/gtykrkrxpk.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gtjjovccfu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tanke756.top/gtfxbrgduo.html

[Q06] 删除列
来源：http://hz.feifeiyinyue.top/gtmzznzdns.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtnkkgdtba.html

[Q07] 删除表
来源：http://hz.xuetiantiany.cn/gtayjokypw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhongyouzk.top/gthpdlkgey.html

[Q08] 创建普通索引
来源：http://hz.xylfe.cn/gtaabtbysc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtokqtvgcv.html

[Q09] 创建唯一索引
来源：http://hz.sweek.top/gtsddlvxnv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtbcfmrxeg.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gtbrcxnvyi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gtqnaxexah.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtmbggqvkl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guannengcc.top/gthoklfose.html

[Q12] 插入后取自增 ID
来源：http://hz.cdnleiting.top/gtsnuouhim.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtwcbcdhlt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtelyooszy.html

[Q13] 忽略重复插入
来源：http://hz.aizwys.cn/gtnmtjdlii.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cucudq.cn/gtjkupqeal.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtcpbvvjfd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xingfuxueyuan.xyz/gtrceisllt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtnuueugxa.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtlfvvikld.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtsvykrsrt.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gtnhlhezbh.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtnlcjzknj.html

[Q17] 条件查询
来源：http://hz.gaohongyu789.top/gteamjcyrx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtbihnagfa.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtanldcttq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnxiangtu.top/gtcwakmqrw.html

[Q19] 范围查询
来源：http://hz.jinyuanbaomall.cn/gtouvvstgb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gthrrvyroa.html

[Q20] IN 列表
来源：http://hz.hammf.cn/gtecsaptqr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtlkvabzch.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gteynkqbet.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guannengcc.top/gtzigvhwcq.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtowvekvkc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtagommaig.html

[Q23] 分页
来源：http://hz.gaohongyu789.top/gtarayrtcb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtezmwjith.html

[Q24] 去重
来源：http://hz.hnxiangtu.top/gtjysqtybq.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtibvoqprz.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtosbpagwz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtwuqhzwmo.html

[Q26] 计数
来源：http://hz.dianchejie.cn/gtuniiumye.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtscgmreuf.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtxytgzqbh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.kuanghao11.cn/gthtdrkxhf.html

[Q28] 求和与平均
来源：http://hz.sweek.top/gtijkftdui.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtdekbxlve.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtjrdydnis.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtpxgynqur.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtrdivrqme.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtzplmrxqk.html

[Q31] 分组后过滤
来源：http://hz.guannengcc.top/gtkyhuulio.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtjezlpzzl.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gtjrwjbxyp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtpiwfqvwj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gtbzgophzy.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtvdhnwypr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nwbrower.top/gtlgusgpqr.html

[Q34] 每组取第一条
来源：http://hz.hysaishi.cn/gttterrfiu.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gthlaeopbl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangkeji.top/gtvahqiqyx.html

) t WHERE rn = 1;
来源：http://hz.zhiwuduotai.top/gtbroaiuvl.html

[Q35] 内连接
来源：http://hz.snrcjt.cn/gtitztisvq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gtrlkmoptn.html

[Q36] 左连接
来源：http://hz.quarkkingdee.top/gtekoacfen.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtrzdiwfag.html

[Q37] 右连接
来源：http://hz.svipenyu.cn/gtumlbesci.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtvqkmhvoz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.havefunace.top/gtnmnijgzh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.feifeiyinyue.top/gtngmerevl.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtgzdtbtoe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtitvnbjzx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gtwyhbmptp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ivvv.top/gtqmupnrce.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangdashe.top/gttvkpismx.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtchlbgsbs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtsnqgamvj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtlsnuvtbw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtabjgwbgv.html

[Q42] 连接条件附加过滤
来源：http://hz.hywenlv.cn/gtgberzjbx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gthopiuxpf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuanzhike.top/gtoceikqqv.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtwfonhdld.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtnerbjdjg.html

[Q44] IN 子查询
来源：http://hz.ppjwa.cn/gtvangomvz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtticgsqoy.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtfvhvedwo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtsawiwmjp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ppjwa.cn/gtosggwpge.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtebuwglnv.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtwcisnuwd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnxiangtu.top/gtctifqjxu.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtpoveqgiy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.svipenyu.cn/gtteiyppvl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangkeji.top/gtfrwzbfeb.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtqezjkxms.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtdvfvnlem.html

[Q50] 批量更新
来源：http://hz.hongshengwenyu.top/gtfgwzszyh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtxpfxfclx.html

[Q51] 用子查询更新
来源：http://hz.xinyue.icu/gtfxtwqhla.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenjidiqi.icu/gtqwnxyaqu.html

[Q52] 删除指定行
来源：http://hz.fzhhl.top/gtvkubbkoz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.bjfxy.top/gtrgoswqdu.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtxhvtvchs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sysykeji.top/gtihkpbzjr.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtgbuqblno.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtsionamka.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gttqvyodlo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnqzz.top/gtilovjccf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtkerbobem.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gaohongyu789.top/gtfoxaxtzr.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtfwrqycyp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtyjewbzaq.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtianneapq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtcbyavvra.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtcpgjjguj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtkzuowhmd.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gthgejspzj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jyoumei.cn/gtqdzpfnyc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ydzc1.top/gtmjgooair.html

[Q61] 移动平均
来源：http://hz.shuidangran.top/gtydygegfo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtxlrdullg.html

[Q62] 分组占比
来源：http://hz.guowangkeji.top/gtqerwwaba.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtiigdxkcj.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtwktyxfmg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cdnleiting.top/gtjhramstm.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtciksvnyj.html

COMMIT;
来源：http://hz.chenjidiqi.icu/gtxqfmzkbi.html

[Q65] 回滚事务
来源：http://hz.yanxiufei.cn/gtdnldncta.html

ROLLBACK;
来源：http://hz.sweek.top/gtredzxpks.html

[Q66] 行锁查询
来源：http://hz.vqdsnc.cn/gtlsubrtvl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtlushmajt.html

[Q67] 设置隔离级别
来源：http://hz.ppjwa.cn/gtmsuquudf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenlongwang.top/gtofwtprgn.html

[Q68] 保存点
来源：http://hz.dianchejie.cn/gtvasmlngb.html

SAVEPOINT sp1;
来源：http://hz.dashuyun.cn/gtemtsvgtb.html

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtjafyjmok.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtrzyoojmz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.guannengcc.top/gtmsdtvmun.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtohsslzuh.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtxsrzhvwk.html

[Q71] 查看建表语句
来源：http://hz.yangfankeji.com/gtxcmsglne.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtnvgxfhof.html

[Q72] 查看索引
来源：http://hz.nwbrower.top/gthblbxzmj.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gtvxspnnlp.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtggyhlopu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gtkucetvqg.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtykjdxcqp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gtiuenuxrp.html

[Q75] 日期格式化
来源：http://hz.chenzaomai.com/gtztfocenh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtenumsbhq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtwdgbhkms.html

[Q76] 按天统计
来源：http://hz.xziqi.cn/gtdvtfdzsf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhiwuduotai.top/gtzkuilaiu.html

[Q77] 时间加减
来源：http://hz.9152youxi.cn/gtvslvchiz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gthyowydzo.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gtzpaidbxo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtbrwvyzda.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtrjjnlras.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtubefnfbi.html

[Q80] 字符串截取
来源：http://hz.chenlongwang.top/gtuzmihczt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtqwokpckk.html

[Q81] 字符串替换
来源：http://hz.yueranfly.top/gtmqsixipx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jiagoushi.top/gtcgjrrnuf.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtuutnoirs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtndvmxldc.html

[Q83] 大小写转换
来源：http://hz.jyoumei.cn/gtybcafgog.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtzoxltahu.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtzyjosnvj.html

SELECT TRIM(name) FROM users;
来源：http://hz.hongshengwenyu.top/gttjlpvqga.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtuaslmfbl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtjggmyyrk.html

[Q86] 读取 JSON 字段
来源：http://hz.havefunace.top/gtjksndlpp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cashguo.top/gtxfjnpitg.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtkctdhcet.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pengpengdd.cyou/gtteqqgaiq.html


<!-- 参考信息 -->