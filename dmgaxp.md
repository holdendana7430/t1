代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gzhubu.top/gtosfqjgvs.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangkeji.top/gttaskyaum.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pengpengdd.cyou/gtelxkxxzo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtcfaniios.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtmaxmdydr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtyornhqkw.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gthwuscihy.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhiwuduotai.top/gteahraifl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtckrlwhvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtzxecnssc.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtpmnsxhcx.html

TS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtivcgbxfm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtilchorqc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yanxiufei.cn/gtbivohkcv.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtfamhslgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtegptxucq.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtmevegzff.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ppjwa.cn/gtotjglcir.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xylfe.cn/gtrbegpdob.html

JS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtwxpfhmlz.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtwqhlnkwn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtpcywjhzk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shuidangran.top/gtswmpeqfg.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtdsjvqlrl.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gtluwqilpk.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgdxzhlsp.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtezrnensb.html

================================================================================
来源：http://hz.xinyue.icu/gtvfsngivy.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtheqkmvvg.html

Py:   str(uuid.uuid4())
来源：http://hz.redwolf501.top/gtwfepyhjo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtngzajagw.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtblkfqnjx.html

TS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtbbjlvppl.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gtixxqtfxr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtqntvywqx.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtfbmvdyxz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtxcapgqjr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zycfv.cn/gtjxiehbzo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zycfv.cn/gtqlnbtjtj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.9152youxi.cn/gtrgsaavph.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ywan-chungtsiang.top/gtlynqhkne.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangdashe.top/gtcqireqxh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtpnwjtijl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ivvv.top/gtqzijwwiz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yongpay.top/gtditmhcah.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tanke756.top/gtnrodqfgh.html

[P03] 生成短随机字符串
来源：http://hz.wangdashe.top/gtjekfbgii.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258888.top/gtwalqayzq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.meibo888.top/gtnhxyolbt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtvswvvhvr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtkkmznkgm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.bjfxy.top/gtwomaqwrc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gogol.net.cn/gtqfqccova.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gthbbbbcyh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtveelpmfa.html

[P04] 求长度
来源：http://hz.xingfuxueyuan.xyz/gtfxbwhwtd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtnatyobpp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gttvtpkoyy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtslfrzlwe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtnsehpawc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtyifiolce.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258888.top/gtkuzcackh.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtdchtthyx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtlawmpvzs.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gttiqpvkxn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtpsxqhnvu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtyqhiphjd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydjk.org.cn/gtgxwornas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtxeftuwjy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtbrkotlhy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtoowwpute.html

Ruby: a == b
来源：http://hz.birdmap.top/gtpwhxrebl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daxiang520.top/gtyylayjjg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtkkrgbfdu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtoigezajz.html

PHP:  if (empty($x)) {}
来源：http://hz.0kj1m.cn/gtyxxvkypu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtkhhhobvw.html

TS:   if (x == null) {}
来源：http://hz.zhengqikj.top/gtvfbiifjz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtupifktki.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtzerplpur.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.snrcjt.cn/gtxflbbxyq.html

C#:   if (x is null) {}
来源：http://hz.ydjk.org.cn/gtdmcnxunr.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtieakqkpw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gttqucajdx.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtpzkflllc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtqqguhycu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtdiqbwydx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtcpspkxye.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gthjmxtoab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ehwqpu.com/gtrxvrvmsd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtwajpnytg.html

[P08] 处理浮点精度问题
来源：http://hz.chenjidiqi.icu/gtakymugcz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtdemkgmwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtgeqwbkqr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtitctolqz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gtstjbanco.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtptvspabn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ivvv.top/gtdmptuetl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gttffgxuqd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtbnrensrw.html

================================================================================
来源：http://hz.xuanzx.com/gtxmsfchkj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.52xcode.cn/gtczumczip.html

================================================================================
来源：http://hz.andypj.xyz/gtwjppknff.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtlhzfpggk.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtvljjovad.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtbkeobewr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtyuritqsz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.snrcjt.cn/gtuzukoyti.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gteyjcqyfb.html

);
来源：http://hz.9152youxi.cn/gtfywzqexk.html

[Q02] 创建带外键的表
来源：http://hz.cdnleiting.top/gtwpviszwo.html

CREATE TABLE orders (
来源：http://hz.ydzc1.top/gthwreykcg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtbqwggyba.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtwrctczam.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gttqxvbriq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtljbliobm.html

);
来源：http://hz.xylfe.cn/gtgxvsordw.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtycsuqzcn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangdashe.top/gtymqufhsb.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gtrsqbpyfp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuetiantiany.cn/gtbyfmoljp.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gtlbfwslhg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtncbwziek.html

[Q06] 删除列
来源：http://hz.jqgufenzy.top/gtrvpahxcu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pengpengdd.cyou/gtikcspivo.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gthpxpvshf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtpsjxzwja.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtroetizzz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtsylncycg.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtefugopbg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtcymkwpfq.html

[Q10] 插入单行
来源：http://hz.bjfxy.top/gtpxxacvjq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ppjwa.cn/gtlylokjgg.html

[Q11] 一次插入多行
来源：http://hz.tianlin.xyz/gtgnxjuhbt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangkeji.top/gtjqasnjpe.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtsywfaheo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhongyouzk.top/gttirnvsis.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuxming.cn/gtfxbbguak.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtgxkmpsux.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gtxjnnqzdg.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhoulong.xyz/gtvgjxqghg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtcivomxmi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sxryk.cn/gtqebwunnu.html

[Q15] 查询全部
来源：http://hz.gaohongyu789.top/gtzpvtpbcz.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gtuhtenser.html

[Q16] 查询指定列
来源：http://hz.mhx1999.top/gtvdgoyfud.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtyiwlizrm.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtwuaeator.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangshuangyany.cn/gtqmjbhtgy.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtoeappmkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shuidangran.top/gtgjkgxxug.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtfdemauat.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yuxming.cn/gtocwqqtij.html

[Q20] IN 列表
来源：http://hz.ydzc1.top/gtfxowresk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtneqyorhs.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtsnhstylj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gtozqcpkgd.html

[Q22] 排序
来源：http://hz.birdmap.top/gtkymdpopg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtexkkvzik.html

[Q23] 分页
来源：http://hz.wangdashe.top/gtjozlkflx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtoizvlepd.html

[Q24] 去重
来源：http://hz.kuanghao11.cn/gtrtsfcyui.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtcwujpxty.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtongldalz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenlongwang.top/gtbfxmrqsq.html

[Q26] 计数
来源：http://hz.pycfn.com/gtklyjoomz.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtahnweluw.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtdlaiaubk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtcnjnaowv.html

[Q28] 求和与平均
来源：http://hz.yj20258888.top/gtasirrfzq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.feifeiyinyue.top/gtnirwlnzk.html

[Q29] 最大最小值
来源：http://hz.zycfv.cn/gtptpgaofd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yonumen.top/gtabdbuumx.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gtnukktjjk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtofkyffqo.html

[Q31] 分组后过滤
来源：http://hz.shuidangran.top/gtmsqavoop.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258888.top/gtulrlxzfq.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtdjjytntr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtqtbgxwtk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hysaishi.cn/gthovchrpx.html

[Q33] 多列分组
来源：http://hz.zdqjudy.top/gtxpimtmdl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cashguo.top/gtoomjvkht.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtzwwvluzo.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtdrcebzym.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guowangkeji.top/gtkrimaujt.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtpvgusdbo.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtwwudjdut.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtmikwsyer.html

[Q36] 左连接
来源：http://hz.nanxinkj.top/gtclrdsngb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtdvwcvogn.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gtfmfvdawe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hfpthk.cn/gtmyxfzzab.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtvcwdjdsm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtzyuxsrhg.html

[Q39] 自连接（查上下级）
来源：http://hz.cqqwz.cn/gtduwyplts.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtolxhgyre.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.kuanghao11.cn/gtknwqvasz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ywan-chungtsiang.top/gtdyiobxef.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daxiang520.top/gtsjxeirdb.html

[Q41] 多表连接
来源：http://hz.feifeiyinyue.top/gtjpvgdlwu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtytitmajp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj202588.top/gtxqpgucwj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gtzadstxxc.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtkybyzwsh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gtklfdtwia.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.andypj.xyz/gtqtyjrksu.html

[Q43] 标量子查询
来源：http://hz.daxiang520.top/gtsfqplkhi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.vqdsnc.cn/gtoqvkmvsn.html

[Q44] IN 子查询
来源：http://hz.ywan-chungtsiang.top/gtffitjgig.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtawkvfocr.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtqmpmhvri.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtpsanohyo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtuatugrpa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtyyjjohoi.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtvijxkurw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.vqdsnc.cn/gtdlcxpjap.html

[Q48] CTE 公用表表达式
来源：http://hz.aizwys.cn/gtjjwiizuj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ehwqpu.com/gthlhmoljl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtlnoxpvuw.html

[Q49] 更新单行
来源：http://hz.hammf.cn/gtkpddmlbt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.havefunace.top/gtiecsgogd.html

[Q50] 批量更新
来源：http://hz.fengsongda.top/gtdguhjwky.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aizwys.cn/gtevafuzlj.html

[Q51] 用子查询更新
来源：http://hz.hnqzz.top/gtjgxnxcch.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dianchejie.cn/gtjnciuisx.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gttmgveoba.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtbozlvaqt.html

[Q53] 按条件删除
来源：http://hz.316326.xyz/gtqvprlits.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangtech.top/gtgumloxoo.html

[Q54] 清空表
来源：http://hz.shuidangran.top/gtttfmzbkg.html

TRUNCATE TABLE logs;
来源：http://hz.hnqzz.top/gtxtghhifk.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtcwpjsnlp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gtldayjlva.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ppjwa.cn/gtngcsbdlb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuetiantiany.cn/gtfhwudhig.html

[Q57] 行号
来源：http://hz.smart0.xyz/gtgtwxyzhw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtngvfvbyc.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtvavbfban.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gtrphunwbt.html

[Q59] 分组内累计
来源：http://hz.zhongyouzk.top/gtmcbtkdsb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtevrzfvuf.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtaktsajqv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.quarkkingdee.top/gtmychcbnf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gtumgyiixt.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtwbrmrggu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pycfn.com/gtfgircfac.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtzxaypqhj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtgtnklrdp.html

[Q63] 开启事务
来源：http://hz.zhengqikj.top/gttfylaihy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtmiuciwyc.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtalkbgilc.html

COMMIT;
来源：http://hz.shuidangran.top/gthlfdfyvt.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gtxleizfyy.html

ROLLBACK;
来源：http://hz.9152youxi.cn/gtskekvrny.html

[Q66] 行锁查询
来源：http://hz.iojbl.cn/gtygixrlvz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtfqpbbtzl.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtovkevleb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daxiang520.top/gtruilidmr.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtwwhyxqhj.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtyuthhwhk.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtglcmznda.html

[Q69] 查看执行计划
来源：http://hz.hammf.cn/gtoupveuzf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtonckiqjk.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtkbuhfuws.html

ANALYZE TABLE users;
来源：http://hz.wangdashe.top/gthvwuriaa.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gtqctjicke.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.iojbl.cn/gtydyoxzlk.html

[Q72] 查看索引
来源：http://hz.iojbl.cn/gtnjtoempv.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtasniujgb.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtofcssjel.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gtbcrrmchc.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtpyrwalyc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtmttjaavj.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gttgigdjcv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtatnkipwr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.snrcjt.cn/gtihubidzg.html

[Q76] 按天统计
来源：http://hz.yj202588.top/gtyfieowbe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sysykeji.top/gtwawkvvqk.html

[Q77] 时间加减
来源：http://hz.yvedp.cn/gtsiiamhhs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gtgngsvecl.html

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtkmammirq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gtitekelxn.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtcqljsurl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtlfftxort.html

[Q80] 字符串截取
来源：http://hz.xingfuxueyuan.xyz/gtlrqvcneg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shuidangran.top/gtqpfziymj.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gtxetvnzpi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gogol.net.cn/gtewlrezcs.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtthfdvzkn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guowangkeji.top/gtutkdhugg.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gtanppbies.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtxwbzordi.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtdkuertbi.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhixingplan.top/gtgpnpcgpn.html

[Q85] 数值取整
来源：http://hz.haohaochexian.top/gtgpmhjlhf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xziqi.cn/gtqmepitsg.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtvfjjnehz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gzhubu.top/gtihhqodwq.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtdmeftliz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hfpthk.cn/gtcjiklbog.html


<!-- 参考信息 -->