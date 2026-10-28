代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtsnezzfvz.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtwbqwseun.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtqmhkwxzh.html

[Q10] 插入单行
来源：http://hz.hammf.cn/gtukmpzbev.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.smart0.xyz/gtovppqzhu.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtrrqtphex.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxuanxn.top/gterbshxef.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gteforlcyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yongpay.top/gtatpqsagz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtjqcnockf.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtablfynpr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gtpbdkxlab.html

[Q14] 存在则更新（upsert）
来源：http://hz.gogol.net.cn/gtdtodkver.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtnbblmkzg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gtbgjrcmdl.html

[Q15] 查询全部
来源：http://hz.guannengcc.top/gteturrhpm.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtverqkxxu.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gtkmlqqedv.html

SELECT id, name FROM users;
来源：http://hz.snrcjt.cn/gtmfotjhtc.html

[Q17] 条件查询
来源：http://hz.52xcode.cn/gtskiwfhvj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gtjmpjaosx.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtmkyslhix.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhijiandao.cn/gtaqcvqzkx.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtoihtyiri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jiagoushi.top/gtnhptsmor.html

[Q20] IN 列表
来源：http://hz.gotoacloud.top/gtbbiezqxu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.svipenyu.cn/gtjzmdhmgm.html

[Q21] 空值判断
来源：http://hz.jinyuanbaomall.cn/gtslvrxxqs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinghuilouyu.cn/gtpauoqvmv.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtounoqxdl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtmfmqvypl.html

[Q23] 分页
来源：http://hz.havefunace.top/gtcmntwunz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtzsibgtov.html

[Q24] 去重
来源：http://hz.kuanghao11.cn/gtzppswjis.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtmebwgeuy.html

[Q25] 只取前 N 条
来源：http://hz.yonumen.top/gtsvotgtzv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ybcxt.top/gthnjlhfgk.html

[Q26] 计数
来源：http://hz.xuetiantiany.cn/gttltiexst.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtkteqcflf.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtdwgvpetf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtksxucthb.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtladosout.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtxxvhryiz.html

[Q29] 最大最小值
来源：http://hz.zhongyouzk.top/gtxncvkopk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gtthzsfcnp.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtiorhmujv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtxttqaknu.html

[Q31] 分组后过滤
来源：http://hz.gotoacloud.top/gtjijxykmv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtiqzfdges.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtsfuiligz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtrgtsaxqn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tanke756.top/gtfhuhzpru.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtemacpmvq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtnowxsdbs.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtxmufzmqw.html

SELECT * FROM (
来源：http://hz.ppjwa.cn/gtejbbjtxo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cheryme.top/gtjfadydbl.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtdqrrrzny.html

[Q35] 内连接
来源：http://hz.birdmap.top/gtplimjgmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtdryyslsd.html

[Q36] 左连接
来源：http://hz.kuanghao11.cn/gtpxtbyjxb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtcohgonam.html

[Q37] 右连接
来源：http://hz.sxryk.cn/gtrwmvnvmr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gtbywlmuwd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gtfwxrpleu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gtsavowdtr.html

[Q39] 自连接（查上下级）
来源：http://hz.jinyuanbaomall.cn/gtqpsdkbor.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cashguo.top/gtqyticldt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhijiandao.cn/gtpfjmsdfw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258888.top/gtxswiwywm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fzhhl.top/gtmbmuqqtu.html

[Q41] 多表连接
来源：http://hz.yuanzhike.top/gtzlqrplbe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtdpensweq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtaxjexukh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangdashe.top/gtkgejkdmw.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gttuchjutg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtrpvqistc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gthtyvjeln.html

[Q43] 标量子查询
来源：http://hz.gaohongyu789.top/gtcjggzeti.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ivvv.top/gtqjtzhvyx.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtwqsibqyj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gtmqgvitzq.html

[Q45] EXISTS 判断存在
来源：http://hz.ywan-chungtsiang.top/gtsgleshpm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtdekhkvtc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtoabjzbyk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gttimbpdqj.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtmycroird.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtstidybzg.html

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gtrjrxjdzv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hongshengwenyu.top/gtxqteklrr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhiwuduotai.top/gteafsbzrt.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gtggpfwlqs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenlongwang.top/gtcbvmkhnz.html

[Q50] 批量更新
来源：http://hz.316326.xyz/gttonhurju.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtzcsuehfx.html

[Q51] 用子查询更新
来源：http://hz.ywan-chungtsiang.top/gttztjgoqg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtwcpdlmfh.html

[Q52] 删除指定行
来源：http://hz.hnqzz.top/gtjsrjiicf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtjololwkl.html

[Q53] 按条件删除
来源：http://hz.sysykeji.top/gtdwdhjewe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenjidiqi.icu/gtczvzdlfk.html

[Q54] 清空表
来源：http://hz.feifeiyinyue.top/gttuargnxk.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gtlhnmttiw.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtbbuwwjkn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenzaomai.com/gtqhwuzhkl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daxiang520.top/gtxorolcrx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gthnkwdpos.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtlpsbmnpx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangtech.top/gteqkcqpfl.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtcgfrhlup.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gzhubu.top/gtbsspzlmv.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gthttspbqy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtlauiojbm.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtoqhpwwge.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj202588.top/gtmmlwosbm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtmuyjvsmc.html

[Q61] 移动平均
来源：http://hz.xuanzx.com/gtuhrsnrgy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhongyouzk.top/gtcmlhoqdp.html

[Q62] 分组占比
来源：http://hz.fengsongda.top/gtpuzlanpp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtjqtutdnx.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtijhgryom.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jlsjyb.cn/gtgkblsfio.html

[Q64] 提交事务
来源：http://hz.ivvv.top/gttjoiugnn.html

COMMIT;
来源：http://hz.nanxuanxn.top/gttkjpcfiz.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtsljgmelc.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtxicobxmr.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtkqxiybec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xinyue.icu/gtjahaqsgs.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtihaoafpl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.feifeiyinyue.top/gtcxzudivo.html

[Q68] 保存点
来源：http://hz.ybcxt.top/gtdllkviln.html

SAVEPOINT sp1;
来源：http://hz.iojbl.cn/gtwqpvjkwb.html

ROLLBACK TO sp1;
来源：http://hz.jiagoushi.top/gtcneshyzk.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gthkzvnexp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtwfnjzurl.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtxiicjsjz.html

ANALYZE TABLE users;
来源：http://hz.nanxinkj.top/gtbmtwnjth.html

[Q71] 查看建表语句
来源：http://hz.9152youxi.cn/gtlbdentax.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ywan-chungtsiang.top/gtqemhytmm.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gthauzofuy.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtnkxwesys.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtmvxwdnfm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgfzy.top/gtdgdktaxp.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gtzygpoobk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydjk.org.cn/gtuquizjkr.html

[Q75] 日期格式化
来源：http://hz.meibo888.top/gtunyfehwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gtesyzhmvz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtbqggfvnl.html

[Q76] 按天统计
来源：http://hz.sxryk.cn/gtxxfeouqr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ehwqpu.com/gtskmgfeex.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtjxlxtdfj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guowangkeji.top/gtpgktxnqd.html

[Q78] 当前时间
来源：http://hz.gogol.net.cn/gtcrxfcgoj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.smart0.xyz/gtbquggdtm.html

[Q79] 字符串拼接
来源：http://hz.jianghu66.top/gtqoupdsdw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtkskwqkuo.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtdqxdopli.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.haohaochexian.top/gtvbxcddju.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtfyrifblk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.redwolf501.top/gtzzbiefxc.html

[Q82] 字符长度与字节长度
来源：http://hz.redwolf501.top/gteblzigwo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gtpefkysng.html

[Q83] 大小写转换
来源：http://hz.sweek.top/gtjzaiyolw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtlpzynavi.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtbkdholrb.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtpfosqgha.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtvzuvkrid.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtmomvgzqb.html

[Q86] 读取 JSON 字段
来源：http://hz.redwolf501.top/gtjwvkzmcw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gaohongyu789.top/gthwlmoayb.html

[Q87] JSON 字段做条件
来源：http://hz.yuanzhike.top/gtowwpijst.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtdhuvmehe.html

[Q88] 行转列（条件聚合）
来源：http://hz.xylfe.cn/gtakjiwtlp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangshuangyany.cn/gthcsjlhwg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jianghu66.top/gtoysdnajj.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtnymxwmzz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gttpmulvxp.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtxjbdndie.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxinkj.top/gtuvrjojxv.html

================================================================================
来源：http://hz.gotoacloud.top/gtptpkwjub.html

R. Bash 专题
来源：http://hz.pycfn.com/gtnggobkiz.html

================================================================================
来源：http://hz.sysykeji.top/gtqpvkwtar.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gthwbpbozl.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gtanfxlepq.html

set -euo pipefail
来源：http://hz.shanyushiyangtech.top/gtkhaddzjk.html

[R02] 变量赋值与使用
来源：http://hz.ywan-chungtsiang.top/gtugcejbne.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtbzhuvvjg.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtjpmibmpm.html

readonly PI=3.14
来源：http://hz.c1oappe.top/gtzptrtdpi.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtptisuoqa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtaodsjgdm.html

[R05] 参数默认值
来源：http://hz.aibaodan.cn/gtdxiombvs.html

name="${1:-default}"
来源：http://hz.gotoacloud.top/gtmoppjmgk.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gtonqpvaed.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtslpwgrmw.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtwpnajvtf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhengqikj.top/gtizbepbdq.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gtcwgwftbr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtlrpyxllb.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gthdfrbqij.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gotoacloud.top/gtnofhpwby.html

[R10] 正则匹配
来源：http://hz.hysaishi.cn/gtayiuutmz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangdashe.top/gtatqjktcm.html

[R11] case 多分支
来源：http://hz.xuanzx.com/gtpqacmcih.html

case "$1" in
来源：http://hz.chenlongwang.top/gtgnxvpajs.html

start) echo "启动" ;;
来源：http://hz.hongshengwenyu.top/gtxvgfmcco.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtwtdcgydj.html

*)     echo "未知命令" ;;
来源：http://hz.cucudq.cn/gtzhpdhmyd.html

esac
来源：http://hz.gaohongyu789.top/gtisvsmiru.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtxlqprraj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sufxvd.cn/gtybxwzpww.html

[R13] for 计数循环
来源：http://hz.jqgufenzy.top/gtrrsbufli.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtifcnpkmt.html

[R14] C 风格 for
来源：http://hz.shanyushiyangkeji.top/gtdcxorgkl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gtjquztnjy.html

[R15] while 逐行读文件
来源：http://hz.daria6918.cn/gtbopplfti.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtapiygebj.html

[R16] until 等待条件
来源：http://hz.cucudq.cn/gtqmhvrfgi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hfpthk.cn/gtccyzjusm.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtkswhuyqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtinqhbjda.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gttycqaopw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtlmdmopcf.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtsxymulss.html

echo "${#arr[@]}"
来源：http://hz.sysykeji.top/gtqygemzlr.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gtfazrimrb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhengqikj.top/gtyetrhpyx.html

[R21] 字符串长度
来源：http://hz.zhoulong.xyz/gtgrzufcum.html

echo "${#s}"
来源：http://hz.birdmap.top/gtxyuqkpfx.html

[R22] 截取子串
来源：http://hz.dashuyun.cn/gtzzttgafo.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtinzkoiqq.html

[R23] 字符串替换
来源：http://hz.cucudq.cn/gtfvikrhhs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtjrvykunz.html

[R24] 大小写转换
来源：http://hz.cashguo.top/gtnfhxexjw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gtrsgtwecv.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtijyabklz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aizwys.cn/gtvkdvyfco.html

[R26] 命令替换
来源：http://hz.hfpthk.cn/gtaqrmmnmg.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gtwjsywsyd.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtesxaueqk.html

echo $((1 + 2 * 3))
来源：http://hz.cucudq.cn/gtqaikhgsg.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtrkwdwzad.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtafsbeohe.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtjanbxfvh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtcrwazpsn.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtvnqbkbjj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhengqikj.top/gtnamylbol.html

[R31] 局部变量
来源：http://hz.jqgufenzy.top/gtgmfxpvgo.html

f() { local x=1; echo "$x"; }
来源：http://hz.cheryme.top/gtroltdzpv.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtcsotncpu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xinyue.icu/gtccbxtort.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtcnpscmkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtuaqmenpn.html

[R34] 退出时清理
来源：http://hz.zhixingplan.top/gtjndgpksc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtxvckgxoj.html

[R35] 后台执行并等待
来源：http://hz.guowangkeji.top/gtktvperav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhoulong.xyz/gtgdtqwski.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtitwacscy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.0kj1m.cn/gtopnkdvrt.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtcbtoohyz.html

files=$(ls -1)
来源：http://hz.zdqjudy.top/gtuzifqlur.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gttyvobkty.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenlongwang.top/gtxuwqduvt.html

[R39] 重定向标准输出与错误
来源：http://hz.havefunace.top/gtxsefjbwj.html

cmd > out.log 2>&1
来源：http://hz.xuanzx.com/gtglccoqlz.html

[R40] 追加写日志
来源：http://hz.zhixingplan.top/gtexpaxpfe.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtztjpsgsh.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtlvmqwgti.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtmdobzxre.html

[R42] 输入重定向
来源：http://hz.xuanzx.com/gtiteupdve.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtnnztaakz.html

[R43] 按名字查找文件
来源：http://hz.zhaomingkeji.xyz/gtnpqkchlx.html

find . -name "*.log" -type f
来源：http://hz.zycfv.cn/gtvrsbmxbj.html

[R44] 按修改时间查找
来源：http://hz.daria6918.cn/gtbzgntyif.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtvohseaox.html

[R45] 批量删除
来源：http://hz.yueranfly.top/gtmbouesev.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtnycogyip.html

[R46] 递归替换文件内容
来源：http://hz.hywenlv.cn/gtvbzmjecp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gtjzppvnvm.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtrbmzgwif.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtwlqtcxmi.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtptqqyfft.html

awk '{print $1, $3}' a.txt
来源：http://hz.ydjk.org.cn/gtoycuezxz.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtlnmswvjh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj202588.top/gtemhrekzl.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtvfzgwjew.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sweek.top/gtbxyhrcpc.html

[R51] 排序去重取前几
来源：http://hz.tanke756.top/gtvvhbrgjs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yanxiufei.cn/gtpvgaczbe.html

[R52] 统计行数
来源：http://hz.hysaishi.cn/gttftfpqag.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtipyfkcke.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtcyfruqdk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtaxeapnqp.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtikaulvxq.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gtzywmbfcx.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gthkcgjbfr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtctnjjdep.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtouoawran.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gtevayprrs.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtojyzgaud.html


<!-- 参考信息 -->