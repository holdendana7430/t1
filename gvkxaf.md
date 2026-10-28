代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aibaodan.cn/gtwwrjoujv.html

[O03] 加锁保护共享数据
来源：http://hz.gotoacloud.top/gtocuryesl.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtcvwkvugr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtxediaisz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cucudq.cn/gtuggbybgl.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtslcrstci.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gtftbmpqkr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtykeaspqx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinyuanbaomall.cn/gtnibjsiti.html

C#:   lock (gate) { shared++; }
来源：http://hz.jlsjyb.cn/gtrpxngewd.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangtech.top/gthqrmyhhr.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtzlssssif.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gtzedyerje.html

JS:   async function f() { await g(); }
来源：http://hz.nanxinkj.top/gtlvgatjbg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gttfvjaudi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gtteqnzzok.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yvedp.cn/gtictadtty.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangdashe.top/gtmaymhisd.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtfkhgcfzd.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gtemuhnmou.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gttjjbymtw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtrwmmlaop.html

JS:   await Promise.all(tasks)
来源：http://hz.cqqwz.cn/gtlrtpicsf.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtlvcwzomb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtzrefvbwk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.52xcode.cn/gtrylhrnvz.html

Ruby: threads.map(&:join)
来源：http://hz.xuanzx.com/gtlacptbla.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pycfn.com/gtinhzfkrr.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gtrcltaqto.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yvedp.cn/gtzaufekew.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ehwqpu.com/gtisalomfj.html

JS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtmruhtrcj.html

TS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gttizaoqie.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenzaomai.com/gtkydohlve.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj202588.top/gtqlsjpsuy.html

Ruby: // fork 块
来源：http://hz.xuanzx.com/gtqqeqwybp.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtatldgrek.html

================================================================================
来源：http://hz.jianghu66.top/gtwogceihp.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gtfpjzsofc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtevdmgzkz.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gtymfdlbjz.html

Py:   str(uuid.uuid4())
来源：http://hz.aibaodan.cn/gtwkzdfnsg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtjcyphari.html

JS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtgiuknlqu.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtsvyebbgg.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gtmdhcexfs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.quarkkingdee.top/gtropjmjpj.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gtcdrxoyxz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gthokkhgiu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtbtmtjhgz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtfqqzftof.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhoulong.xyz/gtgxgnwjfe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtfpfjipsr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtxiguukev.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtmnafqopt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gthrzibjcn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gtnsunwraj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gttyrfdfhf.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtaonwawdl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fengsongda.top/gtumygelrt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gttlrevuvn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtgweimysv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtdqzfkyhm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cashguo.top/gtzekappwd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhijiandao.cn/gtuvfcoxkx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gtooolijax.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hysaishi.cn/gtmnixmtog.html

[P04] 求长度
来源：http://hz.nanxinkj.top/gtdxjizrxz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtytouremp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtblxgimye.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtzgqotmnp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtmynvsjsr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.meibo888.top/gturpfkpkd.html

Go:   len(arr);  len(m)
来源：http://hz.guannengcc.top/gtfggenfge.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtgbopyige.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtmuzyhhad.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gteqllbuhx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gturbeolfu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gtgbxquhra.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtahriwurg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtjgfgcvqn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtivzqejqs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.c1oappe.top/gtwckvfdqv.html

Ruby: a == b
来源：http://hz.iojbl.cn/gtlamiiknc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xziqi.cn/gtqjjxsmax.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258888.top/gtoxfpgjlg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gttvvfeecm.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtueoidefa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtlwebrzvl.html

TS:   if (x == null) {}
来源：http://hz.jiagoushi.top/gtcdyopgrm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtxfepossk.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtyeqxohiq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenjidiqi.icu/gtwhvuyuri.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtcqhudcvk.html

[P07] 防抖与节流
来源：http://hz.gogol.net.cn/gtldicqowb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.redwolf501.top/gtmbfavveb.html

PHP:  // 手写时间戳比较
来源：http://hz.shuidangran.top/gtkqzrmfsg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtywetjaih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtwmsnlzxx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtmgnfwkcw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtegvgfrxq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtxfqjzmec.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yongpay.top/gtzvwlsymz.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtlklbuueh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtbylieukc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtwsbazajn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtnnknbddk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gtfbayxoub.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtzzevxllb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtgsvgwzeq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtefrgppnn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.316326.xyz/gtlneiuvcn.html

================================================================================
来源：http://hz.xylfe.cn/gtdkkwwyyt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtlimaqwhj.html

================================================================================
来源：http://hz.smart0.xyz/gtwrxxvwjm.html

[Q01] 创建表
来源：http://hz.jinyuanbaomall.cn/gtbehuyuts.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtwmkiiqau.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtnlynmccz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtwjpqsnpg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258888.top/gtgrfodkxu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtpwbaprzq.html

);
来源：http://hz.316326.xyz/gtjmmlovrn.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtsuurrrht.html

CREATE TABLE orders (
来源：http://hz.shangyingyoupin.top/gtvoavngvh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtzjdexbag.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gthoijtncc.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtswsjslpa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.316326.xyz/gtloamwrek.html

);
来源：http://hz.fzhhl.top/gtmnstxpfb.html

[Q03] 增加列
来源：http://hz.hongshengwenyu.top/gtsihpqnfd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jianghu66.top/gtaxhmwnap.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtnvwxbscq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtmguyeaug.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtxjnduncq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtqrvesjcg.html

[Q06] 删除列
来源：http://hz.zdqjudy.top/gtfwjuwudv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangtech.top/gtyszknimu.html

[Q07] 删除表
来源：http://hz.iojbl.cn/gttuglxhyg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jlsjyb.cn/gtlxnoxvfm.html

[Q08] 创建普通索引
来源：http://hz.zhengqikj.top/gtubvdence.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gtrgkkefqm.html

[Q09] 创建唯一索引
来源：http://hz.tian-w.cn/gtbwgkfthv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtamsojaai.html

[Q10] 插入单行
来源：http://hz.zhoulong.xyz/gtlmyqipze.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gtspjnxxmh.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtnjqjltnw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guowangkeji.top/gtvaeajvag.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gtladzhhwj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cashguo.top/gtttxnbvhz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtnwgvvjay.html

[Q13] 忽略重复插入
来源：http://hz.hnxiangtu.top/gtcwpspjmb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtviajzpri.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gtojjjfmre.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuetiantiany.cn/gtqwnqfxly.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtynbmentb.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtqtzuuxrn.html

SELECT * FROM users;
来源：http://hz.yj20258.top/gtgxxqihnp.html

[Q16] 查询指定列
来源：http://hz.zhiwuduotai.top/gtsqxhstlf.html

SELECT id, name FROM users;
来源：http://hz.ywan-chungtsiang.top/gtpgszctil.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gtbqtyehtf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangkeji.top/gtgczrygvn.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtfoqfwtzz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gteoaxvvrr.html

[Q19] 范围查询
来源：http://hz.birdmap.top/gtvghuifhl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtcyxvlrll.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtxrbmuqwx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangtech.top/gtlnahhzjo.html

[Q21] 空值判断
来源：http://hz.ydzc1.top/gtcwlafcqb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.iojbl.cn/gtgemwhqlw.html

[Q22] 排序
来源：http://hz.yj202588.top/gtliwygefa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtqhfbrplj.html

[Q23] 分页
来源：http://hz.cucudq.cn/gtoeodhfcy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gticiykaey.html

[Q24] 去重
来源：http://hz.zhengqikj.top/gtlymeyhhg.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtzvpvlfnd.html

[Q25] 只取前 N 条
来源：http://hz.ehwqpu.com/gtphkcdvgp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtzsuwnfvs.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtlllnnxth.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtlstzfiga.html

[Q27] 条件计数
来源：http://hz.fengsongda.top/gtcvojmfwu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtgvzuefgz.html

[Q28] 求和与平均
来源：http://hz.feifeiyinyue.top/gtoejnjxms.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yangfankeji.com/gtycpdiamn.html

[Q29] 最大最小值
来源：http://hz.tian-w.cn/gtcvkuvpjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtmpbrqifo.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtldonzhod.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtoppxpvto.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtmlbctitk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtwflajxdb.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtwxdmmasy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtodmymjxw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtjapszvkx.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtrmzfemoo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtrnttrxuo.html

[Q34] 每组取第一条
来源：http://hz.wangdashe.top/gtymwlimbz.html

SELECT * FROM (
来源：http://hz.daria6918.cn/gttovygieb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigufen.top/gtuntcvrqa.html

) t WHERE rn = 1;
来源：http://hz.316326.xyz/gtxdkfvwsu.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtgbzyqhmz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtfjwcvwkj.html

[Q36] 左连接
来源：http://hz.sxryk.cn/gtimtdtusx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtvflwhhsx.html

[Q37] 右连接
来源：http://hz.fengsongda.top/gtjfroijhz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gttgfflvgo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cdnleiting.top/gteuvxnusu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gtdozximdo.html

[Q39] 自连接（查上下级）
来源：http://hz.fzhhl.top/gtmyfiuypx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nwbrower.top/gtrwtuxtjc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtvlobxmsu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gteaezyjhb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tanke756.top/gtquljqhjn.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtpvdpiosq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtqflruwap.html

JOIN users u ON u.id = o.user_id
来源：http://hz.guannengcc.top/gtjgbglydk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.iojbl.cn/gtnwigemnj.html

[Q42] 连接条件附加过滤
来源：http://hz.feifeiyinyue.top/gttbmriuzh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtjxpigqfb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xziqi.cn/gtzjttltcq.html

[Q43] 标量子查询
来源：http://hz.yj20258.top/gtnykxklkk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.redwolf501.top/gtkdhpeleh.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtgcurzgyx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gotoacloud.top/gtzrnbefgy.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gtuvgwkdgl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtnvufuqsd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangdashe.top/gtfbwypykd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtpumgyttc.html

[Q47] 与平均值比较
来源：http://hz.zhengqikj.top/gtidfwdwxj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtvaxirogo.html

[Q48] CTE 公用表表达式
来源：http://hz.yonumen.top/gtnrpldbva.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cashguo.top/gthtbrxfiv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtxzojwqmp.html

[Q49] 更新单行
来源：http://hz.shuidangran.top/gteuyslern.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxinkj.top/gtpefhvbzv.html

[Q50] 批量更新
来源：http://hz.wangdashe.top/gtvzrhcvpt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gthbtmazul.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gteudrwzzl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtqfsxkkxi.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtjrjnefii.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zdqjudy.top/gtficjfcqw.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtrnsuxaau.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtqvkdhyhv.html

[Q54] 清空表
来源：http://hz.daria6918.cn/gtgooyprbv.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtrzxbcefn.html

[Q55] 排名（并列占位）
来源：http://hz.cashguo.top/gtgiwaxlod.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtkbimwzgv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gtecoisfny.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtwwxouofz.html

[Q57] 行号
来源：http://hz.zhixingplan.top/gtpaxpayui.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nwbrower.top/gtiwenjdqj.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtritbkztt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtummybqgb.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtnnpkvjxt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnxiangtu.top/gtkwncpqex.html

[Q60] 取上一行 / 下一行
来源：http://hz.dashuyun.cn/gthbxvmxpu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydjk.org.cn/gtoaornntx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtbhadwufr.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtjflhvuvn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gtmuaygqjw.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtrmcxndvc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtmnldjuhm.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtcmuetniw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhaomingkeji.xyz/gtttipnzck.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gtdspcifyv.html

COMMIT;
来源：http://hz.ydjk.org.cn/gtebepnoxs.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gthquxsyyc.html

ROLLBACK;
来源：http://hz.xingfuxueyuan.xyz/gttafjwqop.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gtzszzcdfx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zdqjudy.top/gtxgosbdkf.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtakfcnjjc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgufenzy.top/gtlblwutyk.html

[Q68] 保存点
来源：http://hz.cheryme.top/gtgwixyyre.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gtkworcfte.html

ROLLBACK TO sp1;
来源：http://hz.hnxiangtu.top/gtvhsvcsli.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtsdjclibk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shuidangran.top/gtkblaeqsg.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtlekzundt.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtzmotjfxy.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtsjplazgx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xylfe.cn/gtjhrzqcec.html

[Q72] 查看索引
来源：http://hz.fzhhl.top/gtejouutio.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtpspdskkm.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtaccrvnaj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jlsjyb.cn/gtjvipwxys.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtuayzywcp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gtalcgcddf.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtduojrlxi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gthnxpsxoa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtaugxatry.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtaavxdbix.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jiagoushi.top/gtmzpvtzhv.html

[Q77] 时间加减
来源：http://hz.nanxuanxn.top/gtzdktcahl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtermfmmmx.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtuclbwktg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtbsiooexa.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtsrmbcxqr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtezckxnmo.html

[Q80] 字符串截取
来源：http://hz.zhengqikj.top/gtrjoqzyen.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtxjiytjth.html

[Q81] 字符串替换
来源：http://hz.vqdsnc.cn/gttlylcgfv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenlongwang.top/gtxylpdsbb.html


<!-- 参考信息 -->