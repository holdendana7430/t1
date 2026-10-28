代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtluyedoym.html

[O03] 加锁保护共享数据
来源：http://hz.ehwqpu.com/gtwrvfcmxz.html

Py:   with lock: shared += 1
来源：http://hz.jyoumei.cn/gtyyataqsi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yongpay.top/gtdryglftv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gtctrvywju.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtkyzsrzhy.html

Java: synchronized (this) { shared++; }
来源：http://hz.yanxiufei.cn/gtckncyshc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gtzhuvhjrl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtnbouqcbx.html

C#:   lock (gate) { shared++; }
来源：http://hz.zdqjudy.top/gtsvhjsydg.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtkpsbvkpd.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtjxpvnszu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtjoutsfoy.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gteqzflxsr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gtcidiiqwz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtlcknlpft.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.52xcode.cn/gtrieunevv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtgteosiml.html

C#:   async Task F() { await G(); }
来源：http://hz.xingfuxueyuan.xyz/gtulhodcbo.html

[O05] 并发执行并等待全部完成
来源：http://hz.cashguo.top/gtkbggkjzl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.mhx1999.top/gtwfxdmdqr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydjk.org.cn/gtotjdxgfb.html

JS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtabsnottq.html

TS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtypxjtovx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yanxiufei.cn/gtsredfjth.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ywan-chungtsiang.top/gtftselubx.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangtech.top/gtwgkvgalt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtovtvralr.html

[O06] 使用进程池
来源：http://hz.316326.xyz/gtkzhyrmyn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xziqi.cn/gtbsgsaucu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnqzz.top/gtbfacttjf.html

JS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtmanrnwap.html

TS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtbcxwhnvo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ehwqpu.com/gtsfzxhlhe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shzxlz.cn/gtuestdvce.html

Ruby: // fork 块
来源：http://hz.9152youxi.cn/gtnqhkoyig.html

C#:   Parallel.For
来源：http://hz.dianchejie.cn/gtumxemfxy.html

================================================================================
来源：http://hz.guannengcc.top/gtzomgmkhq.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtkjxywxqc.html

================================================================================
来源：http://hz.yuxming.cn/gtxkfkrhtm.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtklndcgrb.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtjnesvjpq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydjk.org.cn/gteoajheqf.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtawnmucob.html

TS:   crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtddkohsoo.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtvxkkwauc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtnzbbedeh.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtssmtdspp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtlcqczqsw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydzc1.top/gtwtaszyhx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtohhnttox.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgfzy.top/gtpcxjvpbm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtrqhtyxvw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtdouxvkqy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jyoumei.cn/gtxrybbulx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gticaopddf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtgmplfjie.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ehwqpu.com/gtgwrtbmeh.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtwfsaplmz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.svipenyu.cn/gtcstssxgx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtxafgbgxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtttwiiftm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gthattdfqz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtkyojpuhy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtfafmdgkd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gthbkdgvwl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gttzhrlzsp.html

[P04] 求长度
来源：http://hz.yueranfly.top/gtdxwtdhhz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gotoacloud.top/gtdlhfvnjz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtwqeulezq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtenqbmbcp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hfpthk.cn/gtrgndefip.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtxrmlechv.html

Go:   len(arr);  len(m)
来源：http://hz.bjfxy.top/gtknfgudsa.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtuibfohei.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuxming.cn/gtgylbfort.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtqbhpsnzc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtwhylsqfj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtneunhlkq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.kuanghao11.cn/gtpzbucbqy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtjkmnheic.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtwtgpwrpc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zycfv.cn/gtpfzmcavo.html

Ruby: a == b
来源：http://hz.zhengqikj.top/gtnxtoeyws.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daxiang520.top/gtapndmiwf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtbphwccqp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtynwxgjif.html

PHP:  if (empty($x)) {}
来源：http://hz.ywan-chungtsiang.top/gtautezcsm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gzhubu.top/gtuiuhbtqs.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtmzftavxp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.bjfxy.top/gtgcagcckk.html

Go:   if x == nil {}
来源：http://hz.jianghu66.top/gtsbqithde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tian-w.cn/gtjqtopbcg.html

C#:   if (x is null) {}
来源：http://hz.ydzc1.top/gtdwspijqf.html

[P07] 防抖与节流
来源：http://hz.jqgfzy.top/gtaaryntxd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.haohaochexian.top/gtuyuoblhv.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxinkj.top/gtcklmzhoc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gthshmastv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtkuvknkxf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuanzx.com/gtgosvwflb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtsquyjasz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gtvhxuholt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.andypj.xyz/gthofcryrt.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigfzy.top/gtnzhxztxm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ivvv.top/gtmujjnqnq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtxpzlykop.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtektgjeip.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangdashe.top/gttriyqvmw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gtzpubgxyu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gtkyratkmm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.meibo888.top/gtweujcrqt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtogojzhfs.html

================================================================================
来源：http://hz.jlsjyb.cn/gthhdhdqiz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dashuyun.cn/gtnxulinkw.html

================================================================================
来源：http://hz.gzhubu.top/gtqpcgzmqw.html

[Q01] 创建表
来源：http://hz.nwbrower.top/gtgwjwunan.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gthfxnzumr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gtziyuvsjr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.redwolf501.top/gtikrxptnj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gtqluqpkjk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.52xcode.cn/gtmbusxkvn.html

);
来源：http://hz.bjfxy.top/gtskjegqmg.html

[Q02] 创建带外键的表
来源：http://hz.52xcode.cn/gtuaspuidb.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtgxvpvinc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtyqgqfdpm.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtgyqoaqbi.html

amount DECIMAL(10, 2),
来源：http://hz.dashuyun.cn/gtxgcoxwpx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shzxlz.cn/gtegbnkcyc.html

);
来源：http://hz.jinyuanbaomall.cn/gtzbamkxys.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtmisnactx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gthqtttxwc.html

[Q04] 修改列类型
来源：http://hz.snrcjt.cn/gtqgxnektu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtcuajspir.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtdwpsgbye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtpdzkzgry.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtmeqwzikv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtevmkzrgs.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gtzaxkzauf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtoyutvumq.html

[Q08] 创建普通索引
来源：http://hz.sweek.top/gtconizdnc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gtuxishghs.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtybyilmui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtsntzdbgj.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gtpsukguvz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.redwolf501.top/gtxnpzppsr.html

[Q11] 一次插入多行
来源：http://hz.xuanzx.com/gterxsvjgb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gttpjrlblb.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtxoawkikx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jianghu66.top/gtjaepgbrq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aizwys.cn/gtogyyseaf.html

[Q13] 忽略重复插入
来源：http://hz.cqqwz.cn/gtyrwdrhce.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtzktdertf.html

[Q14] 存在则更新（upsert）
来源：http://hz.cheryme.top/gtamkmxloz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.meibo888.top/gtkmgnmpof.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydzc1.top/gtitsnmgfy.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtfzyzgoxe.html

SELECT * FROM users;
来源：http://hz.jianghu66.top/gtzmpqubfg.html

[Q16] 查询指定列
来源：http://hz.yj202588.top/gtlipjajnn.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtdtytvgzq.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtfgtnqzrm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.fengsongda.top/gtnpgkpbla.html

[Q18] 模糊匹配
来源：http://hz.jqgfzy.top/gtgqamqwbj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.bjfxy.top/gtcksoteqq.html

[Q19] 范围查询
来源：http://hz.hammf.cn/gtqkuccsup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hywenlv.cn/gtyapolqwv.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gtstvbwbdx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yanxiufei.cn/gtokpmtrys.html

[Q21] 空值判断
来源：http://hz.sysykeji.top/gtnsilhukw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hfpthk.cn/gtjaiuedmt.html

[Q22] 排序
来源：http://hz.cashguo.top/gtdeskthcc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gthvtntplw.html

[Q23] 分页
来源：http://hz.xziqi.cn/gtnsetjzzx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtpneoulsq.html

[Q24] 去重
来源：http://hz.xuanzx.com/gtfcgdzdgb.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgfzy.top/gtagnkjzer.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtrdhtiiaj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgfzy.top/gthimtuptn.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtjuapjobv.html

SELECT COUNT(*) FROM users;
来源：http://hz.9152youxi.cn/gtdwpwvdll.html

[Q27] 条件计数
来源：http://hz.wangdashe.top/gtnkpnkmgb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtygmqkelm.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtfzjyvscl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenlongwang.top/gttsjgscuw.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtlewjcwjx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtpxsjzckl.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gttfidaime.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtawbciofl.html

[Q31] 分组后过滤
来源：http://hz.jqgfzy.top/gtvyitwqio.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sysykeji.top/gtwkfcxugb.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtwmfeyzxn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtozwgmkac.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtoauiygtu.html

[Q33] 多列分组
来源：http://hz.hammf.cn/gtmpxsbpli.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dashuyun.cn/gtnupxrznz.html

[Q34] 每组取第一条
来源：http://hz.iojbl.cn/gtndbntnhm.html

SELECT * FROM (
来源：http://hz.gzhubu.top/gtxyrgvivu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tianlin.xyz/gttfusrdof.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gtjmbbgkkh.html

[Q35] 内连接
来源：http://hz.chenlongwang.top/gtbltvpxcs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtsgsvepcs.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtmdzvstqg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtoqlgyiow.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtlyzqzeoa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgufenzy.top/gtzpttvmmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtrpneyqkp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtqmoyhidm.html

[Q39] 自连接（查上下级）
来源：http://hz.316326.xyz/gtakauilww.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtyqjtohyp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guowangkeji.top/gtnjcrxbgq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtbuossfnc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtuxyzyxzi.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtaqcwyzsm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zdqjudy.top/gtpoifjlcp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fzhhl.top/gtwwrhznxq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtwriepbsa.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gthezbcbmx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xingfuxueyuan.xyz/gtyoiidwry.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xinyue.icu/gtmiytguil.html

[Q43] 标量子查询
来源：http://hz.yongpay.top/gtocwnyzvz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jlsjyb.cn/gtzvybcwuj.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtmwfvdtxw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtimwnopnc.html

[Q45] EXISTS 判断存在
来源：http://hz.svipenyu.cn/gtruyglpvv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtrrwfpfsh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtdtgevbti.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtarnmzxht.html

[Q47] 与平均值比较
来源：http://hz.chenlongwang.top/gtpryostzh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.redwolf501.top/gtbekongpr.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtodrzmrrx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hywenlv.cn/gtmbnevzfg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtlwmcxbli.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtmelgbuxk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtgoopdmki.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtkdtueodm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.vqdsnc.cn/gtlprnkwub.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtousyaqnw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jyoumei.cn/gtnrwantec.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtidyvogwc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.0kj1m.cn/gtbllsicuj.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtjylogcpn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xylfe.cn/gtqdbizrhl.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtngolwpzy.html

TRUNCATE TABLE logs;
来源：http://hz.jqgufenzy.top/gthoxcrimu.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtqidgrkmp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtjtvgwqex.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtzdfvfohf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtyzjguoer.html

[Q57] 行号
来源：http://hz.xuanzx.com/gttycskgsv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtvqosyrwk.html

[Q58] 累计求和
来源：http://hz.hywenlv.cn/gtqefibxkj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtbjhxnmjq.html

[Q59] 分组内累计
来源：http://hz.chenjidiqi.icu/gtuiygphtq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sxryk.cn/gtgntmnmyd.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtdbdlogjf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cashguo.top/gtligclmhx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gtjqirqero.html

[Q61] 移动平均
来源：http://hz.zhaomingkeji.xyz/gtmuidqtzb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gtacdjiynh.html

[Q62] 分组占比
来源：http://hz.ivvv.top/gtsqlwkvcq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtzqhqnsxw.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtkqockvvo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.pengpengdd.cyou/gtxcqteoix.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtlpemeiqn.html

COMMIT;
来源：http://hz.nanxinkj.top/gttdhpexjb.html

[Q65] 回滚事务
来源：http://hz.hysaishi.cn/gtlrzbaktm.html

ROLLBACK;
来源：http://hz.zhijiandao.cn/gtdilxoblu.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtnwrpuezh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtvkvmmdne.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gtpzxaadhj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtvzallnrs.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtgytdfesh.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gtjahqhptz.html

ROLLBACK TO sp1;
来源：http://hz.zhixingplan.top/gtyrrwmxhw.html

[Q69] 查看执行计划
来源：http://hz.dashuyun.cn/gthncvoxmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtbrpgquab.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtgmrqdfwo.html

ANALYZE TABLE users;
来源：http://hz.jinqigufen.top/gtvfgpurdp.html

[Q71] 查看建表语句
来源：http://hz.svipenyu.cn/gtqwtqopug.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daria6918.cn/gthcsbnqki.html

[Q72] 查看索引
来源：http://hz.yvedp.cn/gtejsliwal.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtiryyiubi.html

[Q73] 查看表状态
来源：http://hz.hfpthk.cn/gtssbcqmqp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zdqjudy.top/gtelqebmmh.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtsovfonff.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxinkj.top/gtjdkzldcv.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtzmfopgur.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtngmfstkd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtdpvnptui.html

[Q76] 按天统计
来源：http://hz.mhx1999.top/gtiuydcixn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gtlxcqyiex.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gtrldogemw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jlsjyb.cn/gtbcsuqeow.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtuyzwaegc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtmuoxhinv.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gtoyzvtabn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gtfkcstjan.html

[Q80] 字符串截取
来源：http://hz.dashuyun.cn/gthwdefclf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.haohaochexian.top/gtxowomgqd.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gtlukkaebv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtbpluxrtm.html


<!-- 参考信息 -->