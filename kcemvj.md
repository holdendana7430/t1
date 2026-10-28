代发 wailian999

SELECT * FROM users;
来源：http://hz.zhiwuduotai.top/gtnnapbgny.html

[Q16] 查询指定列
来源：http://hz.cdnleiting.top/gtiucrayjs.html

SELECT id, name FROM users;
来源：http://hz.daria6918.cn/gttxprcfgg.html

[Q17] 条件查询
来源：http://hz.hywenlv.cn/gtbywjiiym.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtfbpvyreo.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtxceltvib.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yvedp.cn/gtynuqtfih.html

[Q19] 范围查询
来源：http://hz.pycfn.com/gtwknisukm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yongpay.top/gtzsbbedyj.html

[Q20] IN 列表
来源：http://hz.shzxlz.cn/gtnbsznewa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xinyue.icu/gtbqmausii.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtmrskoksn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtjnvvaulu.html

[Q22] 排序
来源：http://hz.hnqzz.top/gtujmrnqea.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cashguo.top/gtxctcaakt.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtqnqmohgh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenzaomai.com/gtawogypbi.html

[Q24] 去重
来源：http://hz.gotoacloud.top/gtsnscoiho.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtsqjnjjyg.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtdbnmeshe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtyobubaep.html

[Q26] 计数
来源：http://hz.wangdashe.top/gtzeknwecx.html

SELECT COUNT(*) FROM users;
来源：http://hz.yueranfly.top/gtcywmummh.html

[Q27] 条件计数
来源：http://hz.pengpengdd.cyou/gtzfyuyyje.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtpfapmppp.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtliukpyvw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.andypj.xyz/gtttalhimw.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gthzwdhoul.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jlsjyb.cn/gthxyxavgk.html

[Q30] 分组统计
来源：http://hz.hnxiangtu.top/gtjxbwlnpw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtpxcggapf.html

[Q31] 分组后过滤
来源：http://hz.yj20258888.top/gtjkqgkglq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zdqjudy.top/gtinzuksea.html

[Q32] 分组拼接字符串
来源：http://hz.9152youxi.cn/gtntcjzevh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtfvjvhkth.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhongyouzk.top/gtgghrouys.html

[Q33] 多列分组
来源：http://hz.wangshuangyany.cn/gtogvctefb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gaohongyu789.top/gtgisgftoc.html

[Q34] 每组取第一条
来源：http://hz.ybcxt.top/gtnubcfrcj.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gtredotajf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhijiandao.cn/gtcfcetvho.html

) t WHERE rn = 1;
来源：http://hz.jinyuanbaomall.cn/gtepktjexv.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtinaxfbjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtcypbgauf.html

[Q36] 左连接
来源：http://hz.xuanzx.com/gtcwspfqzv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtjqlzchrq.html

[Q37] 右连接
来源：http://hz.jqgufenzy.top/gtznjwelit.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sweek.top/gtoieqvqwb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jiagoushi.top/gtalxvonlv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtgzjrnbbp.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtxodqvzsz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuxming.cn/gtqcdozvww.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.9152youxi.cn/gtaqtncavz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zdqjudy.top/gtxgumawzf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gttjltecnq.html

[Q41] 多表连接
来源：http://hz.meibo888.top/gtvrcuitjr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dianchejie.cn/gtearlcztj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gtpfnuvjnp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gtdzmygcqj.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtxrmjrkpq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtiekvuknq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtvmqpjehi.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtflamhslx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtugmcdtsm.html

[Q44] IN 子查询
来源：http://hz.gzhubu.top/gtbssrcqln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtwyocqilk.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangkeji.top/gtubpixxui.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtzauzeebe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhongyouzk.top/gthdfrzxed.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtzbtgwnvi.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtgzbcmdgq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtxzjjdptz.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtxsqtnfni.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.andypj.xyz/gtgqsqudrt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gtcomxkuap.html

[Q49] 更新单行
来源：http://hz.chenjidiqi.icu/gtesbjwpgv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtqpdjfnng.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtbfuambhs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtedearopt.html

[Q51] 用子查询更新
来源：http://hz.bjfxy.top/gtxddhzqdw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gtrlydnaqv.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtldtzlklk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtebejvsle.html

[Q53] 按条件删除
来源：http://hz.gaohongyu789.top/gtvjeysdca.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xylfe.cn/gtonxnyodp.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtlmkunncy.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtguyxpsxo.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gthnkzqcfb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gtlohrketz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtusqzeczn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtllmxvdmt.html

[Q57] 行号
来源：http://hz.jinqigfzy.top/gtatyzqzzz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gogol.net.cn/gttsiaglrw.html

[Q58] 累计求和
来源：http://hz.meibo888.top/gtidychlri.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhixingplan.top/gttrgkrtyg.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtvmerogfl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtsnhwdgyn.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gtlpwvzypn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuetiantiany.cn/gtjajyvevx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gthedfptyk.html

[Q61] 移动平均
来源：http://hz.cucudq.cn/gtlyicdfxj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xylfe.cn/gtralynink.html

[Q62] 分组占比
来源：http://hz.xziqi.cn/gtyqbgtwqc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtoqdgggtt.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtyrolatpt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtjfnooxds.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtvebohutn.html

COMMIT;
来源：http://hz.yj20258.top/gtiejppmfh.html

[Q65] 回滚事务
来源：http://hz.xylfe.cn/gtvharhsvd.html

ROLLBACK;
来源：http://hz.yj20258.top/gtwayhwwpu.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtndwrnsgg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtevimurmw.html

[Q67] 设置隔离级别
来源：http://hz.snrcjt.cn/gtpvxkburz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gtuzrxwrgn.html

[Q68] 保存点
来源：http://hz.gotoacloud.top/gtuwjzinjt.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtjzvirvwi.html

ROLLBACK TO sp1;
来源：http://hz.yj20258.top/gtkefeiihs.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtyxhbyzhw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ydzc1.top/gtbikdykrw.html

[Q70] 更新统计信息
来源：http://hz.chenjidiqi.icu/gtacdbpdsd.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtdqcqvxiy.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtxyvabeqv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gtcpaaowxv.html

[Q72] 查看索引
来源：http://hz.jinqigufen.top/gtzvlspemc.html

SHOW INDEX FROM users;
来源：http://hz.chenlongwang.top/gtqmysvyzu.html

[Q73] 查看表状态
来源：http://hz.smart0.xyz/gtpicphluq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtzlbidpcg.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtmiynogva.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtujkzlzdd.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtpszuaird.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtwhhbvlpq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtcqquzpxu.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtjkjfmmqb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gthyprxjsx.html

[Q77] 时间加减
来源：http://hz.52xcode.cn/gteztvnaap.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtwbuvtnhp.html

[Q78] 当前时间
来源：http://hz.kuanghao11.cn/gtfnxriwxb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtupeaxkuz.html

[Q79] 字符串拼接
来源：http://hz.zhiwuduotai.top/gtgloxhgdx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yongpay.top/gtyqdsrhii.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtawwjdmej.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.316326.xyz/gteaewftyj.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtibqvkboz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtzckfquqq.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtaeqwvexg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtlfsxulos.html

[Q83] 大小写转换
来源：http://hz.jqgfzy.top/gthiqmpzao.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtydvxamdt.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangtech.top/gtieafnvcg.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtgavtnplb.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gtmbtfnwte.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhoulong.xyz/gtcjkdqkxg.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtgabqghaq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtwskewwyd.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtnqxovvit.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydjk.org.cn/gtcymrywov.html

[Q88] 行转列（条件聚合）
来源：http://hz.shzxlz.cn/gtgrzszcie.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.mhx1999.top/gtemmhxkkw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtqlsuwequ.html

[Q89] 判断表是否存在
来源：http://hz.jiagoushi.top/gtilkaslfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj202588.top/gtawjffbih.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtltvekhmu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtlrzdelee.html

================================================================================
来源：http://hz.gzhubu.top/gtzoxugsad.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtcyzukydb.html

================================================================================
来源：http://hz.ehwqpu.com/gtvnxlirwp.html

[R01] shebang 与严格模式
来源：http://hz.chenjidiqi.icu/gtjcmvfwrt.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtktzykugq.html

set -euo pipefail
来源：http://hz.xziqi.cn/gtdhlbwfok.html

[R02] 变量赋值与使用
来源：http://hz.havefunace.top/gtktbpoosl.html

name="Tom"; echo "$name"
来源：http://hz.9152youxi.cn/gtrwwjnvwz.html

[R03] 只读变量
来源：http://hz.yangfankeji.com/gtrdcgvglh.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gtqcjvmrrd.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtpvqvcclb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydzc1.top/gtrtkjvzyl.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtypuwasxj.html

name="${1:-default}"
来源：http://hz.pycfn.com/gthzgujbuk.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtyagiyzmp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtnphzmsvp.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtyliwgotb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtfdzevxgc.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtxghouoqp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gttirwzkjk.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtwddpqsbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sxryk.cn/gtkbqciyqr.html

[R10] 正则匹配
来源：http://hz.jlsjyb.cn/gtckoqwwcp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtnxgpagnm.html

[R11] case 多分支
来源：http://hz.tanke756.top/gtztmwtslx.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtxmtpsnjk.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtkbhkiivf.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtcyzrlzpn.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtlcqyscnc.html

esac
来源：http://hz.gaohongyu789.top/gtbvlmfawp.html

[R12] for 遍历文件
来源：http://hz.jqgfzy.top/gtpnfznrep.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nwbrower.top/gteychdlnt.html

[R13] for 计数循环
来源：http://hz.xylfe.cn/gtzlbbdaix.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtgeawjbfo.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gtzjktdtje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtqzrkeqbe.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtsfdhvxpw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtpqpisdcm.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtzecledqu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gtgiwxhhce.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtupppixez.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtyidyrtrq.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtqabocwcj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtvhvzdymc.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtwkflojxu.html

echo "${#arr[@]}"
来源：http://hz.nanxinkj.top/gtuknnqzgj.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtltevrlmr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtxtkiwnfk.html

[R21] 字符串长度
来源：http://hz.chenjidiqi.icu/gtfdpteuxa.html

echo "${#s}"
来源：http://hz.mhx1999.top/gthlboyifj.html

[R22] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtjiivjjfz.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtxqsiocjq.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtquexmwgl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shuidangran.top/gtptunxjph.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtqzmiwkdh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtfbcqjkcq.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtenjoyyji.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenlongwang.top/gtmtzihpqg.html

[R26] 命令替换
来源：http://hz.chenjidiqi.icu/gtnbhghubo.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gthriyqaib.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtrsbrgvsx.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gtxhacjugc.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtpgelelfu.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtcjndcnqs.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtssbstrhs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shuidangran.top/gtkoaoxdav.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtihhredce.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guowangkeji.top/gthrplcjse.html

[R31] 局部变量
来源：http://hz.snrcjt.cn/gtlmqmfbyt.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuanzx.com/gtwcwzdfjt.html

[R32] 参数个数校验
来源：http://hz.svipenyu.cn/gtabvjuiki.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtqmjbzmqt.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtpbryhqdf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtfcfbmnjm.html

[R34] 退出时清理
来源：http://hz.sufxvd.cn/gtdylwwikj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtpbrnbsux.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtnphbqyjz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.redwolf501.top/gtnlnsnkup.html

[R36] 并发执行多个任务
来源：http://hz.smart0.xyz/gtgapvbqir.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gtlsjtjcat.html

[R37] 把输出赋给变量
来源：http://hz.shuidangran.top/gtsqfbfjop.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtwhmtkhgu.html

[R38] 管道串联
来源：http://hz.kuanghao11.cn/gtmvztgozf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtqmzkvvdb.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258.top/gtsdnghvgw.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtbuvjwezv.html

[R40] 追加写日志
来源：http://hz.jinyuanbaomall.cn/gtpmjowmep.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gtnounwnfi.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtslzunzdm.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtjfmteopx.html

[R42] 输入重定向
来源：http://hz.sxryk.cn/gtzyywudwi.html

wc -l < a.txt
来源：http://hz.cheryme.top/gtgqedjctj.html

[R43] 按名字查找文件
来源：http://hz.chenjidiqi.icu/gtalzcloef.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gtxsllcyuw.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtctrgaktk.html

find . -mtime -7 -type f
来源：http://hz.wangshuangyany.cn/gtcinwsjxb.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtsuxruakx.html

find . -name "*.tmp" -delete
来源：http://hz.ybcxt.top/gtnedtarfh.html

[R46] 递归替换文件内容
来源：http://hz.yangfankeji.com/gtfdtphhqw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtyqguowtv.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gtviphtljx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gturgkxpsz.html

[R48] awk 取指定列
来源：http://hz.hongshengwenyu.top/gttocfwqzw.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinyuanbaomall.cn/gtkfmcbyud.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtpvrvyayb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtrnufileb.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtkcfbdsln.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtrivmtnha.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtdejddgsq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.bjfxy.top/gtqwtafees.html

[R52] 统计行数
来源：http://hz.zhijiandao.cn/gtztxdgvym.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtpnlqtoxj.html

[R53] 查看文件头与实时尾
来源：http://hz.xingfuxueyuan.xyz/gtigdtlepg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fzhhl.top/gtoerkvmgh.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtpwhkclce.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtazpvatsz.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtnqbfzyqm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zycfv.cn/gtylinlhhq.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gteyeceakt.html

scp file user@host:/path/
来源：http://hz.guowangkeji.top/gtidkhteto.html

[R57] 远程执行命令
来源：http://hz.wangshuangyany.cn/gtesbhkgbg.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtsxinqtax.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtdaawraqa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhongyouzk.top/gtwikyvbqy.html

[R59] 发 POST JSON
来源：http://hz.shuidangran.top/gthfxbctjp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tanke756.top/gtqalncuta.html

[R60] 只看 HTTP 状态码
来源：http://hz.smart0.xyz/gtzffhepiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtdjnxmlmr.html

[R61] 磁盘占用
来源：http://hz.yuxming.cn/gtflxttfmv.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gtebzdistc.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtmdllyxgs.html

du -ah . | sort -rh | head -10
来源：http://hz.yongpay.top/gtfeodqxhg.html

[R63] 内存与进程
来源：http://hz.9152youxi.cn/gticwffmjh.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gthwxrwpta.html

[R64] 结束进程
来源：http://hz.cdnleiting.top/gtlxxajohl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtgzgwjnka.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtsilzokch.html


<!-- 参考信息 -->