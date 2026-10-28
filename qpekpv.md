代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gttqvmuzru.html

JS:   async function f() { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gtouwwwssv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hywenlv.cn/gtkptsmqfk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aizwys.cn/gtnmvcbjqq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtinebverj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jianghu66.top/gtepfeyhsp.html

C#:   async Task F() { await G(); }
来源：http://hz.pycfn.com/gtwvuteaxd.html

[O05] 并发执行并等待全部完成
来源：http://hz.kuanghao11.cn/gtvcpshvlm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtxxhbofvn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigufen.top/gtdlcazuln.html

JS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtgwojifgy.html

TS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtpkfonsrh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenzaomai.com/gtlvpenmmy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtfrjbrlvp.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gtdartucpc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtpanqwlqy.html

[O06] 使用进程池
来源：http://hz.yonumen.top/gtwevvzuqy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtjvxbazku.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.smart0.xyz/gtcmveczhd.html

JS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtisfqkgct.html

TS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtgidhywby.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hfpthk.cn/gtobocamkm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cashguo.top/gtgtsdrhvl.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtcnsnyfua.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtdoiiwfzg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtchrvlzin.html

P. 常用工具函数
来源：http://hz.cheryme.top/gtbrfsdira.html

================================================================================
来源：http://hz.guannengcc.top/gtqqibmxum.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gttcsdjnjv.html

Py:   str(uuid.uuid4())
来源：http://hz.haohaochexian.top/gtxyfgawix.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtwshjtgim.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtbvfkiveu.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtgzsprevl.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtmgsfvlfm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtllcjofsn.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtrgqfgwyv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daria6918.cn/gtptguasny.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenzaomai.com/gttijudfwd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtwasozxas.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dashuyun.cn/gticgrmtvu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgfzy.top/gtkvzrnnml.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gthjxlozlk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gtfmgqjxuy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hysaishi.cn/gtwydiztsj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtncusfjlf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gttbihtsts.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gthcrjiunq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gtxhkxwghh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ybcxt.top/gtkheoezaz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtkhobemda.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtapeoqnrl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtiaqiwjzc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gttkynkice.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtxbhkoezk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ehwqpu.com/gtvjlvomia.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtyejcfyki.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtvstdoitg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtunyrmhrs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtbondouee.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtfxfpwuhy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtelzvrksc.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtfujzydjz.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtsdkytraa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gtjsxtcdqz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhijiandao.cn/gtzxryznvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangtech.top/gtykjqkwpp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guowangkeji.top/gtufxkqisx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yvedp.cn/gtktkblliy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtakfpswlw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhengqikj.top/gtuqcnhseu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtpnyonpyy.html

Ruby: a == b
来源：http://hz.yangfankeji.com/gtlbixxdvu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gtzdinqwkx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.svipenyu.cn/gtiftzgzpy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.pycfn.com/gtqozkijuf.html

PHP:  if (empty($x)) {}
来源：http://hz.tian-w.cn/gtkljwvmej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gtxvvlsjni.html

TS:   if (x == null) {}
来源：http://hz.fengsongda.top/gtuqizvjna.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtlrhhsflk.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gtthtjztkf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhengqikj.top/gtjfhqchwa.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtkrguqqnm.html

[P07] 防抖与节流
来源：http://hz.snrcjt.cn/gtrxszrgdi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yvedp.cn/gtkxnrqjqo.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtkwrqgyek.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtkgtiisnp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtlijbpxjh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gticiaibkp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigfzy.top/gtpmajqykw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yueranfly.top/gtavlvwfkv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtgjmcnult.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtzjsnzasz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtfciwyymr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtrjfirnre.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hysaishi.cn/gtvjkuzhxn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258.top/gtjizbvxst.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hongshengwenyu.top/gtvxfsmlcu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnqzz.top/gttwxldpxu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangshuangyany.cn/gtnxptfxeo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daria6918.cn/gttmbjilos.html

================================================================================
来源：http://hz.yangfankeji.com/gtmarcxuyc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daxiang520.top/gttatchzhd.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgqshjnnx.html

[Q01] 创建表
来源：http://hz.52xcode.cn/gtkkpeidjl.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gtpyoghjpk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtdhufpqkf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jlsjyb.cn/gtpmccjllk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sysykeji.top/gthogzrrec.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gttyutkqou.html

);
来源：http://hz.chenjidiqi.icu/gtokfwrcfc.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtfhhsufwu.html

CREATE TABLE orders (
来源：http://hz.zhiwuduotai.top/gtlfqnjnpy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtcymhlbfq.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtjfsxaxqv.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtxivpztqr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shzxlz.cn/gttwnlzxif.html

);
来源：http://hz.yueranfly.top/gtsgvpqisx.html

[Q03] 增加列
来源：http://hz.mhx1999.top/gtxqhdpqob.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtdvkbzwvc.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtaolczbcj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shangyingyoupin.top/gtlcsnsvqo.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtlqpvkkxz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cashguo.top/gtfholhdhc.html

[Q06] 删除列
来源：http://hz.cdnleiting.top/gtdmxxhhur.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yongpay.top/gtqaelscgk.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtcgorhuns.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtofjlaijz.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtnpvtspie.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtfilvigiy.html

[Q09] 创建唯一索引
来源：http://hz.xinyue.icu/gtbyuiqhok.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtgemqikyw.html

[Q10] 插入单行
来源：http://hz.iojbl.cn/gtccibpuor.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shangyingyoupin.top/gtlqdqrkdz.html

[Q11] 一次插入多行
来源：http://hz.fzhhl.top/gttdlecmqg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtsaoiqjth.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtswtamksm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gthftquvnh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtskmhdekz.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtpgxirxhk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhixingplan.top/gtnuqvptcl.html

[Q14] 存在则更新（upsert）
来源：http://hz.guannengcc.top/gtlmpqoccl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gthdzmjkgw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtyrxiwouj.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtygafwhah.html

SELECT * FROM users;
来源：http://hz.hongshengwenyu.top/gtqywhlfpn.html

[Q16] 查询指定列
来源：http://hz.c1oappe.top/gtugvqkrcq.html

SELECT id, name FROM users;
来源：http://hz.yangfankeji.com/gtouowqtoi.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gtlyeqspge.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cheryme.top/gtamyzyzks.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gttfvkvjcc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtujfanftx.html

[Q19] 范围查询
来源：http://hz.shanyushiyangtech.top/gtnhevdttl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.snrcjt.cn/gtweygjrsp.html

[Q20] IN 列表
来源：http://hz.yvedp.cn/gtnntkevht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtbyoorjhr.html

[Q21] 空值判断
来源：http://hz.zycfv.cn/gtjnobbzyn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtypyxmzxr.html

[Q22] 排序
来源：http://hz.hfpthk.cn/gtavcmwtph.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haohaochexian.top/gtgpakilqk.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtgyaaqncp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtickauwaf.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gthjgdvztq.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangshuangyany.cn/gtbpankeiy.html

[Q25] 只取前 N 条
来源：http://hz.cqqwz.cn/gtkhxhxeyf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtdlqzfwup.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtwhgjbsmk.html

SELECT COUNT(*) FROM users;
来源：http://hz.aizwys.cn/gtjdzrbwwk.html

[Q27] 条件计数
来源：http://hz.jyoumei.cn/gtbmlvrebx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gtvavbwrjm.html

[Q28] 求和与平均
来源：http://hz.tian-w.cn/gtitebvapc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtlowhgrgb.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtlpvsvzxw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtiwrgpkab.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtbsfiiwvz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtaxoivptw.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtteavjrwh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.mhx1999.top/gtbijqpzwn.html

[Q32] 分组拼接字符串
来源：http://hz.xuetiantiany.cn/gtamhzbkoy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtjqwpgadk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gtlxcddqhc.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtdwlbivdh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gtznnkbfwq.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtahcjmqdu.html

SELECT * FROM (
来源：http://hz.nanxuanxn.top/gtmrvsebuf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.vqdsnc.cn/gtkkvmnjqt.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtwbqtbmnk.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtnamncgvt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtixgbibdq.html

[Q36] 左连接
来源：http://hz.yj202588.top/gtqqesnbip.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtsacyxhoc.html

[Q37] 右连接
来源：http://hz.shanyushiyangkeji.top/gtvglzawde.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtanpqrixv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtumpvmnky.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zycfv.cn/gtlgbpzxst.html

[Q39] 自连接（查上下级）
来源：http://hz.chenzaomai.com/gteuidsllz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtrnqvhybf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.0kj1m.cn/gtchtdhnie.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nwbrower.top/gtbmpuhdgu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtoworkpev.html

[Q41] 多表连接
来源：http://hz.feifeiyinyue.top/gtjybeoinv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtccopcifu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.havefunace.top/gtgdcvbcar.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.meibo888.top/gthwkyttyv.html

[Q42] 连接条件附加过滤
来源：http://hz.tian-w.cn/gtxpxhfdij.html

SELECT u.name, o.amount FROM users u
来源：http://hz.quarkkingdee.top/gtkhlubggm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtuxdaosbi.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gttuykpiio.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtkkvczafx.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gtzfxuuhjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.haohaochexian.top/gtmnkczkmj.html

[Q45] EXISTS 判断存在
来源：http://hz.aibaodan.cn/gtofijhglj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtauxazowx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gttuubmiye.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtjzsdrkcf.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gtsprtjhrc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtffkibkot.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtvjcfwuqq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.haohaochexian.top/gtveahdpsh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtnubwaewm.html

[Q49] 更新单行
来源：http://hz.daxiang520.top/gtrmcoyiaw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daria6918.cn/gtcfxnzoov.html

[Q50] 批量更新
来源：http://hz.tanke756.top/gtbhtiaxpc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shangyingyoupin.top/gtvfjxenjf.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtrlvrgrkh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtoqrcatge.html

[Q52] 删除指定行
来源：http://hz.haohaochexian.top/gtygxkfjkh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xziqi.cn/gtctiyonrx.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtlefcitxe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigfzy.top/gtdrliziua.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gthwsgmvde.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtcltpfbff.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gtfwttbhko.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hongshengwenyu.top/gtcldzujdi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtothjeuki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtkhgkkdox.html

[Q57] 行号
来源：http://hz.daxiang520.top/gthespzdlp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtfgiekewu.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtwxxzqcrp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtxhvgvyrs.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtntejpuot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gtdxtxgyme.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtijhiraod.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtqloftiqa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gtnesugdyr.html

[Q61] 移动平均
来源：http://hz.gotoacloud.top/gtudketibi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtlzejatzt.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gttxjrhqoz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtduozoivl.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gtwsdjibot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtopdmnzqp.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtertcuzkx.html

COMMIT;
来源：http://hz.shanyushiyangtech.top/gtpibjxalh.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtefryjhzv.html

ROLLBACK;
来源：http://hz.snrcjt.cn/gtevjfqfni.html

[Q66] 行锁查询
来源：http://hz.0kj1m.cn/gtljndfjfl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xinyue.icu/gtanwacays.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtyfsjcnrj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gtlxmfkrie.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtdlrdktgi.html

SAVEPOINT sp1;
来源：http://hz.shangyingyoupin.top/gtxgmlksnc.html

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtcnvkapxe.html

[Q69] 查看执行计划
来源：http://hz.xinyue.icu/gtqzuohlzo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sxryk.cn/gtgvgrrxql.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtmcclzzoz.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtaiimexpm.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gtlyoepkjj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtehjviykp.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gtqpygfkge.html

SHOW INDEX FROM users;
来源：http://hz.hfpthk.cn/gtzasyleiv.html

[Q73] 查看表状态
来源：http://hz.meibo888.top/gtmnafcsjt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gtqkcjbuca.html

[Q74] 强制使用索引
来源：http://hz.zhongyouzk.top/gtnpotvrri.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtnkdhttuf.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gthnflutrv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.316326.xyz/gtzeazcpdx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gthejdpkdh.html

[Q76] 按天统计
来源：http://hz.dianchejie.cn/gtozniqpta.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtzggaecid.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtucqhbjsf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ehwqpu.com/gtvnyqetsd.html

[Q78] 当前时间
来源：http://hz.jinqigfzy.top/gtaetlrqrc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gtkqkmavlb.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gtqmrxawre.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtgeilvvnw.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtachusjyn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtaekipwcn.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtjegkbsre.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtgwuukjqv.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gtdcjdxeln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yongpay.top/gtkvqyauxr.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtjkerfeos.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.vqdsnc.cn/gtgggcdiug.html

[Q84] 去除首尾空格
来源：http://hz.cdnleiting.top/gtmmbdldmc.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtyomlclkj.html

[Q85] 数值取整
来源：http://hz.cdnleiting.top/gtcjqrurhw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtoupksauz.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtnealdjor.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shangyingyoupin.top/gttccxoljp.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gthambwpcu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtcedmanff.html


<!-- 参考信息 -->