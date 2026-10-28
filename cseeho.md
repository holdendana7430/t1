代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jiagoushi.top/gttmkdjfeo.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtolauxsnj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtmuahxpti.html

[Q10] 插入单行
来源：http://hz.daria6918.cn/gtjswujubo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtjtdcrmlo.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gtomrrqeik.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtjjwnnrvn.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtgzmflwor.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtgdjsaprx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gtnvfklfmy.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gtnpbuixjc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtwsgndzei.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gthhxnylqf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gthqlppwtc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gtrvvhzmtv.html

[Q15] 查询全部
来源：http://hz.ywan-chungtsiang.top/gtxoxjcrod.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtprgvvyeu.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtiuipwtgj.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtiiruuxrw.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtjulnjqdx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sxryk.cn/gtgbsujjkt.html

[Q18] 模糊匹配
来源：http://hz.jlsjyb.cn/gtuyiwobdt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtpqluwgmg.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtljmldtcg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtwdnlasqi.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtsrbcqlrf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtzqdhoatc.html

[Q21] 空值判断
来源：http://hz.xylfe.cn/gtzonzbdks.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tanke756.top/gtbtgtfsfg.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtmgptcfgc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuanzhike.top/gtkrkldjox.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtbqvkxmry.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtwqkfdgtb.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtyetcshkk.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtsfaymoho.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtkljrkeuk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xingfuxueyuan.xyz/gtvyhrtqoh.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtizokpoat.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtrepqtwhb.html

[Q27] 条件计数
来源：http://hz.dianchejie.cn/gteyetyjih.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtedhxephg.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gtltjedvwz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtrlpyjrbu.html

[Q29] 最大最小值
来源：http://hz.zhaomingkeji.xyz/gtxdfaurdo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pycfn.com/gtizdxjhvt.html

[Q30] 分组统计
来源：http://hz.kuanghao11.cn/gtkhqrqfas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtqvmkxlke.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtbthiwiew.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.bjfxy.top/gtpenlider.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtfhckqhoi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtrnkzzbcz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.9152youxi.cn/gtneeconmj.html

[Q33] 多列分组
来源：http://hz.jinyuanbaomall.cn/gtwtyetpla.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtoaxclmjc.html

[Q34] 每组取第一条
来源：http://hz.zhengqikj.top/gtnbsuwzzt.html

SELECT * FROM (
来源：http://hz.gotoacloud.top/gttqqwakzh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xinyue.icu/gtkfbagqoj.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gtlnugbagc.html

[Q35] 内连接
来源：http://hz.tianlin.xyz/gtseuknzzu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtbovjznbg.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtswtjqsrz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gthortpwdf.html

[Q37] 右连接
来源：http://hz.ivvv.top/gtbzrmfgzj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gtxzbwgtjw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xylfe.cn/gtjkamstzy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gtwfcczcul.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gtwdunxtni.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtmjtwmuty.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtikmlpscb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhongyouzk.top/gttvorwiot.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtaadjtzpw.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gtpfzehdye.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yonumen.top/gtfvywddrk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gaohongyu789.top/gthyojsghh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtjcizjdli.html

[Q42] 连接条件附加过滤
来源：http://hz.xuanzx.com/gtxxayuvcq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.haohaochexian.top/gtxyxyqjkq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sweek.top/gtbdfcygsx.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtwgkvjftr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gthivsblyx.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtofdtyxzr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtvpabslgp.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtismhrrzn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtjwidldnn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxuanxn.top/gtavkpjtxt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtiysxqoub.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtuhauelif.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtnsfjcpqh.html

[Q48] CTE 公用表表达式
来源：http://hz.wangshuangyany.cn/gtwrbmtldr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hongshengwenyu.top/gtyuueuldz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fengsongda.top/gtaahrocxy.html

[Q49] 更新单行
来源：http://hz.52xcode.cn/gtjnhqwodb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtrrzajuhc.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtavdstsuq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtgxedmbzk.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtknhohrfj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guannengcc.top/gtymsnezca.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtgezbudcr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.havefunace.top/gtpovxbtpm.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gthonqwmsh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangkeji.top/gtpffbahek.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gtjosmucdr.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtlcmizasg.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtlqsufwtx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.svipenyu.cn/gtuzpqtfbo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuxming.cn/gtstsqhjjh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtfyopdsjq.html

[Q57] 行号
来源：http://hz.jqgufenzy.top/gtpekdrujz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pycfn.com/gtkeockwpc.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtmnhxscar.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gteebdrodm.html

[Q59] 分组内累计
来源：http://hz.xuanzx.com/gtbmmpupjp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fzhhl.top/gthaylaouj.html

[Q60] 取上一行 / 下一行
来源：http://hz.nwbrower.top/gtdcferyvn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtqmogujpe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.birdmap.top/gtjxslmhuf.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtnqhkeotm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxinkj.top/gtoljwhqyn.html

[Q62] 分组占比
来源：http://hz.gzhubu.top/gtvbylafah.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtpgyumoqn.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtojyagtkd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gotoacloud.top/gtmaivuhog.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gtdwdotaed.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtclwmmtci.html

[Q65] 回滚事务
来源：http://hz.hnxiangtu.top/gtkjygtmnq.html

ROLLBACK;
来源：http://hz.mhx1999.top/gtjdyoznex.html

[Q66] 行锁查询
来源：http://hz.yueranfly.top/gtyncoeaih.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhiwuduotai.top/gtjsorqwhu.html

[Q67] 设置隔离级别
来源：http://hz.gaohongyu789.top/gtswirhtwi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtrqleupvc.html

[Q68] 保存点
来源：http://hz.fzhhl.top/gtcuoquxgi.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtwiwnmlut.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtjqzszhyz.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gttellqstr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gtgkpfukey.html

[Q70] 更新统计信息
来源：http://hz.316326.xyz/gtjdtlouhp.html

ANALYZE TABLE users;
来源：http://hz.xziqi.cn/gthmngupml.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gttfvrewpp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtcronzzib.html

[Q72] 查看索引
来源：http://hz.tianlin.xyz/gtelunqwts.html

SHOW INDEX FROM users;
来源：http://hz.xinyue.icu/gtlsrdqbnk.html

[Q73] 查看表状态
来源：http://hz.0kj1m.cn/gtqmdisxeu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigufen.top/gtsqxsyxud.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtlvocmuqb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yonumen.top/gtbqhtfsad.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtmznhzecs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtwfvmmjau.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.0kj1m.cn/gtndojgoyd.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gttealvprd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtrwilmedr.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtucxmvysh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gtircrbfid.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtntorkzir.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydjk.org.cn/gtiucqktsk.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtlvrlgzkr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuanzx.com/gtnqilimkn.html

[Q80] 字符串截取
来源：http://hz.52xcode.cn/gtqllbtczu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.haohaochexian.top/gtxmkaefjw.html

[Q81] 字符串替换
来源：http://hz.ydzc1.top/gtgpjapqep.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gtgumqdcyg.html

[Q82] 字符长度与字节长度
来源：http://hz.zdqjudy.top/gtquvrnozf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtmexqsfeb.html

[Q83] 大小写转换
来源：http://hz.tian-w.cn/gtutvsmbyv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtumbzyawn.html

[Q84] 去除首尾空格
来源：http://hz.yueranfly.top/gtdtzgfrfp.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gttjgboajw.html

[Q85] 数值取整
来源：http://hz.xylfe.cn/gtapvpemib.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sweek.top/gtiecjwfne.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtziznodkp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgfzy.top/gtokzjtlut.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gtceuqsxjm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daxiang520.top/gtxmascfpq.html

[Q88] 行转列（条件聚合）
来源：http://hz.nwbrower.top/gtmqvugcbj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fzhhl.top/gtrfolseul.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gotoacloud.top/gtrgudclnr.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtetfunjix.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtvjghxhqk.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtuxqybgti.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hfpthk.cn/gtljbcxuud.html

================================================================================
来源：http://hz.tianlin.xyz/gtemuwembk.html

R. Bash 专题
来源：http://hz.cashguo.top/gtiakqlcyn.html

================================================================================
来源：http://hz.yongpay.top/gtnvczhsbj.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtmxytsnjm.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtctbbrgfp.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gtymuxujbm.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gturjpjvtk.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtftwonmvn.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtkcbdaclb.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtdacdiakq.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtwjcxajlw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jianghu66.top/gtophratcj.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtnjfhupfw.html

name="${1:-default}"
来源：http://hz.tanke756.top/gtnkdzbadn.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtoaemcfig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gzhubu.top/gtfxgxrfsy.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gtwamtjnjs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gttixsgfyf.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtbkxtvjwg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fengsongda.top/gtqqnpeieu.html

[R09] 字符串比较
来源：http://hz.chenlongwang.top/gtrnxiyopw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtjugvuabp.html

[R10] 正则匹配
来源：http://hz.yvedp.cn/gtsvwjqwgn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zdqjudy.top/gtzfjuorvw.html

[R11] case 多分支
来源：http://hz.hfpthk.cn/gtdrleqvsq.html

case "$1" in
来源：http://hz.316326.xyz/gthpeypulx.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtbqjztoio.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtpvifdkwn.html

*)     echo "未知命令" ;;
来源：http://hz.gotoacloud.top/gtmrzznooy.html

esac
来源：http://hz.gogol.net.cn/gtjolhbswk.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtpngdgdxg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gtxjouroql.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtsydfwxoh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhixingplan.top/gthcbhjhwf.html

[R14] C 风格 for
来源：http://hz.zhijiandao.cn/gttlvzqjvn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ivvv.top/gtnomsqfkx.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gtvooklsaa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtzwqvsjwx.html

[R16] until 等待条件
来源：http://hz.zdqjudy.top/gtliuwnawj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtkhrcriql.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gtmakzglrv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xingfuxueyuan.xyz/gtkencmanj.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gtjxzpkipm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xingfuxueyuan.xyz/gtdsxkcpnv.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtjrvxuysv.html

echo "${#arr[@]}"
来源：http://hz.zycfv.cn/gtwiodkkzm.html

[R20] 关联数组（字典）
来源：http://hz.shzxlz.cn/gtmiewlccn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gtubmvdumf.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gttmbutbpe.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtpqvekuso.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gthwxlruqx.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtgkyqrtae.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtooboqiqx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtldvvtxfw.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtmdnaqjng.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj202588.top/gtrwvbjlwa.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtatfisqqh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtxtcjobkt.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gtexabqhzp.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtxgfpexsq.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gthquprydl.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtrczxiona.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtfxtuqtva.html

echo "scale=2; 10/3" | bc
来源：http://hz.ydzc1.top/gtiswufbwc.html

[R29] 定义函数
来源：http://hz.tanke756.top/gtpndlkcav.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gthlgrwain.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtuhnqbkaq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gzhubu.top/gtcumzeybt.html

[R31] 局部变量
来源：http://hz.jlsjyb.cn/gtjdozhngu.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtzzvxhvgh.html

[R32] 参数个数校验
来源：http://hz.shangyingyoupin.top/gtcijuvbqc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtsaezyoxq.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtodejksmp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhaomingkeji.xyz/gtkakjlwni.html

[R34] 退出时清理
来源：http://hz.zhoulong.xyz/gtqvnqckti.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtandpzuge.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtwfcribyd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtkuapcrzt.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gtyimpogkc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtjzujmocl.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gtzzxjdhoz.html

files=$(ls -1)
来源：http://hz.zhijiandao.cn/gtjegjinsb.html

[R38] 管道串联
来源：http://hz.tanke756.top/gtrujguklw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gtjkljdfoc.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gttljfazfy.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtyyfiktzx.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtdrrmhafr.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtzibqztbz.html

[R41] 丢弃输出
来源：http://hz.zdqjudy.top/gtlldcvciu.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtorwknwus.html

[R42] 输入重定向
来源：http://hz.tian-w.cn/gtkdckiswy.html

wc -l < a.txt
来源：http://hz.quarkkingdee.top/gtvajmgtfc.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtqdxcrdcf.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtwtjkmcdk.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtbonernwu.html

find . -mtime -7 -type f
来源：http://hz.cucudq.cn/gtzcctsicg.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtvdedygwm.html

find . -name "*.tmp" -delete
来源：http://hz.xuanzx.com/gtzphaltqf.html

[R46] 递归替换文件内容
来源：http://hz.chenlongwang.top/gtlabnoujy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gthtkeplnh.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtywmzrnko.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gtfclridbx.html

[R48] awk 取指定列
来源：http://hz.smart0.xyz/gtshhhjlcb.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtiqqlzxsk.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtxuttqarj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.iojbl.cn/gthkxzagju.html

[R50] awk 求和
来源：http://hz.nanxuanxn.top/gtlzexyomx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtqxyiiutz.html

[R51] 排序去重取前几
来源：http://hz.yvedp.cn/gtocaulqvs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gthnbuwfke.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtdxbbfrwa.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtizmjrrcm.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtgqxpvgom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtuqctooss.html

[R54] 比较两个文件
来源：http://hz.vqdsnc.cn/gtpkvxdhla.html

diff a.txt b.txt
来源：http://hz.quarkkingdee.top/gthmlowxxt.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtqlubgqsz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtszbqsgoa.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtsrgbyeae.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtgupltovk.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtcnfkmjgu.html


<!-- 参考信息 -->