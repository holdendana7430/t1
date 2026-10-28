代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gtzukbxfyo.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtfxvtyllm.html

[O04] 定义异步函数并等待
来源：http://hz.smart0.xyz/gtpuuowexj.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtilwbdwak.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtybwhongn.html

JS:   async function f() { await g(); }
来源：http://hz.shuidangran.top/gtxmrpwcer.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hywenlv.cn/gtbvmbzwxi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gtfwlbbrgc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.havefunace.top/gtswwuvpla.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jlsjyb.cn/gtrhxjndmy.html

C#:   async Task F() { await G(); }
来源：http://hz.dianchejie.cn/gteqxiunte.html

[O05] 并发执行并等待全部完成
来源：http://hz.vqdsnc.cn/gtachxrpqc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.vqdsnc.cn/gtfnpgwngb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtplniotyb.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtxohvbtqe.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtbriutbtm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258888.top/gtuuvahvew.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.redwolf501.top/gtczubplws.html

Ruby: threads.map(&:join)
来源：http://hz.jyoumei.cn/gtyeepptyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hysaishi.cn/gtbrcrqtja.html

[O06] 使用进程池
来源：http://hz.ydjk.org.cn/gtzxqbmytu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gtywdssduw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtlwngdgsi.html

JS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtwfydlrcv.html

TS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtvrzckyxm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.haohaochexian.top/gtczibwedu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangkeji.top/gtbxizrwrx.html

Ruby: // fork 块
来源：http://hz.zhengqikj.top/gtqnwezcem.html

C#:   Parallel.For
来源：http://hz.jinqigfzy.top/gtspdxjrda.html

================================================================================
来源：http://hz.daxiang520.top/gtfyofolyz.html

P. 常用工具函数
来源：http://hz.ywan-chungtsiang.top/gtccomzxyp.html

================================================================================
来源：http://hz.hnqzz.top/gtwkzdnisf.html

[P01] 生成 UUID
来源：http://hz.quarkkingdee.top/gtdhgvgzkw.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtjezvzjkd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtaydafhbu.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtxrtleibl.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtkohgawih.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtnwqqajgf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtfipbdgjx.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtkxbxgoqt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.svipenyu.cn/gtoeksouwk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gtbnktjbyi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgfzy.top/gtnhgdopcw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtuwxebmwl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtexqyxnew.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hfpthk.cn/gtfscpmmoo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtlghmsrbk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hongshengwenyu.top/gtsvsamanr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtgqqskqzx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtyxezdagw.html

[P03] 生成短随机字符串
来源：http://hz.0kj1m.cn/gtpzzmmycj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtfmyslfrg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cdnleiting.top/gtcxirasrf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtdqwwswhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtlgwtkwpc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gttbugzgtn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgfzy.top/gtgjbybalm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xinyue.icu/gtwqmqgbpb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtqcjalkdw.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtbzbateqy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sxryk.cn/gtxlxavqlj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gttrocixtl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtfkqpmiot.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gterprutuc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gtpzckzxdm.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtthqekalo.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtmzcwteja.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.0kj1m.cn/gthczgrkrt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gterekvvcs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtrubigcbf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtlikrfrmq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cheryme.top/gtrtyxgglj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtiwrkpwpu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtihwkxrap.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtikslrsrm.html

Ruby: a == b
来源：http://hz.hysaishi.cn/gtvsraufvh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hongshengwenyu.top/gtjluzswbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuanzx.com/gttrzzmtji.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.vqdsnc.cn/gtghxeypap.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtqlhmolhw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gtlzlhqczh.html

TS:   if (x == null) {}
来源：http://hz.dashuyun.cn/gtjpwoulpj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtiokswtov.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtzhpfdwss.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtysbszqij.html

C#:   if (x is null) {}
来源：http://hz.havefunace.top/gtxvoeojsn.html

[P07] 防抖与节流
来源：http://hz.jinyuanbaomall.cn/gtbctojtmu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gtmdsbytih.html

PHP:  // 手写时间戳比较
来源：http://hz.zhijiandao.cn/gteihfjink.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtdlrfjmta.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtanvcgsgd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtszljluzj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gthwxvoral.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtyaojjokb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gtfmnborhd.html

[P08] 处理浮点精度问题
来源：http://hz.cashguo.top/gtfzepctnw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.iojbl.cn/gtjhuauico.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtjaafstad.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.birdmap.top/gtanvscuag.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtjmxmbdbq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gttwohnwxn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yangfankeji.com/gtxmxuroer.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtiwovjiom.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yangfankeji.com/gtzwcvhkcw.html

================================================================================
来源：http://hz.hfpthk.cn/gtxxhdpkrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinghuilouyu.cn/gthbeuavfn.html

================================================================================
来源：http://hz.cdnleiting.top/gtdhrdpioz.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtaelzrpon.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtfasdhfiu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtpuopbvyj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtraazwkev.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnxiangtu.top/gtidvoybew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydjk.org.cn/gtfbwrvugc.html

);
来源：http://hz.shuidangran.top/gtqttpwlbl.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtnooskhaz.html

CREATE TABLE orders (
来源：http://hz.xylfe.cn/gtwbczujtp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtzygpxyiv.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gtwsumwqlm.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtsiirizyp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtqrzpuvxc.html

);
来源：http://hz.yonumen.top/gtdsucagtm.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtetsyabsk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhaomingkeji.xyz/gtiridrnex.html

[Q04] 修改列类型
来源：http://hz.yj20258888.top/gtwarqfoyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtvoekcxvk.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gthntuoomf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtrxskzefo.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtqzkelpvz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guowangkeji.top/gtldqnfxfo.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gttvglroas.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtisiyizet.html

[Q08] 创建普通索引
来源：http://hz.pycfn.com/gtwcsytwpy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aizwys.cn/gtmamoscxz.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtplftmnyk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtyzlxxyzy.html

[Q10] 插入单行
来源：http://hz.zycfv.cn/gttofbehkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtceprbtzq.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtfiuooldh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.bjfxy.top/gtorqhsrub.html

[Q12] 插入后取自增 ID
来源：http://hz.nanxuanxn.top/gtwjuqyikz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgfzy.top/gttjxhdztf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sweek.top/gtcwrjmhwd.html

[Q13] 忽略重复插入
来源：http://hz.cheryme.top/gtyvtulfgg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gthozyujlo.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgufenzy.top/gtbnnpfbhx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtxdkirebt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zycfv.cn/gtptgyyyec.html

[Q15] 查询全部
来源：http://hz.jqgufenzy.top/gtkhkgidfg.html

SELECT * FROM users;
来源：http://hz.shuidangran.top/gtbrwaszbg.html

[Q16] 查询指定列
来源：http://hz.shangyingyoupin.top/gtflcusack.html

SELECT id, name FROM users;
来源：http://hz.yvedp.cn/gtwpvnedde.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gtuaqxtwwp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtnsoakcck.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtikanoyuj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtonbpnrba.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtogxznwkn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yvedp.cn/gtozcprytc.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gtbysmvcdt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtcxmnpmhv.html

[Q21] 空值判断
来源：http://hz.tian-w.cn/gtekfpfzsr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtckfajvyg.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtbstllwzj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtwuxrpikc.html

[Q23] 分页
来源：http://hz.cucudq.cn/gtasxjdecl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxinkj.top/gtvglygypq.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtoeapcruf.html

SELECT DISTINCT city FROM users;
来源：http://hz.shzxlz.cn/gtodspseks.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtkuezivqd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtpwsvhtlg.html

[Q26] 计数
来源：http://hz.pycfn.com/gttseutaks.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtytenifai.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtmwzwlqzc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtflyafyce.html

[Q28] 求和与平均
来源：http://hz.hongshengwenyu.top/gtwfmbylod.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuanzhike.top/gtbxwxqvwm.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtudvjwbly.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dianchejie.cn/gtpqzuzpbe.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtznugtqei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtskxeciqu.html

[Q31] 分组后过滤
来源：http://hz.pycfn.com/gtujkozivo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gtmexdejzf.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gtwciayssn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtqjjmirgs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258888.top/gtrogqaray.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtodhvessk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtslxsynwu.html

[Q34] 每组取第一条
来源：http://hz.zhaomingkeji.xyz/gtzmivfkjr.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gtyymfuqyi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtlepabpbl.html

) t WHERE rn = 1;
来源：http://hz.zdqjudy.top/gtcnsznjqj.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gtzyafygag.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtubwxtheh.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtordrusia.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtqnmjajtk.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gtargdmehh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pengpengdd.cyou/gtsyzdfcou.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtszftreqj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ivvv.top/gtisajzggy.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtrjanvhyc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenjidiqi.icu/gtwolrkcym.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuanzhike.top/gtlubpnrui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sxryk.cn/gtglfcsxuu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.snrcjt.cn/gtfwhbimog.html

[Q41] 多表连接
来源：http://hz.sxryk.cn/gtyinvyedb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtxtsexamf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtnilciyiw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtceulpjos.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gttfxekzea.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangtech.top/gtltsnakbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhixingplan.top/gtjbldzgud.html

[Q43] 标量子查询
来源：http://hz.sysykeji.top/gtnfsjwxpx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtqmhvyjnz.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gtaveroslf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhixingplan.top/gtrxrqbkng.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gthpubbxxa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtozknpjxo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hysaishi.cn/gtormfuzgo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtuggwyxyj.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtvkdpeuoz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sxryk.cn/gthgfrefcs.html

[Q48] CTE 公用表表达式
来源：http://hz.wangshuangyany.cn/gtfltuhwiy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtzdoudaiu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nwbrower.top/gtmscxtjvt.html

[Q49] 更新单行
来源：http://hz.dashuyun.cn/gtxbkuueap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtmhnwchey.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtoryknkaw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.kuanghao11.cn/gtpradijao.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gteipjyofy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhixingplan.top/gtpdbuioiy.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtnhnxbdur.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtvcbyjotc.html

[Q53] 按条件删除
来源：http://hz.hnxiangtu.top/gtzjhemdxj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtwgklmwsg.html

[Q54] 清空表
来源：http://hz.guannengcc.top/gtjiqinzos.html

TRUNCATE TABLE logs;
来源：http://hz.nanxuanxn.top/gtitcagvyg.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gtovaslniz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gaohongyu789.top/gtaqngmssb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xylfe.cn/gtulmhetel.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.feifeiyinyue.top/gtsmwhjici.html

[Q57] 行号
来源：http://hz.ivvv.top/gtagigwxfe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtqblrksvq.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gtqccbmzau.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.316326.xyz/gtapyssnzv.html

[Q59] 分组内累计
来源：http://hz.xziqi.cn/gtdznbzisc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gzhubu.top/gtjsxtxzoi.html

[Q60] 取上一行 / 下一行
来源：http://hz.nwbrower.top/gtjmkdarld.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtwhazavba.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.9152youxi.cn/gtpqajwmng.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtmtvmxlqu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.mhx1999.top/gtbbdcnqgp.html

[Q62] 分组占比
来源：http://hz.fzhhl.top/gtkkavsiqj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtwrboktao.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gttrqimdmp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gotoacloud.top/gtahrpcjcv.html

[Q64] 提交事务
来源：http://hz.sufxvd.cn/gtkedbgjbk.html

COMMIT;
来源：http://hz.andypj.xyz/gtpnacffhw.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtpsngwohy.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtqoktserg.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtdpqurdxt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtfmdgctqy.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtvoluobcp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtflvobrkq.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtxdxwggal.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gtvxmlygil.html

ROLLBACK TO sp1;
来源：http://hz.yvedp.cn/gttfvevybl.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtbozsijkr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gticficlnh.html

[Q70] 更新统计信息
来源：http://hz.sufxvd.cn/gtwdvubuyu.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtjrtvnzud.html

[Q71] 查看建表语句
来源：http://hz.0kj1m.cn/gtidfvgbno.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhaomingkeji.xyz/gtguevrafo.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtpiueofrw.html

SHOW INDEX FROM users;
来源：http://hz.fzhhl.top/gtdpfncmxr.html

[Q73] 查看表状态
来源：http://hz.gzhubu.top/gtvzwbgrwy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtvaunixul.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtlsfdtpbv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtltqejgaj.html

[Q75] 日期格式化
来源：http://hz.zhixingplan.top/gteuepmrqf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxuanxn.top/gtlepehgul.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtrdbfdemk.html

[Q76] 按天统计
来源：http://hz.sufxvd.cn/gtbzqjolse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dianchejie.cn/gtlsjheout.html

[Q77] 时间加减
来源：http://hz.cashguo.top/gtausjztit.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtlcwfrkrs.html

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtrksjphls.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtystrkiav.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtubyvrgjm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtgaqeqcyg.html

[Q80] 字符串截取
来源：http://hz.cucudq.cn/gtyoisvhmf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxinkj.top/gtcaqvhacw.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtqhkjruwd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtdybjmxev.html

[Q82] 字符长度与字节长度
来源：http://hz.bjfxy.top/gtpzucfmfm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtibrdznvp.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtolophjqn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ybcxt.top/gtcesqgoqc.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtlwkqzxyh.html

SELECT TRIM(name) FROM users;
来源：http://hz.bjfxy.top/gtxqqchmqm.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtxnchbumk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj202588.top/gthwtngnqa.html


<!-- 参考信息 -->