代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtwdrewzzx.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtylbtfpsf.html

Py:   with lock: shared += 1
来源：http://hz.zhiwuduotai.top/gtayyeedvf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.c1oappe.top/gtmcuivixf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxinkj.top/gtdhifnhfw.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtogydlvwd.html

Java: synchronized (this) { shared++; }
来源：http://hz.ivvv.top/gtxcpbilgl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shzxlz.cn/gtcrkcwtfb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtsyshdpxh.html

C#:   lock (gate) { shared++; }
来源：http://hz.cashguo.top/gtqlyuerdo.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtvczhtdib.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtaxyrmvce.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhongyouzk.top/gtjyzglrpf.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gtffjfkdho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.52xcode.cn/gtgmtjbaic.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj202588.top/gtishufcci.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhoulong.xyz/gtnsavzlpc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jianghu66.top/gttirgcdcn.html

C#:   async Task F() { await G(); }
来源：http://hz.birdmap.top/gtsbxyrblb.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtqrhjxnlu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ywan-chungtsiang.top/gtpkzcpfjs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtxnsbpbkc.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtkvrddjjv.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtusaxfprj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtqtzxidff.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shangyingyoupin.top/gtmpivtzcd.html

Ruby: threads.map(&:join)
来源：http://hz.hnqzz.top/gtvdkzetmb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhixingplan.top/gtzvyileaw.html

[O06] 使用进程池
来源：http://hz.snrcjt.cn/gtoazmkhik.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xylfe.cn/gtaguskwml.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtofsmbzwb.html

JS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtqvjkacjz.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gttopfxpyw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhixingplan.top/gtjrxugatt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtptvqvpgu.html

Ruby: // fork 块
来源：http://hz.wangdashe.top/gtnoartoiv.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtfblsxijt.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlmzuefsu.html

P. 常用工具函数
来源：http://hz.sweek.top/gtcjewllmm.html

================================================================================
来源：http://hz.fengsongda.top/gtldkqpyxg.html

[P01] 生成 UUID
来源：http://hz.quarkkingdee.top/gtwkbxcwtk.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtiqtvavlj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtfqjyrvqw.html

JS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtffzuxxdt.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtywgdgvqg.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtkvpfkmzj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtmpaipxvs.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gteixmexqf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gaohongyu789.top/gtjkshbdjf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtrjeobaty.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtboieruct.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hammf.cn/gtwwztqubl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yongpay.top/gtmwgdvbzg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gthklpdwcb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gtjkgcccny.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangshuangyany.cn/gtilzqghop.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtzmtkompp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gtunekhxri.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gtwbfxcvfd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gthszrhquz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtvlhucbol.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtocxabtgd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtrluatymm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.9152youxi.cn/gtosbdktos.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtywmikvel.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtwofbedwg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gttljhvczy.html

[P04] 求长度
来源：http://hz.quarkkingdee.top/gtxdeolijg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cdnleiting.top/gtswwdbcjw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtgbaxqgqy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtgeaeguom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtfstxjqou.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ybcxt.top/gtcudqywkz.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtnocnbfyr.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtmxzunmby.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtbwtgbvwn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.svipenyu.cn/gtairagxsv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hammf.cn/gtoahpmopj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.andypj.xyz/gtniehrqze.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gtbrljovyn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtugntzlti.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtrptbcgef.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtfucrwcub.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtzltbqxtg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtsaojyitf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtggdnqsrn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cqqwz.cn/gtewspzbaq.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtzhgviuny.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtyinxbdxw.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtwmphnphc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtciooqrha.html

Go:   if x == nil {}
来源：http://hz.sysykeji.top/gtzpmiofyo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtbhhctfmf.html

C#:   if (x is null) {}
来源：http://hz.jinghuilouyu.cn/gtskvgarwm.html

[P07] 防抖与节流
来源：http://hz.iojbl.cn/gtkuyuzkwi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangdashe.top/gtevaunxeg.html

PHP:  // 手写时间戳比较
来源：http://hz.sweek.top/gtyspfxhvq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtsnylrfbq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtfribktwi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.birdmap.top/gtyldgfosc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtiezdurso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.c1oappe.top/gtsyuurbhu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yueranfly.top/gtpptfvisq.html

[P08] 处理浮点精度问题
来源：http://hz.wangdashe.top/gtxkbkiwzw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gaohongyu789.top/gtlbiwsdai.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenlongwang.top/gtioplbvjh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtncmwnvur.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gteviainvu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zdqjudy.top/gtjhfjvwdo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gtcuxibrkl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhengqikj.top/gtfmobkzvc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtgmvdcvei.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtrclokolg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aibaodan.cn/gtgrcwtdzq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwbrnpkkw.html

[Q01] 创建表
来源：http://hz.jinqigufen.top/gtejuykasf.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtxixittkm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gtwuucqgbv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtkusczwql.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtgvhjqwfn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtvicnafed.html

);
来源：http://hz.birdmap.top/gtqrbtuljl.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtnemtloew.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gtbjuwettb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtzcrklfzf.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtgnwaxmej.html

amount DECIMAL(10, 2),
来源：http://hz.aizwys.cn/gtuxbmntve.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtbvkskuwk.html

);
来源：http://hz.yongpay.top/gtbxekxnvw.html

[Q03] 增加列
来源：http://hz.hysaishi.cn/gtyhcbftwh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtdorxcksk.html

[Q04] 修改列类型
来源：http://hz.redwolf501.top/gtbawfqdgu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtgbuirxns.html

[Q05] 重命名列
来源：http://hz.yuxming.cn/gtyrpdnist.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yongpay.top/gtlorojdxr.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtjpjritml.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gtfedfkwga.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtttwohdnw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtwjjvqxes.html

[Q08] 创建普通索引
来源：http://hz.guowangkeji.top/gtsqcffavc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtbkernnef.html

[Q09] 创建唯一索引
来源：http://hz.ybcxt.top/gtwkfboirw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtsafdyree.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtcnvgiopo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daxiang520.top/gtonnlwowo.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtxdruavog.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtorlkdmlg.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtntnuecjq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gtmzcflnlq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gttvuvwbju.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtfmgzvtdw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gtpznbfqzc.html

[Q14] 存在则更新（upsert）
来源：http://hz.ehwqpu.com/gtipmsxxxv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigfzy.top/gtogoechrh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gteaifvjwf.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtsqjmzhyj.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gteisiqcgf.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtpcghwipw.html

SELECT id, name FROM users;
来源：http://hz.shzxlz.cn/gtseotontk.html

[Q17] 条件查询
来源：http://hz.shanyushiyangkeji.top/gtzmjnewgv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtgbddodzd.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtiibiarbl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ybcxt.top/gtmlxcvxfj.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gtlvvmscjz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtmsovzgkj.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtesliidim.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.bjfxy.top/gtypdsfbrr.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtnixyepkq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtxdplkatr.html

[Q22] 排序
来源：http://hz.nwbrower.top/gtbxlcxfzi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtqdvnribs.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtrjyevssr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hysaishi.cn/gtiopuvtli.html

[Q24] 去重
来源：http://hz.9152youxi.cn/gtonbpwqbx.html

SELECT DISTINCT city FROM users;
来源：http://hz.yangfankeji.com/gtpgblunsb.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtrtqtpdfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenlongwang.top/gtqpfvscsx.html

[Q26] 计数
来源：http://hz.yonumen.top/gtpvoykqte.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtswdhsjeo.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtoaicpglp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtcaqeslpd.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangtech.top/gtdylsjjoe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gzhubu.top/gtfvjhavxu.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtympyaipe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtcnivfjmq.html

[Q30] 分组统计
来源：http://hz.cqqwz.cn/gtzhdybixc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtncechvwp.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gteletwasn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.c1oappe.top/gtdvcqyhas.html

[Q32] 分组拼接字符串
来源：http://hz.xziqi.cn/gttpkqwope.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtvhcqfzpr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yongpay.top/gtluuhxgku.html

[Q33] 多列分组
来源：http://hz.yueranfly.top/gtfqwudjak.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtizetqtth.html

[Q34] 每组取第一条
来源：http://hz.dianchejie.cn/gtckomtiqy.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtwqccxscc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zycfv.cn/gtcozugeuf.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtvlrafcug.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtlybopdor.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtynzmxazn.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtoypkgaft.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtpkbfxhzg.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtybyklcgd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gtueeljsin.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jyoumei.cn/gtoolszkrk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtulblbakt.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtqybwkkxy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtaijraduq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.kuanghao11.cn/gtofyqwlvq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.redwolf501.top/gtzjxdkpai.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gtcdfsuthj.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gtkhclmoso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tianlin.xyz/gtvahelvqb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cdnleiting.top/gtrvzaeema.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtskuvnlip.html

[Q42] 连接条件附加过滤
来源：http://hz.ybcxt.top/gtzponaktm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.haohaochexian.top/gtqnvffffx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sxryk.cn/gtueqdsafe.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtahnxgmol.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nanxuanxn.top/gtihrlyjxq.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtawsrjzxd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gotoacloud.top/gtiefyiouy.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtwcymswjh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtdivtxhmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.andypj.xyz/gtkytpfcch.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtideeiaya.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gtiatrayzf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nwbrower.top/gtxchiuyyk.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gtepbhpwye.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtnowgartf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jqgufenzy.top/gtcwsouhiw.html

[Q49] 更新单行
来源：http://hz.hfpthk.cn/gtcezpxanb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuanzx.com/gtjfkrkxiw.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtgmsvypss.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxuanxn.top/gtgmtgdktx.html

[Q51] 用子查询更新
来源：http://hz.svipenyu.cn/gttpdzwwoc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sxryk.cn/gtwyrsrqbo.html

[Q52] 删除指定行
来源：http://hz.hfpthk.cn/gtrrnbmmji.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fengsongda.top/gtvabvppjy.html

[Q53] 按条件删除
来源：http://hz.yuanzhike.top/gtuxjfocac.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhijiandao.cn/gtrztmizir.html

[Q54] 清空表
来源：http://hz.ppjwa.cn/gtrziwfckv.html

TRUNCATE TABLE logs;
来源：http://hz.hammf.cn/gtjitlcugt.html

[Q55] 排名（并列占位）
来源：http://hz.pengpengdd.cyou/gtpptcpzup.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinghuilouyu.cn/gtadshhnsf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenjidiqi.icu/gtbbnjohfh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtbtpnnhkt.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtsjuizzpi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtrfxengix.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtsorlcmkc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtxsefzorn.html

[Q59] 分组内累计
来源：http://hz.jiagoushi.top/gttetskahz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zdqjudy.top/gtusigsfsc.html

[Q60] 取上一行 / 下一行
来源：http://hz.yanxiufei.cn/gtdoxktvjy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtkknurmfx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtdchhzmwb.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtgwedybba.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gtmldqijqb.html

[Q62] 分组占比
来源：http://hz.sufxvd.cn/gtzaayjnfd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtnvmloyhd.html

[Q63] 开启事务
来源：http://hz.c1oappe.top/gtcqfzzoff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.vqdsnc.cn/gtpyragddc.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gttwwwfeun.html

COMMIT;
来源：http://hz.52xcode.cn/gtrbhxqnlr.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtbxwcboak.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtazujyzrf.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gtgowgzxsg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtmeefsfol.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtznzpkshn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sweek.top/gtdqzpnnnb.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gtttkhqcrn.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtdhkztzee.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtysrohqeg.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtmlyvvzfr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj202588.top/gtjamklzst.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gthbvlhjbf.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gttbatgwmi.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtjxylqqus.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtertfpdjk.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtyromcjni.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtbtpxvwnz.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtalipxiry.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xingfuxueyuan.xyz/gtpnuldhak.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtkkyovixj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gtdlikrlwd.html

[Q75] 日期格式化
来源：http://hz.hnqzz.top/gtmbrcwwtp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gthliooiht.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtkahbwace.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtwacmuuru.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtcmcanirc.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtwquldvrq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ppjwa.cn/gtucilflta.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtvavagtmx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guowangkeji.top/gtcqseqrar.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gtkpdntpav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtsopiwwhq.html

[Q80] 字符串截取
来源：http://hz.shuidangran.top/gtjnowdkcl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtxaqjroxx.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtssoltfip.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhaomingkeji.xyz/gtsjmkztdi.html


<!-- 参考信息 -->