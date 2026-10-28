代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtyrcetjxs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fzhhl.top/gtttrekrbd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtxbkidffr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtekdtdlkq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtaortnmbp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gtyaxcdpss.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtbmljqmky.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtroztgkfw.html

================================================================================
来源：http://hz.ivvv.top/gtjkmlioma.html

O. 并发与异步
来源：http://hz.hywenlv.cn/gtgnoasivp.html

================================================================================
来源：http://hz.dianchejie.cn/gtsldackld.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtgdpxeyuh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tanke756.top/gtqriuswfu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtzlaluwxr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtnpxvbchg.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtjnodubtz.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gtjsminpfe.html

Go:   go f()
来源：http://hz.sxryk.cn/gtocekuhqj.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtsvluirmh.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gttjewljua.html

[O02] 使用线程池
来源：http://hz.shanyushiyangkeji.top/gtvedqucpj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtgivbkded.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtsbmmxmyu.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtsxmyvcgu.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtzbdohgzw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pycfn.com/gtbidnshff.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.smart0.xyz/gtlijxztpw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gtlgaqqlbt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pengpengdd.cyou/gtckdrfbkb.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gtmvwfknjo.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtjyxermvb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.0kj1m.cn/gttwiochup.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tianlin.xyz/gtmhgywgqm.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtfpzjoyab.html

Java: synchronized (this) { shared++; }
来源：http://hz.kuanghao11.cn/gtnhzrabpz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtbbabdxdk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangshuangyany.cn/gtwbfoyked.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtxelzclel.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtxrzxtcxi.html

Py:   async def f():⏎    await g()
来源：http://hz.chenjidiqi.icu/gtlwzpevrd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shzxlz.cn/gtqfnoxoif.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtrptittth.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtulixeewd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sweek.top/gtufumkxus.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtakfcoqwq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xylfe.cn/gtxkqwpikn.html

C#:   async Task F() { await G(); }
来源：http://hz.ppjwa.cn/gtfwvaynwn.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhengqikj.top/gtytbjhpdt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtbrdliajx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtpsvwzpuv.html

JS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtsedqbftd.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtudvrixbg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtjjyijmhn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtvhjhbojr.html

Ruby: threads.map(&:join)
来源：http://hz.316326.xyz/gtwxmmmypn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtxdwsxfyz.html

[O06] 使用进程池
来源：http://hz.52xcode.cn/gtuxrnwlxd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cucudq.cn/gtjcmwcrmr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gthjeuisbc.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtrlyeujvf.html

TS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtwmqqhycv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtclxeckun.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtwmlcayyu.html

Ruby: // fork 块
来源：http://hz.chenjidiqi.icu/gtfoqbeeei.html

C#:   Parallel.For
来源：http://hz.jlsjyb.cn/gtaaslwexo.html

================================================================================
来源：http://hz.xinyue.icu/gtovclgxqv.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gtmivxtppg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtfxkkmbaf.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gtcmszwhlj.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtsczjdjus.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtijcizdex.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtvcbwobng.html

TS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtqqqzeyil.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtldczcfvb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxuanxn.top/gtqtvtssde.html

Ruby: SecureRandom.uuid
来源：http://hz.hammf.cn/gtrdccrfxe.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhaomingkeji.xyz/gtaolyawkt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shangyingyoupin.top/gtkrhfeoru.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gthxneocan.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gtyhgbjoec.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gtqbmctupz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fengsongda.top/gtsivnybbw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtzcmvwnxh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtjjrgvygz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtduztotdg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtjlbvbvyp.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gtjtiiebof.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtlkmdrbeh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtbrfdvbgq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtqnlgqlmi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gteemtilhs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shzxlz.cn/gtavkbihqq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangdashe.top/gtmwcafafg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.feifeiyinyue.top/gtibqameub.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtnidvaiyy.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtwquzseqk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xziqi.cn/gtlcerepat.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtlhbwowkd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtkekoxyuc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtossnbrkp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ivvv.top/gtfyxpzugt.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtczfioqtk.html

Ruby: x.length;  x.size
来源：http://hz.meibo888.top/gtgwicbjxz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.andypj.xyz/gthylmutja.html

[P05] 判断两个对象内容是否相等
来源：http://hz.snrcjt.cn/gtwdfgrwen.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtvhjiyxxx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ybcxt.top/gtbvifcnwq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtpgxpqfxm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtocpympqu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtulureegu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtngsmyhsi.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtnldkzrlj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jiagoushi.top/gtceuxhqaw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtnmdkiffi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtcmrvnvdp.html

PHP:  if (empty($x)) {}
来源：http://hz.hysaishi.cn/gtstfbkiym.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cashguo.top/gtyqdckpcs.html

TS:   if (x == null) {}
来源：http://hz.snrcjt.cn/gtqbhptrdc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtawxilris.html

Go:   if x == nil {}
来源：http://hz.cashguo.top/gtihbukbao.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gtcgiqiaed.html

C#:   if (x is null) {}
来源：http://hz.xinyue.icu/gtlrxpntvn.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gttucplnud.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gthesbplex.html

PHP:  // 手写时间戳比较
来源：http://hz.smart0.xyz/gtptibwazo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtvendiker.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtmrxkrboz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.bjfxy.top/gtusfokdhf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.bjfxy.top/gttcrvwvlc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jyoumei.cn/gtsyyhqtcx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daxiang520.top/gtumqjyvtb.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtlwlqfojz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cheryme.top/gtonlklidw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj202588.top/gtzwgvhuei.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gthumhqdgw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtjlqekcjs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xingfuxueyuan.xyz/gtzmswhtdp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtuktzurog.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yonumen.top/gtpkdkzwbs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sufxvd.cn/gtcspxdazu.html

================================================================================
来源：http://hz.shuidangran.top/gthuzvktub.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gttuqwnqrm.html

================================================================================
来源：http://hz.ydjk.org.cn/gtrbdswiek.html

[Q01] 创建表
来源：http://hz.shanyushiyangtech.top/gtuijudxov.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtekhlbenf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtgzmphkse.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtkjtcybxi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtvhnwxyho.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtkubpyqty.html

);
来源：http://hz.ppjwa.cn/gtsmqhqckq.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gthlinosfy.html

CREATE TABLE orders (
来源：http://hz.jinqigfzy.top/gtpfvhxtbq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtkvqtjdel.html

user_id INT NOT NULL,
来源：http://hz.jianghu66.top/gtmzivtvtg.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtuphetddr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sufxvd.cn/gtkhzvaskg.html

);
来源：http://hz.gogol.net.cn/gtmxnaecoc.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtingymrtw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtakxlqofy.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtlmhccunt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ybcxt.top/gtmtzqsxlo.html

[Q05] 重命名列
来源：http://hz.zhijiandao.cn/gtoqbeqndi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtpavbnzry.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtdmanczxv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yvedp.cn/gtyaynamxg.html

[Q07] 删除表
来源：http://hz.chenzaomai.com/gteyvjvhiy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtazypokoj.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtansqutvo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sxryk.cn/gtvtigzjuy.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gtjdanvhhy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtmniewcrp.html

[Q10] 插入单行
来源：http://hz.jiagoushi.top/gtvusuqrlt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.svipenyu.cn/gtwjplmmfa.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gttnuoyxjj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gthpgvjteu.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gtlrkryxpy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtuonzickk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gogol.net.cn/gtwusfffch.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtyggyghig.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtwvgqrvjy.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gtuqcamsdc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxinkj.top/gtmczqenjx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nwbrower.top/gtgkzfeibu.html

[Q15] 查询全部
来源：http://hz.jyoumei.cn/gtaapkenxp.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtwzpjyvwm.html

[Q16] 查询指定列
来源：http://hz.xziqi.cn/gtojdtaoso.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtoedevajg.html

[Q17] 条件查询
来源：http://hz.wangdashe.top/gtsvqlfblu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhixingplan.top/gtrbjjcljd.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtvpdsenae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtgimxduhj.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtbkddohtz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtnpmlgnbi.html

[Q20] IN 列表
来源：http://hz.hnqzz.top/gtieixnqyj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtmdfrrmbk.html

[Q21] 空值判断
来源：http://hz.0kj1m.cn/gtvoloisga.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sufxvd.cn/gtxmsqcmnz.html

[Q22] 排序
来源：http://hz.shanyushiyangtech.top/gtulrvqllx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dianchejie.cn/gtdmpanrvu.html

[Q23] 分页
来源：http://hz.yj20258888.top/gtvtvszswt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cucudq.cn/gtreqhotnp.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtcbdjpgmq.html

SELECT DISTINCT city FROM users;
来源：http://hz.pycfn.com/gtzedrdioa.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtxtzlogna.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yangfankeji.com/gtwrgrhkit.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gtclksszsu.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtydtlkhew.html

[Q27] 条件计数
来源：http://hz.redwolf501.top/gtngktximv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtqgeehrju.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gtkuutndpp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cdnleiting.top/gtsofajfpd.html

[Q29] 最大最小值
来源：http://hz.sysykeji.top/gtobjhniuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dianchejie.cn/gtwqsmrsrn.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtohvogtwc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtalrsjmtk.html

[Q31] 分组后过滤
来源：http://hz.yuanzhike.top/gtojwzwfgp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinyuanbaomall.cn/gtzgyfthvy.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtvckzfswg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtqogwedbj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tianlin.xyz/gtmvxgirrj.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtudmqzajm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhongyouzk.top/gtufcsodgc.html

[Q34] 每组取第一条
来源：http://hz.tianlin.xyz/gtlgwkuyfp.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtfqmbqjma.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtfoxgoqol.html

) t WHERE rn = 1;
来源：http://hz.zhoulong.xyz/gtljqthoyg.html

[Q35] 内连接
来源：http://hz.snrcjt.cn/gttcdljhao.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtnzhyyyqy.html

[Q36] 左连接
来源：http://hz.yueranfly.top/gtulaqvams.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtzteedbzh.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtacxohzas.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sufxvd.cn/gtdqoibifz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ppjwa.cn/gtxziqwunx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.kuanghao11.cn/gthtokniwu.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtljfujobq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtxoeakoyx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tian-w.cn/gtvbicwtjv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtgbbirodx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtstwcrlnd.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtwxrgcapj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cucudq.cn/gtkzuukwdg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sweek.top/gtuwpfnmeq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.316326.xyz/gtnmuoefnj.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtzzsoqkdx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtrnnssqfa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pengpengdd.cyou/gtcrlrgiuc.html

[Q43] 标量子查询
来源：http://hz.chenzaomai.com/gtmdmhiaoy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cqqwz.cn/gtylqugkyk.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gthwvxjrvz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daria6918.cn/gtwttkmfnw.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtskeofdqf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtlaxkhtrs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtxbsdimnz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtzcmmenqy.html

[Q47] 与平均值比较
来源：http://hz.jqgufenzy.top/gtlljenpxh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtnhhnhnig.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgufenzy.top/gtcrqprljm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtyhugkxjm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtqdctyrgj.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtvwbrsjsa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.iojbl.cn/gtfwghtkyk.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtnaybitms.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cheryme.top/gttywvlusi.html

[Q51] 用子查询更新
来源：http://hz.yonumen.top/gthmnrennn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtpjmopcvz.html

[Q52] 删除指定行
来源：http://hz.ppjwa.cn/gtbqjgpbhz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtvoqbbjyq.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtvccoznbz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtipqxomfh.html

[Q54] 清空表
来源：http://hz.cqqwz.cn/gtbeyymult.html

TRUNCATE TABLE logs;
来源：http://hz.ywan-chungtsiang.top/gtxkyjlsce.html

[Q55] 排名（并列占位）
来源：http://hz.yuxming.cn/gtqexrhpij.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.c1oappe.top/gtsakuusnd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtsismxwsz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtlnslfzhg.html

[Q57] 行号
来源：http://hz.gzhubu.top/gttmyjvolr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aibaodan.cn/gthgghuffr.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtixpkvgvb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.bjfxy.top/gteflmgxcp.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtsvfzdhes.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zycfv.cn/gtppwmqhin.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtxttaovwi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxinkj.top/gttzddkoze.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.haohaochexian.top/gtwirdcmxh.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtuuvynjbe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtfsvmcrji.html

[Q62] 分组占比
来源：http://hz.yonumen.top/gtbrgqpjfv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtzzelszuz.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtfpdtpxcx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtzkbhsvni.html

[Q64] 提交事务
来源：http://hz.nanxinkj.top/gtxecleuki.html

COMMIT;
来源：http://hz.andypj.xyz/gtoowrdocs.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtmxvuyufl.html

ROLLBACK;
来源：http://hz.hysaishi.cn/gtpzjujagb.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtmnrfiwpr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangtech.top/gtugdmpkcl.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtrixebhpf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenzaomai.com/gttsgrqgxr.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtlezodaif.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gtqzxbmoka.html


<!-- 参考信息 -->