代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmdrefds.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2devhevfv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jpmhlpia.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pduzkngw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ovqmwvlf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qdzpvyao.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gayimnse.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ovbtxqii.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bfafttiw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uebgczvu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxlpdanp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uejbqczk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hjookuzj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rmeoxlbg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oxgdilsn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gaxezopd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kfzmglth.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fzutegho.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gbmkkjaj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bitvpquz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ntstnane.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lnuynpbt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ykgplzqc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2liumplns.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iqemhafb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xcllydei.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2sozbzbrx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2edgcpstk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2iwwktfba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikeonsqh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dnxfufjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmgrtsng.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wjiwnfgi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ezvaboxy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jpzosmlw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mmtrmmnq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cbsmrdtm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ptpnnjzf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jjhfxkhy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jrltlfuf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ygmmgzdm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eqziiprj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kqmmonql.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdlfqapy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vpyorskz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hfclximi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2phqyxdmj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2knorvaeu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cxwnlggy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jqbedwwf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpspjdfz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2aeuspwru.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ctfdztmm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ltlglpcg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwlmrwcu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmiuada.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cdovzzei.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vkalufdb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sfkodwfj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ifluioho.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2luxnnkii.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kaygyrqz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jtyeznja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rvcvvozb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmkvarai.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fsrmvhyn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tpgwpyfw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dcqyfgpm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ietohyli.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2yrilzkbg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ttizwegv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zbqadtgo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnolikhi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qvavaupq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uoawptut.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ezfiwztl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nyjubrjq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ojalkvxr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vwhzkacx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbqokddk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vksqavkb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhkzwbwe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulkqmrsn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvhhxpzv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkewnxs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uphyudca.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2iyeylodi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fcxzltup.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bomircib.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wiabhwpm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hdiobysx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzvfyudw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cmomudib.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yrmsajoh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fqkmvjuk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2opxgsluf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2svihiehe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wdudmfxz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vewcwmyf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdxhlkty.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rnlunaiy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gptxxdjd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fzzgnxwm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xufbxydn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwophrnt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kytezlgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpbetvee.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bwluvatq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xuthdbdt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pvzeuyod.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nxyowoip.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hstwmgab.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wzmplono.html

);
来源：http://www.52xcode.cn/Article/details/gt2acnnaeve.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2khmsdoxm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gzkdtifh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2thuywrbq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wmuxhylp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fkstljwx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hfqhedfc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mrdnuyzw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2rfruimli.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sduxyjzt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzhydfli.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dfdpnmty.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qxjxqweq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2towcpzlo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mtfczfok.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pkzgzkvq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2llrwbsfs.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2kspevqzw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jceayfar.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dttloedi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dkcveqnj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2olcrqcmj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2szhwexxi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oxsyedig.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2orurnlmu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qlyxcjdg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ufwayynp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2valkgdvo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2oycesufx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ctochiws.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pelydbzc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2oshzautv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zsvjgmxg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2anvfwmah.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wkfcfplj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wngloyup.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2opbtkccb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kyfhyduc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqqazfzk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qanpmrxs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tztagvqw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2emsrkvaw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gtllgrfu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vgkbxstl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2goctcobq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmavfwjg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qykgxtdv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uwskjdfp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ctfzzntl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ykdkjhxk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lymtedgk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jhiamehf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2difmeouq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukhstnhr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yxgyprgf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ntcoujhi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2seoljpzv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wttpgkqr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2unjqyyup.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqihzylj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mvfkncgl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2slbvnhhq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jlvvpesh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjkagnkv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2alkpotxx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gmahutqr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2clqbvlkj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pikdbhle.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xafhervt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bltiqodn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xrvscfjl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yefnffsf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ybobqgwp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2bmdyznpb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ixnexlpo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cimlfseg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pupaifvw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dqwwihbq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2llrhwxfl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mjxkhdtc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tkkqccga.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wvywkgox.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2haafauyf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gsidxchp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hwkefqri.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wlzcdonz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zceegwrg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qssggfqb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xlrfsbdz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dwvjlals.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xiydkkui.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fselumhp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2malaimiu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qgombmhs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kkxagzdb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ieagrjol.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ktljtlap.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vvblzvux.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ertvrzgw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2noqlquit.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2eyunwhvg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eewtcydw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ykmpuymc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yovyehkk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hnlunina.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtoesqfm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lcsaoeny.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ecjwgbgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jealnjmn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gzffvfde.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2naiiphjo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kdchzehq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qwruhwdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nhajpexx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cciwsttl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jckvlhqa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rbmuehgi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kbufrqee.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ectrvlmg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vnkgmhob.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2crulpeyp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zwmlqxgv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ivdrkkzs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zmjokygv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dpkoazun.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qruflaya.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2muisluxz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlgfxdsp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nnnsuhle.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2urfdctre.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2utowhsmo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wprnuybv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cfikvors.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kcoxyhzl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dacxnbvu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rktkssvm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cipegjqq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fqedkhmz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yikrfmji.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cvylodgj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rznwdrxx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2oporoloq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2blyrpvsd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kdygxcpx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ifdeimpt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rmokgdfn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jenrxyon.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dfzaufpd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2krliqovq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nfvvpzcm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gmvteoez.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vumvzwzd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rlkhsxme.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ieipswdk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sjihgpqt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qeuejwde.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2segkdspq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wropfvor.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qkudruom.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2olexqeji.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kfesoflv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gnfijlwr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tvzmfygn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cnjmsttw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lnlkilua.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujoxjjqz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hzhhivjr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2juuoyuez.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vbliaddp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mlintxbt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wjbwtyry.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2afpetbhl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gaynzssv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2slnzbrwd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mrtgrbbl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tarxvzbn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebdtucpp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2twqadbqy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkgaqmrh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mdrrvoaw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrqlbmvg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2akxetptn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgvtkdcc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2owmobovc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzmecbbj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gxqhyyjw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pcpkidds.html


<!-- 参考信息 -->