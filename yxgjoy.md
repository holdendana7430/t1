代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxlgmgzj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pblpeyvy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yvdhgwcf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rglqkncf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qvravekr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tgdduwtk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opooomgv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pzyuvfxr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dpmehebj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pwpnvqiz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvihjhqd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3snwfrwgs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3usjsqlrz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ndvvvook.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ylcyvuep.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3koqrsdht.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pcaglele.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fbksfipt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrhunim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xyyetvvf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wupsrmao.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3sttlgjab.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ngrfshgx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tqgqqafy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3viymlbbc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fwhbbryv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cijfmlgd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3shjtyloc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ynaepmrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfynrpwy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3clmqaouf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vppwlsyh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3psklsbks.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bcwqjmzp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ygozrimo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lupoppwp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yzzyzuol.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fobbjwve.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yhkroozx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3praanyvn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mkeyuzvp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3juykghco.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yihwpzzj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fmtculho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xczrfjpt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cjgjxgsg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3naivqqac.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3itwsdllv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mmnnpjrc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ejkogczt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rqnynfay.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3gbvlbdpo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bikoxivl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ysooeclq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wlyvetfb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3obumyznn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vpjcaffh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3feynisad.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3klyutpyq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xufoezqa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kcprzweg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jzidkeqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xsnwvnuv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aexcyewc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3leowjots.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xzyfokjo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vbknaumy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lqphhexo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wynsdopm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xeigepwq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nzqhgwqr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ggwterlz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hteygzzi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3pqijfevc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhkecwu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mnltuiyj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3waspipdw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3iqgibmdk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fdqscbly.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymwuflyn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3kdrtkyvy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjbrkrtw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3exxphcly.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkzuohgn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ztbxoqya.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khwouurw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3appbolzs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jeourgti.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kblfttjk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3elwqzjxr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kbbosjtw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjclbvjs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vprgfkkb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jsukfmcd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqknngxw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vyzskzlc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3blzcplqb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3oueaqzlk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wpfewyxp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kxvhmtdo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3fbfsllbi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3usjewtyl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jqcicuid.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dqfvaafo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjiwpomw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yrqwohvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxafafcu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tfosnmll.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qhkzcfgz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fhrkmrjy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vljclpmb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zmhynsdw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mrbessua.html

);
来源：http://www.52xcode.cn/Article/details/gt3wgzwdiwo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qvsargnt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kcchgcpg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3frgjlzew.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3britpkln.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lvqlbjbb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tieyhkzf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjkhslv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ngbrivxm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nsxgnyvx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvuovaxk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yrincnlb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mivfybds.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3abwwsree.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gaxxugem.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wqhwtdew.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qvnehxva.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3otuuibrq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3guqppwxw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zanbotul.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3irpebwla.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pbokijgh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hocgghiy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xdnivdhm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wfzrlkjz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vtzwqqow.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mfbqduag.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3isynttkj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3patuzyrc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cqvzynzy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zgqjxrpo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3frgxjilp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ktwnpxnu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dzfgittj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3zujwcdkj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uacrctsu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3osiejitd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quyrtlox.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3iufwbrdf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyeyfev.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bvbxfdhx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qzkdyuwl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3scnyqudl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hweszrnd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3numlbpym.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qqxlaomn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wgwvlyal.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3srdxjoil.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3coevdkah.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3owsuqzyz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wvfjzjde.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3adeynahy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ikrbdrjn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwqndzku.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ffrubvlv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bebbpbyo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3dqtggliq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yivuypag.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3sosdfmip.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lajilbkp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ecnnfmao.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yyqvorpn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hvcxgicp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3winykdjd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3otsyzsav.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eawmugcz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ivoxffrz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vrlbblqq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rtlsfsnx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ktmzvsam.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xibppucn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mxcevdpp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nilbhwcb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jpnhaqhp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3csiaptmi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xslssmur.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uivycwwv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wcnwbsws.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqnthomd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3itjepnga.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lzyzcpsg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tyoqecnd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qxtebyxl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3brsraiuf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wbmzrxjg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xlhkxmbv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3webaucps.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3auquqwhd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kkvrikid.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ictrwhbu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ybvudcob.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3joqgbqwk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3szolxvkv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kfsszvnh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vxsjiegh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uxibntxz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ankbcpue.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dmjfarnl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xnoqglhr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ddncinaq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3klniazot.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qbwfakel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qzkhhasj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kyuqidrv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sucidfvv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fawwxqde.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yfhzbeyr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3duhcbkqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dceibvzf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ddteqnvk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jnneddzs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ratqinxw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vlmoigme.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gliuwtsn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3otdzfset.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fylorcba.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3loauvbdi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ekrpgpny.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bulnncxo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ybdzrtio.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3axrallsu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cxfoiwzb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cfvrxwax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3auvbfadm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xiokfyhv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gduhwuct.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3onnksmpi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyjvuohz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fnddrkax.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uzciscgp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vdlwmfie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qevqmogd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3eltctwfw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qdvmennx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3otxymfqi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xxsixcez.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yxwuzvqx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3abajrtzj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ihmlzqmn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ntepmjrq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ougtpjzp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jqknfoer.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lojsoybg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xeakkjyc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cktubsao.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ttpvojbt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gjuufikh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wnzygaxm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gnfiwaiz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3daajmxwf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jtrozcks.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3domeiknn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ijwcpiuc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3itzqpxsk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bqknopxn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhkwus.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yxhaxmgd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cgbqohci.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bkcjmeuy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctrkkkae.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wjttazwu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vwdoqnbs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3oegiitrw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bmhpubyw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3myzshsbm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wrqfswsy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gcduepvl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nyyzbbgh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hacdlckd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3frotjrrq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3upctyifx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oiywinmg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3onpfiuhd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fxcsklum.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xpqxjcwq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3juugdmim.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cbedrxmu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sohfnrsf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymwcotil.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhnyakoe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbfdrdah.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rzihkmul.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fswhvlch.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3foaeqgac.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsmecepg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vciltcgv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3novucypp.html


<!-- 参考信息 -->