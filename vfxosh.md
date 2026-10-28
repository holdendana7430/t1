代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258888.top/gteiebdyyu.html

[Q11] 一次插入多行
来源：http://hz.xinyue.icu/gtrjncoksw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtlfazuete.html

[Q12] 插入后取自增 ID
来源：http://hz.wangdashe.top/gtfoebakho.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xylfe.cn/gteeyaeqta.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtjehnmqef.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gtkcgzgdsj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtktfrugnr.html

[Q14] 存在则更新（upsert）
来源：http://hz.yonumen.top/gtcozympvv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sxryk.cn/gtumiabvri.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shangyingyoupin.top/gtwfkwnegr.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gtmdjmcqgu.html

SELECT * FROM users;
来源：http://hz.zycfv.cn/gtqiamebtv.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtjwkgutur.html

SELECT id, name FROM users;
来源：http://hz.jqgfzy.top/gtyvyzebmt.html

[Q17] 条件查询
来源：http://hz.cheryme.top/gtopopwrrn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtgpghxyld.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtmkcifspg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.9152youxi.cn/gtbzbpkxce.html

[Q19] 范围查询
来源：http://hz.daxiang520.top/gtduelzkyo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtvlqpnmra.html

[Q20] IN 列表
来源：http://hz.cheryme.top/gtthvmwbwn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhijiandao.cn/gtbxvgdwqh.html

[Q21] 空值判断
来源：http://hz.kuanghao11.cn/gttvhzireu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtwzenxzws.html

[Q22] 排序
来源：http://hz.guannengcc.top/gtujqhhlob.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xinyue.icu/gtnzafelsc.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtuicssgji.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtpoubhkys.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtqftgzpzn.html

SELECT DISTINCT city FROM users;
来源：http://hz.hongshengwenyu.top/gtarlriflf.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtesszjjkz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yanxiufei.cn/gtcdjfases.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtoqcjdxmq.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhengqikj.top/gtbhmgrrbb.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtfrqajbsh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daria6918.cn/gtdfollcvb.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtymeyeupm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtxkomroua.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtfencbwyp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuetiantiany.cn/gtrpwjizdh.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtgtobnkgj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtzxpsblox.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtglmjacqh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtnoopgoxd.html

[Q32] 分组拼接字符串
来源：http://hz.gogol.net.cn/gtugphcfuq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gthhjuxltf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yueranfly.top/gtbqrqoqus.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtkmrfkwvi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sxryk.cn/gtvjyxuijh.html

[Q34] 每组取第一条
来源：http://hz.sysykeji.top/gtbldbseke.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtihrckbnz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jianghu66.top/gtkkiwynnm.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gtihafffwx.html

[Q35] 内连接
来源：http://hz.xuanzx.com/gtqpfkrilz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtviircqyb.html

[Q36] 左连接
来源：http://hz.nwbrower.top/gtzyreiocw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtaidvnedm.html

[Q37] 右连接
来源：http://hz.yangfankeji.com/gtultavowx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtkmeqnsei.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daria6918.cn/gtpyxmwltt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gtjlvhqwzd.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtjyfunsjp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gttqzznlal.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tian-w.cn/gtqcmlpznj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtjpixotlj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xziqi.cn/gtfettpgvn.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtroarsjjz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtgmluuogp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuanzhike.top/gtkmlijxsk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuxming.cn/gtnrihbaqu.html

[Q42] 连接条件附加过滤
来源：http://hz.yanxiufei.cn/gtxnwkeakj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xziqi.cn/gtlyazalsu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yanxiufei.cn/gtnuaqqqnn.html

[Q43] 标量子查询
来源：http://hz.jiagoushi.top/gtfdcyqkuk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shzxlz.cn/gtklmcsqbl.html

[Q44] IN 子查询
来源：http://hz.xuetiantiany.cn/gtareknpip.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xziqi.cn/gtkbahdufn.html

[Q45] EXISTS 判断存在
来源：http://hz.ybcxt.top/gtiinifloo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gtthumqxzc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gtchtwvqlu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtwbfbhggc.html

[Q47] 与平均值比较
来源：http://hz.feifeiyinyue.top/gtmixzcexm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.birdmap.top/gtbfmvcsyi.html

[Q48] CTE 公用表表达式
来源：http://hz.yanxiufei.cn/gthnpliekd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gtyrlbjhme.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.vqdsnc.cn/gtmpyeekdn.html

[Q49] 更新单行
来源：http://hz.hongshengwenyu.top/gtcpxyaytp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shuidangran.top/gtgvcyhgnq.html

[Q50] 批量更新
来源：http://hz.aibaodan.cn/gtxfhvujlu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gthqrgfhra.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtktmfknrw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.c1oappe.top/gtyrwhhrdn.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtwlwgudng.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtyfilqgef.html

[Q53] 按条件删除
来源：http://hz.ywan-chungtsiang.top/gtwkqaczsm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangdashe.top/gtrvrgvywd.html

[Q54] 清空表
来源：http://hz.svipenyu.cn/gtzavpchhk.html

TRUNCATE TABLE logs;
来源：http://hz.birdmap.top/gttvadufyr.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtzfpyhntx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daria6918.cn/gtzqspcede.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gttwikdiwx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sufxvd.cn/gtgpbgikbn.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtjqpppumj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgufenzy.top/gtrvhcbbjl.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtrawfdfts.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.feifeiyinyue.top/gthrsmnkkl.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gtprgvnhav.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydjk.org.cn/gtuuatpawc.html

[Q60] 取上一行 / 下一行
来源：http://hz.xziqi.cn/gtzujvewsl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dianchejie.cn/gtovxgqqan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtcmhgvfjg.html

[Q61] 移动平均
来源：http://hz.zhixingplan.top/gtolwxmnvz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtmeqvwluz.html

[Q62] 分组占比
来源：http://hz.cheryme.top/gtvkiyyqyr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtjdfjysqa.html

[Q63] 开启事务
来源：http://hz.redwolf501.top/gtqtsuqtrr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yonumen.top/gtkxkrekyy.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtcamkrbqs.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtumsrftda.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtlsfusiih.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtdlhkmeey.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gtvvzioxbp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtiptxreib.html

[Q67] 设置隔离级别
来源：http://hz.hnqzz.top/gtzirzmbdw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gtkzgtilkr.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtjrqzvuvb.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gthglenqpf.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtcwpaywfy.html

[Q69] 查看执行计划
来源：http://hz.yuanzhike.top/gtwalqgksh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtaervhgjl.html

[Q70] 更新统计信息
来源：http://hz.hnqzz.top/gtcgdfjiue.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gtmnrelphs.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtvdlodimh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtyotcpqjc.html

[Q72] 查看索引
来源：http://hz.sysykeji.top/gtoqiiyqqy.html

SHOW INDEX FROM users;
来源：http://hz.havefunace.top/gtydtberfj.html

[Q73] 查看表状态
来源：http://hz.yangfankeji.com/gtacrswefq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtfofdoead.html

[Q74] 强制使用索引
来源：http://hz.cucudq.cn/gtbmsyuhxy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtdjkqmuxf.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtuefpulpk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtyyavmugn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtcpjjwukt.html

[Q76] 按天统计
来源：http://hz.ivvv.top/gtzcwqdiub.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtajpjxsja.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtgzqtcvvt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtlkmewsam.html

[Q78] 当前时间
来源：http://hz.yj20258888.top/gthdcluezd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnxiangtu.top/gtkfjfbmeg.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtmjofsbhs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dashuyun.cn/gtesvafixg.html

[Q80] 字符串截取
来源：http://hz.sufxvd.cn/gtynrfcavl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gtfmgzsgmo.html

[Q81] 字符串替换
来源：http://hz.zycfv.cn/gteycwxfuc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pycfn.com/gtjxwdqvtm.html

[Q82] 字符长度与字节长度
来源：http://hz.sufxvd.cn/gtbmpbcipq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yueranfly.top/gtuiakumdg.html

[Q83] 大小写转换
来源：http://hz.yj20258.top/gtwxpjpgze.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gttxphwyhv.html

[Q84] 去除首尾空格
来源：http://hz.gaohongyu789.top/gtrulkjmgp.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigufen.top/gtjnqdorme.html

[Q85] 数值取整
来源：http://hz.52xcode.cn/gtzbqnuhvn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xinyue.icu/gtitumuikv.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtpzdzmdfp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daria6918.cn/gtmavoxubm.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtwpjpobnp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtrzfvepxz.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuanzx.com/gtudczoahk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.c1oappe.top/gtwpnlshhq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtfvtidvmu.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtlmzzovgm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dashuyun.cn/gturgqdfjm.html

[Q90] 生成序号列
来源：http://hz.jinqigufen.top/gtfgwhqdbc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtfvbmtflx.html

================================================================================
来源：http://hz.gogol.net.cn/gtsryeptfx.html

R. Bash 专题
来源：http://hz.sweek.top/gtgrehnzqj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcjvpmlzk.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtekypiwju.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtkauzcpnt.html

set -euo pipefail
来源：http://hz.jinqigufen.top/gtcocccgkh.html

[R02] 变量赋值与使用
来源：http://hz.sxryk.cn/gtuiwekhwl.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtbbbpiriw.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gtifsyblns.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtlxzoabnw.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtiqxokmwi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gtyektfuwm.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtcdyhxcne.html

name="${1:-default}"
来源：http://hz.snrcjt.cn/gtaijqebgq.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtmgmnkzbk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtjlmegxbb.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtmeuikfgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xylfe.cn/gtacxfffey.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtxgylydij.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.snrcjt.cn/gtmjokqzfh.html

[R09] 字符串比较
来源：http://hz.svipenyu.cn/gtondpzokv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtwrotnspd.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtrctqqznp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtqibhkghv.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gtvuzfsmai.html

case "$1" in
来源：http://hz.jiagoushi.top/gtevknqxye.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtonxqgijc.html

stop)  echo "停止" ;;
来源：http://hz.yueranfly.top/gtwedabjko.html

*)     echo "未知命令" ;;
来源：http://hz.redwolf501.top/gtlmbsjwce.html

esac
来源：http://hz.jlsjyb.cn/gthfzmgvmf.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtfotfuvjx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yongpay.top/gtbiybydoz.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtwfdcsjwt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtdjiorayp.html

[R14] C 风格 for
来源：http://hz.snrcjt.cn/gtbctridzo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aizwys.cn/gthjietecg.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gttbklhziv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtdfwlyjgb.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtstiysrrg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtzrhrattg.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtnnhddtqo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnxiangtu.top/gtjbqltlsv.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtkmzruihy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gzhubu.top/gtpgjpjhrh.html

[R19] 数组长度
来源：http://hz.cashguo.top/gtfqznoygz.html

echo "${#arr[@]}"
来源：http://hz.cdnleiting.top/gtxpagwvqk.html

[R20] 关联数组（字典）
来源：http://hz.nwbrower.top/gtiyavzvrq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gtupvagpcd.html

[R21] 字符串长度
来源：http://hz.zhaomingkeji.xyz/gtcxtletiq.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtpzudlyik.html

[R22] 截取子串
来源：http://hz.nanxuanxn.top/gtqtofbmpe.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtgbqkvuui.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtxlcgzdno.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtfsdnhbbe.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtknggisgo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtjgverxxk.html

[R25] 去后缀 / 去前缀
来源：http://hz.hongshengwenyu.top/gtwqhhdhno.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gtnjfdoaaj.html

[R26] 命令替换
来源：http://hz.nanxuanxn.top/gthpqlxjdy.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258888.top/gtdcpvvvpi.html

[R27] 算术展开
来源：http://hz.zhaomingkeji.xyz/gtprcpduyf.html

echo $((1 + 2 * 3))
来源：http://hz.xingfuxueyuan.xyz/gttmgmngpb.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtqaztpxke.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtynofmfld.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtzbjstzko.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gthizmkvbf.html

[R30] 函数返回状态码
来源：http://hz.xuetiantiany.cn/gtiyleoxhl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gttyyqgcei.html

[R31] 局部变量
来源：http://hz.zycfv.cn/gtkswhsyfq.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtjcnfzpxj.html

[R32] 参数个数校验
来源：http://hz.ivvv.top/gtvxydgvep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tian-w.cn/gtummrrucw.html

[R33] 捕获错误并提示行号
来源：http://hz.sufxvd.cn/gtghgwvens.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pycfn.com/gtsmvvqwho.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtjeqnakbm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtazkutygc.html

[R35] 后台执行并等待
来源：http://hz.ydzc1.top/gtydutgrvb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gtvwcebqkv.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtzmtcojqo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnxiangtu.top/gtzpoedsmf.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtktphoqpt.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtrvmgfmxi.html

[R38] 管道串联
来源：http://hz.meibo888.top/gtazncsfsg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gtrazarkzj.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258.top/gtwivsoxhk.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtnugpayok.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gthldqjehg.html

echo "log" >> out.log
来源：http://hz.yongpay.top/gtglbveppv.html

[R41] 丢弃输出
来源：http://hz.ywan-chungtsiang.top/gtkagabpyj.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtqdhdcpgn.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtwxsyvygn.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtmxammclj.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtsqgcvgmh.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtvsnnvmrh.html

[R44] 按修改时间查找
来源：http://hz.daxiang520.top/gtruiofeev.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtyxogjjda.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtakoafrve.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gtqzevrniz.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtvetzfigb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangshuangyany.cn/gtgsbisnka.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtywlgjfjk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtrcavmezm.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtcliwunds.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtbapnandm.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtinzboidu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pycfn.com/gtyjpwsldz.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gtahsqxmho.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gttnjtfrne.html

[R51] 排序去重取前几
来源：http://hz.havefunace.top/gtpmbpvese.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtgmrvhbus.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gttmahfqzc.html

wc -l a.txt
来源：http://hz.shanyushiyangtech.top/gteboidmza.html

[R53] 查看文件头与实时尾
来源：http://hz.andypj.xyz/gtervipqgm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtnzwbrxyj.html

[R54] 比较两个文件
来源：http://hz.dianchejie.cn/gtqbvcoutu.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtwniridbx.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtmtpsawew.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xziqi.cn/gtxyyvolhi.html

[R56] 远程拷贝
来源：http://hz.cqqwz.cn/gtwlmnuqaw.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gthosdhddx.html

[R57] 远程执行命令
来源：http://hz.cucudq.cn/gtxjnblsya.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtykjjlevs.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gteffqtuuy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnqzz.top/gtwmzeupmu.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtqwilwrom.html


<!-- 参考信息 -->