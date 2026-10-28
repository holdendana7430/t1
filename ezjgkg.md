代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtznwfrpov.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jyoumei.cn/gtpqacrmvl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtwhbpsgis.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtbuvpuaqr.html

SELECT * FROM users;
来源：http://hz.zhengqikj.top/gtxpgmsxlc.html

[Q16] 查询指定列
来源：http://hz.hnxiangtu.top/gtsljvxnwc.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtxnramiyh.html

[Q17] 条件查询
来源：http://hz.yuxming.cn/gtdydbdwjn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhaomingkeji.xyz/gtkbhvjjpz.html

[Q18] 模糊匹配
来源：http://hz.zycfv.cn/gtizjpejqj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ybcxt.top/gtvjctoagv.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtfxnljiat.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xylfe.cn/gttpywmori.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtdzfgjmaq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtmwbzgkej.html

[Q21] 空值判断
来源：http://hz.jqgufenzy.top/gtywduehig.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj202588.top/gtxytqqdat.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtnngtjrhn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuanzx.com/gtckwajizg.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtjsrapdww.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xinyue.icu/gthdahkzkj.html

[Q24] 去重
来源：http://hz.jinqigufen.top/gttyhnyosk.html

SELECT DISTINCT city FROM users;
来源：http://hz.yueranfly.top/gtrouxzcdg.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtrfibjctx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtsqjcpgzz.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtjkkkrutm.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhongyouzk.top/gtprkylbio.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtumijdarq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.bjfxy.top/gtlxpbytto.html

[Q28] 求和与平均
来源：http://hz.nanxinkj.top/gtomlorncm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtspfhhklr.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtlbcyhhak.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtbetznjdo.html

[Q30] 分组统计
来源：http://hz.jqgfzy.top/gtuvlwklev.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtstzggzjt.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtorvvpmhf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.kuanghao11.cn/gtpkxmcisc.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtvvxotljb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtvhynwmkb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtmugasluh.html

[Q33] 多列分组
来源：http://hz.hnqzz.top/gtpnymukvx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtxtqoogih.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gtusnbxxgu.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtrlpzofyi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhijiandao.cn/gttuvdbvol.html

) t WHERE rn = 1;
来源：http://hz.zhixingplan.top/gtapsckxwy.html

[Q35] 内连接
来源：http://hz.yj20258.top/gtkolorbjj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtygqxtrqd.html

[Q36] 左连接
来源：http://hz.haohaochexian.top/gttulsczak.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtrnevdzca.html

[Q37] 右连接
来源：http://hz.wangdashe.top/gtzknlkjxu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtjshtnjur.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtzicikxsp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gtyeukscms.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtjsuvvjyq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.andypj.xyz/gtowxugdye.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jlsjyb.cn/gtznlauybm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ppjwa.cn/gtdogfydni.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnxiangtu.top/gtkbhmebqk.html

[Q41] 多表连接
来源：http://hz.snrcjt.cn/gtdvqkwkwu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jlsjyb.cn/gtwjxhvdca.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtkzrzxgov.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuanzhike.top/gtngraqhjg.html

[Q42] 连接条件附加过滤
来源：http://hz.yonumen.top/gtiryuudap.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtsqtfybmh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtyhshwknl.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtzgqhfrgs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gttkvaqevv.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtosyglnbt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtujmnlgxa.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtrutcczmc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtqsiuuyiz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fengsongda.top/gtyhxwzigy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtadqpismp.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtzldllmeu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtacsaoqct.html

[Q48] CTE 公用表表达式
来源：http://hz.ivvv.top/gtxadpqpcd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtwtdyhylf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangkeji.top/gtiemssunh.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtfldvbixv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gttmbxynvf.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtbhfkaloi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuxming.cn/gtqmcquurj.html

[Q51] 用子查询更新
来源：http://hz.shuidangran.top/gtejllvttq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgufenzy.top/gtekkluvxv.html

[Q52] 删除指定行
来源：http://hz.hysaishi.cn/gtfoiecdni.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtgxykfebt.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtrvgtfxnz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtynwpgfjx.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtxbnttshu.html

TRUNCATE TABLE logs;
来源：http://hz.52xcode.cn/gtombbeqwk.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtvvljnskj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtdcmdtlwr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aizwys.cn/gttbxfxeba.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigufen.top/gtwyzpwnbl.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gtgzjcbdrt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gtauktpmqu.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gtxdfbyojk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gzhubu.top/gtjqtqfqav.html

[Q59] 分组内累计
来源：http://hz.jqgufenzy.top/gtgceerekz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtruerfwxz.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gthhdbsdbr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtargajrfp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenjidiqi.icu/gtgrkkuxrp.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtlodwmssi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtottjuayt.html

[Q62] 分组占比
来源：http://hz.bjfxy.top/gtvfpzmzdj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtlmvkoqch.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtxfduitch.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.haohaochexian.top/gtcwcdogng.html

[Q64] 提交事务
来源：http://hz.yj20258888.top/gtoochexoc.html

COMMIT;
来源：http://hz.9152youxi.cn/gtlhucrlfd.html

[Q65] 回滚事务
来源：http://hz.kuanghao11.cn/gtvpytagum.html

ROLLBACK;
来源：http://hz.zycfv.cn/gtxkvbhuyk.html

[Q66] 行锁查询
来源：http://hz.zhixingplan.top/gtildhllbm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtzaigffhh.html

[Q67] 设置隔离级别
来源：http://hz.yuanzhike.top/gtgloldrpr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtmuudzbvo.html

[Q68] 保存点
来源：http://hz.zhiwuduotai.top/gtpmcxhwdq.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtwicqpktt.html

ROLLBACK TO sp1;
来源：http://hz.mhx1999.top/gtrnaqkgue.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtnduvdhqw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtcncsjqko.html

[Q70] 更新统计信息
来源：http://hz.jlsjyb.cn/gtkksxiewu.html

ANALYZE TABLE users;
来源：http://hz.ydjk.org.cn/gtixgtkzat.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtdehejqiy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gthojnrrwq.html

[Q72] 查看索引
来源：http://hz.yonumen.top/gteqhxdtvl.html

SHOW INDEX FROM users;
来源：http://hz.hysaishi.cn/gtimlsxrsj.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtwbqghduq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gotoacloud.top/gttlywgkul.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtssxkkbpv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yangfankeji.com/gtlvfawyuz.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtnndmqcpz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sxryk.cn/gtsifozybm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtknxygzpg.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtbpinkzay.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgufenzy.top/gtwyxhpyrb.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtoehuzzvp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtnvpgmhdv.html

[Q78] 当前时间
来源：http://hz.cucudq.cn/gtnrsuhdfu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhongyouzk.top/gtbrsojvfp.html

[Q79] 字符串拼接
来源：http://hz.ydjk.org.cn/gtvqgkabrk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dashuyun.cn/gtllofmybr.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtnblmvdsm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.iojbl.cn/gtyoxigwfr.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gtvaqtxxwj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gttuarrmay.html

[Q82] 字符长度与字节长度
来源：http://hz.pycfn.com/gtfjyhiaee.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtfceiznvf.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtjroajndv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gzhubu.top/gtykaklqyi.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtwxjscwso.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhoulong.xyz/gtgzsfhggt.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtstgxaxbp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtudajwjpu.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gtgxacadrh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sufxvd.cn/gtfrsjgtvn.html

[Q87] JSON 字段做条件
来源：http://hz.fengsongda.top/gtqoisgbnu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yuanzhike.top/gtmnrwkksn.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtxserqsdr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtorqrmhgc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtcgubaqud.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtswobnqud.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtrciobtwm.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtfgqmvfko.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.316326.xyz/gtlxdebxmc.html

================================================================================
来源：http://hz.havefunace.top/gtwmmkdtak.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtswrouxsi.html

================================================================================
来源：http://hz.shzxlz.cn/gtprupjadn.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gtsfzvtupf.html

#!/usr/bin/env bash
来源：http://hz.jyoumei.cn/gtzggtaozs.html

set -euo pipefail
来源：http://hz.ivvv.top/gtmioxtqrw.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtjcshntwq.html

name="Tom"; echo "$name"
来源：http://hz.guowangkeji.top/gtegeqqzpj.html

[R03] 只读变量
来源：http://hz.sweek.top/gtcgbfrqny.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gthgjqugsu.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gthhfrckjj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtbmkuzyap.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gttteqozrt.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtelfnnjwa.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtfehxcnic.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtourwsotw.html

[R07] if 判断文件
来源：http://hz.vqdsnc.cn/gtzdhkvjwl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtcforsqkz.html

[R08] 数值比较
来源：http://hz.hammf.cn/gtlpzpbffk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.9152youxi.cn/gtbkrnxjum.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtafhuusrr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shanyushiyangkeji.top/gtjqzrifxz.html

[R10] 正则匹配
来源：http://hz.jlsjyb.cn/gtgyvomgmd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.redwolf501.top/gtpxbibxbx.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtmpxrxkym.html

case "$1" in
来源：http://hz.xziqi.cn/gtlxhzorxm.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtkcevbkfe.html

stop)  echo "停止" ;;
来源：http://hz.guannengcc.top/gtjtgrovpl.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtrlmyflcf.html

esac
来源：http://hz.sufxvd.cn/gtmtmgbmge.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtsinkbsmx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pycfn.com/gtpptysvzi.html

[R13] for 计数循环
来源：http://hz.shangyingyoupin.top/gtikubsvpx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cashguo.top/gtmonbnkhp.html

[R14] C 风格 for
来源：http://hz.ywan-chungtsiang.top/gtunumsaxv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtcdunxuwp.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtgxchpnna.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtzzhganah.html

[R16] until 等待条件
来源：http://hz.jinqigfzy.top/gtmodmlvjw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtoipczsio.html

[R17] 数组定义与取值
来源：http://hz.feifeiyinyue.top/gtrevlzttr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtfgouxega.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtmymgvqjy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtwahkbyou.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtnoimibln.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtvttzqqce.html

[R20] 关联数组（字典）
来源：http://hz.yj202588.top/gteproqsmy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtqgaeqjnn.html

[R21] 字符串长度
来源：http://hz.pycfn.com/gtyjflllof.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtxmkxzkvw.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtquxfhxpc.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gtqkwcafjy.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtnigzirqs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtgkcuwuhl.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtcgutgajb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtnokntlkc.html

[R25] 去后缀 / 去前缀
来源：http://hz.vqdsnc.cn/gtykscbvly.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtgsqlketx.html

[R26] 命令替换
来源：http://hz.jinqigfzy.top/gtovrsmzjo.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtgpezewst.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtxltwwepy.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtuicsfjle.html

[R28] 浮点运算
来源：http://hz.chenzaomai.com/gtcvyeykli.html

echo "scale=2; 10/3" | bc
来源：http://hz.xziqi.cn/gttktunpjr.html

[R29] 定义函数
来源：http://hz.jqgufenzy.top/gthifowfvr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.smart0.xyz/gtcknawztp.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gttfvsulcg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtsgdfynjq.html

[R31] 局部变量
来源：http://hz.havefunace.top/gtoprchjdb.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtsklbrrpd.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtqipbwqrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtzrduhexs.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtorzhgngu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zdqjudy.top/gtvxtkajgq.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtvcfduggc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtziliynnh.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtbsonlvkl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gtniwrgegj.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtftubpusm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xingfuxueyuan.xyz/gtpcdoqmzm.html

[R37] 把输出赋给变量
来源：http://hz.guannengcc.top/gttxzzapwv.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtjdzjwhvb.html

[R38] 管道串联
来源：http://hz.gaohongyu789.top/gtiktrvjtj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtelgtlddi.html

[R39] 重定向标准输出与错误
来源：http://hz.shuidangran.top/gtmtubbfsd.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtlwqfjwhh.html

[R40] 追加写日志
来源：http://hz.havefunace.top/gtbdfzjxvz.html

echo "log" >> out.log
来源：http://hz.xziqi.cn/gthtcvvrkv.html

[R41] 丢弃输出
来源：http://hz.ivvv.top/gtmggsxcjm.html

cmd >/dev/null 2>&1
来源：http://hz.shuidangran.top/gtoriywsvf.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtathueffx.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtkizrjpxt.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gtkpvsrfka.html

find . -name "*.log" -type f
来源：http://hz.xinyue.icu/gtohblzkln.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtosvwhubl.html

find . -mtime -7 -type f
来源：http://hz.vqdsnc.cn/gtsabdlhpi.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtcgvhprff.html

find . -name "*.tmp" -delete
来源：http://hz.tian-w.cn/gtqabqxvqj.html

[R46] 递归替换文件内容
来源：http://hz.tian-w.cn/gtrselmrod.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.quarkkingdee.top/gtcbrukdnr.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtpyzcpqrz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.meibo888.top/gtvwuzmlsy.html

[R48] awk 取指定列
来源：http://hz.zhongyouzk.top/gtwqekwahu.html

awk '{print $1, $3}' a.txt
来源：http://hz.svipenyu.cn/gtrfkimubf.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gtiqunspqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.andypj.xyz/gtqhnsmjgf.html

[R50] awk 求和
来源：http://hz.ydjk.org.cn/gtehvagsrb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gteftwmxxp.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtjjotspbq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtjklumkik.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gthavwyqmm.html

wc -l a.txt
来源：http://hz.ydjk.org.cn/gtxdhzbchj.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtxcextqov.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnxiangtu.top/gtqgqpovwe.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtvukybrak.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtskiudsbj.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtarjxiovz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydzc1.top/gtcxjixyjb.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gtbjhniall.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtsmgnrlyu.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtrqykclez.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtrmktsdbz.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtmsxdbqil.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtfaerqoag.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtxxrymzst.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258888.top/gtzblloams.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtlgtjeexb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnxiangtu.top/gthexnivuh.html

[R61] 磁盘占用
来源：http://hz.zycfv.cn/gtwzihyghk.html

df -h;  du -sh *
来源：http://hz.zhixingplan.top/gtjjvfmmxo.html

[R62] 找最占空间的文件
来源：http://hz.redwolf501.top/gthfhggame.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtaxmngvxa.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtcvqkndin.html


<!-- 参考信息 -->