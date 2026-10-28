代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtcpdwnpwf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gthiikgzjc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guannengcc.top/gteoxpydxv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtdukeijjl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cucudq.cn/gtctrkkmjt.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtfbnptafg.html

Py:   with lock: shared += 1
来源：http://hz.zhiwuduotai.top/gtxsrqasew.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtowxttida.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gtarkatloy.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtxqmfmbxv.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtmafgteys.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258888.top/gtrpnbzskf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtvqwvtvir.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenjidiqi.icu/gtjlzkldxw.html

[O04] 定义异步函数并等待
来源：http://hz.gaohongyu789.top/gtouddknre.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtixhietkx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtmrbgjtpq.html

JS:   async function f() { await g(); }
来源：http://hz.cucudq.cn/gtyouggorn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pengpengdd.cyou/gtzmpsayfa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sysykeji.top/gtewhjvfho.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yongpay.top/gtulapsgml.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtlnvxwzye.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gtjbecsvvp.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtcxotiefw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydjk.org.cn/gtrqsykmoc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gtapbuukiq.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtpydnzpgm.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtburzlrzb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtlwgsshrl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtcvbsknyt.html

Ruby: threads.map(&:join)
来源：http://hz.hnxiangtu.top/gtyjrsdhsn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gteonaakup.html

[O06] 使用进程池
来源：http://hz.yuanzhike.top/gtubsfgiua.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtubflnrzl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtvzmohwwf.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtkrxbpeyg.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtwiwsnsmg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhoulong.xyz/gtitqitfpz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtszwreuwm.html

Ruby: // fork 块
来源：http://hz.smart0.xyz/gtewnfmlli.html

C#:   Parallel.For
来源：http://hz.wangshuangyany.cn/gtmftqdrpt.html

================================================================================
来源：http://hz.yuxming.cn/gtikyongqg.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtpqbnnvve.html

================================================================================
来源：http://hz.zhijiandao.cn/gtmldudtns.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gthpueeepe.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gtmxxcfffi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtxrenpqdy.html

JS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtcqxbqcdd.html

TS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtdvfnmwlf.html

Java: UUID.randomUUID().toString()
来源：http://hz.aizwys.cn/gtprhnuyeq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhaomingkeji.xyz/gtscqtnkng.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtjuauller.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtdmnpmnkj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtujzbkauq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ehwqpu.com/gtoksecuja.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtowxnnaws.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pycfn.com/gttctmpurj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtejfanpkt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtgdmcxzrk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gtlnnrajcb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtxftibteg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtggytjqvv.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtybfycxpf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gthghigkwy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yangfankeji.com/gtzhnubmnb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtcfrpcauc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gteexglxcn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fengsongda.top/gtnwwyptvz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtoxmcdoaf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnxiangtu.top/gtnpfkmtpy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258.top/gtrfcborno.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gtqxzsmjep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.haohaochexian.top/gtphrvhbsk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtmqezsjtu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtoiatsuxg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.iojbl.cn/gtpcohvigr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtkhgacrib.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtlivoghic.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtmabakoxn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtfsrxpcxn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuanzx.com/gtpregrkke.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aibaodan.cn/gtvvidulpy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtmzqpmvhn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.c1oappe.top/gtuoxsmxxf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtmmudpxte.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gotoacloud.top/gtfoqdnbdp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnqzz.top/gteqrkcjbh.html

Ruby: a == b
来源：http://hz.iojbl.cn/gtpszfxmeb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gttxqmhmag.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtqxnnrqmp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtevpuegcj.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gtyighrzhx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtalchrxtn.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtqiootcay.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gtxvfeywcz.html

Go:   if x == nil {}
来源：http://hz.jinghuilouyu.cn/gtvnwbpkph.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtjsolcghy.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtvukmpkqb.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtoscylkwy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtapnuenxh.html

PHP:  // 手写时间戳比较
来源：http://hz.jiagoushi.top/gtmwtmucth.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gthlifaikd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtaolibvul.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gtkobtpipm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtrhszeihx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gogol.net.cn/gtfixcmykl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dianchejie.cn/gtuesjkcrn.html

[P08] 处理浮点精度问题
来源：http://hz.hnxiangtu.top/gtawdittyx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtfcuqeoyt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sysykeji.top/gtrkhfhntl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gtrpldontg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sysykeji.top/gtnlacdcfs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtswfnxylo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guowangkeji.top/gtmwzjzaxq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hongshengwenyu.top/gttnxwcvgq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtujxtyxxi.html

================================================================================
来源：http://hz.ybcxt.top/gtnmkhczyr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtcpijhgtf.html

================================================================================
来源：http://hz.birdmap.top/gtdgubmjyt.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtnrqvmnln.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtoxzlzloh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gtuoquhjww.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hfpthk.cn/gtrgyuggqy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ppjwa.cn/gtwsvieijf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gttnastrbt.html

);
来源：http://hz.ivvv.top/gtakdbaaad.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtzwlbcksd.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtkpcqmmsz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtrgofiapm.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gtwgjsdert.html

amount DECIMAL(10, 2),
来源：http://hz.yongpay.top/gtkodkeucp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtkmlsiexq.html

);
来源：http://hz.xuetiantiany.cn/gtxocnxwce.html

[Q03] 增加列
来源：http://hz.ppjwa.cn/gtwgzwqaoo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtwaydlwvp.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gttzrdjdmd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtmvryscjy.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtbitxblpv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtxmwljxnn.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtmwrzqxgl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtwlktlbzw.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtnrfbtldb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fzhhl.top/gtrwobxbgv.html

[Q08] 创建普通索引
来源：http://hz.yj20258.top/gtlyoywobt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtyblrwdmj.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtdfovqmay.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtxkcfpmgj.html

[Q10] 插入单行
来源：http://hz.jianghu66.top/gtrfxrhwkt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtdxwbjmxy.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtjezukytt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ehwqpu.com/gtsnykufbw.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtlqpezhce.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuanzx.com/gtkvoeadzu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtprphhdsr.html

[Q13] 忽略重复插入
来源：http://hz.kuanghao11.cn/gthfbyemvx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenjidiqi.icu/gtxnfknayf.html

[Q14] 存在则更新（upsert）
来源：http://hz.yonumen.top/gtonaselsy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sufxvd.cn/gtgqscjvuq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtgfgtzvdk.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gtzpooflhq.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtzirprnye.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtlsfsoloj.html

SELECT id, name FROM users;
来源：http://hz.meibo888.top/gtbqnymiuo.html

[Q17] 条件查询
来源：http://hz.redwolf501.top/gtltrfcgmf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtsfdbydui.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtailxlbtg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtchoznocw.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gthdutpbrm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.haohaochexian.top/gtdbypotvr.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtplzpzues.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cheryme.top/gtmobqvaby.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gtqrrcmwzh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtmtblcbcp.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gtxvkvkurm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtrrhfuegy.html

[Q23] 分页
来源：http://hz.yj20258888.top/gtpiuabzqu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigufen.top/gthvvawilz.html

[Q24] 去重
来源：http://hz.feifeiyinyue.top/gtnblmjgoj.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigufen.top/gtcrqbiydt.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gtwrvjivwv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhijiandao.cn/gtkepsmhob.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtkmkootua.html

SELECT COUNT(*) FROM users;
来源：http://hz.dianchejie.cn/gtddmuoiro.html

[Q27] 条件计数
来源：http://hz.cqqwz.cn/gtgbadzmvx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ppjwa.cn/gtszqzqgum.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtghnqycjs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.snrcjt.cn/gtoontwhsm.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gtellepgyk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.smart0.xyz/gtswejfeuu.html

[Q30] 分组统计
来源：http://hz.ywan-chungtsiang.top/gtgekryoze.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtbfscutfk.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtaxesduvd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hysaishi.cn/gtnjwohknw.html

[Q32] 分组拼接字符串
来源：http://hz.0kj1m.cn/gtemrvhxfz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtqkjyctff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtzkxkosrs.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtysuxjzgq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtcdorelxw.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtinpdtbam.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtmetbhqye.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtyrrmjklm.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtwgryfqec.html

[Q35] 内连接
来源：http://hz.sxryk.cn/gtujirznad.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtxfwaebyy.html

[Q36] 左连接
来源：http://hz.chenlongwang.top/gtawqlwitc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gthjlhbxze.html

[Q37] 右连接
来源：http://hz.yuanzhike.top/gtnbtvyupe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtlrvjtsup.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ivvv.top/gtpjjfyvxi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gtstshmhib.html

[Q39] 自连接（查上下级）
来源：http://hz.haohaochexian.top/gtfigwqqon.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtvoifjftv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nwbrower.top/gtsrdtcgry.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.meibo888.top/gtqkbdkwbe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.c1oappe.top/gtuvotktze.html

[Q41] 多表连接
来源：http://hz.9152youxi.cn/gtvduvjdlo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jianghu66.top/gttwpflpul.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gtkhmwkywq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cdnleiting.top/gtigrwafqm.html

[Q42] 连接条件附加过滤
来源：http://hz.jyoumei.cn/gtdimsvild.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtpclzaocb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gttvdqzizk.html

[Q43] 标量子查询
来源：http://hz.jyoumei.cn/gtefosklcx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xinyue.icu/gtlmfwakrr.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gtyaonkfcb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtnyanaamd.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtubjtmysd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtsjrxnmwl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gtagmtnhrr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtexvemtgq.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gtvdnapmjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gtcoequpez.html

[Q48] CTE 公用表表达式
来源：http://hz.guowangkeji.top/gtbcspsoce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.feifeiyinyue.top/gtkzbkdscq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtrfgcsmjn.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtmgrrmnjf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtfdlsujfw.html

[Q50] 批量更新
来源：http://hz.yanxiufei.cn/gthsuihcag.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgufenzy.top/gtyjfvvmrw.html

[Q51] 用子查询更新
来源：http://hz.0kj1m.cn/gtyzmysluz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuanzx.com/gtlobguqxg.html

[Q52] 删除指定行
来源：http://hz.xuanzx.com/gtopyvxqan.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtratsvzcp.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtvbdgovsg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangkeji.top/gtwetqgifg.html

[Q54] 清空表
来源：http://hz.sufxvd.cn/gtfzjsmqoa.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtxbeeueks.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtjcfcgzhc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.vqdsnc.cn/gthuzbtpve.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnqzz.top/gtowbqvdoc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gturbdlgxy.html

[Q57] 行号
来源：http://hz.yj202588.top/gthgicdnvr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtuvqxquwl.html

[Q58] 累计求和
来源：http://hz.redwolf501.top/gtmeyqxydh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gotoacloud.top/gtgrtfjtzj.html

[Q59] 分组内累计
来源：http://hz.ydjk.org.cn/gthvvfbmtd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cqqwz.cn/gtqoftfuvi.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gthdwfgwcm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.redwolf501.top/gtjckpoelf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtbdjllhwv.html

[Q61] 移动平均
来源：http://hz.hnxiangtu.top/gtiuxrkecq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cheryme.top/gtuypprvhf.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtzrqdyjat.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtmwvjlljn.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtquygsnmd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yongpay.top/gtfxmptuvw.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtmgudhdqd.html

COMMIT;
来源：http://hz.nwbrower.top/gtrfxxwzre.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtpoombilx.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtcmzbdojd.html

[Q66] 行锁查询
来源：http://hz.hammf.cn/gtzqjvpqaw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtjquxtvtl.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gtjnudqlce.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gthjujsbdu.html

[Q68] 保存点
来源：http://hz.jlsjyb.cn/gtwkojxpdy.html

SAVEPOINT sp1;
来源：http://hz.smart0.xyz/gtdfxwmvrm.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtasoezknc.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtvlbmkjvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cashguo.top/gtpavatluh.html

[Q70] 更新统计信息
来源：http://hz.fengsongda.top/gtopfksnvm.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtpdzavqzx.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtgeiihiiv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxinkj.top/gttqezhgmg.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtanfhykex.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtzktysurf.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtelajdscm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shangyingyoupin.top/gtuzbxfpto.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtqtxuhupg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gttmaihlqi.html

[Q75] 日期格式化
来源：http://hz.havefunace.top/gtajkxabrx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtovfghqyt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gtxcjspcmi.html

[Q76] 按天统计
来源：http://hz.cashguo.top/gtzdprpdef.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydzc1.top/gtxhcrcebp.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtnygcqmqq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xziqi.cn/gtouigtukz.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtocrcnbdn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258.top/gthssjmfch.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gtxeugxgsy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.quarkkingdee.top/gtbqxxeflz.html


<!-- 参考信息 -->