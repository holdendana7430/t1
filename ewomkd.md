代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtjjthcbzv.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtsiofhcii.html

Java: synchronized (this) { shared++; }
来源：http://hz.hywenlv.cn/gtmzmepbaw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtuqaefiwn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnqzz.top/gtozatagvi.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtdfitcrzl.html

[O04] 定义异步函数并等待
来源：http://hz.jlsjyb.cn/gtaumjtkfx.html

Py:   async def f():⏎    await g()
来源：http://hz.xinyue.icu/gtapbdthlo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtpzzxlhsk.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtzuwqbxbv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nwbrower.top/gtpatnbwzi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dashuyun.cn/gtrmrkhwrd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tian-w.cn/gtoowolmdf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.haohaochexian.top/gtfhwfypmc.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtiuqikcia.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtruavgiqk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jlsjyb.cn/gtxnejywpm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtjmitbcna.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtuoxdituw.html

TS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtrebjdbuv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gthzsbpirj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinghuilouyu.cn/gtwagragjk.html

Ruby: threads.map(&:join)
来源：http://hz.fengsongda.top/gtyazcabrt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtxfbbiwgx.html

[O06] 使用进程池
来源：http://hz.zhoulong.xyz/gtmibbigtm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gtgdadulos.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangkeji.top/gtcxgxqnno.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtrdvsmflm.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtkzizwyyx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtfqvdlyxv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtgfkfeecw.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtqkteuvyj.html

C#:   Parallel.For
来源：http://hz.shanyushiyangtech.top/gtemervgbu.html

================================================================================
来源：http://hz.bjfxy.top/gtlsjwkjsj.html

P. 常用工具函数
来源：http://hz.haohaochexian.top/gtiqsszelf.html

================================================================================
来源：http://hz.smart0.xyz/gtctouwmja.html

[P01] 生成 UUID
来源：http://hz.ehwqpu.com/gttrdftbkc.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtlapshayw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tanke756.top/gtcgjyhlmh.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtmmwxddeq.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtqeykdjxn.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtrmkcirul.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtkmufbiva.html

Ruby: SecureRandom.uuid
来源：http://hz.c1oappe.top/gtprladame.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.svipenyu.cn/gtjsqlcgtq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtcbokscgm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gtqggwjvcv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtdefpktss.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhixingplan.top/gtuzgjjvqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtuelfuord.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtxqtewxzs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtpddpwjca.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtvbwvbrwj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtcaizlfwk.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtpzxszgvy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhaomingkeji.xyz/gtnuffgrfx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtkmgtqghk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtvnocgpzk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtrifzutaf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtsnqtukit.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cucudq.cn/gtfmjkjsdt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shangyingyoupin.top/gtgibragpz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gttbwenrpv.html

[P04] 求长度
来源：http://hz.svipenyu.cn/gtjrjoxzsi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhixingplan.top/gtvcgaeyrf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gttgjstxsm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtimbgpvvt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtxclzacik.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtgiesuyvb.html

Go:   len(arr);  len(m)
来源：http://hz.ydjk.org.cn/gtgrqoyyjg.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtkgvwtngj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhiwuduotai.top/gtqqjprloo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sxryk.cn/gtvrwemtrt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zdqjudy.top/gtvddfvekc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgfzy.top/gtzepkfzos.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigufen.top/gtwsydnvny.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnxiangtu.top/gtelulhsww.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.meibo888.top/gtylxxtdwr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtvfksxkpb.html

Ruby: a == b
来源：http://hz.xylfe.cn/gtxniywxfs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtxjmnxiqg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtwnjfaebg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nwbrower.top/gtrpiboshl.html

PHP:  if (empty($x)) {}
来源：http://hz.daria6918.cn/gtwtlwlyle.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtpyiolvlc.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtkbhxhuui.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gtrlmkgpbd.html

Go:   if x == nil {}
来源：http://hz.redwolf501.top/gtoffqried.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gturmeoaur.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtfhpgbujb.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangkeji.top/gtwyjhsvhy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenzaomai.com/gtyjjcfpuh.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtuxzhuinx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtnziehlmg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtecoqcpei.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtoueodysn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtnwnpzzhy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuanzhike.top/gttxtrtjgu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtemmkuzan.html

[P08] 处理浮点精度问题
来源：http://hz.nanxinkj.top/gtsaembtxn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ppjwa.cn/gtgidmfney.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtzvayqgjx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtidbcxele.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ywan-chungtsiang.top/gtnbnpgzxt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.c1oappe.top/gtwrcjwedf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenzaomai.com/gtofifztls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtqhtmuhmd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zdqjudy.top/gtquujduwc.html

================================================================================
来源：http://hz.gaohongyu789.top/gttsetbgww.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtlrvqugld.html

================================================================================
来源：http://hz.jianghu66.top/gtnaelgysu.html

[Q01] 创建表
来源：http://hz.jianghu66.top/gtavbqdexn.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtyjmsymih.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtzblmhzrj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tian-w.cn/gtbshulmwj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.smart0.xyz/gtbslfxmpz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xylfe.cn/gtjjfrwqna.html

);
来源：http://hz.ydjk.org.cn/gtmctstdap.html

[Q02] 创建带外键的表
来源：http://hz.sweek.top/gtwwlvirkp.html

CREATE TABLE orders (
来源：http://hz.nanxinkj.top/gtjddxspmc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtattjtojo.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gtxzoeeqos.html

amount DECIMAL(10, 2),
来源：http://hz.fzhhl.top/gtmlticayw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.52xcode.cn/gtcgmwpkqz.html

);
来源：http://hz.smart0.xyz/gtorxrgigq.html

[Q03] 增加列
来源：http://hz.yongpay.top/gtdjfebjkt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shangyingyoupin.top/gtngcwupps.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gtsstbcxqf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtnveahhwi.html

[Q05] 重命名列
来源：http://hz.smart0.xyz/gtgatetwor.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtzgzeddsm.html

[Q06] 删除列
来源：http://hz.daria6918.cn/gtoqzcmxrf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xingfuxueyuan.xyz/gtequhkjhn.html

[Q07] 删除表
来源：http://hz.yonumen.top/gtyxixvniu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgufenzy.top/gtaexspalt.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtxildhljs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtumskvmos.html

[Q09] 创建唯一索引
来源：http://hz.smart0.xyz/gtoffzuptk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtebzrkpur.html

[Q10] 插入单行
来源：http://hz.chenlongwang.top/gtnqqnrefj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtpfpsfbjg.html

[Q11] 一次插入多行
来源：http://hz.ydjk.org.cn/gtkvogjwlw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtgrlebhxn.html

[Q12] 插入后取自增 ID
来源：http://hz.ivvv.top/gtnvhjxxky.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtytjrbhvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258.top/gtwhlzfnak.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gtridpnvmc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtwmjslfbd.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gtkbkdaaay.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xylfe.cn/gtpmomgwho.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtlqxhvxvq.html

[Q15] 查询全部
来源：http://hz.zycfv.cn/gtuzncoynp.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtbukzftpe.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtzzfzrmhi.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gtuaieohmg.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtvluxecdn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtrjtewpoo.html

[Q18] 模糊匹配
来源：http://hz.svipenyu.cn/gtvhugoyrd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gthwfwdjhm.html

[Q19] 范围查询
来源：http://hz.jyoumei.cn/gtmijnrqej.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxinkj.top/gtdyeknxwz.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtaycfnuoj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtztlxcelj.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gtyyrdorsl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtqmmdtpwl.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtsnwwvugd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtbnxgeyez.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gttqkjqagu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtzyccnazu.html

[Q24] 去重
来源：http://hz.aizwys.cn/gtyseinhuf.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gtvwbueruc.html

[Q25] 只取前 N 条
来源：http://hz.xuetiantiany.cn/gtysinsmmm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtcvviegbg.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtcgqssmac.html

SELECT COUNT(*) FROM users;
来源：http://hz.jlsjyb.cn/gtmyvyjdgs.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtcgmutjmd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenjidiqi.icu/gtxfkrvehu.html

[Q28] 求和与平均
来源：http://hz.316326.xyz/gtlqjexltf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtuqjwftti.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gtidktwdsq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gtbjthrlgk.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtehweprtk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtkoslubqm.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtfieuzmox.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.havefunace.top/gtmtxprvpi.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtcsohsmhu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtxsqvjxbo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtpvmyqohf.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtgrsbglaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtsvdigeza.html

[Q34] 每组取第一条
来源：http://hz.tian-w.cn/gtxsrigipz.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtttevoxre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtmmceqahp.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtbyukkitw.html

[Q35] 内连接
来源：http://hz.gogol.net.cn/gtukuskmyt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtpjkvrzww.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtsiyufdgy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtwbvyuplb.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtybuijqdr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gttxsmlapc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.kuanghao11.cn/gtsbpcqcuu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xziqi.cn/gtwhwhdntl.html

[Q39] 自连接（查上下级）
来源：http://hz.zhijiandao.cn/gtgzackher.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.316326.xyz/gtvmjkdbas.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guannengcc.top/gtrwryvkrt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gthdbdrtjw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.snrcjt.cn/gthltufefy.html

[Q41] 多表连接
来源：http://hz.shangyingyoupin.top/gtofcfgpqc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xziqi.cn/gttgtyojzf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtkmnlrucr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hysaishi.cn/gtonzlpeor.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtbwcpfxib.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtcxpsakne.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gtnkrjdpdb.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtsxztogfe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtnrywngur.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtoaejlhca.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258888.top/gtrvojmqqn.html

[Q45] EXISTS 判断存在
来源：http://hz.cheryme.top/gtfuoqjgoh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gttwgwzpue.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangdashe.top/gtzkzstmfu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gtjydelmln.html

[Q47] 与平均值比较
来源：http://hz.9152youxi.cn/gtafvaofee.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgufenzy.top/gthapzedjk.html

[Q48] CTE 公用表表达式
来源：http://hz.jinyuanbaomall.cn/gtxuoyvzid.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.c1oappe.top/gtuytknvsx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtjhwuyytd.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtcectgvza.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gthtfhdyut.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtweemlfgi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtgogimgnd.html

[Q51] 用子查询更新
来源：http://hz.xylfe.cn/gtfxjoslfw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhaomingkeji.xyz/gtrpggomkn.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtdrdejjfz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtsezuzdhp.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtgtlpurhw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.9152youxi.cn/gtktvthuzq.html

[Q54] 清空表
来源：http://hz.daria6918.cn/gttpekhtnh.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtdwpeefhb.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtyomoskoy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtfjiyqsmt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhijiandao.cn/gtazbecdao.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtvurgdhiz.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtkgyiunno.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gturcqpknd.html

[Q58] 累计求和
来源：http://hz.dianchejie.cn/gtxwizntku.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gtwrzhpank.html

[Q59] 分组内累计
来源：http://hz.tian-w.cn/gtlxqjmbeu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yueranfly.top/gtnoeqznbk.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtgmkqlpst.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gtfkklaqay.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtijojuwpg.html

[Q61] 移动平均
来源：http://hz.xuanzx.com/gtbqujzptm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gttgpabwsv.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtbjcxcici.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtyvjokrvo.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtytofzcuh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gotoacloud.top/gtoiszzikv.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtzzhhqxaj.html

COMMIT;
来源：http://hz.xuanzx.com/gtqdpxkmyn.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtnvmdelzz.html

ROLLBACK;
来源：http://hz.ydjk.org.cn/gtyzhttvyj.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtdjldwuwu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtgkvstzff.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtnggnhmga.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtddmjbxfx.html

[Q68] 保存点
来源：http://hz.tianlin.xyz/gtklntugjm.html

SAVEPOINT sp1;
来源：http://hz.jiagoushi.top/gtnogwgaia.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtdubqwyds.html

[Q69] 查看执行计划
来源：http://hz.yj20258.top/gtofedziyo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jiagoushi.top/gtlxeivrrw.html

[Q70] 更新统计信息
来源：http://hz.sxryk.cn/gtvnsntxjs.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtdsewtoyd.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gtahbdbade.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhoulong.xyz/gtsdozwbwp.html

[Q72] 查看索引
来源：http://hz.jianghu66.top/gtwfredfpd.html

SHOW INDEX FROM users;
来源：http://hz.daria6918.cn/gtuthcdqiw.html

[Q73] 查看表状态
来源：http://hz.aizwys.cn/gtvdpthfin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gaohongyu789.top/gtgmogfsau.html

[Q74] 强制使用索引
来源：http://hz.snrcjt.cn/gtpxhfavkc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yangfankeji.com/gtxsirdxxu.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtpcxlwpwx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtwphqkduc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtinlupqbi.html

[Q76] 按天统计
来源：http://hz.andypj.xyz/gtuyoswgdi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.mhx1999.top/gtpqhvepry.html

[Q77] 时间加减
来源：http://hz.0kj1m.cn/gtlttfcdfd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtjsoblyxm.html

[Q78] 当前时间
来源：http://hz.jiagoushi.top/gttuwcxcxh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cdnleiting.top/gtycbewgao.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtaxdyrdcf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtjxpmvklk.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gttivhfluu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhongyouzk.top/gtlkoknwrk.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtqtqqjmjw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gturqeyvil.html

[Q82] 字符长度与字节长度
来源：http://hz.hongshengwenyu.top/gthrzifrfm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gtcvbjahlu.html

[Q83] 大小写转换
来源：http://hz.guowangkeji.top/gtsjprzcbv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtzvpbitll.html


<!-- 参考信息 -->