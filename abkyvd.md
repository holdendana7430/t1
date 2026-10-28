代发 wailian999

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtdlswgdek.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtucycooay.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gttavttcxh.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtaphtmjnk.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtcahrfypo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cdnleiting.top/gtdihedlaj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtfyargusi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dashuyun.cn/gtupvcuvju.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtghfnmmtm.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtcwquzmbk.html

Py:   with lock: shared += 1
来源：http://hz.zhongyouzk.top/gtseyxwntc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtdytumtbk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhaomingkeji.xyz/gtbiwjeefi.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtyfzvfasu.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtfbbmsqpm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtrmgmzgtn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sweek.top/gtmewevzjw.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtjiprcuzg.html

[O04] 定义异步函数并等待
来源：http://hz.fengsongda.top/gtycqthnvt.html

Py:   async def f():⏎    await g()
来源：http://hz.chenjidiqi.icu/gtydqnzkvb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhiwuduotai.top/gtkhhjfdtw.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtrozwoihc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtrmwxpill.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtcbiolezm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cheryme.top/gtzyrxpohj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtvlacklfs.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gtslfjjvwm.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtvtieubvg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtxowsdigz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtefwzkayn.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtwkrumnsy.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtccfhfnjq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hongshengwenyu.top/gtmqmibecr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtlujxmiys.html

Ruby: threads.map(&:join)
来源：http://hz.ywan-chungtsiang.top/gtchtxfygc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtyomumacb.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtkpzuvtlu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtornqqlhu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenzaomai.com/gtxeiemnxu.html

JS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtzzqlakuk.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtclecjpve.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangtech.top/gtkzrspgtb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtepfefeok.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gtzabliqvl.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtlvljvfmy.html

================================================================================
来源：http://hz.yuxming.cn/gtqlpofgdl.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gtpwwtrgmn.html

================================================================================
来源：http://hz.dashuyun.cn/gthezvbdkt.html

[P01] 生成 UUID
来源：http://hz.zhijiandao.cn/gtwsbsiopi.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtipjfwkyv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtwpwmgvdi.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtdypovasg.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtthlslouo.html

Java: UUID.randomUUID().toString()
来源：http://hz.sxryk.cn/gtjqjqbbed.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gttjopcjzv.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtblwpblxx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.haohaochexian.top/gtuwqyzbvh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinyuanbaomall.cn/gtxgxqfppv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtsusypina.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtnjyukkyw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jyoumei.cn/gtfksidndu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ehwqpu.com/gtykikjatg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtwejxstxo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtxyynbvus.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtdexogdsu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtzxzkayvh.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gtvtctanjm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.svipenyu.cn/gtmicduxju.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtyqorprnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtflllnnjl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cdnleiting.top/gtmzdwfcgw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtpwhsjrgh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhijiandao.cn/gtryxwmdcz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zycfv.cn/gtebavmufu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigufen.top/gtqqtubqrs.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtooendvmc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fengsongda.top/gtfbugkmfe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gtzvzftnsk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtrmxjfnws.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tianlin.xyz/gtrtujejur.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258.top/gtsgchvbmg.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gtmmbntrmb.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gtrmfrcmsv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtwavgwpyw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hongshengwenyu.top/gtodrfobjp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ppjwa.cn/gtajpoxbfe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhijiandao.cn/gtrtjcbbmg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yueranfly.top/gtxwsnaeyp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtyuhksfow.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtuivoblge.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.mhx1999.top/gtlboqkncz.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gtfxurhtov.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtfrvihswp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gtqmffjcue.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtivajypdi.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gtzzzlilrv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cheryme.top/gthitmcocn.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtdioovfds.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtbxharjmx.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtwnsjhicy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenjidiqi.icu/gthshrihhj.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtoamhzgky.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtnoanfrux.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtdsoskbcm.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtwzuflruu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gttziircxq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gthatjoktt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.vqdsnc.cn/gtfpijrkna.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ybcxt.top/gtqtpnysoy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtiahhiohq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtrqdwhnyw.html

[P08] 处理浮点精度问题
来源：http://hz.gaohongyu789.top/gtzrcmyhlf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gtrgnwqhkj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gtpyqdddgs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tanke756.top/gtrhppwlry.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtqsajwcjr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnqzz.top/gtyqguywvh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.haohaochexian.top/gtbvjmkebe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtzgvgfifp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shangyingyoupin.top/gtwtrjbtst.html

================================================================================
来源：http://hz.c1oappe.top/gtebmmoyxg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtklerlhqz.html

================================================================================
来源：http://hz.cashguo.top/gthgjsqzzn.html

[Q01] 创建表
来源：http://hz.jinqigufen.top/gtmkdmohym.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtmwmjwkow.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gtgwdbadfn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtkdssnrmy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gtcfzprpva.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dashuyun.cn/gtlhxoypoe.html

);
来源：http://hz.chenjidiqi.icu/gtmxgfcwft.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gtobuwbike.html

CREATE TABLE orders (
来源：http://hz.redwolf501.top/gtlraffmti.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtmaohvfqe.html

user_id INT NOT NULL,
来源：http://hz.redwolf501.top/gtsghlsvkj.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtwczkfeyn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aizwys.cn/gtraovocmb.html

);
来源：http://hz.zhoulong.xyz/gtkidxdfie.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtyixjefru.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhiwuduotai.top/gtdehmgtat.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtyiitovfg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gtghkpsbre.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtlrfkferm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtncdsxiul.html

[Q06] 删除列
来源：http://hz.feifeiyinyue.top/gthqihlmlu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtwpnoiyhu.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtxyymukig.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtfmrbdahn.html

[Q08] 创建普通索引
来源：http://hz.hnxiangtu.top/gtwxnjirru.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtkrwmkewl.html

[Q09] 创建唯一索引
来源：http://hz.jqgufenzy.top/gtcpaqlhil.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtawkxstww.html

[Q10] 插入单行
来源：http://hz.kuanghao11.cn/gtavzmswsl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gthrvkjgqv.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtinkpcuqt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtoefldfqi.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gtofvicauo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ppjwa.cn/gtgkgtrezc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gzhubu.top/gtihrywnfd.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtqguspkdv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinyuanbaomall.cn/gtsjomktcz.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtthtrxyoo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xingfuxueyuan.xyz/gtohtlvyxt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jlsjyb.cn/gtlwrmmwtb.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtdgonqcel.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtftrfftui.html

[Q16] 查询指定列
来源：http://hz.nanxinkj.top/gtddltpvuq.html

SELECT id, name FROM users;
来源：http://hz.ywan-chungtsiang.top/gtcjajtbqb.html

[Q17] 条件查询
来源：http://hz.sxryk.cn/gtihedbxoy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sysykeji.top/gtdowvbjrj.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtdaqtaiyk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yanxiufei.cn/gtxkhhblvs.html

[Q19] 范围查询
来源：http://hz.cashguo.top/gtuluqgxwn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnqzz.top/gtqbolaoss.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtbogabcew.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtyhvkqroz.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gtleunmfcm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daria6918.cn/gtrvjihgbr.html

[Q22] 排序
来源：http://hz.yj20258.top/gttxoknqcd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtoninvbzv.html

[Q23] 分页
来源：http://hz.xziqi.cn/gttkajbbje.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yongpay.top/gtkwyzkdcx.html

[Q24] 去重
来源：http://hz.xuetiantiany.cn/gtasnlzlvz.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258888.top/gtabvmceja.html

[Q25] 只取前 N 条
来源：http://hz.xuetiantiany.cn/gtibqxjmlz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cheryme.top/gtqksrfgsc.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtpjjegher.html

SELECT COUNT(*) FROM users;
来源：http://hz.smart0.xyz/gtzbhtlhgb.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gtroejbpnd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhijiandao.cn/gtntzpzega.html

[Q28] 求和与平均
来源：http://hz.wangshuangyany.cn/gtzgqahypp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yueranfly.top/gtikyvmfna.html

[Q29] 最大最小值
来源：http://hz.tian-w.cn/gtprpkogif.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.smart0.xyz/gtqkcxmzdt.html

[Q30] 分组统计
来源：http://hz.yuxming.cn/gtajuqormv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtukahwphl.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtwsxnmwnx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtkdmoftvo.html

[Q32] 分组拼接字符串
来源：http://hz.yvedp.cn/gttzpcrjuo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtbwcbhzrz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hysaishi.cn/gtsljcvdzi.html

[Q33] 多列分组
来源：http://hz.cashguo.top/gtgbdyffbf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cucudq.cn/gtimexhfoq.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtdwrmirzo.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gttebuuhfk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuanzx.com/gtmetqvafe.html

) t WHERE rn = 1;
来源：http://hz.dianchejie.cn/gtgdwpfaom.html

[Q35] 内连接
来源：http://hz.zhongyouzk.top/gtmgonhvez.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gttrvftekn.html

[Q36] 左连接
来源：http://hz.vqdsnc.cn/gtlnkxmsxs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gtapxjywpk.html

[Q37] 右连接
来源：http://hz.hysaishi.cn/gtjqyrradw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.svipenyu.cn/gtnenbbmjk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gthnnxnyaj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtowttybif.html

[Q39] 自连接（查上下级）
来源：http://hz.sufxvd.cn/gtjcjodwwv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuxming.cn/gtujkrhuzt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.0kj1m.cn/gtmuxzuzds.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhoulong.xyz/gtihnghjzl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pycfn.com/gtwjoizxgx.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gtrepxbojo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gttomrozlq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtdifkbaeq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtkzonatur.html

[Q42] 连接条件附加过滤
来源：http://hz.aizwys.cn/gtcdhkxogj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yonumen.top/gtcxgmjhnc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtsiipyexa.html

[Q43] 标量子查询
来源：http://hz.yj20258.top/gtpitdqexx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtnafojwce.html

[Q44] IN 子查询
来源：http://hz.xinyue.icu/gtzzxkhpnm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtavjpuazl.html

[Q45] EXISTS 判断存在
来源：http://hz.cdnleiting.top/gtlcssgtka.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtczuykqtw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jianghu66.top/gtcgondjgj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtgxarfjma.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gtldapsrlg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtzhqhkonx.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gttddozyvg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.9152youxi.cn/gtrxuqwerr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtgyhotqdu.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gthkggtewh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtncaavgkq.html

[Q50] 批量更新
来源：http://hz.316326.xyz/gtcicjhhlj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtdzazjthb.html

[Q51] 用子查询更新
来源：http://hz.dashuyun.cn/gtxbiwjqjl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenjidiqi.icu/gtcbpnkmas.html

[Q52] 删除指定行
来源：http://hz.pycfn.com/gtiadawnft.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtkthudmso.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtgtlaxvbg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtlrarzytv.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtvcrleixb.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtytmnhiio.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtreaanzfg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtotrlmyun.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtfylfpqqn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sweek.top/gttmscpvrh.html

[Q57] 行号
来源：http://hz.haohaochexian.top/gtkxuzdgtt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtjvftocfj.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtnkyxkhtw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.bjfxy.top/gtvquurber.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtisdjukgf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnxiangtu.top/gtlfrpsend.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gtbftdifxq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.mhx1999.top/gtmwltrlry.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ivvv.top/gtnuqfqpjo.html

[Q61] 移动平均
来源：http://hz.zhixingplan.top/gtjmwfywfd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.316326.xyz/gtdhquhcqh.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtqtvgsgth.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtliiyiwfl.html

[Q63] 开启事务
来源：http://hz.dianchejie.cn/gtuehsmeju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtohuvmkqm.html

[Q64] 提交事务
来源：http://hz.gotoacloud.top/gtrhpcsnla.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtqhkrmnld.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtqeskgqhn.html

ROLLBACK;
来源：http://hz.52xcode.cn/gtsvflivln.html

[Q66] 行锁查询
来源：http://hz.316326.xyz/gtpdbokngp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aibaodan.cn/gtmmemdnew.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtczagtnol.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.52xcode.cn/gttndwyxms.html

[Q68] 保存点
来源：http://hz.xuanzx.com/gtvrsejkmy.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gtjolqiiws.html

ROLLBACK TO sp1;
来源：http://hz.c1oappe.top/gtuadmvlmh.html

[Q69] 查看执行计划
来源：http://hz.jinqigfzy.top/gtdlhpoqxi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gteypygdbz.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtmeezeqso.html

ANALYZE TABLE users;
来源：http://hz.shzxlz.cn/gtsvwcbjev.html

[Q71] 查看建表语句
来源：http://hz.jinqigufen.top/gtcrfbihwg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yanxiufei.cn/gtbyxpuiyn.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gttllezigs.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtccxpogef.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtauznfyyr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtobfypusj.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtqkupqxle.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtpsqmwmoo.html

[Q75] 日期格式化
来源：http://hz.ivvv.top/gttdqgsaou.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ehwqpu.com/gttwljgztv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtiwkhtilg.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtzcmtrhgk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtgohxynmw.html

[Q77] 时间加减
来源：http://hz.fengsongda.top/gtswoyotcn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gtzvumqmkz.html


<!-- 参考信息 -->