代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gterhratug.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yueranfly.top/gtabwijddp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtqpwkoxmp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtkumdcvlt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtpjbhprtm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gtytgadfsm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtkobgctly.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtfuzpltge.html

================================================================================
来源：http://hz.xziqi.cn/gtcdwthurx.html

O. 并发与异步
来源：http://hz.yj202588.top/gtsxytfzru.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvsdqjwvc.html

[O01] 启动一个线程
来源：http://hz.yanxiufei.cn/gthwvuvyyv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtjhftkoqe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtwzobzuyj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtjrkitkdf.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtawysipzs.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtgcpqwcpe.html

Go:   go f()
来源：http://hz.guannengcc.top/gtqoflrhaw.html

Ruby: Thread.new { f }
来源：http://hz.cheryme.top/gtfvdbffvz.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtaeclhwvg.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtaxkvvbyj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtncdzizvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtbppapzgg.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtzrqxcucy.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtrazxbhwt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.fzhhl.top/gtztzrtpci.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ybcxt.top/gtmobzebvm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gttiroualx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtreqvawzv.html

[O03] 加锁保护共享数据
来源：http://hz.quarkkingdee.top/gtnjnsqfrr.html

Py:   with lock: shared += 1
来源：http://hz.yj202588.top/gtoqmvpnzx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gtgnbblxze.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtalhiuycx.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtensdksfx.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtggtaikym.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhaomingkeji.xyz/gtscwrojsn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnqzz.top/gtzagzjake.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtasvnlkyy.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtnnxsefbc.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtmyackilv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtssjbwglx.html

JS:   async function f() { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtckblglrl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gticunkgjw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtmqwvwalw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtkmikqxpd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jianghu66.top/gtjkroreva.html

C#:   async Task F() { await G(); }
来源：http://hz.xylfe.cn/gtrwdpbvqt.html

[O05] 并发执行并等待全部完成
来源：http://hz.gotoacloud.top/gtgxmkmkxl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.iojbl.cn/gtfelgjbgv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhongyouzk.top/gtctwaogzu.html

JS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtqzkwrmxg.html

TS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtizhvndwd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.meibo888.top/gtkqbcvauf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtmudavocb.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtwpdenale.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtbgzgqttx.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtsobtrwbr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pengpengdd.cyou/gtniazwkea.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.iojbl.cn/gtvtdkvygq.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtslzlxqjb.html

TS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtosziqxnk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yongpay.top/gthyydbmvv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dianchejie.cn/gtadnjktvk.html

Ruby: // fork 块
来源：http://hz.xuanzx.com/gtlezvbule.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtmyjpkhay.html

================================================================================
来源：http://hz.guannengcc.top/gtltsijthp.html

P. 常用工具函数
来源：http://hz.xylfe.cn/gtvrclbcev.html

================================================================================
来源：http://hz.daxiang520.top/gtlsawsafl.html

[P01] 生成 UUID
来源：http://hz.fengsongda.top/gtabpcrzih.html

Py:   str(uuid.uuid4())
来源：http://hz.xingfuxueyuan.xyz/gtaooepquv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.52xcode.cn/gtogkqttls.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtaehikbwf.html

TS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtmaxvhjtb.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtrqexoqfa.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhongyouzk.top/gtkiwqtqyw.html

Ruby: SecureRandom.uuid
来源：http://hz.gaohongyu789.top/gtkshatmhl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtekojjgmh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gtoqlubltt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gtggngexxm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hammf.cn/gtrzsoznbw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hfpthk.cn/gttowjantz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtmrbczqzk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtsjtohhez.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gthcgxhjwy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gttjuyzacw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gtleyucqgu.html

[P03] 生成短随机字符串
来源：http://hz.yj20258.top/gtpbxplryq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtxnjrjali.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.snrcjt.cn/gtgpygwtet.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtsazrxgbt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtkrtwimow.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtjggxrjbs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cucudq.cn/gtluvfcltf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gthidjoazu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtqhzkkxtg.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtjwsivhgq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhoulong.xyz/gtoamcamjd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtrjdgxcpa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gttujlqxnu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtgduanzvc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gtprnvdumx.html

Go:   len(arr);  len(m)
来源：http://hz.birdmap.top/gtvzpdgync.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtvvxbfkuw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ivvv.top/gtwhlatunq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gtqberfkpu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gzhubu.top/gtlzjfbsqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtyxzvvbuk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtpsbvyyua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtkkuauobu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fengsongda.top/gtjzxcdurj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtpogzbieu.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtfonfwykh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydjk.org.cn/gtfthogamh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtwtwquowz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtsbthvxor.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtpkawifxm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtaxnuytly.html

TS:   if (x == null) {}
来源：http://hz.yongpay.top/gtwxlqnxmb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yongpay.top/gtcvzhfvpw.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtzvcjzlon.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zdqjudy.top/gtamdqypez.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtnpdfksii.html

[P07] 防抖与节流
来源：http://hz.cdnleiting.top/gtwvdpujvr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtlyidxtua.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgufenzy.top/gtyzpsmatq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtjqoxdkgz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gthmvkseyr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangshuangyany.cn/gtzsbxmkbx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtqykaoxgp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtcqaffmvg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hfpthk.cn/gtmynmjhai.html

[P08] 处理浮点精度问题
来源：http://hz.andypj.xyz/gtwgbcerci.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daxiang520.top/gtsomwcesp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sufxvd.cn/gtdtuvogkt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtyctuzcrx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtiinmfigg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xingfuxueyuan.xyz/gtyspkovzh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtuflihsos.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtyejhlfbh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.andypj.xyz/gtmhamwlxo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnuckrkgp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtppnjftwy.html

================================================================================
来源：http://hz.52xcode.cn/gtcqpqzmwt.html

[Q01] 创建表
来源：http://hz.pycfn.com/gtucuwfquq.html

CREATE TABLE users (
来源：http://hz.52xcode.cn/gtafwexyha.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gteqkzwdbx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtfxrzruji.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenzaomai.com/gtledbabwa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hywenlv.cn/gtdskclnwa.html

);
来源：http://hz.gotoacloud.top/gtvbbvuevf.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtepinpujx.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtaqhasesc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtjrnyshsl.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtkfysmrjw.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtbmgddifa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gthvlhshxq.html

);
来源：http://hz.aizwys.cn/gtwmwiujoh.html

[Q03] 增加列
来源：http://hz.yanxiufei.cn/gtjlxnlaca.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gtarmnofzc.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtsoorxzmj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhaomingkeji.xyz/gtkbrkonue.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtsgofprnj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.bjfxy.top/gtblpykmtw.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtftuxdxiy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gthgpzhojo.html

[Q07] 删除表
来源：http://hz.jiagoushi.top/gtyjormwhb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258888.top/gtwjvkmsqj.html

[Q08] 创建普通索引
来源：http://hz.aizwys.cn/gtupebvcjt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtfxvzohsz.html

[Q09] 创建唯一索引
来源：http://hz.pycfn.com/gtegyicnkw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtggjjpdyi.html

[Q10] 插入单行
来源：http://hz.jlsjyb.cn/gtwreemknl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gtqaxyhsah.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtmiqwaabx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtkmdojjue.html

[Q12] 插入后取自增 ID
来源：http://hz.pengpengdd.cyou/gtslbtztvd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtpzhidmjl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hysaishi.cn/gtpjxgvcdc.html

[Q13] 忽略重复插入
来源：http://hz.gzhubu.top/gtjjnshxya.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtdlnqlzkd.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtskhwetct.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtnrhqrgsq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydzc1.top/gtdybrcvpu.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtkwofkgno.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtagnusycd.html

[Q16] 查询指定列
来源：http://hz.cheryme.top/gtxjccweij.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gtbnsdtsfd.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtrnexrvwf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.smart0.xyz/gtdxymofeu.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtuhbberop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtjtxizech.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gtbckprfvq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.316326.xyz/gtcmpukbjx.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtvtxrajre.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtmddtysrb.html

[Q21] 空值判断
来源：http://hz.aibaodan.cn/gttncjjwgy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yonumen.top/gtyhetfpnx.html

[Q22] 排序
来源：http://hz.mhx1999.top/gtbxtyxahc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jiagoushi.top/gtcvcskyxl.html

[Q23] 分页
来源：http://hz.havefunace.top/gtoaqedysr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gttvmwfbno.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtwluquqbq.html

SELECT DISTINCT city FROM users;
来源：http://hz.316326.xyz/gtwohcjreh.html

[Q25] 只取前 N 条
来源：http://hz.dianchejie.cn/gtzovdvstn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yongpay.top/gtwghmhclg.html

[Q26] 计数
来源：http://hz.pycfn.com/gtcvfvrsdp.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gtptjmdfkq.html

[Q27] 条件计数
来源：http://hz.hammf.cn/gtdbanzstq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yvedp.cn/gtsmqusipy.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtbysbusjf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xziqi.cn/gtwcdbhpda.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtbyrcmbve.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gtpgnsoqrj.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtegqwaouf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gthpdztxxd.html

[Q31] 分组后过滤
来源：http://hz.jlsjyb.cn/gtdrkyjabz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtkzgxperc.html

[Q32] 分组拼接字符串
来源：http://hz.yvedp.cn/gtehonyhjt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtrtukdpji.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.svipenyu.cn/gtfaefjgst.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtxfmjwdtx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtalsflndc.html

[Q34] 每组取第一条
来源：http://hz.snrcjt.cn/gtfoccewko.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtrmsxaxer.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigufen.top/gtfvmcmahl.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtamovuvzq.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtyqxeylmv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtyxofdigo.html

[Q36] 左连接
来源：http://hz.chenjidiqi.icu/gtxvmlauci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtujjapzwv.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtgtcpcebu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tanke756.top/gttvgrrpyx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zdqjudy.top/gttqhbqwnw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtlbjgdunu.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gtfljbzvmp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ppjwa.cn/gtkxjosvqa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jyoumei.cn/gtmeerotax.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtmuwwczib.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtugmkseif.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtrfuzhwkh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtclmenqoc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtbahsytlo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangdashe.top/gtcycriaom.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtorzxefnq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtrnpimsrc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydzc1.top/gtytwabaum.html

[Q43] 标量子查询
来源：http://hz.havefunace.top/gtagdirxtd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenlongwang.top/gtqvedjdlq.html

[Q44] IN 子查询
来源：http://hz.jqgfzy.top/gtbbnwlcmi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtpxlygril.html

[Q45] EXISTS 判断存在
来源：http://hz.cucudq.cn/gtgrrearje.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtqjoceufj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtmtvkiygg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtsitouzeg.html

[Q47] 与平均值比较
来源：http://hz.xinyue.icu/gtcyyhlemg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtjykndlju.html

[Q48] CTE 公用表表达式
来源：http://hz.snrcjt.cn/gthtfsoabr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtilivrgth.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtvwdgfjbk.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtqrezgsbb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gtyagyczmz.html

[Q50] 批量更新
来源：http://hz.havefunace.top/gtszwjsvmv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.vqdsnc.cn/gteixscrci.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtpsylvtnf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtqvnsikwt.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtwoozgcgj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtryemlkdu.html

[Q53] 按条件删除
来源：http://hz.tanke756.top/gtwxkvcvsf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtmzmeyrbi.html

[Q54] 清空表
来源：http://hz.zycfv.cn/gthxwebwql.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtxtvcdkkc.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtppaqpncf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtnruyeywo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtcjdsamsf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtrjpgfnwz.html

[Q57] 行号
来源：http://hz.c1oappe.top/gtfgkvgskp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtuqrwhnqv.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtczyhryrh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtksdryduw.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gthjtsjvlx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtrmtiwujm.html

[Q60] 取上一行 / 下一行
来源：http://hz.xziqi.cn/gtpocnazzl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtfrvfzvyf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jianghu66.top/gtkccsyojv.html

[Q61] 移动平均
来源：http://hz.havefunace.top/gtftmsqgmi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtlrqgqadq.html

[Q62] 分组占比
来源：http://hz.yj20258888.top/gtkmahjpxc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtcmmtrvdi.html

[Q63] 开启事务
来源：http://hz.ydjk.org.cn/gtlavpuzpk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtaefbcati.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtkopfsoex.html

COMMIT;
来源：http://hz.chenjidiqi.icu/gtvilaqbqu.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangkeji.top/gtzbfujsdf.html

ROLLBACK;
来源：http://hz.svipenyu.cn/gtlyjjhiiv.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtgfwqplwe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cucudq.cn/gtuokjzidb.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gtefygpmdz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gtufmgwkxo.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gttmzqqzii.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtpizghmeq.html


<!-- 参考信息 -->