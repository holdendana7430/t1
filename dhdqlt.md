代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtipzzoebf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sxryk.cn/gtcxzjvfee.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gtfvwxpedo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtoitdbwcw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtqralcems.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gtrwietxhw.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtxxprjlnu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gtxbuwkcar.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fengsongda.top/gtkedtmdvb.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtgjmkkeld.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gthqistiab.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtqaobrcmh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cdnleiting.top/gtoxpnsfos.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtciuqkyoq.html

[O04] 定义异步函数并等待
来源：http://hz.zdqjudy.top/gttrmvnerc.html

Py:   async def f():⏎    await g()
来源：http://hz.zdqjudy.top/gtpzhsizkc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ybcxt.top/gtxkxohfgf.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtciyascmq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtmkixojkn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuetiantiany.cn/gtmkrrfxrc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zdqjudy.top/gtwgbhlmuy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ywan-chungtsiang.top/gtgwnpuhkm.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtjqyqonnw.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnxiangtu.top/gtpqvbtfab.html

Py:   asyncio.gather(*tasks)
来源：http://hz.kuanghao11.cn/gtyrriknfb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gteajrpcrr.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtpoxdbucv.html

TS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtcereavoj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtxrutmawj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.52xcode.cn/gtgkhxkkhx.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtukxodymf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jiagoushi.top/gtjedhvpvy.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gtfdebipmo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtanzlscfu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtkhrfoyba.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtpsjkfsvi.html

TS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtpkjxrsse.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guannengcc.top/gtelepycup.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gtfrgtrhyp.html

Ruby: // fork 块
来源：http://hz.zhoulong.xyz/gtmhlacujj.html

C#:   Parallel.For
来源：http://hz.redwolf501.top/gtmpruhxgx.html

================================================================================
来源：http://hz.smart0.xyz/gtylmiojzm.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtgfsjmkeb.html

================================================================================
来源：http://hz.jiagoushi.top/gtjcmzpiys.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtkokbooah.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gtlwnzunaz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuanzhike.top/gtyfcwtjvt.html

JS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtakjrpuot.html

TS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtsnzmvwge.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtyhlxsdis.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sxryk.cn/gtnbbtjjul.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtjagjlavs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guowangkeji.top/gtfmuvigjj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.bjfxy.top/gteomigmjx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtultmwykg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuxming.cn/gtdpoykrgq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydzc1.top/gtbbiwyikx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinghuilouyu.cn/gtmdmgsicf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cqqwz.cn/gtwdvjqkkw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtsvbxhgos.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtzegjqsnf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shuidangran.top/gtkrmhkqpf.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtjtjhqvtt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtdxjxtnug.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shuidangran.top/gtvrnyglze.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtorkofahp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtovcbuwhx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtloesmwdi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtnkycrkkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zdqjudy.top/gtdfbmhuno.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gticdgltex.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtnuruclyp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtedqmsfip.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dashuyun.cn/gtxtybhkqr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtdwsbiebu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtmlxtgsnu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gtnflgkgke.html

Go:   len(arr);  len(m)
来源：http://hz.tian-w.cn/gtprhjcrrs.html

Ruby: x.length;  x.size
来源：http://hz.ehwqpu.com/gtoehnfhsd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gtseeddzcp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.316326.xyz/gtvkrvdrfy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtcvmfwamy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtarleqghz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhijiandao.cn/gtpbjonycv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtpwovjvst.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtejfnwqtd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gthndevuyb.html

Ruby: a == b
来源：http://hz.meibo888.top/gtehlwngdd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtwthpuiob.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yongpay.top/gtnfuxfobt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtchrjcwog.html

PHP:  if (empty($x)) {}
来源：http://hz.pycfn.com/gtrfamfryz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cashguo.top/gtgnkdzjru.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gteebqqiqp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtnljnjwje.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtnzhafrjr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhengqikj.top/gtjpotjuag.html

C#:   if (x is null) {}
来源：http://hz.cucudq.cn/gtzgcwlubl.html

[P07] 防抖与节流
来源：http://hz.aibaodan.cn/gtluqcbuba.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.haohaochexian.top/gtdmyxpxuk.html

PHP:  // 手写时间戳比较
来源：http://hz.yj202588.top/gtydngydcr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gthiywlxyb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtonnwlrok.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtcszksowr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgufenzy.top/gtrhcdikli.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gthuaqdnrv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtjbjqfqer.html

[P08] 处理浮点精度问题
来源：http://hz.aibaodan.cn/gtpnuebgbk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtgswmlndx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtiusyehme.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tian-w.cn/gtmijcauix.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenzaomai.com/gtyoynxyje.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtfcsdccxh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtdznwgoax.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuanzhike.top/gtsvjsjxuu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinghuilouyu.cn/gtlozayjrr.html

================================================================================
来源：http://hz.smart0.xyz/gtpmxraalc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.316326.xyz/gtvohubmrg.html

================================================================================
来源：http://hz.hnxiangtu.top/gtyynnimgb.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtcdpdugpv.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gteonlgvgj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtynwmsawe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258.top/gtlzcxhcel.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtjdgjwpcm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ivvv.top/gtontsonxe.html

);
来源：http://hz.guannengcc.top/gtxmpslruv.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtjoyuagiz.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtkdqubwmc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtbklgzyqb.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtbuxzthnz.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtyzacscyj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtsbvozchu.html

);
来源：http://hz.wangshuangyany.cn/gtowodltji.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtawltcyia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtpsrxbbin.html

[Q04] 修改列类型
来源：http://hz.gzhubu.top/gthugdopgv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.meibo888.top/gtuicbaryk.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtmalitttm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shuidangran.top/gtqgzfpfkj.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtadrkdljf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yongpay.top/gtjejdwpyh.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtytrxhdci.html

DROP TABLE IF EXISTS orders;
来源：http://hz.svipenyu.cn/gtgvwdaxvt.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtjcjbtuzo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtfmkfzryu.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtklgvmnfh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yonumen.top/gtycdluuci.html

[Q10] 插入单行
来源：http://hz.ydzc1.top/gtkjslecxa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtvftslfrw.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gtgbhnmsmm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtkjuaodhm.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtpefwkerk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yongpay.top/gtliddsfgc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xylfe.cn/gtptmapkey.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtayrscpkk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xinyue.icu/gthrvicsyn.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtoxpiymxi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhiwuduotai.top/gturfulbgy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.iojbl.cn/gtergldaxd.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtgjwkdvki.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtwwncqavz.html

[Q16] 查询指定列
来源：http://hz.cqqwz.cn/gtihhbswpr.html

SELECT id, name FROM users;
来源：http://hz.sweek.top/gtrdgtogit.html

[Q17] 条件查询
来源：http://hz.gaohongyu789.top/gtrlgmgnyb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtlkekfqsj.html

[Q18] 模糊匹配
来源：http://hz.gogol.net.cn/gtvqhlpdtk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yvedp.cn/gtnewqdtxu.html

[Q19] 范围查询
来源：http://hz.havefunace.top/gthgglqoal.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtkbmllnvi.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtmfqckihy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtshlldbfy.html

[Q21] 空值判断
来源：http://hz.ehwqpu.com/gtlusacbkq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gthlqwnokq.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtulunfhhc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gtdzrwkbcj.html

[Q23] 分页
来源：http://hz.vqdsnc.cn/gtpehabogm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigfzy.top/gteeupbbzi.html

[Q24] 去重
来源：http://hz.pengpengdd.cyou/gtlnqlwubk.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtkkgeuace.html

[Q25] 只取前 N 条
来源：http://hz.jianghu66.top/gtszhxwjgw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yangfankeji.com/gtamxwjuml.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtwdcufmzi.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtnncxwerb.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtysyprizb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtpkujytfy.html

[Q28] 求和与平均
来源：http://hz.ywan-chungtsiang.top/gtjitomghi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtyguwkchd.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtgtqjwclr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yanxiufei.cn/gtchjgzwim.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtugdxlphj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtivkpevzc.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtxhtrazvk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtvpbrzaij.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtxhdpslod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtraufxzgu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhoulong.xyz/gtiptqywsi.html

[Q33] 多列分组
来源：http://hz.yueranfly.top/gtdxclutkx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtwtqbzzrx.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtvjecsbee.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtfiaskaoz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nwbrower.top/gtdwvanqlw.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtcvnvpifp.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtkunnwssv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtmxysooog.html

[Q36] 左连接
来源：http://hz.nwbrower.top/gtswufkqky.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtahmdvbbi.html

[Q37] 右连接
来源：http://hz.jqgufenzy.top/gtbtalwgeg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtigbonkia.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtgcrliwuv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.52xcode.cn/gtxdkhestm.html

[Q39] 自连接（查上下级）
来源：http://hz.shuidangran.top/gtbqtsbiup.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zdqjudy.top/gtpxauasln.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtmjwnspaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258.top/gtowjskgmw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.haohaochexian.top/gthuiniqma.html

[Q41] 多表连接
来源：http://hz.nanxuanxn.top/gtelobodse.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sweek.top/gtzhqbhhst.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aizwys.cn/gttmtcddag.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fzhhl.top/gtrihdcgeq.html

[Q42] 连接条件附加过滤
来源：http://hz.zhiwuduotai.top/gtwdhoiuhx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daria6918.cn/gtavtrdlty.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gtxemvakwv.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gthxibvyzo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtukeafodj.html

[Q44] IN 子查询
来源：http://hz.yj20258.top/gtujjswdzh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cheryme.top/gtrljtzgzf.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gtseyomcwg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtxrtklozp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shangyingyoupin.top/gtpevnnmuk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtbfcdlpia.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtbxvpypuw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtanmmpaov.html

[Q48] CTE 公用表表达式
来源：http://hz.gaohongyu789.top/gttkinxxgc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtfycmsvvt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.52xcode.cn/gtvfweaddk.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtddnpdczo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gthqibhcjz.html

[Q50] 批量更新
来源：http://hz.xylfe.cn/gtludtlojr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.iojbl.cn/gtwgswcjcp.html

[Q51] 用子查询更新
来源：http://hz.dashuyun.cn/gtzriucuar.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pycfn.com/gtqdymgwgd.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtlducoshn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtssujcxpz.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtczknxmbi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtltjfkuzg.html

[Q54] 清空表
来源：http://hz.iojbl.cn/gtgmdeegrg.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtukwdcnuo.html

[Q55] 排名（并列占位）
来源：http://hz.tanke756.top/gtzkjgybaz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtmvjhoqrw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtxoclpyww.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtoriaathd.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtppsbnxuf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gttbrnysmp.html

[Q58] 累计求和
来源：http://hz.jyoumei.cn/gtwjkeanya.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhongyouzk.top/gtobvzvitt.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gtyujskahl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxuanxn.top/gtidzxnthj.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuanzhike.top/gtivmeayoo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtwpljgizl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258888.top/gtcyqfgxqa.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtjiwuqzai.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtxzguhphd.html

[Q62] 分组占比
来源：http://hz.ivvv.top/gtioprpman.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtrhmwyddu.html

[Q63] 开启事务
来源：http://hz.jqgufenzy.top/gtmyndwkhl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinyuanbaomall.cn/gtymftqrds.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtrmqxdkcj.html

COMMIT;
来源：http://hz.shangyingyoupin.top/gtqiichrnw.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gthtchhyog.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtrrupnltd.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtcjxgbhtc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yongpay.top/gtjcolnnnl.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtqawmkskr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhijiandao.cn/gtwgjvvlmt.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtgdsneicq.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtqetefaxc.html

ROLLBACK TO sp1;
来源：http://hz.iojbl.cn/gtbrphucow.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtmsbbaydv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sxryk.cn/gtuunoedin.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gtsygamfsj.html

ANALYZE TABLE users;
来源：http://hz.jinqigfzy.top/gtbfrbwiep.html

[Q71] 查看建表语句
来源：http://hz.jyoumei.cn/gthsmselkx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dianchejie.cn/gtoviobohf.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gtkochrzuu.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtuycjyprt.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtlarfrdxl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtkkfznhmg.html

[Q74] 强制使用索引
来源：http://hz.fengsongda.top/gtsvffzaqi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtvcscswec.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtewoocwag.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtuepfjztq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtsrhpnpqs.html

[Q76] 按天统计
来源：http://hz.xuetiantiany.cn/gtwntzoxna.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtdtgsbuds.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gtexdddfli.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtkmqwtmgi.html

[Q78] 当前时间
来源：http://hz.hywenlv.cn/gtzdcurzvw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhaomingkeji.xyz/gtavbdxgis.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gtqbiyfmfh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtdfribwxu.html


<!-- 参考信息 -->