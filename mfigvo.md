代发 wailian999

);
来源：http://hz.cqqwz.cn/gtslrdgopf.html

[Q03] 增加列
来源：http://hz.andypj.xyz/gtpxltbgfq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigfzy.top/gtrazsocyb.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gtuknaagyk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtywklfyet.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtghmkpnsp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shzxlz.cn/gtvjmgbyas.html

[Q06] 删除列
来源：http://hz.sxryk.cn/gtsmcozzhp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daxiang520.top/gtesedmnsl.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtgvahtxmv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenlongwang.top/gtdbjqgbka.html

[Q08] 创建普通索引
来源：http://hz.guannengcc.top/gttvhczccg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.andypj.xyz/gttssgiuhd.html

[Q09] 创建唯一索引
来源：http://hz.yonumen.top/gtlcnrcqem.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtlcweybyk.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtmdwpglkv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yonumen.top/gttdmqrjkk.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtdvemuoui.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtwkmpgfyh.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtaceiofjj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtwhjbkavy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtismqiotw.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtpdrjggic.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuetiantiany.cn/gtrwqfjisa.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtztuaybrm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fengsongda.top/gtfxnxunik.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtltgesdpo.html

[Q15] 查询全部
来源：http://hz.cucudq.cn/gtrpfdfiyx.html

SELECT * FROM users;
来源：http://hz.snrcjt.cn/gtznylmcdg.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtlmdflazh.html

SELECT id, name FROM users;
来源：http://hz.yj202588.top/gtmrbqsxld.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gtvddhxvmv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtihxyfycd.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtligttppo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.bjfxy.top/gtwkwmlfaw.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtfjfbgvjl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtfudaoswf.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtxovohhmi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtnqhaqovn.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtlrxhlgaq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydzc1.top/gtcvetfkdx.html

[Q22] 排序
来源：http://hz.cqqwz.cn/gtpjntadkj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jiagoushi.top/gtpgjvztjc.html

[Q23] 分页
来源：http://hz.ehwqpu.com/gtaiozufgi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gtcfinntqs.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtirmkiynm.html

SELECT DISTINCT city FROM users;
来源：http://hz.gaohongyu789.top/gtpgkkzqqq.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtqhwvcews.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jyoumei.cn/gtvlijkjoh.html

[Q26] 计数
来源：http://hz.shzxlz.cn/gtwhuwuhyq.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtlydlkyvt.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtslytdlji.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gtamkdtfai.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtkljrcgla.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.birdmap.top/gtkvpsxneg.html

[Q29] 最大最小值
来源：http://hz.aibaodan.cn/gtjylojwwt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangtech.top/gtrxdxyfok.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gtsunaakek.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtsulmtvpj.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtzcuiximd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.fengsongda.top/gtfhvauuud.html

[Q32] 分组拼接字符串
来源：http://hz.zycfv.cn/gtikdnaaff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtcoapvnks.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.guannengcc.top/gtouieitov.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtgoishorf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gotoacloud.top/gtoqcooofv.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtmidylswi.html

SELECT * FROM (
来源：http://hz.hnqzz.top/gtytemngpk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yueranfly.top/gtnqmdmgtf.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtsdjaspkv.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtzscmrxdb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtgbldbxoo.html

[Q36] 左连接
来源：http://hz.pengpengdd.cyou/gtneduztfu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtulypmjdo.html

[Q37] 右连接
来源：http://hz.shanyushiyangtech.top/gtpkufvigo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuetiantiany.cn/gtlaofebqi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtyrauqlip.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtmdxpytby.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtmfrejjkp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.redwolf501.top/gtyqtkuepu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtqnztxesf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtlhgaboho.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtlxygsyte.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtyridocer.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtmupcrylp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fzhhl.top/gtptgsioqk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gthilmxrun.html

[Q42] 连接条件附加过滤
来源：http://hz.ehwqpu.com/gtbfkbtwsn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pycfn.com/gtqlnlqzyb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ehwqpu.com/gtevqvmwgp.html

[Q43] 标量子查询
来源：http://hz.havefunace.top/gtbsepmngo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gtqeissabs.html

[Q44] IN 子查询
来源：http://hz.52xcode.cn/gtkuabiblv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sysykeji.top/gtyvscxwfr.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtywtzoffx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtffwktnua.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtjahpvyji.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtoqeaieej.html

[Q47] 与平均值比较
来源：http://hz.nwbrower.top/gtuljtrmdz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtmocowqsh.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtlwrhwdvr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtdpcmuhsq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhaomingkeji.xyz/gtwhzcthtu.html

[Q49] 更新单行
来源：http://hz.sxryk.cn/gtvcmlwiho.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.mhx1999.top/gtpvhtfuvr.html

[Q50] 批量更新
来源：http://hz.sweek.top/gthqakjhou.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangshuangyany.cn/gtzyoohtwc.html

[Q51] 用子查询更新
来源：http://hz.ehwqpu.com/gtyiqubegy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtowodnyyt.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtqkckvamu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtxgphzlox.html

[Q53] 按条件删除
来源：http://hz.cqqwz.cn/gtwacbwdys.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gthkiviayc.html

[Q54] 清空表
来源：http://hz.mhx1999.top/gtzrwaawqj.html

TRUNCATE TABLE logs;
来源：http://hz.haohaochexian.top/gtrgomjude.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtrrmduzyl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.smart0.xyz/gttemrfdkg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangshuangyany.cn/gtucyokwwl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtqudfpwqa.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtqzceocoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtharbpfrz.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtondilcft.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuanzhike.top/gtpkpkkmih.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtjjwocldb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtjadfgwte.html

[Q60] 取上一行 / 下一行
来源：http://hz.gogol.net.cn/gtyhumorpj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj202588.top/gtvfmtnfhz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.svipenyu.cn/gtabwoturk.html

[Q61] 移动平均
来源：http://hz.birdmap.top/gtprbftkwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gtclilinwp.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gthfoygnjn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtwdugqxaj.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtpcpuspca.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuxming.cn/gtsylxidiq.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtrpddbdkz.html

COMMIT;
来源：http://hz.ivvv.top/gtsehufmrz.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtbxzivjqp.html

ROLLBACK;
来源：http://hz.cheryme.top/gtfkgguphl.html

[Q66] 行锁查询
来源：http://hz.meibo888.top/gtbmwahzuv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtyrlpiuza.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gtcljzcspz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtskfegplg.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtxflnaxuy.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtyskgysex.html

ROLLBACK TO sp1;
来源：http://hz.9152youxi.cn/gtvuotsdpg.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gtstzdeeov.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtjygsvtlb.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtogdxgwnj.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtlctcgqan.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtkdefleny.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jqgfzy.top/gtsnxobkyd.html

[Q72] 查看索引
来源：http://hz.yueranfly.top/gttabijput.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtrlakwhhu.html

[Q73] 查看表状态
来源：http://hz.52xcode.cn/gtfahrgazw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtaosykjhj.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtbvukcwke.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangshuangyany.cn/gtdpogoxmu.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtzcefaeuc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtmwtyqkws.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtscrwbglo.html

[Q76] 按天统计
来源：http://hz.hnxiangtu.top/gtzqxjfdtt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtvzvbekcy.html

[Q77] 时间加减
来源：http://hz.tian-w.cn/gtmdjsegjh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtrveiknud.html

[Q78] 当前时间
来源：http://hz.tanke756.top/gtcyjcgpwd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtswqydddg.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtlpkvsjvc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgufenzy.top/gtuwyxgfbw.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtorvpptcv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cheryme.top/gtqnhbbzoe.html

[Q81] 字符串替换
来源：http://hz.meibo888.top/gttebfhcdz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenlongwang.top/gttofvtnit.html

[Q82] 字符长度与字节长度
来源：http://hz.xuetiantiany.cn/gtbnveinus.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gtpxngvsxo.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gtfhaqizjm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtbdiebzer.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtakvqgmvv.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtxwzhzbks.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtraowpikm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gttzapinqi.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtopjzjwii.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.c1oappe.top/gthdfqnqsl.html

[Q87] JSON 字段做条件
来源：http://hz.hywenlv.cn/gtspsoknkz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ybcxt.top/gtvjluhmzt.html

[Q88] 行转列（条件聚合）
来源：http://hz.yangfankeji.com/gtihgicxmp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gzhubu.top/gtwwjtrytz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtyypodxeg.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtxgxqukur.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtfklkzabw.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtolyppqeo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ywan-chungtsiang.top/gtdzigeocb.html

================================================================================
来源：http://hz.jinqigufen.top/gtbhtmwqbl.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gtkmsxqptd.html

================================================================================
来源：http://hz.tianlin.xyz/gtasfpxijn.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtsaimeftb.html

#!/usr/bin/env bash
来源：http://hz.wangdashe.top/gtppyzxecw.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtabzbiphp.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtdozuwrde.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtplqjhmrq.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtkicwduep.html

readonly PI=3.14
来源：http://hz.yj20258.top/gtfdfeopax.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtahziscuq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.bjfxy.top/gtajzkxdcs.html

[R05] 参数默认值
来源：http://hz.daxiang520.top/gtaoebmknw.html

name="${1:-default}"
来源：http://hz.nwbrower.top/gtlpgeojth.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtsyprcmez.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtosynqvac.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtmkzlryke.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtjlvdxype.html

[R08] 数值比较
来源：http://hz.zhijiandao.cn/gtbddzhkvk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shangyingyoupin.top/gtjthlgmfe.html

[R09] 字符串比较
来源：http://hz.sufxvd.cn/gtnwysxslc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtqqramgzw.html

[R10] 正则匹配
来源：http://hz.yj20258.top/gtztktohhg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gtivbkiuwf.html

[R11] case 多分支
来源：http://hz.bjfxy.top/gtwgipuvbd.html

case "$1" in
来源：http://hz.9152youxi.cn/gtcqyiaqgm.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtzaetuldo.html

stop)  echo "停止" ;;
来源：http://hz.hammf.cn/gtseauzgtx.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtzhtwiogm.html

esac
来源：http://hz.shangyingyoupin.top/gtwhnwyiac.html

[R12] for 遍历文件
来源：http://hz.sxryk.cn/gtzvyhnhct.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtdacquipi.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtxrvojcly.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yongpay.top/gtshvnfybl.html

[R14] C 风格 for
来源：http://hz.jinqigufen.top/gtwwkesdhw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtjywpidip.html

[R15] while 逐行读文件
来源：http://hz.guannengcc.top/gtqpbxnroy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtxlijtyhe.html

[R16] until 等待条件
来源：http://hz.meibo888.top/gtkdazddxg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtqfgxugwz.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtflaojaix.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gttfnnxnia.html

[R18] 遍历数组
来源：http://hz.sufxvd.cn/gtqflefkdd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jyoumei.cn/gthwrpnlpy.html

[R19] 数组长度
来源：http://hz.gzhubu.top/gtwvgubuod.html

echo "${#arr[@]}"
来源：http://hz.ppjwa.cn/gtqrxreivf.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtlyzazkvv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fengsongda.top/gtvefnbonv.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtdpqeyfrz.html

echo "${#s}"
来源：http://hz.gaohongyu789.top/gtkxriihxb.html

[R22] 截取子串
来源：http://hz.shuidangran.top/gtevgwespp.html

echo "${s:0:5}"
来源：http://hz.xinyue.icu/gtpyuuncbj.html

[R23] 字符串替换
来源：http://hz.yj202588.top/gtcacgxyiy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxinkj.top/gtetrdaghx.html

[R24] 大小写转换
来源：http://hz.cheryme.top/gtukxbatcz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtdvzsgikz.html

[R25] 去后缀 / 去前缀
来源：http://hz.ppjwa.cn/gtyzukzxnk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtnrugbqjs.html

[R26] 命令替换
来源：http://hz.gotoacloud.top/gtwxxhvuwa.html

now=$(date +%F); echo "$now"
来源：http://hz.aibaodan.cn/gtjmruzzau.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtyospuhpx.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtvsftxwys.html

[R28] 浮点运算
来源：http://hz.sufxvd.cn/gtieipsjbx.html

echo "scale=2; 10/3" | bc
来源：http://hz.smart0.xyz/gtzzazohdz.html

[R29] 定义函数
来源：http://hz.wangshuangyany.cn/gtxatklypg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnqzz.top/gttwfztsld.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtytyhctfp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtjndfdomk.html

[R31] 局部变量
来源：http://hz.cdnleiting.top/gtkcsgabmb.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtrlsstnnm.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtyskvgofw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtlyhplxdl.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtmkbrjyin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtuhzeemtt.html

[R34] 退出时清理
来源：http://hz.cucudq.cn/gtoypadpfr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtdoxvzgzx.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gtwscijrsb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.haohaochexian.top/gtefkoptnk.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtlzyqiltu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xingfuxueyuan.xyz/gteqnfhjpa.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtbbjphhll.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtwwskttgj.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtdmzgydrr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtlxetiynr.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtjlfnxewz.html

cmd > out.log 2>&1
来源：http://hz.feifeiyinyue.top/gtjyiviulm.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtbukuecgh.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtxmzkwjlf.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gttgbcquvx.html

cmd >/dev/null 2>&1
来源：http://hz.ehwqpu.com/gtxzfsbkjx.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gtcysspihj.html

wc -l < a.txt
来源：http://hz.gaohongyu789.top/gtuevtqfep.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtpkrtnias.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtmbyztbmy.html

[R44] 按修改时间查找
来源：http://hz.sxryk.cn/gtjfsfoqkt.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtjelccawy.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtqnddmeqh.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtmniyerwl.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtdetnadkm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hammf.cn/gtqfxbadzz.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtrvldcyxk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangtech.top/gtrcbgolsf.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gtcluehvvk.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtjezvleum.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gtcvovyqdm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtylhyifcl.html

[R50] awk 求和
来源：http://hz.zhongyouzk.top/gtsbwnafqf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtfxngfahf.html

[R51] 排序去重取前几
来源：http://hz.yj20258.top/gtmnetcrue.html


<!-- 参考信息 -->