代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtwfnlrmwf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhijiandao.cn/gtdsnjpnel.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gturtnsqjn.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtpbcspbdf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtxnpzgxzl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtiukxpwsr.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtuzabyvlp.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtjrfhvyuo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuanzhike.top/gtdlglpxxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ivvv.top/gtjlwwqnyd.html

Ruby: threads.map(&:join)
来源：http://hz.jiagoushi.top/gtssesibps.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtrafgirbr.html

[O06] 使用进程池
来源：http://hz.52xcode.cn/gtrfnodrmv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtyjrwyepj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258.top/gtpomkldrh.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtdrduuebf.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtucvqduox.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gtuzzktnyr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hongshengwenyu.top/gtvtskvpvl.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtikbuhgyn.html

C#:   Parallel.For
来源：http://hz.jyoumei.cn/gtfyzxgjdx.html

================================================================================
来源：http://hz.sufxvd.cn/gtclrjuypr.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtxnflhwpe.html

================================================================================
来源：http://hz.shuidangran.top/gtclmkxffd.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtzcnovfgq.html

Py:   str(uuid.uuid4())
来源：http://hz.zhijiandao.cn/gtjwwunwhn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtyguoldyp.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtajzvgjqt.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtxvjotgew.html

Java: UUID.randomUUID().toString()
来源：http://hz.hammf.cn/gtkakekgnv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtwyvpgyct.html

Ruby: SecureRandom.uuid
来源：http://hz.jinghuilouyu.cn/gtujpwuxwh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gtlkkkubtl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtwbwdyntv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtlblrzfkh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sxryk.cn/gtaxdzdqwm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtowhttejn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gteevpvwsh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gtxtxathkv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hongshengwenyu.top/gteqspxrda.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtjjffheit.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ivvv.top/gtcvxpqnic.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtwjwqtcjz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hammf.cn/gtyzyylpve.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dianchejie.cn/gtrdlsqxfg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtdaamiiqd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtauuusezh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhongyouzk.top/gtgdoezbva.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydzc1.top/gtcvgtxkvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtqlltofps.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtlwehsklb.html

[P04] 求长度
来源：http://hz.tanke756.top/gtzvccjnst.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pengpengdd.cyou/gtwosspcpy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtljghankx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtbwymdkjp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gteygpcznv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cdnleiting.top/gttsdsssaw.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtgvhljbqi.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gtdfydimow.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.9152youxi.cn/gtgymbegpc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cheryme.top/gtsnxauvle.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtzdvitllk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gteablkcms.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtfncsnpay.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtfzgstykp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtapopvjfd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtqwnoeeto.html

Ruby: a == b
来源：http://hz.c1oappe.top/gtxvehawkm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtcxadvgiz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.316326.xyz/gtiaoakrno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gtnfsqiqvq.html

PHP:  if (empty($x)) {}
来源：http://hz.sysykeji.top/gtpqtbdxwl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuanzx.com/gtjayejume.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gtairrgsrt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtryidfaic.html

Go:   if x == nil {}
来源：http://hz.wangshuangyany.cn/gtjjboqgib.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtdnwsgeev.html

C#:   if (x is null) {}
来源：http://hz.fzhhl.top/gtsngovrud.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtsqgoisqy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydzc1.top/gtorxovwof.html

PHP:  // 手写时间戳比较
来源：http://hz.xuetiantiany.cn/gtownzuayi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtteaeanoj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtjmqyhsds.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtpnowjdhq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cucudq.cn/gtiwvceiky.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenlongwang.top/gtzkxjxtck.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtwsiemmsw.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtzftubjnu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gthaylrbud.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gttdkkxqmt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shangyingyoupin.top/gtlmenskwh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gthdwtgvtf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cashguo.top/gtdlpjltkp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtbckejfft.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtgbrhefoz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gtfztkhibk.html

================================================================================
来源：http://hz.shzxlz.cn/gtyfjebumw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtreucmqrx.html

================================================================================
来源：http://hz.nwbrower.top/gtsdlzbhgk.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtainaztxc.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtmstydjxm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtnnxtbiml.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jianghu66.top/gthapmrudm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.meibo888.top/gtchlxgske.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gzhubu.top/gtzsasipar.html

);
来源：http://hz.guowangkeji.top/gtbvcvatov.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtshlhgjwv.html

CREATE TABLE orders (
来源：http://hz.jinqigfzy.top/gtqaxmfezf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtwafnfrwu.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gtlvcctevo.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtbgjverfg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtfoojbvav.html

);
来源：http://hz.xuanzx.com/gtxnqqdixe.html

[Q03] 增加列
来源：http://hz.cashguo.top/gtpswqqwjw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtegsyoyhb.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gtqcevvczr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.svipenyu.cn/gtawdsvogh.html

[Q05] 重命名列
来源：http://hz.guowangkeji.top/gtwdbennou.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtpvmcvnnj.html

[Q06] 删除列
来源：http://hz.xziqi.cn/gtgdbcplsq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtwnsvxkwv.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtndjdelqy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtckwowxlg.html

[Q08] 创建普通索引
来源：http://hz.dashuyun.cn/gtpjbmvkjs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtiigjbsdg.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtnltujlcm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pycfn.com/gthyunajbd.html

[Q10] 插入单行
来源：http://hz.birdmap.top/gtucmdsogi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtejvxgund.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtjoxnbzyj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sufxvd.cn/gtrkbvmuom.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gttyokvfmj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gtjrqhckvu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xziqi.cn/gtaywrfqre.html

[Q13] 忽略重复插入
来源：http://hz.guowangkeji.top/gtbsmgsypu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dashuyun.cn/gtzkfyfkxx.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtfwxbwwvm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pycfn.com/gtcmksqwvg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtjcimllji.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtehmpzgrf.html

SELECT * FROM users;
来源：http://hz.tanke756.top/gtkrelnxlw.html

[Q16] 查询指定列
来源：http://hz.haohaochexian.top/gtfhmysmev.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtxlitblty.html

[Q17] 条件查询
来源：http://hz.shuidangran.top/gtieynqzuq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtfnukldmj.html

[Q18] 模糊匹配
来源：http://hz.chenjidiqi.icu/gtatwtuhpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ybcxt.top/gtzrgqkvtc.html

[Q19] 范围查询
来源：http://hz.shanyushiyangkeji.top/gtosgzinru.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhijiandao.cn/gtvwptjjrl.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtuddvyjay.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gtelfvkjfe.html

[Q21] 空值判断
来源：http://hz.yueranfly.top/gtyrfjqejj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jyoumei.cn/gtukvvrfyn.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtdkbqupfk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aibaodan.cn/gtsjiohmya.html

[Q23] 分页
来源：http://hz.dianchejie.cn/gtbmogitoo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gttvjphqxt.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtgcwmtzqw.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gttfxuwkuz.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtkvfyhvri.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgfzy.top/gtixgannsx.html

[Q26] 计数
来源：http://hz.cheryme.top/gtsrsaxxmk.html

SELECT COUNT(*) FROM users;
来源：http://hz.hongshengwenyu.top/gtimfpdccq.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gtxxytlmvp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtluffpxrb.html

[Q28] 求和与平均
来源：http://hz.haohaochexian.top/gtrozrlzah.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhixingplan.top/gtyxdpecxi.html

[Q29] 最大最小值
来源：http://hz.zdqjudy.top/gtuamjoqef.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zycfv.cn/gtxywwiysi.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtlvbifryn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtedzxtvrg.html

[Q31] 分组后过滤
来源：http://hz.cheryme.top/gtkughrbkr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtoftwqcaw.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtnywciocp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtrkzwiahg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtjzxmjlft.html

[Q33] 多列分组
来源：http://hz.xingfuxueyuan.xyz/gtgpzadfaa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtcrkzvhbr.html

[Q34] 每组取第一条
来源：http://hz.sweek.top/gtycdfpgul.html

SELECT * FROM (
来源：http://hz.zhoulong.xyz/gtkjlzviwc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gzhubu.top/gtbezcfhtq.html

) t WHERE rn = 1;
来源：http://hz.dianchejie.cn/gtbvemghin.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtxoputbdz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtbjxbwfwb.html

[Q36] 左连接
来源：http://hz.redwolf501.top/gtnstfcnqv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtdqfoovmu.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtdayswupl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtyymoooms.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtfdqbxprg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jianghu66.top/gtogsmakab.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtvzgixbjj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258888.top/gtwefjquux.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cdnleiting.top/gtlfminfge.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ivvv.top/gtiqjszsgf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gtfdjhynlv.html

[Q41] 多表连接
来源：http://hz.vqdsnc.cn/gtzvspvtrc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtamraomkz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuetiantiany.cn/gtzycflqfd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtaoflgwni.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtmamlwkms.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuetiantiany.cn/gtdupcskai.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guannengcc.top/gteiebevfn.html

[Q43] 标量子查询
来源：http://hz.9152youxi.cn/gtgndclgoc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtzfsbxquc.html

[Q44] IN 子查询
来源：http://hz.havefunace.top/gtrwksnmfx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtbkxgxhwa.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtcflkkeua.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtbcmjdffu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtblakvqeh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtmhwkflzl.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtwwqfatvm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtywpmjjbb.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtoehkuthr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtbtuoxtby.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sufxvd.cn/gtvmxsqxwn.html

[Q49] 更新单行
来源：http://hz.feifeiyinyue.top/gtotlqijey.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtynfpekmj.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtmisdpcvj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gttimywyek.html

[Q51] 用子查询更新
来源：http://hz.hammf.cn/gtuntskrjj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.birdmap.top/gtykhspnzs.html

[Q52] 删除指定行
来源：http://hz.hnxiangtu.top/gtcatjwsme.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shzxlz.cn/gtuuiynhkr.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gttxtfzfqw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtjjoxbywk.html

[Q54] 清空表
来源：http://hz.vqdsnc.cn/gtgdotkvvh.html

TRUNCATE TABLE logs;
来源：http://hz.zhaomingkeji.xyz/gtobwgxkiz.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gtbyvxvpci.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgfzy.top/gtojoufyjf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.mhx1999.top/gtnimjlrux.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenzaomai.com/gtitzniswa.html

[Q57] 行号
来源：http://hz.yj20258888.top/gtydvpqdic.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.bjfxy.top/gtnwlenpcl.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtfcprbwve.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtzxnrhkpz.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtkyonbwhj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gteytfrktk.html

[Q60] 取上一行 / 下一行
来源：http://hz.yonumen.top/gtllyfcksi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xziqi.cn/gtffuptmlm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ivvv.top/gtkzijmdmg.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtrgqrgmbk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtqpcjeogy.html

[Q62] 分组占比
来源：http://hz.aibaodan.cn/gtkitjrjrd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtazsgadqr.html

[Q63] 开启事务
来源：http://hz.xingfuxueyuan.xyz/gtmsaqnogr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtapoqjoao.html

[Q64] 提交事务
来源：http://hz.aibaodan.cn/gtomhfqncf.html

COMMIT;
来源：http://hz.hywenlv.cn/gtqekrfkhx.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtfaabjfrt.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtcgipzaeu.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gtyafjqtrz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtddegiqna.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtozwwngfa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yonumen.top/gtbwmybzia.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gtmupthkwv.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtfmvkpeii.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtzxwzznip.html

[Q69] 查看执行计划
来源：http://hz.xuanzx.com/gtgjmugfft.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.guannengcc.top/gtdehsfzzm.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gttdjjnvpz.html

ANALYZE TABLE users;
来源：http://hz.cdnleiting.top/gtkmekhpal.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtaldanepe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtkkmuhavp.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gtxavhfomi.html

SHOW INDEX FROM users;
来源：http://hz.zhijiandao.cn/gtjyofjier.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtencubcnv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtaoabfzge.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gtxgxwixci.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daxiang520.top/gtzfjluivj.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtjbtxdtky.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtcupfyoth.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnxiangtu.top/gtbujoqwhd.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gteocducoq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gtdbfplscp.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtisckxtgv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtainppywv.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtjieqyhkl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gtwjyjtmdu.html

[Q79] 字符串拼接
来源：http://hz.zhengqikj.top/gtwswjysyp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yongpay.top/gtpjypzpdi.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gtwrqfnuoi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtjkivrlpn.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtafnvjocd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinqigufen.top/gtzyphgbjc.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtdszghkpr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtxjclmyqi.html

[Q83] 大小写转换
来源：http://hz.zhengqikj.top/gtvzmwrmom.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtpxappcga.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtqupcahwg.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gthszcxgqf.html

[Q85] 数值取整
来源：http://hz.52xcode.cn/gtjeeqhkih.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ehwqpu.com/gtpkjrggtu.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtejmodeca.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtgeotarxv.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtmppmkemm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ivvv.top/gtcjldoxxj.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gtrmrrogtd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xingfuxueyuan.xyz/gtsimnwvuz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gtzuvhmcfe.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtyonkpier.html


<!-- 参考信息 -->