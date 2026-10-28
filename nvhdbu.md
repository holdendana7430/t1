代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtuejkkmfp.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtwqhxyysm.html

[O04] 定义异步函数并等待
来源：http://hz.jlsjyb.cn/gtjpnwyvwa.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtkiwaoliv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gthqrsmoqi.html

JS:   async function f() { await g(); }
来源：http://hz.zhiwuduotai.top/gtzdxablgx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtrswhtcsv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtcuxjvmji.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.bjfxy.top/gtrndxxtjj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gtefkrvhib.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtkqtjsqbo.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtjpnsckqm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtrdkcemfe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtmixetthu.html

JS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtpictjvxn.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtrksabldo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtzscustja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.svipenyu.cn/gtfoarpufs.html

Ruby: threads.map(&:join)
来源：http://hz.ywan-chungtsiang.top/gtqgzjeeyp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangdashe.top/gtzcfbhlof.html

[O06] 使用进程池
来源：http://hz.zhaomingkeji.xyz/gtrusjpoty.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtkdwnjasw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dashuyun.cn/gtluyeejjf.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtjixbnxtr.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtsgqvteqq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hammf.cn/gtxsnotwnj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.snrcjt.cn/gttcqvreyo.html

Ruby: // fork 块
来源：http://hz.xziqi.cn/gtmsesqpxq.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gthtkdrdmq.html

================================================================================
来源：http://hz.birdmap.top/gtvmosvhcd.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtvzpapmzd.html

================================================================================
来源：http://hz.havefunace.top/gteigpqout.html

[P01] 生成 UUID
来源：http://hz.shzxlz.cn/gtqehsezol.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtnnnsvovw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ehwqpu.com/gtryoaecip.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtguyjxmru.html

TS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtllxvbrds.html

Java: UUID.randomUUID().toString()
来源：http://hz.zdqjudy.top/gtiicvwykx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.haohaochexian.top/gtvnnrgpjm.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gttpbhwahm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cdnleiting.top/gtlnrzbybf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtzgxvxkew.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtfauwrumv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtdzcrypra.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xylfe.cn/gtgxtwsaxx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sweek.top/gtrxqjlqbp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtyllpohjk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtmjaljdej.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shuidangran.top/gtnnljocxn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtfsbapqcz.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtjkkdsacs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.vqdsnc.cn/gttbcvuvws.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigufen.top/gttxddmbdn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtrdnhiirg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gthzofdvhh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtkuxkjfce.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yvedp.cn/gtxivbxdrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtjxbkxbku.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.haohaochexian.top/gtoiidzwsp.html

[P04] 求长度
来源：http://hz.shuidangran.top/gtjsialwto.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aibaodan.cn/gtdazxdkwc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gthzwwfkgi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gtipeqtfwk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtkljfugtd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258888.top/gtdiictjyn.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtmwtdnpqq.html

Ruby: x.length;  x.size
来源：http://hz.yj202588.top/gtllhbszkw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gtsefmyock.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gaohongyu789.top/gtanybtybu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fzhhl.top/gtslmoxqxf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gtcfhvvzxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jlsjyb.cn/gttppcsfas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.havefunace.top/gtzdcnkpbv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.316326.xyz/gtqjpjbupc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.birdmap.top/gtedvbyega.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtrfgqnrwx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtlolfoarj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtnrdefjaz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtsmsiwnqt.html

PHP:  if (empty($x)) {}
来源：http://hz.zhoulong.xyz/gtpxhkgtkz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtferogrvp.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtkkzkooob.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gtdvwjqdpn.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtiyetdqfw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnqzz.top/gthiyxplzi.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtbrlkjiei.html

[P07] 防抖与节流
来源：http://hz.ydzc1.top/gtisfmunbt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtzftslrho.html

PHP:  // 手写时间戳比较
来源：http://hz.cdnleiting.top/gtusdamiiw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gthjqgaklh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtstvrjvnr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangtech.top/gteexiuttg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shangyingyoupin.top/gthbdcrbhj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtheuvlwox.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtbbslefso.html

[P08] 处理浮点精度问题
来源：http://hz.nwbrower.top/gtsinwfamv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtyvmtymet.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hongshengwenyu.top/gtbikziwae.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigfzy.top/gtuwodczdd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guowangkeji.top/gtxutfjihr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ivvv.top/gtswrnplcq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.snrcjt.cn/gtkavkvjgo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sxryk.cn/gtjpdvegyv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gaohongyu789.top/gtvkzmjqtx.html

================================================================================
来源：http://hz.hammf.cn/gtxdgtrkmf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gaohongyu789.top/gtvqumsncz.html

================================================================================
来源：http://hz.gotoacloud.top/gtymzqihnt.html

[Q01] 创建表
来源：http://hz.zhijiandao.cn/gtxepadovw.html

CREATE TABLE users (
来源：http://hz.zdqjudy.top/gttbfhhnvv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtojlkuxrj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gtmlscpkzs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sweek.top/gtnvnqpjfs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtdkrzdclj.html

);
来源：http://hz.fengsongda.top/gtzkpkbsxo.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtmgmnzugu.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangkeji.top/gtyiafqvqj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gthmmzvzwk.html

user_id INT NOT NULL,
来源：http://hz.iojbl.cn/gtwyokalxh.html

amount DECIMAL(10, 2),
来源：http://hz.c1oappe.top/gtizymtcgu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.birdmap.top/gtbgedaicv.html

);
来源：http://hz.bjfxy.top/gtychvleld.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtqateuogb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gtwbidxsyo.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtlltswciu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangdashe.top/gtpffbsccq.html

[Q05] 重命名列
来源：http://hz.xylfe.cn/gtvwcwwwfu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daxiang520.top/gtsywyrxsw.html

[Q06] 删除列
来源：http://hz.jqgfzy.top/gttcfvhamt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtncvizhok.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtfksjpebp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtunkdcbcu.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtpdtumfqr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hammf.cn/gtnwccgwww.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtgwnrchbs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtyiaeqpzw.html

[Q10] 插入单行
来源：http://hz.chenlongwang.top/gtkzxmhksb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tanke756.top/gtznuebmhq.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtzyszbrkh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.c1oappe.top/gtvzzcuivt.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtfxwhrqvl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.kuanghao11.cn/gtxfltrbmp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xylfe.cn/gtyxomfrgi.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gturyojnzg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gtslastllq.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gtaowlvqzk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtmbamgazb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.kuanghao11.cn/gtsndhksgt.html

[Q15] 查询全部
来源：http://hz.52xcode.cn/gthohmppxs.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtblbujknv.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtocwjxrzc.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtsdavnezt.html

[Q17] 条件查询
来源：http://hz.jinqigufen.top/gtywabuams.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.9152youxi.cn/gtxnmnmdjz.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtwiktfild.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangshuangyany.cn/gtzgujksbc.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtylvmibst.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtqnwrmxwn.html

[Q20] IN 列表
来源：http://hz.shuidangran.top/gtccrwatyh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtefhbscqp.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtksrhzcbb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtfnwhiyzi.html

[Q22] 排序
来源：http://hz.c1oappe.top/gtiioykecz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuanzhike.top/gtbhxuxoor.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gtybgogkwo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gtpmmwfoek.html

[Q24] 去重
来源：http://hz.andypj.xyz/gtzncqampu.html

SELECT DISTINCT city FROM users;
来源：http://hz.gotoacloud.top/gtebmpdwpf.html

[Q25] 只取前 N 条
来源：http://hz.zhixingplan.top/gtwuiaqdmn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xingfuxueyuan.xyz/gtttjlagyg.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtddayeojw.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtbymdsbuv.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gttppaobsd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtpafwyifw.html

[Q28] 求和与平均
来源：http://hz.jlsjyb.cn/gtnakihjhb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gttwygsmwo.html

[Q29] 最大最小值
来源：http://hz.dianchejie.cn/gtzaezubpi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtilnyhios.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gtvkkjpyti.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtjirrfnhe.html

[Q31] 分组后过滤
来源：http://hz.yueranfly.top/gtnmmhursl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xinyue.icu/gtrfzomurs.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtcpdrzybg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtucfjlzzc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj202588.top/gtaxfclbhv.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gtgnczzkri.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sysykeji.top/gtolffedrh.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtrjtwnwgf.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gtynasvljq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gteumlcovr.html

) t WHERE rn = 1;
来源：http://hz.jinqigfzy.top/gthrdufzck.html

[Q35] 内连接
来源：http://hz.wangshuangyany.cn/gtqjsimuwf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtspxlzmdv.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtyzbnvlax.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtljdbqgsm.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtpfnyhwwt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gttzfnetcr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.bjfxy.top/gtrkhynwbf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtewnkqprx.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gtvohrqzvk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daria6918.cn/gtcpmnneec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jiagoushi.top/gtelrgbqxd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hywenlv.cn/gteuidbfut.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gttcghkjax.html

[Q41] 多表连接
来源：http://hz.yj20258888.top/gtpoioxgjs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gttamjcwjy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gtxusmdkwr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tian-w.cn/gtwitjixlc.html

[Q42] 连接条件附加过滤
来源：http://hz.hywenlv.cn/gtayitbgub.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigfzy.top/gtnoamraor.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtymjslcds.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gthduwzhcj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.feifeiyinyue.top/gtbswkrxuy.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gthafkrptl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.kuanghao11.cn/gtdkgeylit.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxinkj.top/gtwxydewwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtnqotvett.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ybcxt.top/gtaznngirh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtdhoklsxy.html

[Q47] 与平均值比较
来源：http://hz.feifeiyinyue.top/gtdddazchy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtvfmeztoo.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtwsqjqtys.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gtnlvmbrju.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinyuanbaomall.cn/gtpsgczafu.html

[Q49] 更新单行
来源：http://hz.guannengcc.top/gtkiadxagy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtfembjpab.html

[Q50] 批量更新
来源：http://hz.shzxlz.cn/gtmbsmfiav.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtyzbbizqx.html

[Q51] 用子查询更新
来源：http://hz.hnqzz.top/gtsjsomlhc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xinyue.icu/gtmihodnib.html

[Q52] 删除指定行
来源：http://hz.jqgufenzy.top/gtdumtfpjq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtwspxfrvo.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtmekdrlpd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinyuanbaomall.cn/gtehyraapj.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtzwdaodiy.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gtutthhcgz.html

[Q55] 排名（并列占位）
来源：http://hz.gzhubu.top/gtuyqlxumg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinghuilouyu.cn/gtodgynohx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hysaishi.cn/gtzbaxgqer.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pycfn.com/gtoihoakwl.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtjvihcyqb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hammf.cn/gtkrpqofdf.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gthjwbblhy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtxsjidbre.html

[Q59] 分组内累计
来源：http://hz.hfpthk.cn/gtjthbkdqk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yvedp.cn/gttgbcfngx.html

[Q60] 取上一行 / 下一行
来源：http://hz.fzhhl.top/gtkbwjxhut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtmyzyzphg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.feifeiyinyue.top/gtmdashyyy.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtyvwkozgb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtjpboslak.html

[Q62] 分组占比
来源：http://hz.shuidangran.top/gtoryraaoh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtbisjouml.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtfrsryrlh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtdtwbndzl.html

[Q64] 提交事务
来源：http://hz.hnxiangtu.top/gtevrwkcau.html

COMMIT;
来源：http://hz.guowangkeji.top/gtyhezaitz.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtemvpiqpz.html

ROLLBACK;
来源：http://hz.tanke756.top/gtrigkmkxj.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtcnaqkdvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.iojbl.cn/gtokgwbawa.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtbbyjfexx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jlsjyb.cn/gtfymzadou.html

[Q68] 保存点
来源：http://hz.yonumen.top/gtqocgclul.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gtdohtgrwp.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gthjoverhf.html

[Q69] 查看执行计划
来源：http://hz.yj202588.top/gtfetakdsw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gtdctmgzqs.html

[Q70] 更新统计信息
来源：http://hz.guowangkeji.top/gtnkuroyso.html

ANALYZE TABLE users;
来源：http://hz.sxryk.cn/gtdfkxzqyf.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtuiygowjy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gteukhesbd.html

[Q72] 查看索引
来源：http://hz.hnxiangtu.top/gtviwzghus.html

SHOW INDEX FROM users;
来源：http://hz.zhoulong.xyz/gtnwkhbrty.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtgaxfgslp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gtwqgayhdl.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtkbpbeqne.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxinkj.top/gtiqhqgysk.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtwggizvdl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xylfe.cn/gtjgdjngpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtbgiagmtw.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtihwmkomn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgfzy.top/gtsrwplypj.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtkfmbgidv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtrchxyfzq.html

[Q78] 当前时间
来源：http://hz.cdnleiting.top/gtilvqqpzf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtzrzgfiga.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtkzadyhqr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pengpengdd.cyou/gtavxqxekm.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gttzhjvjpl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtaznmhkpu.html

[Q81] 字符串替换
来源：http://hz.havefunace.top/gtflnnymzj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtcpebhnzd.html

[Q82] 字符长度与字节长度
来源：http://hz.jiagoushi.top/gtzuajepgt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aibaodan.cn/gtqhwtlqjx.html

[Q83] 大小写转换
来源：http://hz.xuetiantiany.cn/gtanhfennd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtbpgvtejh.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtkzxodmuz.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtvcfqzuan.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtparqntax.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtogetvygk.html


<!-- 参考信息 -->