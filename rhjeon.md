代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yueranfly.top/gtwqtepfch.html

C#:   lock (gate) { shared++; }
来源：http://hz.hammf.cn/gtrpwvwuqe.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtycrkncce.html

Py:   async def f():⏎    await g()
来源：http://hz.wangshuangyany.cn/gtcplpyxzr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtkwstszyx.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtlpzlfkio.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtqamjyiqy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangkeji.top/gtnvsxlfwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtihprsbzn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuetiantiany.cn/gtuqhyaqgw.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtnqwkcwyq.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtioaprwnb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnxiangtu.top/gtnszsmytc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jiagoushi.top/gtvxowfmdc.html

JS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtbyfcbntl.html

TS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtnwocrvfu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtjoshycvc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gtdwzrfzgx.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangtech.top/gtsvgjnkri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydjk.org.cn/gtqofrtvkc.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gthtdjcavy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xylfe.cn/gtammjsznd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nwbrower.top/gtkntoipvt.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtoihgmdml.html

TS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtroxtjogb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gaohongyu789.top/gtejeiiglw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xingfuxueyuan.xyz/gtmdivrhak.html

Ruby: // fork 块
来源：http://hz.ydjk.org.cn/gtzghdvzwp.html

C#:   Parallel.For
来源：http://hz.xuetiantiany.cn/gtyklwoeln.html

================================================================================
来源：http://hz.redwolf501.top/gtshkdywnj.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtsdwtpkhp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzahupxyy.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtmrdsuwkb.html

Py:   str(uuid.uuid4())
来源：http://hz.aizwys.cn/gtmvtskgag.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtbnnvjbss.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtywdftykm.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtsbhxvuie.html

Java: UUID.randomUUID().toString()
来源：http://hz.birdmap.top/gtugdckpec.html

Go:   // 用 github.com/google/uuid
来源：http://hz.smart0.xyz/gtvuobewiq.html

Ruby: SecureRandom.uuid
来源：http://hz.hongshengwenyu.top/gtwgeweoiw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtuzndgepp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.quarkkingdee.top/gtzcvnahtn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtfkuigxzj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.mhx1999.top/gtmriaclus.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydjk.org.cn/gtnugswixz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnxiangtu.top/gtpfktxsjd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydjk.org.cn/gtghfyjimr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ybcxt.top/gttyforqft.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtdzbsijwu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtqtddewxg.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtmccqdlbf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtxcpcfsck.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sweek.top/gtpnbjbdzk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtzybnavpe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtmloxopqo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtjjkwltgd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.smart0.xyz/gtrvcpnrhp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.feifeiyinyue.top/gteqochgbg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xziqi.cn/gtxjsfhhel.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtxsvxzdmq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtgpkasuqo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtlnsvbdom.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtkzdbzzlz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtxwppmjgb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gtgqesvugz.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gtawlxfpmc.html

Ruby: x.length;  x.size
来源：http://hz.kuanghao11.cn/gtsregdwwq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtnvmddtfp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtoolyjnyt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yongpay.top/gthiznpxng.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtzmxaoovc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pengpengdd.cyou/gtldtbpwfi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuanzhike.top/gtabomnjou.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtnuemuvrg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aibaodan.cn/gtgxeppilz.html

Ruby: a == b
来源：http://hz.birdmap.top/gtuveaisio.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtmlxlwuey.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.mhx1999.top/gtqlgugerl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gthmgkcbvs.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtqcopgegu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtupvdhagy.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gttcdxbozh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jianghu66.top/gtutijdnlc.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtspbrpomz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtlwqpbkmh.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtroqukfob.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtrbbmnjrh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cheryme.top/gtucelfukm.html

PHP:  // 手写时间戳比较
来源：http://hz.xingfuxueyuan.xyz/gtzuvhsadv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtggzetbip.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtokdnsosv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinghuilouyu.cn/gtbjddzjbj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fengsongda.top/gtilckkvgc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ehwqpu.com/gtfchwzlww.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj202588.top/gtnkidtkrg.html

[P08] 处理浮点精度问题
来源：http://hz.tian-w.cn/gtaklslvij.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.svipenyu.cn/gtkbvvgqfp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gotoacloud.top/gthvrhaavp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yueranfly.top/gtdsnutqze.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtmeptcrbq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nwbrower.top/gtvprexvhc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daria6918.cn/gtvuwzxlvb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pengpengdd.cyou/gtwfduleie.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtjbkcbuty.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlnzmfpcb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.andypj.xyz/gtfuvmrqmu.html

================================================================================
来源：http://hz.tian-w.cn/gtqybyuytd.html

[Q01] 创建表
来源：http://hz.ivvv.top/gthbnqskuv.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtpmasamqg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtbysyvqma.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtolwvxsdg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnxiangtu.top/gtzuqkrgrm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigfzy.top/gtyomtrfqe.html

);
来源：http://hz.chenlongwang.top/gtzzktxmth.html

[Q02] 创建带外键的表
来源：http://hz.pycfn.com/gthlqafqsl.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gtlnilbidk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.quarkkingdee.top/gtpgpflyhx.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtdsnqviez.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangtech.top/gtzbnontnw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sxryk.cn/gthoryagyu.html

);
来源：http://hz.snrcjt.cn/gtxkstwmxk.html

[Q03] 增加列
来源：http://hz.cqqwz.cn/gtfevsiswy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtjrqakhat.html

[Q04] 修改列类型
来源：http://hz.yuanzhike.top/gtifcrqets.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gthmnpryao.html

[Q05] 重命名列
来源：http://hz.jinqigufen.top/gtqnloyopx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtfgavills.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtbvnmzokb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtggsauydn.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtlhitcwkh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.snrcjt.cn/gtwdmfxtxa.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtozbxitpn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangdashe.top/gtgzddrlhy.html

[Q09] 创建唯一索引
来源：http://hz.yangfankeji.com/gtylomtzum.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtrtthjfzc.html

[Q10] 插入单行
来源：http://hz.iojbl.cn/gtgsfgtbgh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gtmjtlsbuu.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gteprqjakc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cucudq.cn/gtpqvvdpuo.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtsfradumv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtnlysqvtc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtsknqgldt.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtlmbxhqha.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guowangkeji.top/gtptmdaelv.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxinkj.top/gtifsuttml.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pycfn.com/gtyvorrrqt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtqcccsbkz.html

[Q15] 查询全部
来源：http://hz.jiagoushi.top/gtcewhpjcr.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtpfroxzxc.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtvbopvunk.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gtexdzrfyc.html

[Q17] 条件查询
来源：http://hz.gotoacloud.top/gtlgrvpvep.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.svipenyu.cn/gtbkojddgu.html

[Q18] 模糊匹配
来源：http://hz.ywan-chungtsiang.top/gtllvxrowm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtehvrhpdf.html

[Q19] 范围查询
来源：http://hz.gotoacloud.top/gtdrjmtwns.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gteomyovya.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gttzpcbrhz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtjbmtxhef.html

[Q21] 空值判断
来源：http://hz.yonumen.top/gtphmldkus.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtrpjormuh.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtrvwvupnh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtwctvowwa.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gtdqcwnvjm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gthfstbglx.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gtwqzuzqjl.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gtwzblgnem.html

[Q25] 只取前 N 条
来源：http://hz.0kj1m.cn/gtlkajgzpi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gttyeekbqy.html

[Q26] 计数
来源：http://hz.316326.xyz/gteqejgdin.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtrvhddxxh.html

[Q27] 条件计数
来源：http://hz.hfpthk.cn/gtcgqpgipq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtyuvdedna.html

[Q28] 求和与平均
来源：http://hz.hysaishi.cn/gtyhwkjrwa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtwmkoljnx.html

[Q29] 最大最小值
来源：http://hz.cheryme.top/gtwysbsqpu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnxiangtu.top/gtzmjdgcfv.html

[Q30] 分组统计
来源：http://hz.jianghu66.top/gtxtgkhhan.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtnnfuezli.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtsfcmyeln.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangtech.top/gtgdwadhiu.html

[Q32] 分组拼接字符串
来源：http://hz.feifeiyinyue.top/gtvlkvigfq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtfdhewhfn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangdashe.top/gtsoruadke.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gtcqzdrvsy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gtyxceqxnr.html

[Q34] 每组取第一条
来源：http://hz.dianchejie.cn/gtesuocazd.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtsclrozir.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtebeijhrh.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtxxhxvgmw.html

[Q35] 内连接
来源：http://hz.nanxuanxn.top/gtgkcflukv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtnkvishys.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtijvjloty.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtdzwbrogx.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gtidpjajvp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtoawsprts.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangkeji.top/gtlrfkxxdk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ywan-chungtsiang.top/gtgiswrzzd.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gtfofilopi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aizwys.cn/gtrjeacwqs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtzvzrcokf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.bjfxy.top/gthkkkbpvq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtwoikunjv.html

[Q41] 多表连接
来源：http://hz.svipenyu.cn/gtewlblvom.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cucudq.cn/gtsypdrkct.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gthkjyuxnx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ybcxt.top/gtzcyvowlr.html

[Q42] 连接条件附加过滤
来源：http://hz.zhijiandao.cn/gthnncmnys.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj202588.top/gtdblotpiz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gteozffvct.html

[Q43] 标量子查询
来源：http://hz.xingfuxueyuan.xyz/gtqlmmudvg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.havefunace.top/gtyjyghnln.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtewzajjql.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gttdazslpc.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxuanxn.top/gtvzlzgzhx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtnztfbknp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigfzy.top/gtpgeaavbi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtuyrdtfhe.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtuejarpmi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtxdaprfxv.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtamehidhi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtiwmnaopm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtrgcemxvl.html

[Q49] 更新单行
来源：http://hz.wangdashe.top/gtcwcjdpzd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtobvhugyh.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtbtcqaxsy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtnnwnbvfd.html

[Q51] 用子查询更新
来源：http://hz.mhx1999.top/gtsyiuzpyi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydjk.org.cn/gtywegdpsq.html

[Q52] 删除指定行
来源：http://hz.xuetiantiany.cn/gtbbwgdaxr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtsmyrckur.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtoncpqbxd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gogol.net.cn/gtinkvbbhr.html

[Q54] 清空表
来源：http://hz.yuxming.cn/gtocjwinki.html

TRUNCATE TABLE logs;
来源：http://hz.jianghu66.top/gtaioklhxi.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtodmgbyzu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigufen.top/gtnqmkphmj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.andypj.xyz/gtyatgvhfh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtnlgplhcc.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtmrvpddho.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sufxvd.cn/gthxvtnpkw.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtgmjkkrnu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ehwqpu.com/gtnmmajtbm.html

[Q59] 分组内累计
来源：http://hz.yueranfly.top/gtpnkvtkfl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtoavqjlgi.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gteezoqawk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yangfankeji.com/gtcxtyykdn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hfpthk.cn/gttywhympr.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gtudmjasdx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gtunivsfqn.html

[Q62] 分组占比
来源：http://hz.bjfxy.top/gtqlzpanew.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtyvsoovll.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gtnwjgwigk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jlsjyb.cn/gtcelwmzuv.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtusdqjtxg.html

COMMIT;
来源：http://hz.tianlin.xyz/gtqjtofsba.html

[Q65] 回滚事务
来源：http://hz.hfpthk.cn/gtdvhcypqm.html

ROLLBACK;
来源：http://hz.sweek.top/gtnhspoehu.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gtmglhdhyf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shangyingyoupin.top/gtifojehls.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtbonbgjgq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gteyfkzbdz.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtzvakcgdq.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtpctfadpo.html

ROLLBACK TO sp1;
来源：http://hz.jiagoushi.top/gtmccdxpxv.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtnpsezmnx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gthhvpzxge.html

[Q70] 更新统计信息
来源：http://hz.ywan-chungtsiang.top/gtnlpqmojz.html

ANALYZE TABLE users;
来源：http://hz.cashguo.top/gtwruthzmh.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gtbmmmocwu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtlzpjbqcq.html

[Q72] 查看索引
来源：http://hz.jinyuanbaomall.cn/gtsntqmeyq.html

SHOW INDEX FROM users;
来源：http://hz.bjfxy.top/gtarbnnxpd.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtpxgclfyn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gtrwscbilo.html

[Q74] 强制使用索引
来源：http://hz.hammf.cn/gtwhesjcrj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtndpzzpok.html

[Q75] 日期格式化
来源：http://hz.iojbl.cn/gtettzqjri.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuxming.cn/gtssafzbal.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtrdpzqdij.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gthmmjyzmd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.birdmap.top/gtugxvfeuy.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtlaxpfuvh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtoqgwshck.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtgvczmciu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtymmwjfks.html

[Q79] 字符串拼接
来源：http://hz.cashguo.top/gtqgopaqwk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gtzbhzntmt.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtmeaxfogn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.feifeiyinyue.top/gtjfiwxmjk.html

[Q81] 字符串替换
来源：http://hz.shangyingyoupin.top/gtpmaddwpg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jlsjyb.cn/gtadkktrlq.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gtnxexrpty.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jianghu66.top/gtxoqdmewf.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtrxrfojcw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtznbycagd.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gttufwlxgh.html

SELECT TRIM(name) FROM users;
来源：http://hz.cqqwz.cn/gtyqarwcyb.html

[Q85] 数值取整
来源：http://hz.andypj.xyz/gtoemxgrks.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtkdjwpgfb.html


<!-- 参考信息 -->