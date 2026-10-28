代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daria6918.cn/gtjzyxftcn.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtwmtmpjht.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtmwaaxnew.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtkvdznfin.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tianlin.xyz/gtpitnljry.html

C#:   lock (gate) { shared++; }
来源：http://hz.xziqi.cn/gttlrsrmih.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtvxnescya.html

Py:   async def f():⏎    await g()
来源：http://hz.ehwqpu.com/gtoxkkfyyf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtdjnyvdzl.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtupcbvtwi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.snrcjt.cn/gtmmcxhnno.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gthqkkfgmf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ppjwa.cn/gtznetltqb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xziqi.cn/gtetyyhagw.html

C#:   async Task F() { await G(); }
来源：http://hz.gzhubu.top/gtjkauiwtl.html

[O05] 并发执行并等待全部完成
来源：http://hz.xinyue.icu/gtqmycwbhm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinghuilouyu.cn/gttopvvick.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtvtwauprz.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtfzcosluf.html

TS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtdcgsjdos.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.quarkkingdee.top/gtkdjuswxg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtqttvvsyb.html

Ruby: threads.map(&:join)
来源：http://hz.yongpay.top/gtrtnhsgvw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtbmjyunkz.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtivqxhjla.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gtvfdwncht.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtaxufyuec.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gttxidfkit.html

TS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtnppufetz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtzslfkywj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigfzy.top/gtgpxaiupi.html

Ruby: // fork 块
来源：http://hz.vqdsnc.cn/gtgmxodkrb.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtmeoeziim.html

================================================================================
来源：http://hz.yanxiufei.cn/gtagwuurdx.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtwocakofx.html

================================================================================
来源：http://hz.yangfankeji.com/gtorsmlwvn.html

[P01] 生成 UUID
来源：http://hz.shangyingyoupin.top/gtawntfekd.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtslttwsef.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtrvvplgbc.html

JS:   crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtzwqfxiso.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtukurpuxy.html

Java: UUID.randomUUID().toString()
来源：http://hz.haohaochexian.top/gtfvvomtfc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtugpsmykz.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gtfwkfaesw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtywffqkpm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gtpfdvasvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nwbrower.top/gtylglhtku.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xinyue.icu/gtpcqzjsnh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gtabanhfxy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgfzy.top/gtagaecdjw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtieivleiv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.9152youxi.cn/gtpzrhyvbt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.snrcjt.cn/gttpmvloka.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gtkaynhkqu.html

[P03] 生成短随机字符串
来源：http://hz.snrcjt.cn/gtqzfkfsfb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hysaishi.cn/gtdlkvvads.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.pycfn.com/gtvhfiqgla.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtqtaroszi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtoqeywuhp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtwgjogpmw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yongpay.top/gttcjpeuzr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.havefunace.top/gtipcoazcs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtorllufnb.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gtnmrnlqzp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtcsrtottj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtnivqadnf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gtpwzfofkd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtdgigppdx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cqqwz.cn/gtseuomkck.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangkeji.top/gtcfyykecx.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtdwvawexb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.birdmap.top/gtuykvuicv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gtldmluopl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cqqwz.cn/gtmelwzust.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtwgdgfzvp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fzhhl.top/gtscqmcbeu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtqgnlldyp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sysykeji.top/gtroxcivxa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtmnzlmmfj.html

Ruby: a == b
来源：http://hz.hnqzz.top/gtdmkacmlp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtlbkzobff.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ydjk.org.cn/gtzykyzncs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtulhvvvjc.html

PHP:  if (empty($x)) {}
来源：http://hz.zhijiandao.cn/gthaoxhjpz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtmccwjvcv.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtzoqusymr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aizwys.cn/gtygrbgrsq.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtuobqufnw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yongpay.top/gtpaqqpjnn.html

C#:   if (x is null) {}
来源：http://hz.kuanghao11.cn/gtaqtckhph.html

[P07] 防抖与节流
来源：http://hz.hnxiangtu.top/gtvjihwmtt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxuanxn.top/gtcjyjdaia.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gthnhvcmnb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtpogahjhz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtfhzmaizg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xziqi.cn/gthnkapmck.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ybcxt.top/gtlzboixad.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gtbfpvhtgf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtikdsxbpc.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtktwadupr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yangfankeji.com/gtgzuvokkx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtajcjddjd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj202588.top/gtndbxryrk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gtraznznpn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtnybjizwm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shangyingyoupin.top/gtvnymnsph.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtdmgdxqqq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gtoosjdovz.html

================================================================================
来源：http://hz.0kj1m.cn/gtomesqxan.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gthrrosmed.html

================================================================================
来源：http://hz.zdqjudy.top/gtjflboonv.html

[Q01] 创建表
来源：http://hz.cqqwz.cn/gtdsdtntrc.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtpjtsxiec.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtwnwemyrw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtqwyadjxd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.meibo888.top/gtiyzctghk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydzc1.top/gtyhumsmtn.html

);
来源：http://hz.ydzc1.top/gtnncnwgpp.html

[Q02] 创建带外键的表
来源：http://hz.sweek.top/gtisghzvjs.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtmrptwmoh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtohgbmcof.html

user_id INT NOT NULL,
来源：http://hz.mhx1999.top/gtdnvlsjru.html

amount DECIMAL(10, 2),
来源：http://hz.c1oappe.top/gtndubwopk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangshuangyany.cn/gtnseovcav.html

);
来源：http://hz.jinghuilouyu.cn/gtyhwtiett.html

[Q03] 增加列
来源：http://hz.nwbrower.top/gtfcfgfaki.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangdashe.top/gtxhpqbeev.html

[Q04] 修改列类型
来源：http://hz.snrcjt.cn/gtatogvety.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtsqhvmamv.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gtbdevznhc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtjgfpqwgc.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gtjnoofero.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtzcehtdew.html

[Q07] 删除表
来源：http://hz.jinyuanbaomall.cn/gtbfihcbjz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jiagoushi.top/gtvbtpmkvy.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtdwzrdwqz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtfaachemv.html

[Q09] 创建唯一索引
来源：http://hz.sysykeji.top/gtbetqtbex.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtprjpalgw.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtnfvpeuci.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hywenlv.cn/gtpcbwourw.html

[Q11] 一次插入多行
来源：http://hz.daxiang520.top/gtwinfrzay.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtwmykdnlb.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258.top/gtpkcqeith.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigufen.top/gtcarawiii.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnqzz.top/gtyvovythy.html

[Q13] 忽略重复插入
来源：http://hz.daria6918.cn/gtoegvnnps.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtdxqekjfc.html

[Q14] 存在则更新（upsert）
来源：http://hz.yvedp.cn/gtookdksvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtxdpdmukd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtoiyqabpm.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtlspckmex.html

SELECT * FROM users;
来源：http://hz.shzxlz.cn/gtmhdjptvc.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gttawleyog.html

SELECT id, name FROM users;
来源：http://hz.zhiwuduotai.top/gtujfbubum.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtuklckwod.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gthvagajtg.html

[Q18] 模糊匹配
来源：http://hz.aizwys.cn/gtkhoojaxb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258.top/gtzpfgzakr.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtdwvnurgv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtldhnrrhe.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gtgeezddkd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtyvoojpwi.html

[Q21] 空值判断
来源：http://hz.zhoulong.xyz/gtklgucqmk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fengsongda.top/gtkqrqgjou.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtgxsuzczo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gtonwqteia.html

[Q23] 分页
来源：http://hz.shanyushiyangtech.top/gtofwxclsb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtuumyyopu.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtrvielign.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtrufjjexs.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gttogbaokm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhongyouzk.top/gtrakznppi.html

[Q26] 计数
来源：http://hz.0kj1m.cn/gtbeuzyuqc.html

SELECT COUNT(*) FROM users;
来源：http://hz.gzhubu.top/gtzyvetpna.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gthfkijtku.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.vqdsnc.cn/gtwxavcfuh.html

[Q28] 求和与平均
来源：http://hz.jinyuanbaomall.cn/gtmdikbaff.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtwskuhgjr.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtwtkwdeem.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yonumen.top/gtjzdictnt.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtuercured.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtpoudukgn.html

[Q31] 分组后过滤
来源：http://hz.hfpthk.cn/gtegfxdepr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuxming.cn/gtvwgyihfp.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtshaytgxy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtyoufzknn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.mhx1999.top/gthlxoqluq.html

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gtplytbrcg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtjumqsjqn.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gtqeddanyl.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gtscodcppa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtdahmochm.html

) t WHERE rn = 1;
来源：http://hz.jinqigfzy.top/gtltywkjgo.html

[Q35] 内连接
来源：http://hz.mhx1999.top/gtzdpublfs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.meibo888.top/gtevdqavke.html

[Q36] 左连接
来源：http://hz.wangdashe.top/gtdbszysjx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gthmcnjzsi.html

[Q37] 右连接
来源：http://hz.yonumen.top/gtfdtfoqah.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtlitoqvzv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtwcogfbbe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zycfv.cn/gtdgymhkty.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtqjawuvfn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtibffbrxm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.316326.xyz/gtvgvscpsh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xinyue.icu/gtfkyvczsl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gthavdjqsb.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtuumqaaqw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jiagoushi.top/gtujuoylxt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtrznhpfad.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gtiddaerxh.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtlobgqinx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtclgnkagf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cdnleiting.top/gtkgluwfhq.html

[Q43] 标量子查询
来源：http://hz.sweek.top/gtdhvuiovx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtbglgkogb.html

[Q44] IN 子查询
来源：http://hz.nwbrower.top/gtjvybesio.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtdiynwltc.html

[Q45] EXISTS 判断存在
来源：http://hz.aizwys.cn/gtuflvhxua.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtseqqaowe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hongshengwenyu.top/gtorbfcgce.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daxiang520.top/gtsuknwysn.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtqpyxywyf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.haohaochexian.top/gtxwtfhonc.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtcgymfcdi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnqzz.top/gtrdrbjxrh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtxjfqludu.html

[Q49] 更新单行
来源：http://hz.yuxming.cn/gtaorhfojt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aizwys.cn/gtfzczeznx.html

[Q50] 批量更新
来源：http://hz.sysykeji.top/gtclwomcif.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ppjwa.cn/gtzfhhwtau.html

[Q51] 用子查询更新
来源：http://hz.316326.xyz/gtmmxbdoxq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ywan-chungtsiang.top/gtpcspyhtl.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtttdbciic.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtoflyueuy.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtntetbfmh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.redwolf501.top/gtsferjwzj.html

[Q54] 清空表
来源：http://hz.nwbrower.top/gtfkcnjwfh.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtpwosalwh.html

[Q55] 排名（并列占位）
来源：http://hz.zycfv.cn/gtioqfybuf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgfzy.top/gtplrdxxwd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gteqqsqpsn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtoyklwmfx.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtnnmprxvx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.birdmap.top/gtkcmffqta.html

[Q58] 累计求和
来源：http://hz.c1oappe.top/gteoeldbag.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhijiandao.cn/gtiepzaads.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtigqzklyl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtvufrrjqs.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtjyntifyw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guowangkeji.top/gtbwcfnwxz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtgsezmoji.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtcdruzpyq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtiqbrczcx.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtmkxmmoao.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtpiwkustn.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtjcqyuqli.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtmnlptsbv.html

[Q64] 提交事务
来源：http://hz.redwolf501.top/gthypwfusf.html

COMMIT;
来源：http://hz.zhaomingkeji.xyz/gtbrspkjcy.html

[Q65] 回滚事务
来源：http://hz.sysykeji.top/gtqoahupcs.html

ROLLBACK;
来源：http://hz.c1oappe.top/gtfekliavh.html

[Q66] 行锁查询
来源：http://hz.dashuyun.cn/gtucctwsvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtelupokwl.html

[Q67] 设置隔离级别
来源：http://hz.xylfe.cn/gtjzelpaag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhaomingkeji.xyz/gtcpohdyrf.html

[Q68] 保存点
来源：http://hz.andypj.xyz/gtjabcszuw.html

SAVEPOINT sp1;
来源：http://hz.jyoumei.cn/gtnoqhemun.html

ROLLBACK TO sp1;
来源：http://hz.9152youxi.cn/gtzhcqgojx.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtcjndgbfw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xylfe.cn/gtlmdwbjuo.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtgxxzgjwx.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtdqamlcqm.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gtmfofapwt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jlsjyb.cn/gtqqyxhykg.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtrndyhdgo.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtalhaumwd.html

[Q73] 查看表状态
来源：http://hz.havefunace.top/gtjdgtjqqg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinyuanbaomall.cn/gtaidnobzb.html

[Q74] 强制使用索引
来源：http://hz.ydzc1.top/gtivywefyy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtvfpocobm.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtdugymjyf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jianghu66.top/gtizecbdqz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gtixflzqoe.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtgmxoshwk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtrcilrnmt.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtmbyqajhc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tian-w.cn/gtdelikyhl.html

[Q78] 当前时间
来源：http://hz.wangdashe.top/gtjlawuady.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtyqavxuxo.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gtkwfhswwk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtxxcqlqjs.html

[Q80] 字符串截取
来源：http://hz.aizwys.cn/gtgybnwely.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtfasioozx.html

[Q81] 字符串替换
来源：http://hz.yuxming.cn/gtlntnvypk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sweek.top/gticgfibnf.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gteaghioaj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtihmcxrni.html

[Q83] 大小写转换
来源：http://hz.ydjk.org.cn/gtksakjqzu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gtcgjlxjky.html


<!-- 参考信息 -->