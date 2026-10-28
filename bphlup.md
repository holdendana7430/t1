代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ppjwa.cn/gtfujtenqv.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtermtkgvb.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtzjwvkthn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtwdrzbxax.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gogol.net.cn/gtlisuoqnu.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtsxqpqfwi.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gteavixwnm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtwarvrvnf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinyuanbaomall.cn/gtnmmtvfdk.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtyxbsfakg.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtntbwgidy.html

Py:   async def f():⏎    await g()
来源：http://hz.gaohongyu789.top/gtlmahorrv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtepxhrlti.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtmwfvxgzh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtnkxtivqc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtouxqxybj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtukpboiev.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtweactuao.html

C#:   async Task F() { await G(); }
来源：http://hz.yj202588.top/gtfjqhiupk.html

[O05] 并发执行并等待全部完成
来源：http://hz.gaohongyu789.top/gtyfskochv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gtxosogdgy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gttzokceok.html

JS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtdlyxszjx.html

TS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtveptkprv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtjwxvcwdi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hysaishi.cn/gtqocrjxpx.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gttlshdmlm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtlsdxrsea.html

[O06] 使用进程池
来源：http://hz.hfpthk.cn/gtmgyqdbuu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtkxonemja.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.316326.xyz/gtlfhjoagb.html

JS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtrspulopp.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtcdgjsjqk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtgfamktai.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtsrmoivef.html

Ruby: // fork 块
来源：http://hz.xinyue.icu/gtifrlgpkk.html

C#:   Parallel.For
来源：http://hz.svipenyu.cn/gtqhkjnucv.html

================================================================================
来源：http://hz.cashguo.top/gtxnahzvtq.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtuuazhess.html

================================================================================
来源：http://hz.jyoumei.cn/gtfyjqetum.html

[P01] 生成 UUID
来源：http://hz.quarkkingdee.top/gthrapxigc.html

Py:   str(uuid.uuid4())
来源：http://hz.ivvv.top/gtjjgdzguq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtymfxwgxj.html

JS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtmpomttto.html

TS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtfcoyoaea.html

Java: UUID.randomUUID().toString()
来源：http://hz.vqdsnc.cn/gtpvqsihww.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtehwbnhei.html

Ruby: SecureRandom.uuid
来源：http://hz.tanke756.top/gtfavhkicm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hywenlv.cn/gteafwkxxi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gttwcyfako.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtrvtjajrd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gzhubu.top/gtzpmpuesi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258888.top/gtlgvwhkxv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.feifeiyinyue.top/gtzxaduons.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gtqeowdqzu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtegucimlk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zdqjudy.top/gtinbbvdei.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtaknqvgkz.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangtech.top/gtwnaplbxo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guowangkeji.top/gtxsyunass.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gaohongyu789.top/gttkkxgpvp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtisuvgxac.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtrzbtasyx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtjeuljyqp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yangfankeji.com/gtwcbmsmak.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yanxiufei.cn/gtzgruddzp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.redwolf501.top/gtnnawwiar.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtqxqqstqc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.c1oappe.top/gtzuonlfsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtuayrrepw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtjbicwmfp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtqdrsxwiu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yonumen.top/gtmxiemsxr.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtgsiitpoz.html

Ruby: x.length;  x.size
来源：http://hz.jqgufenzy.top/gttncgoagx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gogol.net.cn/gtojgjkqmr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gtztswteri.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtogpdgsje.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhixingplan.top/gtwunetgwk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtimfbnlzv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtbefxpgyg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jyoumei.cn/gtozepzllt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.svipenyu.cn/gthgqxqdju.html

Ruby: a == b
来源：http://hz.gogol.net.cn/gtklnmkmvh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtqksghmrd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.smart0.xyz/gtqreuahif.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtscnnpnxz.html

PHP:  if (empty($x)) {}
来源：http://hz.gogol.net.cn/gtrxmerzfc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gtjxdpgsaq.html

TS:   if (x == null) {}
来源：http://hz.wangdashe.top/gtvefvrcdk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtikfmdgfy.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtjlfajgqx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gtsetnvmyx.html

C#:   if (x is null) {}
来源：http://hz.hnxiangtu.top/gtrpswsppk.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtqxvfcjst.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtswvlkncw.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtlplqrims.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtsjqpczcq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtuqnrqmfm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gzhubu.top/gtdmchcwzd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtacdywysw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.haohaochexian.top/gtinzxotat.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sysykeji.top/gtjthwubah.html

[P08] 处理浮点精度问题
来源：http://hz.yangfankeji.com/gtvkiqlkrz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnqzz.top/gtnpbxozrv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.redwolf501.top/gtkxemelgc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtbcnsyplh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtvqcjzmre.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtqltukfjm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gtnliuocvu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtdixrhvgg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gtijboirlx.html

================================================================================
来源：http://hz.ybcxt.top/gtfzeqvtep.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxinkj.top/gtkeqsuqsq.html

================================================================================
来源：http://hz.jiagoushi.top/gtkknvtynl.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtnmmnvxxo.html

CREATE TABLE users (
来源：http://hz.52xcode.cn/gtibyyiplk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtkeyrswxa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtpiqfoamm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zycfv.cn/gtnquzfnog.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aizwys.cn/gtkelohfkk.html

);
来源：http://hz.daria6918.cn/gtjsfawksh.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtoavxmwqq.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtowpfzjkh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtlryfikaz.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtqgvdebcr.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtjmedzlhe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gogol.net.cn/gtyhngovir.html

);
来源：http://hz.andypj.xyz/gthxiykjvd.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtbdklufyq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yanxiufei.cn/gtitxrnxaj.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtvnxtcyvk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gtkknqcmll.html

[Q05] 重命名列
来源：http://hz.jiagoushi.top/gtcoxuxrey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.0kj1m.cn/gtiduzwppl.html

[Q06] 删除列
来源：http://hz.52xcode.cn/gtxrzscnli.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jyoumei.cn/gtmebagfol.html

[Q07] 删除表
来源：http://hz.shanyushiyangkeji.top/gtshscpprd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtxkmnsthc.html

[Q08] 创建普通索引
来源：http://hz.pycfn.com/gtgtexrfjb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtwwhiuige.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gtfbtsqixe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.haohaochexian.top/gthxmusqzy.html

[Q10] 插入单行
来源：http://hz.tianlin.xyz/gtkbamnfcx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cdnleiting.top/gtitgsiptz.html

[Q11] 一次插入多行
来源：http://hz.jqgfzy.top/gtiuudopyc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtggspuqup.html

[Q12] 插入后取自增 ID
来源：http://hz.gotoacloud.top/gtynbsyqqt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangdashe.top/gtiskclxjl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtzpurrxms.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gthssytrpi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gtomfkcvee.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtfnwbhnbo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtjfranucb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtywvvmtsq.html

[Q15] 查询全部
来源：http://hz.hammf.cn/gtsrkvrrif.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtrbtzgsgr.html

[Q16] 查询指定列
来源：http://hz.nanxinkj.top/gtjhdrsjok.html

SELECT id, name FROM users;
来源：http://hz.jlsjyb.cn/gtzbgnjcyq.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtvylmygsa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtlbggauns.html

[Q18] 模糊匹配
来源：http://hz.sweek.top/gtmkdxoksv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258888.top/gtjyjnjcmx.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gtxhshezej.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtldkyocbt.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtpcnbdcpj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gthuoiqumz.html

[Q21] 空值判断
来源：http://hz.yvedp.cn/gtmdnyobsw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtyehdplhw.html

[Q22] 排序
来源：http://hz.gzhubu.top/gtdmlhnbsv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gttcwgoecr.html

[Q23] 分页
来源：http://hz.yangfankeji.com/gtblqjraae.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.iojbl.cn/gtdtcjzjgd.html

[Q24] 去重
来源：http://hz.yj20258888.top/gtsjynbmuq.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gthfxttnxf.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtsoajjijo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtnffzhmek.html

[Q26] 计数
来源：http://hz.daxiang520.top/gtjuapbaxl.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gthsfiopmr.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtclbieifv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.quarkkingdee.top/gtsrcwrpfs.html

[Q28] 求和与平均
来源：http://hz.sweek.top/gtrnjzusyi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gttvqjtcbd.html

[Q29] 最大最小值
来源：http://hz.nanxinkj.top/gttcmjnxwt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtuxmqoami.html

[Q30] 分组统计
来源：http://hz.zycfv.cn/gtwatmdgvc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtqaordkqs.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtmgelkaot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.mhx1999.top/gtpbadonpk.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtfdgjtvnv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtcqkewiif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gttijkgjyl.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtladjvipf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangdashe.top/gtblvbmwuf.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtwgtsodxr.html

SELECT * FROM (
来源：http://hz.ehwqpu.com/gtiddiwvax.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinyuanbaomall.cn/gtrxyfzoie.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtdidxvgvp.html

[Q35] 内连接
来源：http://hz.chenjidiqi.icu/gteyocflgz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.meibo888.top/gtrzufvfdl.html

[Q36] 左连接
来源：http://hz.nanxinkj.top/gtmewinmta.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtxvxnbzbc.html

[Q37] 右连接
来源：http://hz.ehwqpu.com/gtpkhtkkzg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gaohongyu789.top/gtwkcrqxwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shzxlz.cn/gthmckjukh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtkvtenonn.html

[Q39] 自连接（查上下级）
来源：http://hz.sufxvd.cn/gtcbjazymz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yangfankeji.com/gtiewkrrnc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhijiandao.cn/gtxorpdxss.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtsqsojrjz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj202588.top/gtpwvankek.html

[Q41] 多表连接
来源：http://hz.hywenlv.cn/gtbhefpuub.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xingfuxueyuan.xyz/gtcixvyhuc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydjk.org.cn/gtjxqqsnpx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtowycacno.html

[Q42] 连接条件附加过滤
来源：http://hz.aibaodan.cn/gtahgaavlf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gthmgsxotb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtcfhwvszs.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtkhwmhqya.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shzxlz.cn/gtolngycih.html

[Q44] IN 子查询
来源：http://hz.jqgfzy.top/gtyrdugadm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigufen.top/gtslxylyeo.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gteprwenel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtvbnalvqo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtbczdrqsc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtrjenvafv.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtqwjewsvr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zycfv.cn/gtjrhhbcyu.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtzqdttbll.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gtumttgpds.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtjetigwwj.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtmrzdidlx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtrchkplnd.html

[Q50] 批量更新
来源：http://hz.hysaishi.cn/gtzrpxpaov.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtwbtpnkde.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtsdybytus.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.snrcjt.cn/gtcxtydviu.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtefygwliq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtykgvwtdh.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtvnbgifpc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtbcizmrxl.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtqvsrhcdi.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtklscswpr.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtytsrxsoo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtjakmtviv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtqscfrtyl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtjgdmfrrq.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtixdnlxlw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258.top/gtucnflklr.html

[Q58] 累计求和
来源：http://hz.snrcjt.cn/gtlppmxuys.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtcnavlkbm.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtgyftqmsj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtfkfqrcfl.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtfoyyvfnk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtmapyfmho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gaohongyu789.top/gtpwyzkpek.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtohwftdzo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtkuoucqxz.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtcsdqlxmf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtqywskyxh.html

[Q63] 开启事务
来源：http://hz.kuanghao11.cn/gtmisehdzx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtmxupvzww.html

[Q64] 提交事务
来源：http://hz.ydjk.org.cn/gtpmfajzfp.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtvjacydwd.html

[Q65] 回滚事务
来源：http://hz.snrcjt.cn/gtpslynann.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtbpzxtnfa.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtwiwejilw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xylfe.cn/gttiqqaxqo.html

[Q67] 设置隔离级别
来源：http://hz.fengsongda.top/gtgkwebpuo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtyuvkgupd.html

[Q68] 保存点
来源：http://hz.pycfn.com/gtdslhmmed.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtqxgqcprc.html

ROLLBACK TO sp1;
来源：http://hz.aibaodan.cn/gtksnzfoju.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gtspqtubsd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtpvjjnatz.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtehthqtlm.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtnfkrtosl.html

[Q71] 查看建表语句
来源：http://hz.ybcxt.top/gtzcnjcgyz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtfhwedgvh.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtlfcpcffo.html

SHOW INDEX FROM users;
来源：http://hz.xuetiantiany.cn/gthymwlxez.html

[Q73] 查看表状态
来源：http://hz.bjfxy.top/gtxzaxxqaw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yvedp.cn/gthovywyac.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtfztfwkie.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zdqjudy.top/gtaekjyqjv.html

[Q75] 日期格式化
来源：http://hz.iojbl.cn/gtltwafirh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shzxlz.cn/gtmldilpxf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuetiantiany.cn/gtcqddiwjq.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtnhuxtfjp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.vqdsnc.cn/gtaejqbxup.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtkqclwtuf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gtlucfmjfd.html

[Q78] 当前时间
来源：http://hz.zdqjudy.top/gtzynhicgv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtjnkyneyz.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gtfbzkgrdx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gtffxmtldw.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtakkzfkft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtjulbjtvh.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtrbexbeaf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtenjzodyn.html


<!-- 参考信息 -->