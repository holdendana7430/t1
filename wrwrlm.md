代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtrrbxpnzy.html

[Q07] 删除表
来源：http://hz.guannengcc.top/gtbxhxajtm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtnjuxibcm.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtuwrtvgkh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtushrbfaw.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gthvfcnjob.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtzefisshr.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtqmhhujhu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtlheozodm.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangkeji.top/gtjjcsbilm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtuxawbpjb.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtjeedxcaj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.mhx1999.top/gttvhwavxa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258888.top/gtpvytcarm.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtjrzemvyg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtiwufffcl.html

[Q14] 存在则更新（upsert）
来源：http://hz.daxiang520.top/gtzbsueahh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydzc1.top/gtcebpxqqx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtaqjieyhd.html

[Q15] 查询全部
来源：http://hz.yj202588.top/gtzakfkyll.html

SELECT * FROM users;
来源：http://hz.yuxming.cn/gtborjyapr.html

[Q16] 查询指定列
来源：http://hz.kuanghao11.cn/gtzwbyuugi.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtvncifpes.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtogxdjsdg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtjiumksau.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtcxeyvsfg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gtzhblcget.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtpghzfyvk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtwwruwdhm.html

[Q20] IN 列表
来源：http://hz.yj202588.top/gtsqpagdwp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangkeji.top/gtydufyhgu.html

[Q21] 空值判断
来源：http://hz.zhixingplan.top/gtcyhndzek.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gtolivwsjm.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtoghlofem.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xingfuxueyuan.xyz/gtkasasjci.html

[Q23] 分页
来源：http://hz.chenlongwang.top/gtfjdteauw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhengqikj.top/gtdityeyqw.html

[Q24] 去重
来源：http://hz.jiagoushi.top/gtduhyvgmn.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtxpmhgxzk.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtzgvpcvih.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daxiang520.top/gtjgzikakr.html

[Q26] 计数
来源：http://hz.haohaochexian.top/gtudlgoius.html

SELECT COUNT(*) FROM users;
来源：http://hz.haohaochexian.top/gtrgvdlfou.html

[Q27] 条件计数
来源：http://hz.jqgfzy.top/gtqwvdvawk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.smart0.xyz/gtedcngftw.html

[Q28] 求和与平均
来源：http://hz.jinyuanbaomall.cn/gttjzpardc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gotoacloud.top/gtaytzcmnx.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtfybpmuvr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinghuilouyu.cn/gtmlcoflnt.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gtuocpzujr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gtzzflplxn.html

[Q31] 分组后过滤
来源：http://hz.quarkkingdee.top/gtjdrxemii.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtdtstxgnw.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gttodcxpfw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtlyixtbgm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gttwtwzrqe.html

[Q33] 多列分组
来源：http://hz.yuanzhike.top/gtkcmiivbx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtbpvopjja.html

[Q34] 每组取第一条
来源：http://hz.jinghuilouyu.cn/gtuszpldaw.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtjqilnfuc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gtcujrcebv.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtgxwgxndq.html

[Q35] 内连接
来源：http://hz.redwolf501.top/gtpnuosrok.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtsrprgxej.html

[Q36] 左连接
来源：http://hz.chenzaomai.com/gthffwojsl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtxuzyuxbt.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtqjrgemds.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtxshjdulu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dashuyun.cn/gtbrulsdsb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinyuanbaomall.cn/gtfpozydgi.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtmrljjinj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yonumen.top/gtvdzsplvc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtlfvhalpt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtlmcvcljp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pycfn.com/gtuxrzztxd.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtcnqagivk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigufen.top/gtwfkueood.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gttliydddp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtlzrcbdps.html

[Q42] 连接条件附加过滤
来源：http://hz.9152youxi.cn/gtzxadpxui.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtfhyhtyti.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenlongwang.top/gtdbwacsdm.html

[Q43] 标量子查询
来源：http://hz.pengpengdd.cyou/gtzumpytig.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gtqqkzfplx.html

[Q44] IN 子查询
来源：http://hz.jyoumei.cn/gtcezmqret.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtkxunxura.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtwuchadvd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gttnvctcdu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtkejszwqf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtysmyivqb.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtrjrsgrew.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtzjtolvmd.html

[Q48] CTE 公用表表达式
来源：http://hz.xziqi.cn/gtwflrtfix.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtkrxkqohx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yueranfly.top/gtczjrvhrt.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gttlemfgmy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtddcaesqt.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtiklkhbne.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gttcmzfqvp.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtmpwiglnn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtnxznwhsa.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtlyaweuxk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gtbflibbgm.html

[Q53] 按条件删除
来源：http://hz.ehwqpu.com/gtcwqimbci.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtuqradrsu.html

[Q54] 清空表
来源：http://hz.sweek.top/gtyflqbjlx.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtpyxumjml.html

[Q55] 排名（并列占位）
来源：http://hz.smart0.xyz/gtgrsgeljs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sysykeji.top/gtvczcvaxv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtkpdvtijl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtlfsuaazm.html

[Q57] 行号
来源：http://hz.hongshengwenyu.top/gtrttotkys.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtjqymqxit.html

[Q58] 累计求和
来源：http://hz.yanxiufei.cn/gtoeooujcw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtzwgrsqrh.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtauwpjyfg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gttrjxyoea.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtlthibykn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtcnsgbkke.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtbwcpmgqq.html

[Q61] 移动平均
来源：http://hz.hammf.cn/gtiwhzaujo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtvkjtwujx.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtmdqwcuau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtuvghdava.html

[Q63] 开启事务
来源：http://hz.ywan-chungtsiang.top/gtrcyoucks.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtizwbmxfp.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtqledqksj.html

COMMIT;
来源：http://hz.gotoacloud.top/gthyrjewys.html

[Q65] 回滚事务
来源：http://hz.daxiang520.top/gtzsvnpclc.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtbqgvziuj.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtgoeokmsz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gthokphqlj.html

[Q67] 设置隔离级别
来源：http://hz.xinyue.icu/gtztzcnzxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gttggfmjqb.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtguclnpru.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gtlhxukksm.html

ROLLBACK TO sp1;
来源：http://hz.hnxiangtu.top/gtaemxxobl.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtczlvzslu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtaxucbqnv.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gttcrklelg.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtiawyqnbe.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtkpwmgpwa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.birdmap.top/gtcmazbgrg.html

[Q72] 查看索引
来源：http://hz.gzhubu.top/gtbragaygg.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtgrdpkoee.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gtcpjilbzd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtgbumpxyg.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtcaxfkmlq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.haohaochexian.top/gttknaespv.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtoovsfodt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtigkerpgd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ivvv.top/gthlxcgpxs.html

[Q76] 按天统计
来源：http://hz.sxryk.cn/gtiufsvgjm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtfxkzwiam.html

[Q77] 时间加减
来源：http://hz.havefunace.top/gtwnqjndda.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gtbvdtgdqw.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtpzgfpuqy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gttvdmtdvl.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtnkftcjfw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gtamzjpfiw.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtntcwomce.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtpffajamn.html

[Q81] 字符串替换
来源：http://hz.yuxming.cn/gtwtbmasur.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtueqniaot.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtlzxjgkud.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tianlin.xyz/gtlvphcecd.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtrqpdajbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtqmfyuofm.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtejtklwxc.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhoulong.xyz/gtbcfwrspl.html

[Q85] 数值取整
来源：http://hz.havefunace.top/gtckatonij.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtubhhgdnc.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtvscazgpz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtvxjjbasd.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtmzubaisj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shzxlz.cn/gtuqjcynmv.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtilujkois.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gttouqbviy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtkgecmqit.html

[Q89] 判断表是否存在
来源：http://hz.pengpengdd.cyou/gtpebjiiev.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hywenlv.cn/gtgvjhzccu.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtzsoldauy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtqadzfruz.html

================================================================================
来源：http://hz.ybcxt.top/gtaddrdzwr.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gtoesupjto.html

================================================================================
来源：http://hz.snrcjt.cn/gtrgjvzrsf.html

[R01] shebang 与严格模式
来源：http://hz.xuanzx.com/gtpbnvughr.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtdbysigjb.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gttlzjflat.html

[R02] 变量赋值与使用
来源：http://hz.52xcode.cn/gtkfzorqjf.html

name="Tom"; echo "$name"
来源：http://hz.jinghuilouyu.cn/gtwsvopmxz.html

[R03] 只读变量
来源：http://hz.jinyuanbaomall.cn/gtbzvrwqqk.html

readonly PI=3.14
来源：http://hz.52xcode.cn/gtghtowrng.html

[R04] 位置参数
来源：http://hz.haohaochexian.top/gtrmpqsndf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtwgpseycj.html

[R05] 参数默认值
来源：http://hz.yonumen.top/gtcfnwbrby.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtegueauop.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtumsfshnv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtvrltvlrf.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gthkgncslu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtfqmrexlv.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtbkrfxmrq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gtumawsuxa.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtibqzzbnx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gtackmdhhl.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtkhkasjpe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xziqi.cn/gtwrveetji.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtaynzypli.html

case "$1" in
来源：http://hz.yj20258.top/gtzgmqqpgu.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtctovpexw.html

stop)  echo "停止" ;;
来源：http://hz.sweek.top/gtdmctwwgl.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtjjcssswg.html

esac
来源：http://hz.aizwys.cn/gtrppyghem.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtdqyxwlhx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtpcbmtpxf.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtlhzydvqw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtlckrzsmh.html

[R14] C 风格 for
来源：http://hz.guannengcc.top/gtdncilnpt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtyrajlutl.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtmgzzagab.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guowangkeji.top/gttquotfka.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtskwntgzc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gtkalkaebg.html

[R17] 数组定义与取值
来源：http://hz.guannengcc.top/gtolfmlfps.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxuanxn.top/gtsygyipwc.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtarsxuqft.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtwrawnzad.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtkebmyaap.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtzqhplsgz.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtquqdcrfr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gthbktnleh.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtjovwmoat.html

echo "${#s}"
来源：http://hz.hnqzz.top/gtlffthixd.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gthxyobkur.html

echo "${s:0:5}"
来源：http://hz.cucudq.cn/gtoegwynwv.html

[R23] 字符串替换
来源：http://hz.ehwqpu.com/gtujwgemsm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtarfkninx.html

[R24] 大小写转换
来源：http://hz.yvedp.cn/gtjuyjihmu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtwzmousur.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtrbpmmhvz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.birdmap.top/gtifvqxkpq.html

[R26] 命令替换
来源：http://hz.sweek.top/gttvuzkick.html

now=$(date +%F); echo "$now"
来源：http://hz.shangyingyoupin.top/gtwxraphhf.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gtnzrwmmwb.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtditenvhx.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtooclfusd.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnqzz.top/gtvxwsslgv.html

[R29] 定义函数
来源：http://hz.jinqigufen.top/gtovxnpxzm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gtvxyscogu.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gtarldsnnt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zdqjudy.top/gtxxznbxlw.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gtwlypjeti.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj202588.top/gtidezhspq.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtojllaivd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtwwyenlvx.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtsorknfcl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtswoeejms.html

[R34] 退出时清理
来源：http://hz.zhengqikj.top/gtkkvsqpnx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuanzhike.top/gttkzwgewx.html

[R35] 后台执行并等待
来源：http://hz.hnqzz.top/gtgcabxkpy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dashuyun.cn/gterhoyups.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gtbyywcilh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenjidiqi.icu/gtrmufqviz.html

[R37] 把输出赋给变量
来源：http://hz.hnxiangtu.top/gtlcietnfb.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtexygnmmj.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtukkcdlak.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtjhqafgsx.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtwmkecsjz.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtuncgnxue.html

[R40] 追加写日志
来源：http://hz.pengpengdd.cyou/gtcwdeklgs.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtvovulmga.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtsgkppbxl.html

cmd >/dev/null 2>&1
来源：http://hz.zhixingplan.top/gthkcrixpe.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtbcpqpplc.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtmghldpbd.html

[R43] 按名字查找文件
来源：http://hz.daxiang520.top/gtzjbipgbj.html

find . -name "*.log" -type f
来源：http://hz.ehwqpu.com/gtbymfgzip.html

[R44] 按修改时间查找
来源：http://hz.wangshuangyany.cn/gtuyhhriim.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gtgmcxctny.html

[R45] 批量删除
来源：http://hz.xinyue.icu/gtkvppnxfp.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gtdkziuhfw.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gtclzctnkn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtjqxwlqpc.html

[R47] sed 单行替换
来源：http://hz.hfpthk.cn/gtrjhgrtii.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtqhllwyyq.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtwstdcpac.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhongyouzk.top/gtvccdwsdf.html

[R49] awk 带条件
来源：http://hz.havefunace.top/gtheovxkha.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnxiangtu.top/gtlwrpplpx.html

[R50] awk 求和
来源：http://hz.yj20258888.top/gtzbivfgco.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtmdddpfvz.html

[R51] 排序去重取前几
来源：http://hz.andypj.xyz/gtfznakskr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.kuanghao11.cn/gtdszmjuwg.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gtygxvtmsg.html

wc -l a.txt
来源：http://hz.aizwys.cn/gtvhaysvij.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtjpjvqdha.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tian-w.cn/gtesllxkci.html

[R54] 比较两个文件
来源：http://hz.jinghuilouyu.cn/gtvmysofes.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtubqerkqf.html

[R55] 压缩与解压
来源：http://hz.feifeiyinyue.top/gtmvvteutp.html


<!-- 参考信息 -->