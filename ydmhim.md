代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtcyypthlm.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtsqvhzuta.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtsexuoadl.html

Py:   async def f():⏎    await g()
来源：http://hz.guannengcc.top/gtlplakqow.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtugalwnem.html

JS:   async function f() { await g(); }
来源：http://hz.cqqwz.cn/gtnvtkfqey.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.9152youxi.cn/gtjqibhadh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gtppsvfjku.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gtxifaltfk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gthtnmfqaz.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gtdroumleg.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtjptouqwu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sysykeji.top/gtpuatcudc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gtntcmpekp.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtphlawmrz.html

TS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtewzyjubx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xziqi.cn/gtodkvwvpg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gtuwzmmnrz.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gttnqivomq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yueranfly.top/gtpwpfcvwg.html

[O06] 使用进程池
来源：http://hz.zhiwuduotai.top/gtsnlqttsh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ivvv.top/gtipajlanw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dianchejie.cn/gtjvgxumpk.html

JS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtwhctqzdq.html

TS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtrfojoevn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtxfkedwwn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gthbxgnbvz.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gthxnodepr.html

C#:   Parallel.For
来源：http://hz.zdqjudy.top/gtpxrzmpes.html

================================================================================
来源：http://hz.9152youxi.cn/gtgodfbrxo.html

P. 常用工具函数
来源：http://hz.havefunace.top/gtfyiagtis.html

================================================================================
来源：http://hz.nwbrower.top/gtrhdbqtdi.html

[P01] 生成 UUID
来源：http://hz.fengsongda.top/gtgghjjoxe.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtcvutocpj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenjidiqi.icu/gtqyyseraa.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtmtagyaox.html

TS:   crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gtkpcuefel.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtqbcxkkfu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuetiantiany.cn/gtajzqvnuk.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtvgiztqag.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtvsoqjwlp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtobpomruo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgfzy.top/gtgwxtwnlk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gttatqwfcw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtcofqfwfj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gthnarjxwr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtqvgrbciw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gtajwaueia.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ppjwa.cn/gtundphrjn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gthewmopmd.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gtpozuustw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jiagoushi.top/gtetwkxril.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jyoumei.cn/gtrvlheycg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtwyuqtafj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtzggoxmay.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtbanwmoza.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtbuafcigl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtlakpssel.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtgsamhkqw.html

[P04] 求长度
来源：http://hz.jianghu66.top/gtiubvakes.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gthrzbfnde.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gtwsrpnvmi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtingnjfhb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtbhrkksuq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtmlfswnvv.html

Go:   len(arr);  len(m)
来源：http://hz.tanke756.top/gtvfjzdxlz.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangkeji.top/gtcafksxlo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhoulong.xyz/gtcksdqtgo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jyoumei.cn/gtzetbayxe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtvmuwepwe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zdqjudy.top/gtwgzocrqu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gteivscvxr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtgieuybkg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtywzbtbqg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtnypcgnbu.html

Ruby: a == b
来源：http://hz.hfpthk.cn/gtngshalvb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtdmgkjilv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.bjfxy.top/gtcmgzcbvr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xylfe.cn/gtafpkkafx.html

PHP:  if (empty($x)) {}
来源：http://hz.havefunace.top/gtqytzyuiu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtfgaimrmh.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtzfdbbuao.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtmbbazbll.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gtqcaxuebk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ywan-chungtsiang.top/gtmthuowjw.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtbcczjabu.html

[P07] 防抖与节流
来源：http://hz.c1oappe.top/gtxfwoyfmv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtndwfyich.html

PHP:  // 手写时间戳比较
来源：http://hz.jiagoushi.top/gtoycsmpgq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtnoqmeukz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtiqwzhmux.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenzaomai.com/gtsaueoilr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yongpay.top/gtjzcjubze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtfvilvkae.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jiagoushi.top/gtjoqzbqtx.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtjffiigau.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtslpwpdzj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yvedp.cn/gtsozdyzvs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtwvgflugd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtwbcniujh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtodwydoma.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtkmsxuisy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhijiandao.cn/gthcbhttiv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cdnleiting.top/gtkolesrbt.html

================================================================================
来源：http://hz.yj20258.top/gtdakfutam.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jlsjyb.cn/gtcmvzbdjr.html

================================================================================
来源：http://hz.sysykeji.top/gthbagiewf.html

[Q01] 创建表
来源：http://hz.cheryme.top/gtkzajidhu.html

CREATE TABLE users (
来源：http://hz.zhengqikj.top/gtnjbibrvn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gtwqhctefh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtazwhutmy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtdayznwjy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtdfjdlvsf.html

);
来源：http://hz.hongshengwenyu.top/gtchjynxwx.html

[Q02] 创建带外键的表
来源：http://hz.yueranfly.top/gtijzwfjas.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtjwswilhz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtuhdnqgvk.html

user_id INT NOT NULL,
来源：http://hz.chenjidiqi.icu/gtxzafkllm.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangtech.top/gtmdfmaxog.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ivvv.top/gtwbwfdmzw.html

);
来源：http://hz.xylfe.cn/gtxicnijol.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtyvnwwlpu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtxnmmdvmc.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gthjzoefds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtifadpggt.html

[Q05] 重命名列
来源：http://hz.yj202588.top/gtdgukpinm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtapnmjdph.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtdrhmutit.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenlongwang.top/gtwhqgauxq.html

[Q07] 删除表
来源：http://hz.9152youxi.cn/gtzdfwuurq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xylfe.cn/gtgzsdbnym.html

[Q08] 创建普通索引
来源：http://hz.hongshengwenyu.top/gtbrtusbne.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtfpidzthk.html

[Q09] 创建唯一索引
来源：http://hz.jianghu66.top/gtjgbuaxhc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtmjxwniom.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtavmivrqx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gtlufhtywe.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtuabvhjmb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtvcsenxcc.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtdgovibcc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangkeji.top/gtpmbreyyv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258.top/gtvzixptws.html

[Q13] 忽略重复插入
来源：http://hz.jlsjyb.cn/gtqjicimwz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtcmwtumxd.html

[Q14] 存在则更新（upsert）
来源：http://hz.haohaochexian.top/gtnkmnxhsb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tian-w.cn/gtscmqbhqr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtufarkjlb.html

[Q15] 查询全部
来源：http://hz.quarkkingdee.top/gtqkvhwytg.html

SELECT * FROM users;
来源：http://hz.aizwys.cn/gtoayvmvjl.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gtcdbmqgcy.html

SELECT id, name FROM users;
来源：http://hz.sufxvd.cn/gtmojllsnw.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtyqijvluv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gogol.net.cn/gtinxscotn.html

[Q18] 模糊匹配
来源：http://hz.redwolf501.top/gtyenvjeom.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtzolztooi.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gtpzagqpls.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gttosmxedr.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtigjnohhj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guowangkeji.top/gtvjedatpx.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gtgvzblggs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yvedp.cn/gtynqweben.html

[Q22] 排序
来源：http://hz.gogol.net.cn/gtxvuzwsxe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhiwuduotai.top/gtotkohctw.html

[Q23] 分页
来源：http://hz.sxryk.cn/gthejfzlfu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtduvithhc.html

[Q24] 去重
来源：http://hz.dianchejie.cn/gtszhrtlwi.html

SELECT DISTINCT city FROM users;
来源：http://hz.dashuyun.cn/gtnrruhtgf.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gtynhrrtdd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtveaosdwh.html

[Q26] 计数
来源：http://hz.yj20258.top/gtqqtymkda.html

SELECT COUNT(*) FROM users;
来源：http://hz.jiagoushi.top/gtonrtcvtr.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtovqetaja.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtlokfbsus.html

[Q28] 求和与平均
来源：http://hz.hongshengwenyu.top/gtjgiybdrb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangtech.top/gttbiqcwfm.html

[Q29] 最大最小值
来源：http://hz.jinqigfzy.top/gtsntgnuew.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gtgxoqlrus.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtcjowahgt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtifvafzsp.html

[Q31] 分组后过滤
来源：http://hz.0kj1m.cn/gtervineuq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gthywdbxne.html

[Q32] 分组拼接字符串
来源：http://hz.sufxvd.cn/gtpheymizm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtajhwmyan.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtuijciswf.html

[Q33] 多列分组
来源：http://hz.ydjk.org.cn/gteumaihrl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nwbrower.top/gthtaoohfa.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtsuvleziq.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtwwarwpnb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuetiantiany.cn/gtpixhhtxg.html

) t WHERE rn = 1;
来源：http://hz.gogol.net.cn/gtmcsiqfql.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtczzvqvvb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtayewsmve.html

[Q36] 左连接
来源：http://hz.jinyuanbaomall.cn/gtgjbnfesq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtgnyltplq.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtzwyiyfiu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gthblqxjij.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj202588.top/gtemwyhcyz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtlwjblrik.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtcmzdycjr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yonumen.top/gtrjnioqkz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtpksncizb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtdmrvmpsk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtogtctmfz.html

[Q41] 多表连接
来源：http://hz.bjfxy.top/gtpuzwshkj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtvqejfhhr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydjk.org.cn/gtxltuptgj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cdnleiting.top/gtivcugzeo.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtszlierau.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yonumen.top/gtpelnhvdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtxnpzqaeb.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gtiwaefunz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtzhnonded.html

[Q44] IN 子查询
来源：http://hz.tian-w.cn/gtdeomufdn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtwipboxfp.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxuanxn.top/gtnsvshnfv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtkkabhpdx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.bjfxy.top/gtbhgisewy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtlwgvsbhp.html

[Q47] 与平均值比较
来源：http://hz.xziqi.cn/gtckjdcdcu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sxryk.cn/gtyktnpgtm.html

[Q48] CTE 公用表表达式
来源：http://hz.yangfankeji.com/gtvgwziers.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtvmnyvohp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtyqbywmlv.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtntxwcbti.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtabaaqpky.html

[Q50] 批量更新
来源：http://hz.jqgufenzy.top/gtjsbnscgo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtyzrzgbfc.html

[Q51] 用子查询更新
来源：http://hz.ywan-chungtsiang.top/gtcgwsqari.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtqgvannon.html

[Q52] 删除指定行
来源：http://hz.shangyingyoupin.top/gtauxerbkd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtvybstamr.html

[Q53] 按条件删除
来源：http://hz.jqgfzy.top/gtfssevyvw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gtkicejxpu.html

[Q54] 清空表
来源：http://hz.yj20258888.top/gtpmeuwmme.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtqydwpoxd.html

[Q55] 排名（并列占位）
来源：http://hz.zhaomingkeji.xyz/gthyfafxjy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.smart0.xyz/gtshfpljgq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258.top/gtdhbnjbzy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtjkkwzugs.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtqvrmqbru.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtunwnvhxr.html

[Q58] 累计求和
来源：http://hz.cucudq.cn/gtawcroiac.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtgkfovwqv.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gthjjyxqji.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtelameyqu.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnxiangtu.top/gtwsrmfqvx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hammf.cn/gtdjzajzqd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tianlin.xyz/gtjwpxncqz.html

[Q61] 移动平均
来源：http://hz.gogol.net.cn/gtjrvnyqvu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtyntjqdwj.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gtbpqhimtp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtdqzamhil.html

[Q63] 开启事务
来源：http://hz.hysaishi.cn/gttucihvhd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gogol.net.cn/gtnhjvzobk.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtgrdipccs.html

COMMIT;
来源：http://hz.svipenyu.cn/gtbnmouefw.html

[Q65] 回滚事务
来源：http://hz.ydjk.org.cn/gthukropgp.html

ROLLBACK;
来源：http://hz.hnxiangtu.top/gtqwergnfu.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtodpxufac.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jlsjyb.cn/gtzotgowng.html

[Q67] 设置隔离级别
来源：http://hz.guannengcc.top/gttxczjcae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtotwvgifz.html

[Q68] 保存点
来源：http://hz.jlsjyb.cn/gtudqiwpgy.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gtfanajvea.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtprbwccdi.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gtaxnumaqz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aibaodan.cn/gtswvyzmfq.html

[Q70] 更新统计信息
来源：http://hz.pengpengdd.cyou/gtponxnisc.html

ANALYZE TABLE users;
来源：http://hz.gotoacloud.top/gtfdanaize.html

[Q71] 查看建表语句
来源：http://hz.chenjidiqi.icu/gtkwgrrxfl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtresvvqvv.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtrrhstoba.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtwpxoacol.html

[Q73] 查看表状态
来源：http://hz.sweek.top/gtlppzjcpj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtavoycpjb.html

[Q74] 强制使用索引
来源：http://hz.nanxuanxn.top/gtryfjkjpv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtnuxgtpyj.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtnsescfqi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtjobfcaet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtlwhoxmvm.html

[Q76] 按天统计
来源：http://hz.cdnleiting.top/gtkxylndxc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtvhpzbsrc.html

[Q77] 时间加减
来源：http://hz.kuanghao11.cn/gtjobcwtpx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.kuanghao11.cn/gtottpopsa.html

[Q78] 当前时间
来源：http://hz.guannengcc.top/gtggnsxkzd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zycfv.cn/gtsmcdexoq.html

[Q79] 字符串拼接
来源：http://hz.zhixingplan.top/gtszasaois.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtlpuuxvxz.html

[Q80] 字符串截取
来源：http://hz.ydzc1.top/gtxsmjwlgi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gthbmnflhv.html

[Q81] 字符串替换
来源：http://hz.c1oappe.top/gtpzgtgmrh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ivvv.top/gtoflzqdjz.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258888.top/gtbhtycipg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtnsolwxeq.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtyfemmumz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangdashe.top/gttjsdjhjk.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtzmzdtmrm.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258.top/gtshrjsgyc.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtjaprypex.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtgjqohnkm.html


<!-- 参考信息 -->