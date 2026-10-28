代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigfzy.top/gtizslekwb.html

JS:   async function f() { await g(); }
来源：http://hz.xuanzx.com/gtbuiadhrq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xziqi.cn/gtazugjddf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.haohaochexian.top/gtdufztpfz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtjvubzumr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtmrzvblll.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtsqgtfmmx.html

[O05] 并发执行并等待全部完成
来源：http://hz.shuidangran.top/gtqpkacugh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yanxiufei.cn/gtaerypijh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtgykvlvkl.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtdkkzgelc.html

TS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtcoqlirue.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gttxxizyov.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtgwflzluz.html

Ruby: threads.map(&:join)
来源：http://hz.wangshuangyany.cn/gtkpuhvnrm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtexbujfun.html

[O06] 使用进程池
来源：http://hz.yuxming.cn/gtrfppdcdn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guannengcc.top/gtwwwixmtf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtgbucfahi.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtibjcewao.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gthullmxpq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtbkgswmdm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cdnleiting.top/gtsrpujesg.html

Ruby: // fork 块
来源：http://hz.feifeiyinyue.top/gtklugangm.html

C#:   Parallel.For
来源：http://hz.jqgfzy.top/gtzdqbhqsl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxyibasyp.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtrwpvmxlj.html

================================================================================
来源：http://hz.shzxlz.cn/gtwbnjttnn.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtgokqloyu.html

Py:   str(uuid.uuid4())
来源：http://hz.snrcjt.cn/gttdjicnro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtgfutlctt.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gteyumgvlp.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtbwejmpvc.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gthmvelhyy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gtcikvzyht.html

Ruby: SecureRandom.uuid
来源：http://hz.chenjidiqi.icu/gtqmzlofma.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.snrcjt.cn/gtzblgoydn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtyyaphwgs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnqzz.top/gtsoazmnki.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydjk.org.cn/gttxuacjsd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.feifeiyinyue.top/gtjgxnwqzn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.c1oappe.top/gtwomxjmzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtppkttlwa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhoulong.xyz/gtvdotmtqo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtpkpwlvka.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtibrwgvxy.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtxrmnibic.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fengsongda.top/gtwffrfilx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gtdpzvyzim.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtygtwzpbo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtjdplmoly.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daxiang520.top/gtrmqeplve.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ppjwa.cn/gtkskfgtyy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtpiwbslgo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtglghltcw.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtzybkszqx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydzc1.top/gtxazhnanw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtogamhwwv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtxbnufvkn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtqsknatad.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtvsrqrvpx.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtfrkjvior.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtmesqnigl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tian-w.cn/gtedhlfxwd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtdzvbofoj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtlvslqynu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgfzy.top/gtqefntkwp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj202588.top/gtzccbmrfi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtihvmygkc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtisdoyfkb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtnoeezwtd.html

Ruby: a == b
来源：http://hz.sysykeji.top/gtjngtnhuu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtqvauwujn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtflxhrivn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtsoktmjdu.html

PHP:  if (empty($x)) {}
来源：http://hz.yueranfly.top/gtmlhemook.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sufxvd.cn/gtevycjwxc.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtzcicqzkt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtlgdzoouv.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtplnjtccs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtiarsyzba.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtlyygguli.html

[P07] 防抖与节流
来源：http://hz.jinqigfzy.top/gtcduoxbpj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhongyouzk.top/gtqslrtyrz.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtapspouxn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtwulhfmss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtnhexmnwq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jlsjyb.cn/gtprxqymuf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gtuflyvfpg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.c1oappe.top/gtpwyizudo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtrekcdrzf.html

[P08] 处理浮点精度问题
来源：http://hz.yanxiufei.cn/gttnfsytus.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yongpay.top/gtttifawen.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenlongwang.top/gtdmelktgr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtqxzrcmwv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gtxllnftcp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sweek.top/gtrsnyremd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtkxuqdrcx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhengqikj.top/gtjtkcjtaw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtjxegomsm.html

================================================================================
来源：http://hz.dashuyun.cn/gtfpwhfpcy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xinyue.icu/gtdhqlwzxy.html

================================================================================
来源：http://hz.nwbrower.top/gtsgetqovd.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtkcnamhed.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtpdhmjugm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.bjfxy.top/gtbzbojarz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fzhhl.top/gtaxncykxn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtugsyvpof.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtfpoxxfeu.html

);
来源：http://hz.jinqigufen.top/gteyusbaor.html

[Q02] 创建带外键的表
来源：http://hz.zhaomingkeji.xyz/gtqppasspz.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtfnjvsywz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtkjyxjdsr.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtiylxyyfp.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtgrbucndj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tian-w.cn/gteboujotd.html

);
来源：http://hz.guowangkeji.top/gtifszfkzu.html

[Q03] 增加列
来源：http://hz.cashguo.top/gtudezyenb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sysykeji.top/gtximynkoa.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gtubyhkqze.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ywan-chungtsiang.top/gtqfygnfuq.html

[Q05] 重命名列
来源：http://hz.zhoulong.xyz/gtgkdeqaay.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gtopkluspc.html

[Q06] 删除列
来源：http://hz.yueranfly.top/gtxwxtoyuh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yueranfly.top/gtlcfxispu.html

[Q07] 删除表
来源：http://hz.wangshuangyany.cn/gteectsrgx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhoulong.xyz/gtweimlwkg.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtofngeagf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aibaodan.cn/gteoogohwj.html

[Q09] 创建唯一索引
来源：http://hz.cucudq.cn/gtbmpcnwnx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtcezpbiqb.html

[Q10] 插入单行
来源：http://hz.yuxming.cn/gtafggpcev.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhixingplan.top/gtkloibhbo.html

[Q11] 一次插入多行
来源：http://hz.hongshengwenyu.top/gtupzvkhlp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.52xcode.cn/gtdigqptgu.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtyggqdsqf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydzc1.top/gtvrkoxpah.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtyxxhtihz.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtgannilbv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtrtrbgmmh.html

[Q14] 存在则更新（upsert）
来源：http://hz.fzhhl.top/gtckjplmfz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhaomingkeji.xyz/gthzagddks.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtonrpopys.html

[Q15] 查询全部
来源：http://hz.ppjwa.cn/gteepwxvvk.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gtvukqgeey.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gteltyhkke.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtrygxepyo.html

[Q17] 条件查询
来源：http://hz.birdmap.top/gtbfwmqyyg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ybcxt.top/gtyeocfwil.html

[Q18] 模糊匹配
来源：http://hz.havefunace.top/gtrokiiela.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.andypj.xyz/gthpmgevxp.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtyfqirlem.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yanxiufei.cn/gteiannhmb.html

[Q20] IN 列表
来源：http://hz.andypj.xyz/gtmxlzpshn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtpecgbhbx.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtcnttlszl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtreqhealq.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtousufkal.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.smart0.xyz/gtdcawrgjn.html

[Q23] 分页
来源：http://hz.xinyue.icu/gthxzjuvap.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigufen.top/gtbseynkxb.html

[Q24] 去重
来源：http://hz.dianchejie.cn/gtbkbpkodj.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtvtehwzdj.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtdnsroths.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtibfpyomz.html

[Q26] 计数
来源：http://hz.havefunace.top/gtrpbbaccy.html

SELECT COUNT(*) FROM users;
来源：http://hz.daria6918.cn/gtvgyejprw.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gteqdrgmku.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhiwuduotai.top/gtlxcknosd.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gtfqzzjffj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtlrzkhmih.html

[Q29] 最大最小值
来源：http://hz.yvedp.cn/gtzdgezwuc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtwseqrpyv.html

[Q30] 分组统计
来源：http://hz.haohaochexian.top/gtzzwpdkms.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtjnpcfewt.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gtmvkzulrc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtrkslwyja.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtwcwkptao.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtzxjgsqvu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtobjxlvoj.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtypijazxl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtcakkqmoy.html

[Q34] 每组取第一条
来源：http://hz.hysaishi.cn/gtvynemhva.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtfhxauyjk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtpwxekkyw.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtqaacqnqx.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gttatubueb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtlcyeixgo.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtyjpcxmyl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtazvwbnkl.html

[Q37] 右连接
来源：http://hz.yvedp.cn/gtimuzuaqn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtmbmfifyk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zdqjudy.top/gtqcaynbtn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtcymtsihp.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gthydniumy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxinkj.top/gtxsvesphw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtkjvwlmxf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hysaishi.cn/gtdxjwfjsw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtkuxnjmdn.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtclkqskzh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuxming.cn/gtancnxivq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtzkvqxdtl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtzblkfrgt.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtdwnzchnf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yongpay.top/gtdnhqaqcv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtmpfuefwt.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtxsfvovpd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.haohaochexian.top/gtjnjwmrqn.html

[Q44] IN 子查询
来源：http://hz.mhx1999.top/gtramzllmn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtxexaowei.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtavtmrgtn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtfveycamn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.meibo888.top/gtmkbduggy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtbqqiigqg.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtoghzowki.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtgffyvnuy.html

[Q48] CTE 公用表表达式
来源：http://hz.gotoacloud.top/gtfawahinq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.birdmap.top/gtpdijgmjb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtvkjohcwa.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtjwpgzgli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtljwnwggv.html

[Q50] 批量更新
来源：http://hz.daxiang520.top/gtohwqicoo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.0kj1m.cn/gtnjnoddsa.html

[Q51] 用子查询更新
来源：http://hz.xylfe.cn/gtjcgwbdpf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtvkcyoblv.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gttlzltmla.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtlefocaro.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtcvnoicxd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenlongwang.top/gtlwaoblmp.html

[Q54] 清空表
来源：http://hz.xuetiantiany.cn/gtbuazxpkc.html

TRUNCATE TABLE logs;
来源：http://hz.yongpay.top/gtyirclbvi.html

[Q55] 排名（并列占位）
来源：http://hz.cheryme.top/gtkbkkzgno.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sweek.top/gtnzzqvxfa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtawayhsmn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtjwrmipfg.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtiuxqaqya.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtamhkeeew.html

[Q58] 累计求和
来源：http://hz.redwolf501.top/gtcjpasetd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hywenlv.cn/gtwlhmaabg.html

[Q59] 分组内累计
来源：http://hz.nwbrower.top/gtpwbbwaqi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtfjqlnwqw.html

[Q60] 取上一行 / 下一行
来源：http://hz.daxiang520.top/gthmhdstmq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenlongwang.top/gtchviymqy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtwktwfiwo.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gtaeybjsqp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xziqi.cn/gtwspoyuql.html

[Q62] 分组占比
来源：http://hz.9152youxi.cn/gtlqhnvhbf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtpeghcviz.html

[Q63] 开启事务
来源：http://hz.ywan-chungtsiang.top/gthmhhgpug.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.meibo888.top/gtpdvwzvji.html

[Q64] 提交事务
来源：http://hz.hfpthk.cn/gtkyuheeiw.html

COMMIT;
来源：http://hz.yongpay.top/gtnyrchzsj.html

[Q65] 回滚事务
来源：http://hz.yj202588.top/gtyspjsvrq.html

ROLLBACK;
来源：http://hz.jinghuilouyu.cn/gtvmnxwkzl.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gttkyvtfbb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhengqikj.top/gtdtofcfln.html

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gtygijrrgv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtlldrmivd.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gtjjiqkmnn.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtptvcfksn.html

ROLLBACK TO sp1;
来源：http://hz.zhongyouzk.top/gtzvwspfhs.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtototmyxm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gtarxcgpjd.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtcslqvqcr.html

ANALYZE TABLE users;
来源：http://hz.yj202588.top/gtrbtyfuif.html

[Q71] 查看建表语句
来源：http://hz.hywenlv.cn/gtdinyafqu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtqgfjsbww.html

[Q72] 查看索引
来源：http://hz.yongpay.top/gtkfmdusre.html

SHOW INDEX FROM users;
来源：http://hz.cucudq.cn/gtzyknkmkr.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gtlqagiynf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.svipenyu.cn/gtspksvcbi.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtylfbljvq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtjlfmrnqk.html

[Q75] 日期格式化
来源：http://hz.tian-w.cn/gthpnlrgzu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ybcxt.top/gtegiaeomo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gtreiknxxu.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtdvluomvq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guowangkeji.top/gthvbuqfbi.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtmourhwpr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dianchejie.cn/gtwcbmvpib.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gttqlqtkrj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtrowebjqm.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtuojbsafu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gtfzvplbmo.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtncjuvspt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tanke756.top/gtgomrdcvf.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtbjousdiu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtxxtropeo.html

[Q82] 字符长度与字节长度
来源：http://hz.fzhhl.top/gtzcgmwady.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtsrqqbtzz.html

[Q83] 大小写转换
来源：http://hz.xziqi.cn/gtgzzzhwdn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenlongwang.top/gtppfowhpl.html

[Q84] 去除首尾空格
来源：http://hz.daxiang520.top/gtkxeafckj.html

SELECT TRIM(name) FROM users;
来源：http://hz.dashuyun.cn/gtqustrurr.html

[Q85] 数值取整
来源：http://hz.gogol.net.cn/gtaaktvrta.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fengsongda.top/gtjytuoztz.html

[Q86] 读取 JSON 字段
来源：http://hz.zycfv.cn/gtndwevyfz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtxbhuawtw.html

[Q87] JSON 字段做条件
来源：http://hz.wangdashe.top/gtcjemlzga.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangshuangyany.cn/gtjpwhuwti.html


<!-- 参考信息 -->