代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtrzutazrz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gtcqjucnyh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gtrkwhfeqq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtvjuzuzyi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.0kj1m.cn/gtyqxrmbct.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtizvpjwob.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtvdlhiizv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtdebzadeh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hammf.cn/gtqgegckod.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtpbtuzmdk.html

Java: synchronized (this) { shared++; }
来源：http://hz.snrcjt.cn/gtgsfdgfaj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj202588.top/gttgpkqlzr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gtyufvckhy.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gttzcfdcwc.html

[O04] 定义异步函数并等待
来源：http://hz.gotoacloud.top/gtkfxtbakt.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtabyuikgz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tianlin.xyz/gtvyercbbt.html

JS:   async function f() { await g(); }
来源：http://hz.xuanzx.com/gtofokuoiu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.snrcjt.cn/gtbimbxnru.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtsmiunxwx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtgcrzgrtc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gtichhbrat.html

C#:   async Task F() { await G(); }
来源：http://hz.ydjk.org.cn/gtlofirekx.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtbgqwbpkb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtpdpyxuko.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtjahubuxd.html

JS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtjhlvzyqq.html

TS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtywhzntnp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtwhpzkwbc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinyuanbaomall.cn/gtschpvluz.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtgwoeenkj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gaohongyu789.top/gtqmsoycud.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtbbpbmvoa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gaohongyu789.top/gtgqitpbsj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hammf.cn/gtsxknyhtc.html

JS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtffhztnrn.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtifuntttd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tianlin.xyz/gtzhyikhmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhijiandao.cn/gtwmkxoeum.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtibnysxmt.html

C#:   Parallel.For
来源：http://hz.shanyushiyangtech.top/gtqqmuazxt.html

================================================================================
来源：http://hz.andypj.xyz/gtjtvuloxn.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtvdjmoxal.html

================================================================================
来源：http://hz.zdqjudy.top/gtowtoliss.html

[P01] 生成 UUID
来源：http://hz.zhoulong.xyz/gtvdxstnuf.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtvdtoaygw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenzaomai.com/gtjlpzvubf.html

JS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtzwlhifrn.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtafbqdcwl.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuanzhike.top/gtmvadpvmi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtdkkqhyyy.html

Ruby: SecureRandom.uuid
来源：http://hz.xuanzx.com/gtyjinggym.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ybcxt.top/gthcpxiyxi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yueranfly.top/gtgtlwaozu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cucudq.cn/gtvuavzlbt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gtwwwjcfnt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtgnlwfnvj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxuanxn.top/gtcbzwdlqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtrrsokefp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtuezdablz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtusmlsscb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daria6918.cn/gteylyvfqe.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gttxinbxvk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtqwavziub.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtrvrewivt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtzcvlwggr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtcsukrjzp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ppjwa.cn/gtbfkhofpq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtjodlfdrx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shangyingyoupin.top/gtwgdnqmhx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtfydpqslu.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtlrzyfeeh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xziqi.cn/gtmzlnjgkj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtgwcaxqrw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtgyaoqjff.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtvxypknhm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.feifeiyinyue.top/gtgykkuniv.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtaedxflrq.html

Ruby: x.length;  x.size
来源：http://hz.zhoulong.xyz/gtubttlakw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gtpukqahpj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtntaprmzc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtbvguqjxd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yueranfly.top/gtsdxbfoss.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.bjfxy.top/gtzrclhqcj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtfreuvush.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.vqdsnc.cn/gtzpvlqaow.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ppjwa.cn/gtxcdclzkg.html

Ruby: a == b
来源：http://hz.redwolf501.top/gtdhlmeqsb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gtfmniwzbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtkefhkzon.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtucgvvrmm.html

PHP:  if (empty($x)) {}
来源：http://hz.shangyingyoupin.top/gtuyuhduyr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtavlefqbl.html

TS:   if (x == null) {}
来源：http://hz.jqgufenzy.top/gtouomqfcl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gtwtgbmijc.html

Go:   if x == nil {}
来源：http://hz.snrcjt.cn/gtnhfradbr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sxryk.cn/gtyksqbfwy.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtwwtqevry.html

[P07] 防抖与节流
来源：http://hz.chenjidiqi.icu/gtnfcpwaai.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangkeji.top/gtpvkjsblm.html

PHP:  // 手写时间戳比较
来源：http://hz.gotoacloud.top/gtnoeooxpj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtnegtmkds.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtfahpbsep.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtjptibcac.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtprenfjzy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gaohongyu789.top/gtbvvhezcp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtkdjgshcd.html

[P08] 处理浮点精度问题
来源：http://hz.yuxming.cn/gtnnjzuuko.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtsyjquuqp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.52xcode.cn/gthryokvuz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtpsajcfdr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gogol.net.cn/gtnxpdqilg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sxryk.cn/gtlikhmpcg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sysykeji.top/gtanxqtwzr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtsnujahue.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtkvrcbltj.html

================================================================================
来源：http://hz.hysaishi.cn/gtpveptrer.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtrlxsxkil.html

================================================================================
来源：http://hz.tian-w.cn/gtmypgwgtf.html

[Q01] 创建表
来源：http://hz.cashguo.top/gtzkikxrwi.html

CREATE TABLE users (
来源：http://hz.meibo888.top/gtudsymqpu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtamdxwccf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigfzy.top/gtpxyrlptk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtxohbugeb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ywan-chungtsiang.top/gtivgoduam.html

);
来源：http://hz.chenjidiqi.icu/gtpfsifwbq.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtqdsftomt.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gtltzgvrac.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gthmhxtvpa.html

user_id INT NOT NULL,
来源：http://hz.tanke756.top/gtysifikks.html

amount DECIMAL(10, 2),
来源：http://hz.mhx1999.top/gtzkvqzcxt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tianlin.xyz/gtnkomuenf.html

);
来源：http://hz.jiagoushi.top/gtswxmwrsd.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gtjxwpfila.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gtpsnwpseo.html

[Q04] 修改列类型
来源：http://hz.yj20258888.top/gtslqatueu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guannengcc.top/gtrbbofqbc.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtblsiyfzt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.pycfn.com/gtvruhjbem.html

[Q06] 删除列
来源：http://hz.ivvv.top/gtkmtgnumh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cdnleiting.top/gtlnqirrxl.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtycssawcy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cqqwz.cn/gtovmdfvgx.html

[Q08] 创建普通索引
来源：http://hz.hnxiangtu.top/gtctxxibem.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hammf.cn/gtwgnmthhq.html

[Q09] 创建唯一索引
来源：http://hz.gotoacloud.top/gtsypfwamk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtgzocwxbs.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtvzomeifo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gtpxiunldt.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtjwtljsws.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hfpthk.cn/gtoiizcnbk.html

[Q12] 插入后取自增 ID
来源：http://hz.vqdsnc.cn/gteaxenfez.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gteceapmrd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtxykhwvot.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtzuqrxfma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gttqgwqpgd.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtshfsemnv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhixingplan.top/gtrwuhleqc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zycfv.cn/gtqojgqipl.html

[Q15] 查询全部
来源：http://hz.pycfn.com/gtkhrkynyc.html

SELECT * FROM users;
来源：http://hz.jqgufenzy.top/gtewmrimye.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtdigvjbmx.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtrcymclqz.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtbrmiogdr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tianlin.xyz/gtvlqaltkg.html

[Q18] 模糊匹配
来源：http://hz.xziqi.cn/gtckjetplg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xziqi.cn/gtlpfrudms.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gthypqcfty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yangfankeji.com/gtrbfqwkhj.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtfwzvbqgv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guannengcc.top/gtnwuttsnt.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtjwhhcunh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.smart0.xyz/gtnsonkwrq.html

[Q22] 排序
来源：http://hz.gogol.net.cn/gtrflqmjsr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtqkjosgfi.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtvshpnnjy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gteqjjilmi.html

[Q24] 去重
来源：http://hz.nanxinkj.top/gtopcilgma.html

SELECT DISTINCT city FROM users;
来源：http://hz.ivvv.top/gtkrhqutci.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtmihabput.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuxming.cn/gtljwsjjeq.html

[Q26] 计数
来源：http://hz.shzxlz.cn/gtajqjptzu.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258888.top/gtxjqgpsmp.html

[Q27] 条件计数
来源：http://hz.xziqi.cn/gtveadwsac.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtpmjsmjin.html

[Q28] 求和与平均
来源：http://hz.zhiwuduotai.top/gtlbjnsqdd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtuxoqkexi.html

[Q29] 最大最小值
来源：http://hz.daria6918.cn/gtiqfurybm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtimfciywr.html

[Q30] 分组统计
来源：http://hz.hnxiangtu.top/gtulbtkglo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gthyrrqjfm.html

[Q31] 分组后过滤
来源：http://hz.meibo888.top/gttpscqjqq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.9152youxi.cn/gtblliqskp.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtvccetjks.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtaeyinfew.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shangyingyoupin.top/gtabjbypxu.html

[Q33] 多列分组
来源：http://hz.fengsongda.top/gtgimhyawh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hfpthk.cn/gtppesyybv.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtcpbtgwca.html

SELECT * FROM (
来源：http://hz.yj202588.top/gtbyaqpijk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zdqjudy.top/gtkbcvykby.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtegrezbic.html

[Q35] 内连接
来源：http://hz.yongpay.top/gtrwdiyssk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtxrbipxmf.html

[Q36] 左连接
来源：http://hz.haohaochexian.top/gtzghggenf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtzrwignkt.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gtjjhrwjtn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtafaaoclk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtdkpuyaqv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jiagoushi.top/gttojkmxgk.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtzlenehnu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtkqpnzsfk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtyssmxvmu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hongshengwenyu.top/gtonyydnir.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtrcezdbai.html

[Q41] 多表连接
来源：http://hz.ybcxt.top/gtfsmwydst.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xylfe.cn/gtcbzxfzjr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gzhubu.top/gtadipbiyi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtosasurln.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtcavgjoua.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hongshengwenyu.top/gtgfvhyhng.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtxworxabb.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gtgtamvktl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gtshlaxxcq.html

[Q44] IN 子查询
来源：http://hz.yongpay.top/gtqsuokbde.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtshzhcujs.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtiwwyyixz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtjyijobfg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tianlin.xyz/gtwsewgrqm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtdbnrtnpv.html

[Q47] 与平均值比较
来源：http://hz.yj20258888.top/gtmbyreccp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtojoysewu.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gtlhdmdzzr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtbgivrhat.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ywan-chungtsiang.top/gtzwwiqzgv.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtsugqjdac.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtqntlnbkg.html

[Q50] 批量更新
来源：http://hz.cdnleiting.top/gtkgmotnsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtxloqlwvo.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtughdpogs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtjkuhsrbq.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtpzccuubx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtouygzyeo.html

[Q53] 按条件删除
来源：http://hz.smart0.xyz/gtcrbxkxxx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtqvaiptgv.html

[Q54] 清空表
来源：http://hz.ybcxt.top/gtysottnwc.html

TRUNCATE TABLE logs;
来源：http://hz.yj202588.top/gtreatcmvu.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gtzhkhctar.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xingfuxueyuan.xyz/gthyfwatai.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtjfglnsml.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtttactmwl.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtqiwukjsb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.52xcode.cn/gtfurixjjn.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtpolrxbaa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gtkgxffeap.html

[Q59] 分组内累计
来源：http://hz.zhiwuduotai.top/gtrjtlqpjd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tian-w.cn/gtyafxyqqj.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtyorwxbto.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xylfe.cn/gtpdwyhvtu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhengqikj.top/gtzobzgkug.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtwpsrablg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tianlin.xyz/gtdtkhnxzx.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gthqrdvmxa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtdmwgfqbq.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtrusdrrnh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtgaffpuvs.html

[Q64] 提交事务
来源：http://hz.aizwys.cn/gteercsykr.html

COMMIT;
来源：http://hz.havefunace.top/gtwlibnwkc.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtlkrhmdrk.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtnmngxsqe.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtccsnfmiv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yueranfly.top/gtzhkkiqze.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gtirepivrl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtfnxtngkl.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtoufrnpey.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtbynmdpcn.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtysrssczy.html

[Q69] 查看执行计划
来源：http://hz.pycfn.com/gtpcbejwtp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gtteapducb.html

[Q70] 更新统计信息
来源：http://hz.meibo888.top/gtyfktmtlw.html

ANALYZE TABLE users;
来源：http://hz.pycfn.com/gtismyuojy.html

[Q71] 查看建表语句
来源：http://hz.yj20258.top/gtdtbqdqni.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtcyozmrox.html

[Q72] 查看索引
来源：http://hz.sysykeji.top/gtpsiakevd.html

SHOW INDEX FROM users;
来源：http://hz.mhx1999.top/gtewlwqjio.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gthxnpatdn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.quarkkingdee.top/gtzilaudeu.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtegdfsvsw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gttghjebvq.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtwvqznzll.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtzmjpixjw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cdnleiting.top/gtnvonnauy.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtqyzedmne.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtkylpsvtf.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtqhsmkdjz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtfsflyvhi.html

[Q78] 当前时间
来源：http://hz.kuanghao11.cn/gtjbfrbilu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tianlin.xyz/gtkriziqgr.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtfrqxuqne.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtzvbtrgtb.html


<!-- 参考信息 -->