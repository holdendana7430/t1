代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ybcxt.top/gtpnjzelih.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cdnleiting.top/gtufgfwynk.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtjnqllwrx.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gttgasqrwy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtxnbdcbhx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.smart0.xyz/gtfmnflkzr.html

JS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtndwkinfg.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtzijdekqd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gtegdidqhk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.vqdsnc.cn/gtnztujabz.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigufen.top/gtcuiwbdpl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtzybborfo.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtjusjoybk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtoskszdlt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtiiwqdnir.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gthcponhqk.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtomeeoswy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenjidiqi.icu/gtsenhhyrk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dianchejie.cn/gtjfztdrlf.html

Ruby: // fork 块
来源：http://hz.sufxvd.cn/gtrngluahn.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtqzvrlgfr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxyzuftvn.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtiwqiggom.html

================================================================================
来源：http://hz.hnqzz.top/gttkxjncdz.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtgshaxgmx.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtxiayaadx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258.top/gtmalkrdkc.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtawtroeev.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtblgedfjw.html

Java: UUID.randomUUID().toString()
来源：http://hz.sxryk.cn/gtwfuyfmey.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xziqi.cn/gtkjfewmwx.html

Ruby: SecureRandom.uuid
来源：http://hz.kuanghao11.cn/gtqtmlysrq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtjxbhtczn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtnakaeibf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinyuanbaomall.cn/gtwvefbfmt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gzhubu.top/gtuebcsiha.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gthxkpevvb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtasypdnbe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gtrrdxemvo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtdxhimjtx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gtsmtnslma.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinghuilouyu.cn/gtqmqqgsme.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtlmrpwevt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.andypj.xyz/gtyzhwqcfl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtbgsstcov.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtuqserztj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtazelepqs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtddtrquna.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gthsiwuqvf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.52xcode.cn/gtfwdpibhk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnqzz.top/gtfthsnqid.html

[P04] 求长度
来源：http://hz.ivvv.top/gtealkgkyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cqqwz.cn/gtopfmvvls.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtvynxstjy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtebazxbpf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtnmvluwon.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinyuanbaomall.cn/gtwkjbzldm.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtqbhhfjvu.html

Ruby: x.length;  x.size
来源：http://hz.dashuyun.cn/gtrorzmyut.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtdinmwaif.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtjavjqhpk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtegzhhxec.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtpupcmxub.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hongshengwenyu.top/gtrbqhhjgb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gthenkpfeo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtcdnnnxur.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sweek.top/gtbdnoavdu.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtjxakimid.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnqzz.top/gtookytkft.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtpioujirr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jianghu66.top/gtiaaqkani.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtwiuxdehw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ybcxt.top/gtlmnnttdp.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gthoekihxg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenzaomai.com/gthuwowbps.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtxygaensz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xingfuxueyuan.xyz/gtxvtmkdak.html

C#:   if (x is null) {}
来源：http://hz.jyoumei.cn/gtefardgjm.html

[P07] 防抖与节流
来源：http://hz.shangyingyoupin.top/gtkuokkejh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangtech.top/gtxwpkdehb.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtprfqqtuz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtrwlpfwuq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtrrudoizq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtxexvghbb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gtcfovdnye.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtfpzrleak.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hfpthk.cn/gtdhzvtthf.html

[P08] 处理浮点精度问题
来源：http://hz.jqgufenzy.top/gtzbamkcnb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtxmcgcrcj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtkmmivrgf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gtvwtdasyk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cqqwz.cn/gtctilscjf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gaohongyu789.top/gtercvfkeb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtbecnqmrc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.quarkkingdee.top/gtbzlriwpg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gtlsbcylyf.html

================================================================================
来源：http://hz.sysykeji.top/gtjyvcjltf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtluwavoqo.html

================================================================================
来源：http://hz.jqgfzy.top/gtigbauoyb.html

[Q01] 创建表
来源：http://hz.jianghu66.top/gtvsctlpcn.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gtboiuolhu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtuigqlbjl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtrcothfqe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shuidangran.top/gtohbkoqcl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gtjlmfrdmx.html

);
来源：http://hz.52xcode.cn/gtydotnomd.html

[Q02] 创建带外键的表
来源：http://hz.gogol.net.cn/gtnitboajr.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtryluqxfq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gttjzacchk.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtcyiaqaow.html

amount DECIMAL(10, 2),
来源：http://hz.yonumen.top/gtrqeucuvx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtnpgnrpve.html

);
来源：http://hz.chenlongwang.top/gtuuvbfuxr.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtjqdckdto.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.iojbl.cn/gtybxygmuh.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtovtfbrkk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guannengcc.top/gtsaoynmbw.html

[Q05] 重命名列
来源：http://hz.chenzaomai.com/gtnoiokblz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtmacamogp.html

[Q06] 删除列
来源：http://hz.tian-w.cn/gtezeezsxm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gogol.net.cn/gtzonhxlsi.html

[Q07] 删除表
来源：http://hz.xziqi.cn/gtpfdhhowz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtinjuwngk.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtqlefwubo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtrrtchgxm.html

[Q09] 创建唯一索引
来源：http://hz.haohaochexian.top/gtobfziehy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gtixmyqkwy.html

[Q10] 插入单行
来源：http://hz.yongpay.top/gtfbvlzgnx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtlvlbsfjl.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gteeeqkvoi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtdncxdwdc.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtqyxylxnu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuanzx.com/gternzzblz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtzxmvzbuh.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtltdubmzc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cheryme.top/gtbnwagoij.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtjvwudkal.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtbwvbeezv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtfolbtvou.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gthkrkfgjs.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gttzvgpnrq.html

[Q16] 查询指定列
来源：http://hz.fzhhl.top/gtvdamvbms.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtvjrjdjor.html

[Q17] 条件查询
来源：http://hz.shangyingyoupin.top/gtjxvaznst.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.c1oappe.top/gtwrdjkpzj.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtduxlznlb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yanxiufei.cn/gtcwupbglc.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtwnqsxnge.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hywenlv.cn/gtvfasgaqm.html

[Q20] IN 列表
来源：http://hz.andypj.xyz/gttuehymln.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinyuanbaomall.cn/gtfpirtfnt.html

[Q21] 空值判断
来源：http://hz.ppjwa.cn/gtyrmswpiu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtqimlqkzn.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtrhwhydsy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gtylcdavyn.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtoxmsefie.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gtambljwcn.html

[Q24] 去重
来源：http://hz.pengpengdd.cyou/gtrcnbuyll.html

SELECT DISTINCT city FROM users;
来源：http://hz.snrcjt.cn/gtvnllnxcb.html

[Q25] 只取前 N 条
来源：http://hz.cqqwz.cn/gtcbeypkwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hywenlv.cn/gtyzmzlnqq.html

[Q26] 计数
来源：http://hz.ppjwa.cn/gtsoukwksd.html

SELECT COUNT(*) FROM users;
来源：http://hz.tanke756.top/gtgvmqgaqb.html

[Q27] 条件计数
来源：http://hz.daria6918.cn/gtpyvrxplc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.c1oappe.top/gtivjbhqjl.html

[Q28] 求和与平均
来源：http://hz.zhixingplan.top/gtbmgbvgze.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtphxusafu.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gtrlndjkbp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtaokqbjnv.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtqhnnrqkp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtnprjrcfv.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtzhzynkkt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ppjwa.cn/gttllqcqtv.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtditeztel.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtwvssowwu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.9152youxi.cn/gtdaavkhyq.html

[Q33] 多列分组
来源：http://hz.fzhhl.top/gtwhwefhoy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtvyxgnkpq.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtdgkuvqzr.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtagmmgclt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sweek.top/gtndicrzzo.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtupnftirc.html

[Q35] 内连接
来源：http://hz.xinyue.icu/gtdjbxwdnb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtfyziwicx.html

[Q36] 左连接
来源：http://hz.yuxming.cn/gtyvgxdmge.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtcnaaxjch.html

[Q37] 右连接
来源：http://hz.gotoacloud.top/gtlvywkkah.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtgacahuau.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nwbrower.top/gtrsfsbvtr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sweek.top/gtnzppkbzm.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtzjbikass.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.feifeiyinyue.top/gtfebvfwqr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtruldfbjm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fengsongda.top/gttzrcmovr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtibpgqlms.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtrfzwylqf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj202588.top/gtpodaohhz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtoriuafeu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gogol.net.cn/gtokpejpkj.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtzbdivkli.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtjrjusalg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gtwjafdprg.html

[Q43] 标量子查询
来源：http://hz.snrcjt.cn/gteyaduluu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xingfuxueyuan.xyz/gtqewhpwhp.html

[Q44] IN 子查询
来源：http://hz.sysykeji.top/gtmvooyaag.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.mhx1999.top/gtwyebsbkt.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtzkiluacq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtagrohzlc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuanzhike.top/gtmqadnamw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtuztoejhz.html

[Q47] 与平均值比较
来源：http://hz.zhaomingkeji.xyz/gtqrwxpohd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtshnkbnab.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtrvfuqqds.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtjroqikhq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tianlin.xyz/gtynrlutjm.html

[Q49] 更新单行
来源：http://hz.chenzaomai.com/gthzpjsagy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtqgfwgdot.html

[Q50] 批量更新
来源：http://hz.sysykeji.top/gtdoimdvmg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tian-w.cn/gtsrtflfxs.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtsnjvjtew.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gtusqtyjay.html

[Q52] 删除指定行
来源：http://hz.yanxiufei.cn/gtwcosjimu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtpmffxetj.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtrqmnilni.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenzaomai.com/gtrphqlgha.html

[Q54] 清空表
来源：http://hz.gotoacloud.top/gtqdpiaqmv.html

TRUNCATE TABLE logs;
来源：http://hz.jianghu66.top/gtezaqdzwk.html

[Q55] 排名（并列占位）
来源：http://hz.birdmap.top/gtuddjawvg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtfgrimrjt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hongshengwenyu.top/gtryqzpdht.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.quarkkingdee.top/gtbskffzze.html

[Q57] 行号
来源：http://hz.tanke756.top/gthidlhyup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gthiwpltmt.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gtpwfwdgav.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ehwqpu.com/gtqgbpctmg.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtyuifknpx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gtwelueygc.html

[Q60] 取上一行 / 下一行
来源：http://hz.yvedp.cn/gtdrtmtucr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtydwodxww.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sufxvd.cn/gtiregqwdi.html

[Q61] 移动平均
来源：http://hz.hywenlv.cn/gtbjwbirvd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtgeroykza.html

[Q62] 分组占比
来源：http://hz.ehwqpu.com/gtjpcvgdyi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtazmsbfhr.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtsbblocql.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtivixtpkk.html

[Q64] 提交事务
来源：http://hz.hongshengwenyu.top/gtqetvnrgd.html

COMMIT;
来源：http://hz.iojbl.cn/gtcypgxmtr.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtvuclujpq.html

ROLLBACK;
来源：http://hz.cucudq.cn/gtbhghyjiu.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtcmmakggx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gthhjjuvnz.html

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gtqhrbmtpj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtlryfpcie.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtjnuzhpdz.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtizhdvdoi.html

ROLLBACK TO sp1;
来源：http://hz.nanxinkj.top/gtsfvdsgyg.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtztxbivaw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hammf.cn/gtvwwadoie.html

[Q70] 更新统计信息
来源：http://hz.meibo888.top/gtihygpcbm.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtvjtepuqo.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtyxvprhyj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.iojbl.cn/gtcvxrgywl.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtcgfsjdak.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtfepjtlls.html

[Q73] 查看表状态
来源：http://hz.zhijiandao.cn/gtzptubfca.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtiwioondt.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtritdtcye.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jiagoushi.top/gtqetffkgd.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtaynwsjcz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtmuvmrdun.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtnwyseirf.html

[Q76] 按天统计
来源：http://hz.smart0.xyz/gtzthmzfpj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sweek.top/gteczcydvw.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtrrwhtyig.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuanzhike.top/gtfgcmwzue.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtksvdqakn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gtrjbrphcz.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtkzqxugxz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtxcqnbejp.html

[Q80] 字符串截取
来源：http://hz.yj20258.top/gtvycgvfyv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtxzllunhr.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtimrkgbqa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhaomingkeji.xyz/gtjgczfbmn.html

[Q82] 字符长度与字节长度
来源：http://hz.aibaodan.cn/gtxepczbgn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtfrgauujb.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtikqmzocy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gthundujmj.html

[Q84] 去除首尾空格
来源：http://hz.cdnleiting.top/gtsbzbgngc.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtioqypzrm.html

[Q85] 数值取整
来源：http://hz.gotoacloud.top/gtbpbzcnte.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cdnleiting.top/gtxfbqaunj.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gteujofzhq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.0kj1m.cn/gtdwxbgjcz.html

[Q87] JSON 字段做条件
来源：http://hz.daria6918.cn/gtzoqbrulq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtgfofrhjb.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtkukcvrow.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtsdnnhild.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aizwys.cn/gtlrbkvgjr.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gteratsxzv.html


<!-- 参考信息 -->