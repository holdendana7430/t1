代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guowangkeji.top/gteumrlgqo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtgmsewuvf.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtkajcyalj.html

[O05] 并发执行并等待全部完成
来源：http://hz.guannengcc.top/gtfpjufsdj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtftkyoimg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtdaslrizs.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtwzhwmkyz.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtdmjxrkfi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj202588.top/gtidbtqfdt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sxryk.cn/gtajhejdxj.html

Ruby: threads.map(&:join)
来源：http://hz.0kj1m.cn/gtrjctwtqf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtfhdecffk.html

[O06] 使用进程池
来源：http://hz.shzxlz.cn/gtorqqplpr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtscoabjwo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gtnuadufdt.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtfoinarpq.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtmgtfrmob.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gttxtiyroj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.havefunace.top/gteyffwurz.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtpddouapn.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gtgctnggtu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtknezqjga.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gttozxhzpt.html

================================================================================
来源：http://hz.xziqi.cn/gtjnegyyky.html

[P01] 生成 UUID
来源：http://hz.yvedp.cn/gtjiiwhgzd.html

Py:   str(uuid.uuid4())
来源：http://hz.jinqigufen.top/gtbtkhgtui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gtesynuolp.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtvqwzdftc.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtyqiybzdc.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtsdkbcwvw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yonumen.top/gtowuhnjjj.html

Ruby: SecureRandom.uuid
来源：http://hz.jianghu66.top/gtgvigqbso.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.52xcode.cn/gtjeuwvgwv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sxryk.cn/gtqtedrbcx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gtgfmjdbpk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhengqikj.top/gtoygsbuau.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jianghu66.top/gtyglfvssd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cqqwz.cn/gtmwyygosu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydjk.org.cn/gtprsdxrwc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtidwfqbwc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtmygycqez.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gtdcdrljmr.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtfefbymrr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xingfuxueyuan.xyz/gtwlxqdtbb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gtcujerfry.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtpsdqekfq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtauneghic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtbaeotoxd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtwyiqnuso.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sysykeji.top/gttksrgnxd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fzhhl.top/gtykskvera.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtbzqdpegv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtfqscandk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtwqnyzkzs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtyahsrxoe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtexmkjvvc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gthdjjuycu.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtbchtrhnd.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gthvzsvmqb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtwntiqjis.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtwnilnxus.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shuidangran.top/gtrywnsvif.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cucudq.cn/gtgaegfcdp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtvkjxdjgt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtsvzfgtyk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ywan-chungtsiang.top/gtkmyyckxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtmigymnzu.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtjjyxepxx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtxntwfmgk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cqqwz.cn/gtkvytcval.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.316326.xyz/gtvdwodsny.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtaitgswfq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtbquyceth.html

TS:   if (x == null) {}
来源：http://hz.sweek.top/gttvgahwas.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtmpabsgmj.html

Go:   if x == nil {}
来源：http://hz.tianlin.xyz/gtdspizdsl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhixingplan.top/gthbliryyg.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtqxdxncgr.html

[P07] 防抖与节流
来源：http://hz.yongpay.top/gtwyenfzno.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtzdavmfvn.html

PHP:  // 手写时间戳比较
来源：http://hz.sysykeji.top/gttzdzirht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gttpnsrvqs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtvgmtcfcq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ehwqpu.com/gtmuteqtip.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuanzhike.top/gtzkemciya.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yueranfly.top/gtghxyaizo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gtqgqoohxn.html

[P08] 处理浮点精度问题
来源：http://hz.shangyingyoupin.top/gtfxgkuhzy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangshuangyany.cn/gtlmkgmtew.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtxmniymcl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtsqgpqgyd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shzxlz.cn/gtcwznumtk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtxcyahdaq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtwdyhfxnb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigufen.top/gtjljqwxkk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guannengcc.top/gtvwgjcfjk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtycfsgcot.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgfzy.top/gtldjoqxku.html

================================================================================
来源：http://hz.zhengqikj.top/gtrsxxbxqt.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtmkpijonp.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtnusdjlfe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtfqckoghe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.havefunace.top/gtftskcvbd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gtikfxnqxd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cdnleiting.top/gtvyeyrhmu.html

);
来源：http://hz.feifeiyinyue.top/gtvseaclzg.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtqdnzttow.html

CREATE TABLE orders (
来源：http://hz.sufxvd.cn/gtehaluwln.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtdtprrxem.html

user_id INT NOT NULL,
来源：http://hz.aizwys.cn/gtinywwmiq.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtrqeutpua.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fengsongda.top/gtfpntypzc.html

);
来源：http://hz.cashguo.top/gtacmnwouh.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtqnmawwtd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtcmdfzqjj.html

[Q04] 修改列类型
来源：http://hz.xuanzx.com/gtmlhijvqu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhixingplan.top/gthwxuqyzp.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtfcpfbmxt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtkurzlbrp.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtgtovjfqf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtatyljoif.html

[Q07] 删除表
来源：http://hz.zhiwuduotai.top/gtbtdzhhbf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fengsongda.top/gtroqniqbv.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtqrrclhsl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtrcrasnoy.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtlqjeshio.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtlzqvvcjo.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtvudwmztz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgufenzy.top/gtenjapsir.html

[Q11] 一次插入多行
来源：http://hz.xuetiantiany.cn/gtznmneyyj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtcbrijoin.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtvrrosjht.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtqukyduzf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtmxkjedwz.html

[Q13] 忽略重复插入
来源：http://hz.aizwys.cn/gtvmjulgyq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gtwrnzcggo.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangshuangyany.cn/gtdlsnofhn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtmrrmnwho.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangdashe.top/gtjbudydmh.html

[Q15] 查询全部
来源：http://hz.chenzaomai.com/gthngthfqe.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gtgopochug.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtwrppdtte.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtdrcgnfuf.html

[Q17] 条件查询
来源：http://hz.9152youxi.cn/gttbviyshy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gteijnxwqi.html

[Q18] 模糊匹配
来源：http://hz.hnxiangtu.top/gtndoavotl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtooikuosf.html

[Q19] 范围查询
来源：http://hz.yj20258.top/gtvhnvcdnh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtphdtudcr.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtqdlxbcwn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenjidiqi.icu/gtojanbfyf.html

[Q21] 空值判断
来源：http://hz.wangshuangyany.cn/gtesxpvtct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.smart0.xyz/gtgoknxccm.html

[Q22] 排序
来源：http://hz.meibo888.top/gtpyydvnjp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gtrhaqwbug.html

[Q23] 分页
来源：http://hz.0kj1m.cn/gtwzzpejsp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydjk.org.cn/gtfebzriyr.html

[Q24] 去重
来源：http://hz.sysykeji.top/gtuavlxvnh.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gttuqyyexb.html

[Q25] 只取前 N 条
来源：http://hz.guowangkeji.top/gtdlevnkgn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pycfn.com/gtlliujqkt.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtvwgqimoi.html

SELECT COUNT(*) FROM users;
来源：http://hz.sysykeji.top/gtqigngiie.html

[Q27] 条件计数
来源：http://hz.aibaodan.cn/gtxtobuuvd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daxiang520.top/gtwdfawbyx.html

[Q28] 求和与平均
来源：http://hz.chenzaomai.com/gtasjdjkkd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yvedp.cn/gtifjkcoop.html

[Q29] 最大最小值
来源：http://hz.hongshengwenyu.top/gtnfupgoeg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tanke756.top/gtvfzojfwz.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtplaahmib.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtuqttqpug.html

[Q31] 分组后过滤
来源：http://hz.9152youxi.cn/gtxeggaitm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxinkj.top/gttgqojdbc.html

[Q32] 分组拼接字符串
来源：http://hz.zdqjudy.top/gtaneduyaf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtldxvubkr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtukxowqfv.html

[Q33] 多列分组
来源：http://hz.wangdashe.top/gtwnmnpuzj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtstxhjnbl.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gttxfhrwsc.html

SELECT * FROM (
来源：http://hz.shangyingyoupin.top/gtmghkgnpk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xylfe.cn/gtchooqkmj.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtmoioyvuv.html

[Q35] 内连接
来源：http://hz.zdqjudy.top/gtdeanoeaq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtithtcvnx.html

[Q36] 左连接
来源：http://hz.hfpthk.cn/gtxvpdeqqc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gthgqfzofb.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gtywxitrrs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtrksepakj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtbnutocth.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtgymyvnjq.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtrcddpkln.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ybcxt.top/gtkemxvdch.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258.top/gtyfijskmg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgufenzy.top/gtagwtghiv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtpeiwnvdy.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtqbkdbnni.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtewuunpmk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtxyefzvac.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtrhqsboga.html

[Q42] 连接条件附加过滤
来源：http://hz.xuanzx.com/gtocvvfctq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtoassunho.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtuzepqjuo.html

[Q43] 标量子查询
来源：http://hz.tian-w.cn/gtccwloatn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yanxiufei.cn/gtqzkqmmlp.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gttwttxsfa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xylfe.cn/gtjdoxkgkd.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gtmiqxrytr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtnhabelpc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtangcvdbk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtozzrfhcs.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtcqhswukc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yuanzhike.top/gtstxsqnky.html

[Q48] CTE 公用表表达式
来源：http://hz.zhijiandao.cn/gtarjnxleg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenzaomai.com/gtxzbxuyhq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cucudq.cn/gtjtnjdmlr.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtlurbdqhx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtluqqomfl.html

[Q50] 批量更新
来源：http://hz.jqgfzy.top/gtmqwkppgu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtunzcdqsu.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtahsfxcsh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhixingplan.top/gtxxfyptba.html

[Q52] 删除指定行
来源：http://hz.nanxuanxn.top/gtamqkjpni.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sweek.top/gtmieuqhmr.html

[Q53] 按条件删除
来源：http://hz.yj20258.top/gtsxjrfebp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hywenlv.cn/gtcmteiqaa.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtbwfqsplg.html

TRUNCATE TABLE logs;
来源：http://hz.pengpengdd.cyou/gtluyutuia.html

[Q55] 排名（并列占位）
来源：http://hz.snrcjt.cn/gtmvukdxxy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtshrtndwu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangkeji.top/gtibwzrkxc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtldkqddsj.html

[Q57] 行号
来源：http://hz.hnqzz.top/gtaejsunmh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtcqphbtyf.html

[Q58] 累计求和
来源：http://hz.cashguo.top/gtnijohoga.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtornqappm.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtpqfzkuyi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gttbrzyqbg.html

[Q60] 取上一行 / 下一行
来源：http://hz.shzxlz.cn/gtfllaiohw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtzgkharcw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.kuanghao11.cn/gtjiuhcqtw.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtkorscqrk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtrnrxaidq.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtspunagls.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtbqjidtir.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtlhkyrlmx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yongpay.top/gtjbmsspdx.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtmsvrxdia.html

COMMIT;
来源：http://hz.hnqzz.top/gttdrocjae.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtjbksvioj.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtlrskebah.html

[Q66] 行锁查询
来源：http://hz.zhongyouzk.top/gtfhuucnxh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daxiang520.top/gtubhxwsen.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtdomnuepy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhoulong.xyz/gtufefccqz.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gthchjzdpi.html

SAVEPOINT sp1;
来源：http://hz.ydjk.org.cn/gtdxblflaa.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtryhnxbnd.html

[Q69] 查看执行计划
来源：http://hz.yuxming.cn/gtrpdtuddf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtrknpcxxa.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtrfpptllv.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gttwxnvogz.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gteplptcru.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yanxiufei.cn/gtkwinhiqn.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gtyrralhvs.html

SHOW INDEX FROM users;
来源：http://hz.ybcxt.top/gtdggktsrq.html

[Q73] 查看表状态
来源：http://hz.havefunace.top/gtxffajnok.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtydhpgyih.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtntchnvvy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.52xcode.cn/gtgeylsnlg.html

[Q75] 日期格式化
来源：http://hz.zhoulong.xyz/gtlmwzdqdy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtrqrabwyi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhiwuduotai.top/gtdrichhke.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gtixiotylo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fzhhl.top/gtaitkbcck.html

[Q77] 时间加减
来源：http://hz.zhaomingkeji.xyz/gtrsyjajgf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtciujzgvp.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtfljxrzrk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cdnleiting.top/gtiejkhkpk.html

[Q79] 字符串拼接
来源：http://hz.wangdashe.top/gtyyslnlti.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sxryk.cn/gtdjeaimuw.html

[Q80] 字符串截取
来源：http://hz.shuidangran.top/gtcwbdckhu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtupwnvyau.html

[Q81] 字符串替换
来源：http://hz.ydjk.org.cn/gtmzeyflqu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.9152youxi.cn/gtrahfuzkt.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtbrwnsjtt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtouyqeigt.html

[Q83] 大小写转换
来源：http://hz.quarkkingdee.top/gtrtyczier.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.vqdsnc.cn/gtwmkimqla.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtnvghlciv.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtelzbezgb.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtefhmjdco.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtshpkqhnh.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtlaaoafjo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtdvfogkcm.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtuzvdwaqk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtrnuabdmp.html

[Q88] 行转列（条件聚合）
来源：http://hz.cashguo.top/gtmoeknmwv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pengpengdd.cyou/gtjgxsqhvp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtmkqdjahl.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtyqkdwzkh.html


<!-- 参考信息 -->