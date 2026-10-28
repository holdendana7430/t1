代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.andypj.xyz/gtolipobwk.html

Go:   go f()
来源：http://hz.c1oappe.top/gtvkdzwuoj.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gtvfunfpjf.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtdwdmsypx.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtegivbfqt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtwgbrqscn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtvslrlugm.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtnxrtjyma.html

TS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtubiczjgz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yonumen.top/gtdyrjlcqc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gtinbcrutg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtywkzzetv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gthjtqmhcm.html

[O03] 加锁保护共享数据
来源：http://hz.zhengqikj.top/gtxcpykkkf.html

Py:   with lock: shared += 1
来源：http://hz.jinqigfzy.top/gtwsenbkhi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tianlin.xyz/gtcbdpzsgc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.bjfxy.top/gtrlllkkxr.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtyvmdyrur.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuanzx.com/gtzbkztisy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nwbrower.top/gtzfbjozlt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtmmuobopq.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtuwptqwuj.html

[O04] 定义异步函数并等待
来源：http://hz.316326.xyz/gtyuchctqv.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtqdexsccv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtkxjnewki.html

JS:   async function f() { await g(); }
来源：http://hz.meibo888.top/gtdaupljfj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pycfn.com/gtrolsdvqz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtswwqhfit.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtbdodjrmx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtbfazrbfz.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtjssspdsm.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtowzlckyx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gthqljxzhl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtjfhoifoz.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtdodvtuzv.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtbbhwxzjy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gtpwxhmcfs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yongpay.top/gtqlxeoypa.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtrcomgtpy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ybcxt.top/gtbxqtmzhg.html

[O06] 使用进程池
来源：http://hz.jlsjyb.cn/gtrlrdksla.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtvjpgceex.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtbfvqlwcs.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtgnagxpnc.html

TS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gthpvtfhmm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtkcrsomeo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangtech.top/gttmjmvuna.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtqdnxoajl.html

C#:   Parallel.For
来源：http://hz.iojbl.cn/gtrbjzelpx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtiinpltsv.html

P. 常用工具函数
来源：http://hz.xylfe.cn/gtcaakfzsq.html

================================================================================
来源：http://hz.quarkkingdee.top/gterghiqyz.html

[P01] 生成 UUID
来源：http://hz.feifeiyinyue.top/gtqxbukjcq.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtyhceexef.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtafyhtxpm.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtddllwxjk.html

TS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtscchefju.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtfcheoeng.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtruzckptj.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtjwxbfrbt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ppjwa.cn/gtensfkeab.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cdnleiting.top/gtjgxikbdw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.dianchejie.cn/gtkzuurgvk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gtxzazpeat.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtxmowtfkj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cucudq.cn/gtdzrlgffl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yueranfly.top/gtorgujtdb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtdwprkiqs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sxryk.cn/gtxpvvhxub.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangdashe.top/gtsrdldqov.html

[P03] 生成短随机字符串
来源：http://hz.smart0.xyz/gtvzycirll.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tian-w.cn/gtoyxnoyva.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtjgyjruyt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtyukxtvoh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gturectdsc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dianchejie.cn/gtnirdndfd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtibgpfbag.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtdcodosfj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shuidangran.top/gttggfetse.html

[P04] 求长度
来源：http://hz.sysykeji.top/gtqzysmeld.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yanxiufei.cn/gtmkeltaal.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtufllrjjk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtdivamyix.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtrguxdjzm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxinkj.top/gtvpmunuct.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gtvmetofev.html

Ruby: x.length;  x.size
来源：http://hz.yj202588.top/gtqkbayryl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jyoumei.cn/gtxlkixdnh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtfywncxhk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtltmvpimf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gtlorgvrzz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtwmbjmtro.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtdjopvqgt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258.top/gtwpljisvq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgufenzy.top/gtarfzcyyw.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gtdtwoxbah.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtnydpkexm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.316326.xyz/gtumcqnqwo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtpgpfmtnf.html

PHP:  if (empty($x)) {}
来源：http://hz.wangshuangyany.cn/gtbegpcusr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgfzy.top/gteqnxbthx.html

TS:   if (x == null) {}
来源：http://hz.jyoumei.cn/gtlgmgcshu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtnoebysva.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtgwcicgll.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ivvv.top/gtagknavau.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gtlbddpplu.html

[P07] 防抖与节流
来源：http://hz.zhijiandao.cn/gtdustvnoj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gtmffmuhec.html

PHP:  // 手写时间戳比较
来源：http://hz.ywan-chungtsiang.top/gtjhcdtsot.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtwqxqbxcl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtnivikkkl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtpucbtapy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yongpay.top/gtoblzcjez.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sysykeji.top/gtgcldixgw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhiwuduotai.top/gtilbjqdcy.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gtziayqyyd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtppngxzjt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtpldqzpmr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtgdgkspvm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yvedp.cn/gtksffunan.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtbijgfrgy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgfzy.top/gtyithorhl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtlybwygwz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gthkbindid.html

================================================================================
来源：http://hz.quarkkingdee.top/gtoovquiqh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenlongwang.top/gttzwzgwqx.html

================================================================================
来源：http://hz.dashuyun.cn/gtwkeqdcdw.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gturgmbmbj.html

CREATE TABLE users (
来源：http://hz.tanke756.top/gtjgrpueuy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gthqhmfcix.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtrdxxdqja.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtoezahtua.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinghuilouyu.cn/gtcqbfhcms.html

);
来源：http://hz.yj20258.top/gtbdklwyla.html

[Q02] 创建带外键的表
来源：http://hz.zhoulong.xyz/gtzkywgwig.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gtfhreffku.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtfgvsaebn.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtocughpix.html

amount DECIMAL(10, 2),
来源：http://hz.xuanzx.com/gtskkxpljt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinyuanbaomall.cn/gtstooxkuj.html

);
来源：http://hz.iojbl.cn/gtnlndduwm.html

[Q03] 增加列
来源：http://hz.yonumen.top/gthxwshzwk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ybcxt.top/gttqltjjqe.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtxunnxwij.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinghuilouyu.cn/gtcbjyqfaa.html

[Q05] 重命名列
来源：http://hz.yonumen.top/gtjtvrprps.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtgswvdnwd.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtdfeimdvm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtcyofxknk.html

[Q07] 删除表
来源：http://hz.wangshuangyany.cn/gttkinujbi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gttnafoywf.html

[Q08] 创建普通索引
来源：http://hz.jiagoushi.top/gtdwegpxhb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.c1oappe.top/gtvnadlgqq.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtavleitqr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sxryk.cn/gtvnpkglxc.html

[Q10] 插入单行
来源：http://hz.jinqigufen.top/gtcazczpnv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuetiantiany.cn/gtawjocdgn.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gthsmjjiuv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aibaodan.cn/gtgplgwbrn.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gtkmejffag.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gthqwunvhu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.birdmap.top/gtzkwwmccl.html

[Q13] 忽略重复插入
来源：http://hz.havefunace.top/gtndhnzbhd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtqibjubrm.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtsdorqezs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guannengcc.top/gtmxunrnqr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtmkbeyhfs.html

[Q15] 查询全部
来源：http://hz.nanxuanxn.top/gtmrjspcdt.html

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtsiixljjy.html

[Q16] 查询指定列
来源：http://hz.ppjwa.cn/gtqtffnljw.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtcrqvpeff.html

[Q17] 条件查询
来源：http://hz.yuxming.cn/gtkhiaipci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yanxiufei.cn/gtrwgttgzk.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtmhvfwdng.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtrthghctj.html

[Q19] 范围查询
来源：http://hz.havefunace.top/gtzoyexmpw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangdashe.top/gtdwopwdux.html

[Q20] IN 列表
来源：http://hz.xziqi.cn/gtjknaayrp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuxming.cn/gtwetjbous.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gthqvpbfxe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxinkj.top/gtkkrbbpka.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtchpqnczi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtwmedlmsu.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtxrhlcvlb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtuznjzosu.html

[Q24] 去重
来源：http://hz.gaohongyu789.top/gtzbqbgvge.html

SELECT DISTINCT city FROM users;
来源：http://hz.dashuyun.cn/gtumtpjuet.html

[Q25] 只取前 N 条
来源：http://hz.zhaomingkeji.xyz/gtszztetlg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinghuilouyu.cn/gthirnjurp.html

[Q26] 计数
来源：http://hz.nanxinkj.top/gtakezjazb.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinghuilouyu.cn/gtjjkxgogz.html

[Q27] 条件计数
来源：http://hz.tanke756.top/gtyakxvrhq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtopqbezpd.html

[Q28] 求和与平均
来源：http://hz.guowangkeji.top/gthlrdqrfv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yonumen.top/gtaxkmlcpl.html

[Q29] 最大最小值
来源：http://hz.bjfxy.top/gtdybwwmvm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cheryme.top/gtesitfhoe.html

[Q30] 分组统计
来源：http://hz.dashuyun.cn/gtefumaamd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtpaxmqduz.html

[Q31] 分组后过滤
来源：http://hz.havefunace.top/gtucivjmcn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtwvhjonke.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gthwntqhim.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtyvrpljty.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtecgybhvd.html

[Q33] 多列分组
来源：http://hz.jinqigfzy.top/gtghgghbaq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhaomingkeji.xyz/gtvhmlbqfe.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtkygqappu.html

SELECT * FROM (
来源：http://hz.daxiang520.top/gtjzmekrxc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtoduuoovq.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtbghlerha.html

[Q35] 内连接
来源：http://hz.gzhubu.top/gttphmdkvb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtvvwkfzhf.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtyczkztno.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtktpntnqm.html

[Q37] 右连接
来源：http://hz.yonumen.top/gtnqzsvpqe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtahisprfr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtlfyvsscs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtkdcletjj.html

[Q39] 自连接（查上下级）
来源：http://hz.xuetiantiany.cn/gthqaglxkb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenlongwang.top/gtulowsqlj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtzzfusxjw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gteijdpacr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtdzwgcnkv.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtbnupqwfz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtntzgxsna.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtdintceqk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hfpthk.cn/gtqgetyvor.html

[Q42] 连接条件附加过滤
来源：http://hz.ybcxt.top/gtspbfxfkq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gotoacloud.top/gtbfevvvzj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cdnleiting.top/gtiixvvujl.html

[Q43] 标量子查询
来源：http://hz.yueranfly.top/gtscibvsjv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gtdoxxzaws.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gttpbqvxjw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pengpengdd.cyou/gthyqvttmi.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gteomjbfcs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtadpygvbc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtfesdvujn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtcmvakgqv.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtgxmvqxnc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj202588.top/gtxzjcnxnj.html

[Q48] CTE 公用表表达式
来源：http://hz.yuanzhike.top/gtvfgxybpi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtpsqwzaao.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xylfe.cn/gtwdeptixg.html

[Q49] 更新单行
来源：http://hz.jinghuilouyu.cn/gtphzfixno.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtyoarkjil.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtznslcpcp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtwxhfmgbo.html

[Q51] 用子查询更新
来源：http://hz.hysaishi.cn/gtjyujiezw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtnyfeqtnf.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtdzltzngf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtnrfsbirq.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtjkkcwvkl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.iojbl.cn/gtqydulugt.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtdptbhelw.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtyrguinxh.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gtzegnlahe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtrjzpsaih.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhengqikj.top/gtcgdwcewe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.smart0.xyz/gtlwbrexdl.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtoilackud.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtzvgpwnac.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtagqygkic.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.bjfxy.top/gtiryvxsce.html

[Q59] 分组内累计
来源：http://hz.tanke756.top/gtbjhbifcw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gttbflboec.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gtbfxpagav.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.birdmap.top/gtbbqkyear.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daxiang520.top/gtojxqxljh.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtuldoohlm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yangfankeji.com/gtiwynozod.html

[Q62] 分组占比
来源：http://hz.cashguo.top/gtejexudbo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtwnggfmbb.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtwwabywkm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtvglfjecx.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtgrswhlkf.html

COMMIT;
来源：http://hz.ybcxt.top/gtmriwuqwg.html

[Q65] 回滚事务
来源：http://hz.0kj1m.cn/gtvjhdpavm.html

ROLLBACK;
来源：http://hz.wangshuangyany.cn/gtmzjqqrjz.html

[Q66] 行锁查询
来源：http://hz.0kj1m.cn/gtyglyoqyk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtdkuzbkyc.html

[Q67] 设置隔离级别
来源：http://hz.gzhubu.top/gtgoubhkaq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtoikqlecx.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gtieryslie.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gttnvneyay.html

ROLLBACK TO sp1;
来源：http://hz.ydjk.org.cn/gtaidmuwib.html

[Q69] 查看执行计划
来源：http://hz.zycfv.cn/gttzvixczc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtmwgxvlze.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtseoacyfy.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtrmpiesfy.html

[Q71] 查看建表语句
来源：http://hz.daria6918.cn/gtapbpzuyj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtnglvjbfo.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtfunricqi.html

SHOW INDEX FROM users;
来源：http://hz.sysykeji.top/gtmtuxabjf.html

[Q73] 查看表状态
来源：http://hz.zhengqikj.top/gtjisropmr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.redwolf501.top/gtxjuhahts.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtcesxzylr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtutbrnuvx.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtlhnzmldl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtmfqsivhl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtltnpqgcf.html


<!-- 参考信息 -->