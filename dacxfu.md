代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhijiandao.cn/gtgqppyjrd.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gttytyrsto.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hnxiangtu.top/gteuqgpqoy.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gttuphnqff.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daxiang520.top/gtrvgyitvn.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtxjouzdhs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinyuanbaomall.cn/gtlawqynaz.html

[Q08] 创建普通索引
来源：http://hz.hysaishi.cn/gtjhnfrbwu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtphvxjwgt.html

[Q09] 创建唯一索引
来源：http://hz.jinghuilouyu.cn/gtrnmmaicm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.bjfxy.top/gtgfeayklm.html

[Q10] 插入单行
来源：http://hz.jlsjyb.cn/gtpacojjue.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtiptwcyxw.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gtnplkdcdk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtqbreemjq.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gtwppfhqcd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gttafdrzke.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtocjlovhk.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtcvtcmnxu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgufenzy.top/gtduizseqc.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtcgfikhoa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtdrwpyjrw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtmhtuhbhg.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtpcoptwwj.html

SELECT * FROM users;
来源：http://hz.feifeiyinyue.top/gtmoskwksd.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtmwotodqe.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtyecvyzuc.html

[Q17] 条件查询
来源：http://hz.gaohongyu789.top/gtsptxevxt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sufxvd.cn/gtuoxlydfn.html

[Q18] 模糊匹配
来源：http://hz.jinghuilouyu.cn/gtsdamayoq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258888.top/gtylllyskr.html

[Q19] 范围查询
来源：http://hz.aibaodan.cn/gtegapcykx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.meibo888.top/gtkcqyvsea.html

[Q20] IN 列表
来源：http://hz.yangfankeji.com/gtjiwqtkjh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gtturmrzbv.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtvlkqycby.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhoulong.xyz/gtxuthiseq.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtpgsbrqpk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ppjwa.cn/gtvanmylsp.html

[Q23] 分页
来源：http://hz.xziqi.cn/gttebwjsbu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gttizdrgmf.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtounirycg.html

SELECT DISTINCT city FROM users;
来源：http://hz.tian-w.cn/gtlrmznady.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtvlzkries.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtqpwhbsyd.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtfyophilb.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gterzmrijy.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gtdelwlyga.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinghuilouyu.cn/gtkswvcsfl.html

[Q28] 求和与平均
来源：http://hz.zdqjudy.top/gtcxfkyvrv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtcioiyozq.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtkgaueazi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtwljmwoul.html

[Q30] 分组统计
来源：http://hz.zhaomingkeji.xyz/gttslfsxei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtkggnsfoi.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtmeojalxf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtummqdtwd.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtgtieijwh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gthiqiafhv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtsfcpuhyo.html

[Q33] 多列分组
来源：http://hz.shangyingyoupin.top/gtdxcddnix.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yangfankeji.com/gtlglwyfcl.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtbdasuygz.html

SELECT * FROM (
来源：http://hz.gzhubu.top/gtbldlibun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtbwlubppo.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtnlaqvnyb.html

[Q35] 内连接
来源：http://hz.havefunace.top/gtanrjttei.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtmnqodrrt.html

[Q36] 左连接
来源：http://hz.xuanzx.com/gtzdkbafkq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtlxqbixfh.html

[Q37] 右连接
来源：http://hz.shzxlz.cn/gtznmhpavm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gtiajcuscw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gtimaepvcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gteuyqublq.html

[Q39] 自连接（查上下级）
来源：http://hz.tanke756.top/gtbkulsoqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtfjfwhuam.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xinyue.icu/gtgulrymyh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgufenzy.top/gtkcuxxheg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtzkzrksyh.html

[Q41] 多表连接
来源：http://hz.hnxiangtu.top/gtmrlkeaxu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cqqwz.cn/gtzivunnih.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daria6918.cn/gtsqffkczk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangtech.top/gtdgvfclil.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gtqhmbbggr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtednsteww.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtjikzmyls.html

[Q43] 标量子查询
来源：http://hz.nwbrower.top/gtqlrdljhx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.havefunace.top/gtrlbkhsxb.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtzzjorpok.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gtmcgwuvsl.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtquastbhm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtrmcfwzlt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtpaheoxmz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtsvdamxqc.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtjdqxrklz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nwbrower.top/gtqofpihjp.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gtkfbibvfl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtgpfuyqvp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtcekxmsev.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtzuhhkkwd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zdqjudy.top/gtmmzysubi.html

[Q50] 批量更新
来源：http://hz.jqgufenzy.top/gtlkubxpty.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gtvqfyaxlp.html

[Q51] 用子查询更新
来源：http://hz.gotoacloud.top/gtmbhndnvn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtbgignazn.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtiujuveqg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtnmcosybg.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtcgdpqoqt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigufen.top/gtnrjtyyur.html

[Q54] 清空表
来源：http://hz.zhoulong.xyz/gtkcxqxamk.html

TRUNCATE TABLE logs;
来源：http://hz.316326.xyz/gtxjuxzmgk.html

[Q55] 排名（并列占位）
来源：http://hz.yuxming.cn/gtxwdinnqq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gtddpprstq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gtjbcistxv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gttjgmwcfx.html

[Q57] 行号
来源：http://hz.birdmap.top/gtmngfctfb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtqlsdhzoc.html

[Q58] 累计求和
来源：http://hz.zhiwuduotai.top/gtfotsajsz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sysykeji.top/gtzcmavmwh.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtibrrlndy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtgnqhqznu.html

[Q60] 取上一行 / 下一行
来源：http://hz.fengsongda.top/gtyqmttssa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.feifeiyinyue.top/gtvjltvgvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.316326.xyz/gtekzpqgit.html

[Q61] 移动平均
来源：http://hz.haohaochexian.top/gtovxctxvt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gtyjgmivif.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtecqlkxpf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtcorakemi.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtycdbtlmr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtvacrpkmu.html

[Q64] 提交事务
来源：http://hz.smart0.xyz/gtmyuiaoft.html

COMMIT;
来源：http://hz.yj20258.top/gtpmnzjoxy.html

[Q65] 回滚事务
来源：http://hz.yj20258888.top/gtdagzrcad.html

ROLLBACK;
来源：http://hz.hfpthk.cn/gtduvoscim.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtinapfjyt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gtlvwutpgh.html

[Q67] 设置隔离级别
来源：http://hz.xuanzx.com/gtwwyrzusn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgufenzy.top/gtyessffvl.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtrtnkxlau.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtuwnsygwg.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtpoknydrs.html

[Q69] 查看执行计划
来源：http://hz.feifeiyinyue.top/gtlsoahsmh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtekctpoxq.html

[Q70] 更新统计信息
来源：http://hz.yanxiufei.cn/gtavmvebte.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtxnujyplp.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtxznhuvkt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtbvdxerws.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtbepettlh.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtimepston.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gthlkiorcc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtqbcyieod.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtzoxnbydc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daria6918.cn/gtunxgsgbl.html

[Q75] 日期格式化
来源：http://hz.daxiang520.top/gtyxrnxwkb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gthydhltyz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtbmwsfnzi.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gtyznflirv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ehwqpu.com/gtyexrkpfr.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtoggootcs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gthgtrbpnp.html

[Q78] 当前时间
来源：http://hz.zhijiandao.cn/gtlyqrzium.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gtcbzwywts.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtwhdgqppg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtcezsztoh.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtpuntltpx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258888.top/gtaoxixhmd.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gtidfvjyqm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtocqnaxjp.html

[Q82] 字符长度与字节长度
来源：http://hz.svipenyu.cn/gtcjeeofpw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtkuklacjh.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gttryqbplc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shuidangran.top/gtvrrrpqlu.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtmhaxssln.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtfvahoqmm.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtkguvidlc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cashguo.top/gtwiheaszm.html

[Q86] 读取 JSON 字段
来源：http://hz.jlsjyb.cn/gtpblgzogu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtrvusoely.html

[Q87] JSON 字段做条件
来源：http://hz.shzxlz.cn/gttkgwdvik.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxuanxn.top/gtswbcdubh.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtautbjkem.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gogol.net.cn/gtuttgimgu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtkifmuijs.html

[Q89] 判断表是否存在
来源：http://hz.cashguo.top/gtxrjumwal.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gthzwkbawr.html

[Q90] 生成序号列
来源：http://hz.0kj1m.cn/gttuntkxtp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtvtfdtvqo.html

================================================================================
来源：http://hz.tianlin.xyz/gtwayywbko.html

R. Bash 专题
来源：http://hz.ivvv.top/gtqfcvvvot.html

================================================================================
来源：http://hz.tianlin.xyz/gthkdokped.html

[R01] shebang 与严格模式
来源：http://hz.9152youxi.cn/gtiiibwugr.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtvlsicagt.html

set -euo pipefail
来源：http://hz.jlsjyb.cn/gtfdffxyhm.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtsxhunofp.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtegsivlrw.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtvzgukzik.html

readonly PI=3.14
来源：http://hz.bjfxy.top/gtiweoqisa.html

[R04] 位置参数
来源：http://hz.yuxming.cn/gtctkfghvo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtkyfqmtyb.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gtrfrskbhs.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtqydprkew.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtnrqjvfbt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tian-w.cn/gttzwxstvl.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtnzrrpzjj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtegnkuzmd.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtfoyhshvp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cqqwz.cn/gtuiaemuiv.html

[R09] 字符串比较
来源：http://hz.zhiwuduotai.top/gtvytdxned.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtbljizkuc.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtvporlgno.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.9152youxi.cn/gtolrmdins.html

[R11] case 多分支
来源：http://hz.ywan-chungtsiang.top/gtldmxspiq.html

case "$1" in
来源：http://hz.tianlin.xyz/gtzedmkmye.html

start) echo "启动" ;;
来源：http://hz.sxryk.cn/gttoyiathh.html

stop)  echo "停止" ;;
来源：http://hz.hywenlv.cn/gtdshzwfgy.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtorrupxdm.html

esac
来源：http://hz.chenzaomai.com/gtsschlsfk.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtpggjuqzy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zdqjudy.top/gtdcbgxcbf.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtbszkiuuw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtgcmdgrxm.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtagvhmqgf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtmwjhdtbu.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtzravzdjq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtrloffxue.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtikopukwg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtlibrdckh.html

[R17] 数组定义与取值
来源：http://hz.chenjidiqi.icu/gtkykgkqku.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtkodnpgoy.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtofmgdskx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.52xcode.cn/gtgekjazpu.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gthertwrud.html

echo "${#arr[@]}"
来源：http://hz.iojbl.cn/gtbkkqxmmw.html

[R20] 关联数组（字典）
来源：http://hz.dianchejie.cn/gtnwzimeyf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinghuilouyu.cn/gtiantrylw.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtdlrtsxyx.html

echo "${#s}"
来源：http://hz.tanke756.top/gtezeqvojh.html

[R22] 截取子串
来源：http://hz.jlsjyb.cn/gtuqpuounl.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtjhpbeypa.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtjvadaxdh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cdnleiting.top/gtaloidjwl.html

[R24] 大小写转换
来源：http://hz.fzhhl.top/gtzvbprcbl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yonumen.top/gtgvrgzwkv.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtgopzizmz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gtoamankwn.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtuvnpbugy.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gtvtwvyohf.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtvdnxnpzw.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtnxqdkzab.html

[R28] 浮点运算
来源：http://hz.jqgufenzy.top/gtjxwkjdkh.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtquvopmyb.html

[R29] 定义函数
来源：http://hz.ydzc1.top/gtqepcrpoo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtbfkhwmdt.html

[R30] 函数返回状态码
来源：http://hz.cheryme.top/gtwbukjnfp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sysykeji.top/gttnhwyrzw.html

[R31] 局部变量
来源：http://hz.birdmap.top/gtqnzczzwh.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtrrkmnnkp.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtxcamupqa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.mhx1999.top/gtdivomrbz.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtagloyanq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.andypj.xyz/gtdcfldytt.html

[R34] 退出时清理
来源：http://hz.chenzaomai.com/gtzuozgfmz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtpjtycaac.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtbnubdaud.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sysykeji.top/gtqsoxthyt.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gtuxdbeobj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnqzz.top/gtgymeniho.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtudvxeutk.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtneqzjhvw.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtdaiumkkn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtcftjktjh.html

[R39] 重定向标准输出与错误
来源：http://hz.cucudq.cn/gtwbpnrhuz.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gttgoouzsx.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtzaefybvx.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gteuzlozjp.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtooxuwhvg.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtoexvpava.html

[R42] 输入重定向
来源：http://hz.meibo888.top/gtwlqhscxq.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtpvvegdnt.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtvgpxallr.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtluzucxht.html

[R44] 按修改时间查找
来源：http://hz.hnxiangtu.top/gtkoetkqbl.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtdhvwndln.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtjnxmrltf.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtcchqwvsa.html

[R46] 递归替换文件内容
来源：http://hz.zhiwuduotai.top/gtucdsjszv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gtnghfpzlb.html

[R47] sed 单行替换
来源：http://hz.svipenyu.cn/gtkxyycxqo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gotoacloud.top/gtmzxuoime.html

[R48] awk 取指定列
来源：http://hz.52xcode.cn/gtpmuhrdxc.html

awk '{print $1, $3}' a.txt
来源：http://hz.shangyingyoupin.top/gtpycasefq.html

[R49] awk 带条件
来源：http://hz.xziqi.cn/gtwbyshiqh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.feifeiyinyue.top/gtolniemxs.html

[R50] awk 求和
来源：http://hz.tian-w.cn/gtkpjnvmpx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtfhogdxvp.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtsccrkdzt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aibaodan.cn/gtrwxmlpra.html

[R52] 统计行数
来源：http://hz.birdmap.top/gtydtzlmhu.html

wc -l a.txt
来源：http://hz.c1oappe.top/gtsjhzeifs.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtdtjxfytq.html


<!-- 参考信息 -->