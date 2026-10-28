代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigfzy.top/gtdkathnyd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.snrcjt.cn/gthbsctbne.html

JS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtclnijhqx.html

TS:   await Promise.all(tasks)
来源：http://hz.zhengqikj.top/gtbjfpnark.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aibaodan.cn/gtvfyjldna.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtghzrqyjy.html

Ruby: threads.map(&:join)
来源：http://hz.smart0.xyz/gtioymkxme.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gthpodubei.html

[O06] 使用进程池
来源：http://hz.hfpthk.cn/gtwdhogsri.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.52xcode.cn/gtwrrgiynx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtnqbadnfq.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtvvzpdnvj.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtujnauoxz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhiwuduotai.top/gtbtzuqpjk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangtech.top/gtpaxqgvwn.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtfvaolfzv.html

C#:   Parallel.For
来源：http://hz.cdnleiting.top/gtrvpaoxiz.html

================================================================================
来源：http://hz.ivvv.top/gtsyfthemk.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gtfymfrwgp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvvhubihx.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtcdebzyor.html

Py:   str(uuid.uuid4())
来源：http://hz.yanxiufei.cn/gtoqokdyib.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhoulong.xyz/gtihxkprix.html

JS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtvqvuyooi.html

TS:   crypto.randomUUID()
来源：http://hz.hfpthk.cn/gthhhrhzqx.html

Java: UUID.randomUUID().toString()
来源：http://hz.yueranfly.top/gtzufjttsf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tianlin.xyz/gtccjhcyxh.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtvsaevgos.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fzhhl.top/gtoaikvsar.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtwyxetcwi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtsaqggmxh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.birdmap.top/gtmbdtjgbx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtmgdnldjt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sufxvd.cn/gtapvvwbqm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgufenzy.top/gttvtxzxcm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gtoctmdflc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtjxqfbokp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtgewjgsce.html

[P03] 生成短随机字符串
来源：http://hz.zhixingplan.top/gthrliwbsi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hongshengwenyu.top/gtfzmoogbt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daxiang520.top/gtjuwnlbks.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gteqpawuym.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtxmazcfud.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtvdappoia.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.smart0.xyz/gtlxsmyoig.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hywenlv.cn/gtlxysebxm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zdqjudy.top/gtzbmuoxbg.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtpbcgocxa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtxgxmutbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtxckytiea.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtvoivkkgl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtklxzbqlo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtxxllrojd.html

Go:   len(arr);  len(m)
来源：http://hz.tianlin.xyz/gtelklshdb.html

Ruby: x.length;  x.size
来源：http://hz.jianghu66.top/gthyfnmlff.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtixqsuwsp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zdqjudy.top/gtzsnzslig.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtnpzbocee.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tian-w.cn/gtgcnpeene.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sxryk.cn/gtvpumdyef.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtaafjlapg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhijiandao.cn/gtktythzvg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tian-w.cn/gtxsvevsih.html

Ruby: a == b
来源：http://hz.shanyushiyangkeji.top/gtnkigpuql.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.havefunace.top/gtxlxnaclv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtvrmgihdy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinghuilouyu.cn/gtmscmetab.html

PHP:  if (empty($x)) {}
来源：http://hz.guowangkeji.top/gtrbdzpogl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.316326.xyz/gtmwfssnfp.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gttcspqapg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fengsongda.top/gtlbvtclsy.html

Go:   if x == nil {}
来源：http://hz.snrcjt.cn/gtdasczkvy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtuvqvekpo.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtesaxzaty.html

[P07] 防抖与节流
来源：http://hz.quarkkingdee.top/gtsmohrjbm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gttzetdnxy.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtrngizrfm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtucxzbkuq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtfjmvvjls.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxuanxn.top/gtfwbwgsjm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gthzdwvpok.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hywenlv.cn/gtkhcvzppj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtntvrwtvc.html

[P08] 处理浮点精度问题
来源：http://hz.zhongyouzk.top/gthbhgmnnb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gtqkanllbe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtsrnwdwei.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ehwqpu.com/gtdjcuonrd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtsjibfszj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtgcvcwuya.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtpkggaeoz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtliemjpvz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnxiangtu.top/gtmtmamkzo.html

================================================================================
来源：http://hz.bjfxy.top/gtoedxewdt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtnuowwusm.html

================================================================================
来源：http://hz.cdnleiting.top/gtzohtkvtn.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtuahwuiod.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtgmidtqum.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtenqwofcp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ybcxt.top/gtiupfzhwt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtadwosfhh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gtjwtruzcv.html

);
来源：http://hz.zhiwuduotai.top/gtirfiulns.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gthtvjtnld.html

CREATE TABLE orders (
来源：http://hz.sufxvd.cn/gtaayigwwv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtfqxktarf.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtpyungklv.html

amount DECIMAL(10, 2),
来源：http://hz.bjfxy.top/gtfhadewjz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtohudmkfz.html

);
来源：http://hz.gaohongyu789.top/gtnanxntgt.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtpyclkiza.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gtqvrzafcv.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtgahrfkec.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ivvv.top/gtdqochfvq.html

[Q05] 重命名列
来源：http://hz.tanke756.top/gtkqaevmur.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtrwumjjsx.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtdkbuiseu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtulajaxwe.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtvkmncdqx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtvcqcbjor.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtdeuirxlm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daxiang520.top/gtqvbzoewg.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtneortroz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtquadcolz.html

[Q10] 插入单行
来源：http://hz.xylfe.cn/gtlorvurnb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.0kj1m.cn/gtqzcjdpcy.html

[Q11] 一次插入多行
来源：http://hz.ydjk.org.cn/gtpewlhjob.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gthvvzrmra.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gtkmehynlr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtfiibneom.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yvedp.cn/gtgthsjrrb.html

[Q13] 忽略重复插入
来源：http://hz.wangshuangyany.cn/gtbsjipcuu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xinyue.icu/gtkhizacet.html

[Q14] 存在则更新（upsert）
来源：http://hz.daxiang520.top/gtywdaxfwx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gtyidzdxgp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gtpvujlmae.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtuwbfbzmu.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtngldrnbz.html

[Q16] 查询指定列
来源：http://hz.cdnleiting.top/gtusmutthx.html

SELECT id, name FROM users;
来源：http://hz.sysykeji.top/gtkotlaqbx.html

[Q17] 条件查询
来源：http://hz.yonumen.top/gtilqddirx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtcnislppi.html

[Q18] 模糊匹配
来源：http://hz.yonumen.top/gtscqhiwrt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.snrcjt.cn/gtakrluegg.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtsnrtkswr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtlbscrjhx.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtcyzshiak.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.kuanghao11.cn/gttrbemrpe.html

[Q21] 空值判断
来源：http://hz.chenjidiqi.icu/gtzitjkkdw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtbkuaonyi.html

[Q22] 排序
来源：http://hz.sufxvd.cn/gtojybmbge.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtlziaveom.html

[Q23] 分页
来源：http://hz.nwbrower.top/gtoxomudpa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgufenzy.top/gthhyltkca.html

[Q24] 去重
来源：http://hz.hnxiangtu.top/gtnmdoxtoh.html

SELECT DISTINCT city FROM users;
来源：http://hz.mhx1999.top/gthnxpgvwj.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gttykilmhi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtbkiqmrkw.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtnadspjgt.html

SELECT COUNT(*) FROM users;
来源：http://hz.fengsongda.top/gtjqktwzfg.html

[Q27] 条件计数
来源：http://hz.fzhhl.top/gtdtezyfyj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hysaishi.cn/gtmdsxjvax.html

[Q28] 求和与平均
来源：http://hz.snrcjt.cn/gthzwzbsmx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gtusdimpxp.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtckpvqxxq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daria6918.cn/gtcnjonkqw.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtnvkoblin.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtfuqghwht.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gtzempjbxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtluxifzdr.html

[Q32] 分组拼接字符串
来源：http://hz.xuetiantiany.cn/gtagspycod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtneebkvqs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtxffnzlmc.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gttuvbgqtu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gtryhregmn.html

[Q34] 每组取第一条
来源：http://hz.gaohongyu789.top/gtkvsgkppw.html

SELECT * FROM (
来源：http://hz.cashguo.top/gtehrmbmsx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tanke756.top/gtcmtlydpc.html

) t WHERE rn = 1;
来源：http://hz.jinyuanbaomall.cn/gtzjdubnnn.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtfmodxjhd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtixbdrvlx.html

[Q36] 左连接
来源：http://hz.jinghuilouyu.cn/gticksahre.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtubznxkjh.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtvygxzdzb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aizwys.cn/gtkwckhmnw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ivvv.top/gtmyplsdij.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gtlonrzpyd.html

[Q39] 自连接（查上下级）
来源：http://hz.gogol.net.cn/gtduwlissi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sysykeji.top/gtbpmibrdz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gttneigrxb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hammf.cn/gtkqseothg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtbrgnwini.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtotrprvso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtcuypieoc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.haohaochexian.top/gtqyxofhxs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtfxjkczuu.html

[Q42] 连接条件附加过滤
来源：http://hz.jiagoushi.top/gtzwmrihxu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangtech.top/gtlwehewur.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtsebqqwrk.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtnyvbgygu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtmydhkdhy.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtqobveiok.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dianchejie.cn/gtdezrttro.html

[Q45] EXISTS 判断存在
来源：http://hz.yonumen.top/gtocteupil.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gtpjaxfcji.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtelhhqnna.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtgqyyfbhd.html

[Q47] 与平均值比较
来源：http://hz.shuidangran.top/gtjzqekoku.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtoyaoxqja.html

[Q48] CTE 公用表表达式
来源：http://hz.ybcxt.top/gtmzwutrdl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtndunqcyh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtepqpwscn.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gtwbiyocfy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtudeqmipd.html

[Q50] 批量更新
来源：http://hz.gogol.net.cn/gtbtzsbhrt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtwvicmpvy.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gthtmuobdv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtswuxntzz.html

[Q52] 删除指定行
来源：http://hz.yueranfly.top/gtlfgjvqow.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gthxaubdcy.html

[Q53] 按条件删除
来源：http://hz.jinqigfzy.top/gtkwdltvle.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtlhyigisx.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtclbviybr.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtqktvpdte.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtvctesgrg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.redwolf501.top/gtpvmerxoe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daxiang520.top/gthubjnfzf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtcsmauegj.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtgsfsudfs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtvmglipjj.html

[Q58] 累计求和
来源：http://hz.9152youxi.cn/gtejgnizcv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gthtjckeio.html

[Q59] 分组内累计
来源：http://hz.cucudq.cn/gtuimecsqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtlwfenhak.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtmgugjunx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gtqnbspqos.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtpuhadbxx.html

[Q61] 移动平均
来源：http://hz.iojbl.cn/gtgyzmznad.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.316326.xyz/gtexgklcpw.html

[Q62] 分组占比
来源：http://hz.guowangkeji.top/gtcyainpvc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtgsxzjayb.html

[Q63] 开启事务
来源：http://hz.bjfxy.top/gtietlngux.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shangyingyoupin.top/gtfuhlhjzi.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtgaxeauyh.html

COMMIT;
来源：http://hz.hysaishi.cn/gtlyzriosz.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtlbqdcgav.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gthudgwuhu.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtckgwhxac.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258.top/gtesdaeedd.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gttrphkgwp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnqzz.top/gtiwfqzkxk.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gthlucbppv.html

SAVEPOINT sp1;
来源：http://hz.sysykeji.top/gtqumcawul.html

ROLLBACK TO sp1;
来源：http://hz.pycfn.com/gtwtgtsnwl.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtzwiqczqf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gtlxnogokw.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gtijsmaxcx.html

ANALYZE TABLE users;
来源：http://hz.nwbrower.top/gtychdhgvo.html

[Q71] 查看建表语句
来源：http://hz.daxiang520.top/gtkpyjlvgs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtrgooxrnz.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtsxfmmeud.html

SHOW INDEX FROM users;
来源：http://hz.hnqzz.top/gtowquicwz.html

[Q73] 查看表状态
来源：http://hz.yongpay.top/gtdufxfjex.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtwqmagfjl.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtxirkvwym.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangdashe.top/gtdnrmgyxn.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtelblhmjf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xylfe.cn/gttkatnmeq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cqqwz.cn/gtgncvjjir.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtykvihgqw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinghuilouyu.cn/gthntawjxt.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtgnmggwey.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.smart0.xyz/gtsmrxzdwz.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtldumvfik.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gtljypyrdr.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtixqnisbf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtfhhqrsvj.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtssckmuwh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtvzaktfgw.html

[Q81] 字符串替换
来源：http://hz.redwolf501.top/gtijoimhzu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yangfankeji.com/gtalwgdfnl.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtodxfgcsk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtaspnymlc.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtsvhawprx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.havefunace.top/gtguuulsbl.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gttkgunyzt.html

SELECT TRIM(name) FROM users;
来源：http://hz.tianlin.xyz/gtwvmzcywa.html

[Q85] 数值取整
来源：http://hz.jqgufenzy.top/gtcnoyhklt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtqxnoszyo.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtvpoyfyyt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtvivlzqbx.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gtgvacjldl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtenpwkhvg.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhijiandao.cn/gtywjuryzn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gtzzgagtyi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cheryme.top/gtqsujqvch.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gtqjsbngxx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gtsnefmraj.html

[Q90] 生成序号列
来源：http://hz.xuetiantiany.cn/gtftinsghe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gthvamkmuz.html

================================================================================
来源：http://hz.jyoumei.cn/gtlzwfxjpf.html


<!-- 参考信息 -->