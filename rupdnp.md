代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtkmvaoxei.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtfptmcwcs.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtnggslhwz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gtnspvzepu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daria6918.cn/gtuuesoggj.html

C#:   lock (gate) { shared++; }
来源：http://hz.iojbl.cn/gtlzjaskhp.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtlsheyfwj.html

Py:   async def f():⏎    await g()
来源：http://hz.jlsjyb.cn/gtwvufutaj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtjpbqjbga.html

JS:   async function f() { await g(); }
来源：http://hz.yueranfly.top/gtcpaheopr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gthbtjmdci.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenlongwang.top/gtafabpazc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtbabqisfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtanktxoqb.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtwhskzfgw.html

[O05] 并发执行并等待全部完成
来源：http://hz.tian-w.cn/gtymghetlx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daxiang520.top/gtnejgnayd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ivvv.top/gtgngjhcsm.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtbudupmhb.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtriuaeror.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhaomingkeji.xyz/gtrjxityuy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinyuanbaomall.cn/gtyhqonmlj.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gtgfpbbtxf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtkpapodkh.html

[O06] 使用进程池
来源：http://hz.guowangkeji.top/gttiukrhno.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtqalhuzzp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.316326.xyz/gtuzwiifxc.html

JS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtqhohtyjd.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtjpcxevbf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnqzz.top/gteimbhekw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ybcxt.top/gtjmizitrn.html

Ruby: // fork 块
来源：http://hz.xuetiantiany.cn/gtjazqmeon.html

C#:   Parallel.For
来源：http://hz.birdmap.top/gtevighyce.html

================================================================================
来源：http://hz.zhengqikj.top/gtqxaqgicm.html

P. 常用工具函数
来源：http://hz.yangfankeji.com/gtehsxglur.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlebnflsj.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gthvfcqwhx.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtoumdgnrg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtzrnpncqu.html

JS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtlnhqhkny.html

TS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtkvmgteuo.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtbtqyvvii.html

Go:   // 用 github.com/google/uuid
来源：http://hz.bjfxy.top/gtgrrkdqvz.html

Ruby: SecureRandom.uuid
来源：http://hz.guowangkeji.top/gteiypiini.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtauumqaoy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gttvsskrlg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxuanxn.top/gtwmtfkqqc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtecnaxwel.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhongyouzk.top/gtzvpntzod.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shzxlz.cn/gtgqaehbju.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtlvruyajz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nwbrower.top/gttcsztobq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhixingplan.top/gtmzknephu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ybcxt.top/gtorwusaim.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gtgmvzdprf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ehwqpu.com/gtdopbajqm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtrlhenrjt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtecagszjz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtvbimeqmp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtuywbyejn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.svipenyu.cn/gtrfnrtpom.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shuidangran.top/gtqamgvktd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dashuyun.cn/gtixqxtisg.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtjozsylzb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.vqdsnc.cn/gtgnyksnzm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258.top/gtkasurvgq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtqyzovakk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtoegamqyy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenjidiqi.icu/gtzjdzpqww.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigfzy.top/gtqueifexr.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gttxqvetme.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sufxvd.cn/gtfamijvcj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tian-w.cn/gtrfzoztrt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yvedp.cn/gtdhmzkiwl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gtpldjzfzu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtbzpheiom.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gttmxqkfgl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aizwys.cn/gtalnrrbcl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gthjahksfi.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtjbozjvmw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hammf.cn/gtceojeaxi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtvtqqrhdg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtzvjyvgbu.html

PHP:  if (empty($x)) {}
来源：http://hz.ehwqpu.com/gtiulhmzlk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.smart0.xyz/gtqmvktvem.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtgoqqgves.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtyjhhtatr.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gthwvnupdg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtnfdrxcmo.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtslaqreiq.html

[P07] 防抖与节流
来源：http://hz.chenlongwang.top/gtbzhdflsr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhengqikj.top/gtmcvcbfmn.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gthskfnvqx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtdsxukpfg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtiiobtfnr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hysaishi.cn/gtfxzudgfx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daxiang520.top/gtaqocgprx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.haohaochexian.top/gtplkurdbk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aibaodan.cn/gtjtbutziy.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtpgukxfmv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtlvigbvgw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtztaguaow.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtmkzegfms.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtyrliwlix.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtpggxknnq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtgpyfdepp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aibaodan.cn/gtuafticre.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jianghu66.top/gtnrekrerb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwvtchbqj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtmozosfnf.html

================================================================================
来源：http://hz.gzhubu.top/gtokkcvddj.html

[Q01] 创建表
来源：http://hz.xuetiantiany.cn/gtroexmixb.html

CREATE TABLE users (
来源：http://hz.pycfn.com/gtqujdzkmg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtukqizuan.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtdpyrdapl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtdsgycwpw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtxqbabjgw.html

);
来源：http://hz.aibaodan.cn/gtxhsbiabi.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtogbtiaie.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtrmgwmjeb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtfxaxpujt.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtabhxsyaq.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtdhxfnvwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gtemljcrkf.html

);
来源：http://hz.yueranfly.top/gtbopiqsue.html

[Q03] 增加列
来源：http://hz.ydzc1.top/gtndviqfpi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ehwqpu.com/gtyecmwsab.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtjfrbedpw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtncjjvezp.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtfbnidkhq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtnthficzq.html

[Q06] 删除列
来源：http://hz.xingfuxueyuan.xyz/gtbbpqzgiu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.andypj.xyz/gtsltwzrhs.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtpbutlgpb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jiagoushi.top/gtwtlsyzml.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtxomlynsr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xziqi.cn/gtctqfkvuz.html

[Q09] 创建唯一索引
来源：http://hz.xuetiantiany.cn/gtifhnzqph.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gttpwcpirl.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtkpmlmezf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigufen.top/gtmglswcpn.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gttraqryzm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtusiamvhb.html

[Q12] 插入后取自增 ID
来源：http://hz.shzxlz.cn/gtezbrkzyf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtlprcfsxb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtnpgpqvcp.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtjadwqkkx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gthqgrqdii.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtmqpxosvy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtqkwypwdv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aizwys.cn/gtihuydhqw.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gthgjizbvk.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtsjlitklc.html

[Q16] 查询指定列
来源：http://hz.gotoacloud.top/gtgfptmbyb.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtwaipkadh.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gthxmecnsf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pycfn.com/gtdgrewpuk.html

[Q18] 模糊匹配
来源：http://hz.andypj.xyz/gtkgxbpbuu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jyoumei.cn/gtdynhxkai.html

[Q19] 范围查询
来源：http://hz.sufxvd.cn/gtcxtfprch.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cashguo.top/gtpiddfueh.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtuddwmgru.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtsppwksmf.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtmfzodrpr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydzc1.top/gtedmgufgc.html

[Q22] 排序
来源：http://hz.jinyuanbaomall.cn/gtbssfpycd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gtqawngduc.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtcvgeodtm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xylfe.cn/gtmpkfqykl.html

[Q24] 去重
来源：http://hz.havefunace.top/gtqksvpwto.html

SELECT DISTINCT city FROM users;
来源：http://hz.dashuyun.cn/gtnzebcear.html

[Q25] 只取前 N 条
来源：http://hz.jianghu66.top/gtaphpsrrb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtjczarppd.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtjiihstbf.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtdpjokgck.html

[Q27] 条件计数
来源：http://hz.bjfxy.top/gtezylyiyx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtgsoazpjy.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtmfscreva.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtyliauglb.html

[Q29] 最大最小值
来源：http://hz.zhixingplan.top/gtnghoakst.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gtyrdwgwxj.html

[Q30] 分组统计
来源：http://hz.xuanzx.com/gtvaimemcz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtiboefjzt.html

[Q31] 分组后过滤
来源：http://hz.ydzc1.top/gtqxwgpjjp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtqwbqozil.html

[Q32] 分组拼接字符串
来源：http://hz.andypj.xyz/gtdewkynqg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtiwdsqyqg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtwishisso.html

[Q33] 多列分组
来源：http://hz.gotoacloud.top/gtygpioges.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cheryme.top/gtmhptyzqs.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtaiifczsj.html

SELECT * FROM (
来源：http://hz.fengsongda.top/gtdrjjlpzz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shangyingyoupin.top/gtugtrirxv.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtfitaesxo.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gthjdygumi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtzumvastt.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtgejzdcab.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtrnsayrpl.html

[Q37] 右连接
来源：http://hz.yj20258.top/gtyymznmqb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtznsnkahn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gtglofsgnv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.wangshuangyany.cn/gtfsqdtxln.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258888.top/gtfctahixd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.haohaochexian.top/gtrcabtzcf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jiagoushi.top/gtvftclmbq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtwjvbgikn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xinyue.icu/gtxogrqojc.html

[Q41] 多表连接
来源：http://hz.yuxming.cn/gtsuunxvhh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.mhx1999.top/gtfrqptltn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtqmhpxhof.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fengsongda.top/gtevjwulis.html

[Q42] 连接条件附加过滤
来源：http://hz.guannengcc.top/gttzdmfeui.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtzkxewwom.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gthcvwjxac.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gthocmsgyc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258.top/gtkxzrevef.html

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtkyqtjrnf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtrsgqlcxq.html

[Q45] EXISTS 判断存在
来源：http://hz.tanke756.top/gtylhzjekz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtivyqkoyo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tian-w.cn/gtnbyroqhx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtpyulsckh.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gtgjuzmkmc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ywan-chungtsiang.top/gtilomwblp.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gtfxcusvnm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtsmflbwzp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtslsglszq.html

[Q49] 更新单行
来源：http://hz.cheryme.top/gtkwiwhjdn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.havefunace.top/gtwkvodqde.html

[Q50] 批量更新
来源：http://hz.yuanzhike.top/gtravdhwop.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtqwcjfsmz.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtzgqbbtbd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tianlin.xyz/gtrratpwkj.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtijblpdrr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258.top/gtepnrqpqw.html

[Q53] 按条件删除
来源：http://hz.jianghu66.top/gtqrzrubxd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gtmktjbgip.html

[Q54] 清空表
来源：http://hz.yonumen.top/gtgluqxadn.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gtpsvjxxfs.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gttglixjdp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jianghu66.top/gtxtqxnmol.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ybcxt.top/gtfsgllspx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtbwnisptv.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtyiudvebn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtjdvscqgu.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtpstwrzft.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sweek.top/gtqyxkfspb.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gtsndvhbur.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.smart0.xyz/gtuosyxdzl.html

[Q60] 取上一行 / 下一行
来源：http://hz.shzxlz.cn/gtewpzkbdh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gtcggpfelp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.c1oappe.top/gtgkrwpfyw.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtffknhfpn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtadwukyyc.html

[Q62] 分组占比
来源：http://hz.vqdsnc.cn/gtcbyxgjnd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtsupohyvo.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gtxjmvednt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtohxjyujj.html

[Q64] 提交事务
来源：http://hz.iojbl.cn/gtagbokzol.html

COMMIT;
来源：http://hz.hysaishi.cn/gtaerfbzzb.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtfxabcebm.html

ROLLBACK;
来源：http://hz.xingfuxueyuan.xyz/gtzxtxkitm.html

[Q66] 行锁查询
来源：http://hz.xuetiantiany.cn/gtrxnfmjbx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtwmkxobse.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtnosxfeur.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenlongwang.top/gttljpwqhn.html

[Q68] 保存点
来源：http://hz.chenlongwang.top/gtzsvsqerf.html

SAVEPOINT sp1;
来源：http://hz.shanyushiyangkeji.top/gtzpviiyqg.html

ROLLBACK TO sp1;
来源：http://hz.vqdsnc.cn/gtuijqtixq.html

[Q69] 查看执行计划
来源：http://hz.yj20258888.top/gtulakukag.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gttbhlcqkj.html

[Q70] 更新统计信息
来源：http://hz.dianchejie.cn/gtamvydwlo.html

ANALYZE TABLE users;
来源：http://hz.ydjk.org.cn/gtoteavobh.html

[Q71] 查看建表语句
来源：http://hz.ybcxt.top/gtsdeeyyaz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtmmvczylj.html

[Q72] 查看索引
来源：http://hz.sweek.top/gtucovhdzs.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gtrzqppgbe.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gthcrslunt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtaalijnfm.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtuqwohygm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gttruombqc.html

[Q75] 日期格式化
来源：http://hz.chenlongwang.top/gtzqqhryhd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gtozpvnkdc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jlsjyb.cn/gtvoxeyzbc.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtsauqymrk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtcvxjvfem.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gtjwpzyrzu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtidaaxpmy.html

[Q78] 当前时间
来源：http://hz.dianchejie.cn/gtgknjvhik.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guowangkeji.top/gtiolyzrnl.html

[Q79] 字符串拼接
来源：http://hz.cheryme.top/gtrchmjpwm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtarhwzyvy.html

[Q80] 字符串截取
来源：http://hz.ywan-chungtsiang.top/gtsmbjsxdw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jianghu66.top/gtrfabbwrv.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtfcdmgptv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtsriivjeo.html

[Q82] 字符长度与字节长度
来源：http://hz.ywan-chungtsiang.top/gtofbbgcsf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtmaootkcd.html

[Q83] 大小写转换
来源：http://hz.yj20258888.top/gttoodtmhw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ybcxt.top/gtheomeiyu.html


<!-- 参考信息 -->