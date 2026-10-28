代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gteppyhcgt.html

[Q07] 删除表
来源：http://hz.hywenlv.cn/gtansvapfj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtfaaovpad.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gtbgsjonzu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gtmnhbcfbb.html

[Q09] 创建唯一索引
来源：http://hz.daria6918.cn/gtrlhrmnbn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jianghu66.top/gtishiugze.html

[Q10] 插入单行
来源：http://hz.jlsjyb.cn/gtsnufslzw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhaomingkeji.xyz/gtqtidiima.html

[Q11] 一次插入多行
来源：http://hz.vqdsnc.cn/gtdrhgcuba.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxinkj.top/gtbvqausdm.html

[Q12] 插入后取自增 ID
来源：http://hz.jianghu66.top/gtvcqecyxo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.andypj.xyz/gtkzfvpwkr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinghuilouyu.cn/gtirribsgo.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtntzsuxig.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gtgxixbobl.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gttodhlsvf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shuidangran.top/gtlrdtfhfd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhoulong.xyz/gtkslgvyeh.html

[Q15] 查询全部
来源：http://hz.ppjwa.cn/gtkiewryvm.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtcucqgxgm.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtjrbconvq.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtrgqycgtm.html

[Q17] 条件查询
来源：http://hz.havefunace.top/gtkxbxgyca.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangtech.top/gtyxfitlzy.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtoedmjugy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gtimcjndqn.html

[Q19] 范围查询
来源：http://hz.chenjidiqi.icu/gtagoqesyh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gthrdcuarc.html

[Q20] IN 列表
来源：http://hz.nanxinkj.top/gtxznbbwgg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtslgvbnwj.html

[Q21] 空值判断
来源：http://hz.chenjidiqi.icu/gtmyptpqnm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtwfvrveqx.html

[Q22] 排序
来源：http://hz.havefunace.top/gtesgebaxw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shangyingyoupin.top/gtswbmaelb.html

[Q23] 分页
来源：http://hz.cdnleiting.top/gtpyafsgls.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtagwaiudz.html

[Q24] 去重
来源：http://hz.tian-w.cn/gtxrbhsuka.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhijiandao.cn/gtysyzyxbq.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtxzpaplxu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtjeyablee.html

[Q26] 计数
来源：http://hz.ywan-chungtsiang.top/gtpletgnaz.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtghpcvypk.html

[Q27] 条件计数
来源：http://hz.xylfe.cn/gtkqskujcx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnxiangtu.top/gtocvikmvk.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtdsrnwsoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gtqykkcwnr.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gtrxbatkuh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinghuilouyu.cn/gtuhwsvacl.html

[Q30] 分组统计
来源：http://hz.cqqwz.cn/gtgjjambdu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtkyfrmfkn.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gtbfddsdhu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtdafuxbva.html

[Q32] 分组拼接字符串
来源：http://hz.ybcxt.top/gtqmtwqulb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtjzduwgsv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gterjifbpt.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtvlkpciko.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sxryk.cn/gtwdevchfs.html

[Q34] 每组取第一条
来源：http://hz.aibaodan.cn/gtdfccpopv.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gtiruyuwny.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hfpthk.cn/gtoawqhyyn.html

) t WHERE rn = 1;
来源：http://hz.pengpengdd.cyou/gthnanadca.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtirfdthnv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtmgfvdiim.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtnefsnovd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtsiieeezj.html

[Q37] 右连接
来源：http://hz.gogol.net.cn/gtestesoeh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenlongwang.top/gtqczcgetn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj202588.top/gtqfwhoorw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aizwys.cn/gtmvkjqwaj.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtynrwmpht.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtaumsbypj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtbenigikf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gthshyiave.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yanxiufei.cn/gtwwlgxduo.html

[Q41] 多表连接
来源：http://hz.hammf.cn/gtaiuesapy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cdnleiting.top/gtzcokckkm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hammf.cn/gtxpyjmchq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hywenlv.cn/gtdwsofmyv.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gttjewovxw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtbdgrtron.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.snrcjt.cn/gtyhlqjktd.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtxlvdwcgr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhengqikj.top/gtvpdwcett.html

[Q44] IN 子查询
来源：http://hz.ydzc1.top/gtgvjkhdax.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gaohongyu789.top/gtjufyrpag.html

[Q45] EXISTS 判断存在
来源：http://hz.wangdashe.top/gtqetqohng.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtvvoepybd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gthcjgdqid.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtsifktqef.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtpprfaoaa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtmwlhfjfi.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtwmavbqho.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gteaptzbry.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtqjtwzlza.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtqpkrwvsp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sxryk.cn/gtvdmlzzdl.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtilmmxukk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.andypj.xyz/gtbpunmfps.html

[Q51] 用子查询更新
来源：http://hz.ydzc1.top/gtftjdpwfz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtlkkyphxm.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtinwrfcdk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.c1oappe.top/gtfnmybbjn.html

[Q53] 按条件删除
来源：http://hz.yj20258888.top/gtrpypuuns.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtqtmqppki.html

[Q54] 清空表
来源：http://hz.jiagoushi.top/gtdwenhxjh.html

TRUNCATE TABLE logs;
来源：http://hz.cqqwz.cn/gtwrtsrsus.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtecvtqmgv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtjebbpwlu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtqqreodwx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gttiedvjeh.html

[Q57] 行号
来源：http://hz.jqgfzy.top/gtqdfugsyi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tanke756.top/gtxjdpagzz.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtstlwdcwk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtzjqobgnk.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gthgmcjhyo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zycfv.cn/gtnytfrdwk.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtcrohmywm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnxiangtu.top/gtyorspiml.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dashuyun.cn/gtynywitwp.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtekvhiaae.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gthztcirpn.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtzchaaegp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtwskoolbi.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtzotyjpjr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtuohxxhjv.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtlxpyxiab.html

COMMIT;
来源：http://hz.pycfn.com/gtspvdqqlf.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gtwsggnmbb.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtozaalcnl.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtlzlotkek.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtdmttuohq.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtgtmeyfqz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtmtzochzn.html

[Q68] 保存点
来源：http://hz.pycfn.com/gtqjlwpuey.html

SAVEPOINT sp1;
来源：http://hz.yonumen.top/gtonpnspyp.html

ROLLBACK TO sp1;
来源：http://hz.hysaishi.cn/gtxjufcnni.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtryyobmra.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shangyingyoupin.top/gtmtjhzuon.html

[Q70] 更新统计信息
来源：http://hz.yuxming.cn/gtzwibdquk.html

ANALYZE TABLE users;
来源：http://hz.yonumen.top/gtpcfvgldw.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtohdgxrru.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.feifeiyinyue.top/gteqvbxeur.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtdwhkynls.html

SHOW INDEX FROM users;
来源：http://hz.yj20258888.top/gttznczilq.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtkxvaalnh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtowwtinpk.html

[Q74] 强制使用索引
来源：http://hz.aibaodan.cn/gtxkatnfcn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hammf.cn/gtqsvhnlhr.html

[Q75] 日期格式化
来源：http://hz.jyoumei.cn/gtqhgakcme.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtvkdevchh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtwxpvdnyx.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtblvcqqoi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtvnzzsmcs.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtuzrhbwnj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhengqikj.top/gtwsuopzdd.html

[Q78] 当前时间
来源：http://hz.cucudq.cn/gtwczblzyd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtoemelxtw.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gthxtkfeal.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhongyouzk.top/gtsrapixic.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtoyyikudq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.andypj.xyz/gtdcbvgtoc.html

[Q81] 字符串替换
来源：http://hz.ydjk.org.cn/gtcwfrgngs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtrpmbzzyw.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gteqbmhwzn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jiagoushi.top/gtwfrsmqwy.html

[Q83] 大小写转换
来源：http://hz.ydjk.org.cn/gttkfbmuvf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gogol.net.cn/gtfzhvmnjy.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gthkarvpjg.html

SELECT TRIM(name) FROM users;
来源：http://hz.birdmap.top/gtngcoqwnb.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gttuxeqjgx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtgoxnpsok.html

[Q86] 读取 JSON 字段
来源：http://hz.havefunace.top/gtwidqkbwa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtinnvjybl.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtorexteof.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtpzqkhnju.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gtcnjjzvwl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtfnrhbijb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuetiantiany.cn/gtttvazmqx.html

[Q89] 判断表是否存在
来源：http://hz.cheryme.top/gtcxcjlgrb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtrvcctfsm.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtvpqfpdyc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtukkthzcn.html

================================================================================
来源：http://hz.nanxinkj.top/gtvfyidpqt.html

R. Bash 专题
来源：http://hz.ivvv.top/gtgjesjuui.html

================================================================================
来源：http://hz.birdmap.top/gtwvlbbudz.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtlzieytgk.html

#!/usr/bin/env bash
来源：http://hz.kuanghao11.cn/gtwjjounfh.html

set -euo pipefail
来源：http://hz.haohaochexian.top/gtyghtnvyb.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtcouicaft.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangtech.top/gtboaggrmz.html

[R03] 只读变量
来源：http://hz.52xcode.cn/gtysdinkzs.html

readonly PI=3.14
来源：http://hz.havefunace.top/gtxswomamz.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtnfnryvbb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gtvkwcntct.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtwhmdqljg.html

name="${1:-default}"
来源：http://hz.shanyushiyangtech.top/gtriqxnywo.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtgsusywnt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtoprauwpf.html

[R07] if 判断文件
来源：http://hz.cashguo.top/gtftuqndnm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gotoacloud.top/gtpxfogdoh.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtjidbqykl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtgcdqbvct.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtczmpxuvk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtlkaahvaj.html

[R10] 正则匹配
来源：http://hz.yanxiufei.cn/gtfscmlvtv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtexfxwsba.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtmvwmisto.html

case "$1" in
来源：http://hz.xinyue.icu/gtylkxgtqa.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtypypaocg.html

stop)  echo "停止" ;;
来源：http://hz.wangdashe.top/gtkpxxnsty.html

*)     echo "未知命令" ;;
来源：http://hz.ydzc1.top/gtlugeymmn.html

esac
来源：http://hz.316326.xyz/gteoivmvqx.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtcnzdgwht.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gtiqmhthaj.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtgfbyjtkt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtuoqualmv.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtieghglat.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtmcopnxrg.html

[R15] while 逐行读文件
来源：http://hz.fengsongda.top/gtixhkfgci.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yvedp.cn/gtyhxcdwkm.html

[R16] until 等待条件
来源：http://hz.haohaochexian.top/gthanrfrjv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtpekbgxpi.html

[R17] 数组定义与取值
来源：http://hz.gotoacloud.top/gtzgzvnqfe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtogexhaqu.html

[R18] 遍历数组
来源：http://hz.yj20258888.top/gtmetnotmy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dianchejie.cn/gtdyvxyytb.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gthavyamvs.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gtrlowtcxc.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gtckfwnnvq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtfyejkdxp.html

[R21] 字符串长度
来源：http://hz.yj20258.top/gtmqngmaky.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtasdyfrdw.html

[R22] 截取子串
来源：http://hz.hnxiangtu.top/gtmebegxyf.html

echo "${s:0:5}"
来源：http://hz.yongpay.top/gtfyciioag.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtvxuguaot.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gtlfurdkqy.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtzmucmkdh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtmguwmxeq.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtwrgbzdxx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtqjkomqkg.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtvvgkmfeg.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtpatsaqcj.html

[R27] 算术展开
来源：http://hz.jqgufenzy.top/gtkffrnyoh.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtixaytljj.html

[R28] 浮点运算
来源：http://hz.pengpengdd.cyou/gtgjwcwlaa.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydzc1.top/gtdtmidtyk.html

[R29] 定义函数
来源：http://hz.dashuyun.cn/gtpppzwifk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gogol.net.cn/gtnsnpmvxt.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtzjojeujo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gtpkrjdpuc.html

[R31] 局部变量
来源：http://hz.ppjwa.cn/gtumbhppor.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtxtgfbzel.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtgjskaccv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gtnankspth.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gtiezvpjky.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtpafcovui.html

[R34] 退出时清理
来源：http://hz.hammf.cn/gtwgwboieq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtfpjxokzp.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gtjidrijyu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gteiiijndh.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gtuyosdfrx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gotoacloud.top/gtjkpvqmsu.html

[R37] 把输出赋给变量
来源：http://hz.gaohongyu789.top/gtxczzjhch.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtdpjbjdmy.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtaklsirsx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtmvzbictq.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtluicnrpa.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gteyuyzfop.html

[R40] 追加写日志
来源：http://hz.wangshuangyany.cn/gtxnahjhsg.html

echo "log" >> out.log
来源：http://hz.dashuyun.cn/gtvqjpdoui.html

[R41] 丢弃输出
来源：http://hz.tanke756.top/gtzgfwlsij.html

cmd >/dev/null 2>&1
来源：http://hz.zhixingplan.top/gtvjqyimmd.html

[R42] 输入重定向
来源：http://hz.pengpengdd.cyou/gtkundxwhg.html

wc -l < a.txt
来源：http://hz.pycfn.com/gtjduwnrxt.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtojbsjgaf.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtserbppme.html

[R44] 按修改时间查找
来源：http://hz.xuanzx.com/gtgaujpaav.html

find . -mtime -7 -type f
来源：http://hz.nwbrower.top/gthlkpraop.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtwwowlnyb.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtjtavdlzb.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtozywrrux.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gtfwzimael.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gtldhvzdtj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhixingplan.top/gtsaaqipey.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtcxoukzsi.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtnxbnqtrj.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtmwanoovq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtetlrszfh.html

[R50] awk 求和
来源：http://hz.tianlin.xyz/gtygdfrijx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fengsongda.top/gtyomdmutw.html

[R51] 排序去重取前几
来源：http://hz.jinqigfzy.top/gtotsyytff.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtfkrznirg.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gtgzolejxj.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtkywshtwg.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtuhlremau.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.iojbl.cn/gtdlyzbklk.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtfksbcqvq.html

diff a.txt b.txt
来源：http://hz.dashuyun.cn/gtvicegxml.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtzmgamvqp.html


<!-- 参考信息 -->