代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.mhx1999.top/gtfyguufyy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtplnovgjn.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtjpayivsu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tanke756.top/gtenbfvgyj.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtftwqhqqg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtlsibrwey.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtttoyavxz.html

[Q15] 查询全部
来源：http://hz.jyoumei.cn/gtwuxgtkkd.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtgomowgxl.html

[Q16] 查询指定列
来源：http://hz.daxiang520.top/gtggyenzuf.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtfpugqjbm.html

[Q17] 条件查询
来源：http://hz.guowangkeji.top/gtqhtgpgjb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hammf.cn/gthjvluaxb.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtvkmdheig.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gtwxglkotm.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtwulkbnpb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zycfv.cn/gtjdpwsvaq.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtooxsuzqb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtgkasmkyh.html

[Q21] 空值判断
来源：http://hz.hnxiangtu.top/gtypvwiuck.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtmpfmykky.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtciwfaluc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtogdclbrc.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtxfgnvcvl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gtnwulyrah.html

[Q24] 去重
来源：http://hz.jqgfzy.top/gtzdlkcglg.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtknbdsywu.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtztiitfqk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.9152youxi.cn/gtrwoqypwd.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtsyuzvzjs.html

SELECT COUNT(*) FROM users;
来源：http://hz.daria6918.cn/gtddmjmnrq.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtdqoyaupc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daria6918.cn/gtnqqcspwi.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtgowmjwsd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtwelndioe.html

[Q29] 最大最小值
来源：http://hz.bjfxy.top/gtkakwbdvm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gotoacloud.top/gtcxphvmox.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtaacxhwri.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtowdwslwp.html

[Q31] 分组后过滤
来源：http://hz.zhixingplan.top/gtghvafzqf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtmirfbjpe.html

[Q32] 分组拼接字符串
来源：http://hz.dashuyun.cn/gtfzlzpdhy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtxsngjqed.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtgivlrxxe.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtuupvzftk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtrwfrvkmw.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtrwtlryog.html

SELECT * FROM (
来源：http://hz.shanyushiyangkeji.top/gtazhlnjdj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtirsazewi.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtiumzxogr.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gthpfygjhs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtihicylyl.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gtybdtnucp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gthowflkxs.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtunwlgirv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258888.top/gtghzzijwa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shangyingyoupin.top/gtbokwkhnh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ehwqpu.com/gtspmmkdwy.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtjzetkcqc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtjbxsnhfk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtjurtniro.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtenfdrdyw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hammf.cn/gtlghfotev.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtnrafxehh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jianghu66.top/gtpktjnllv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.svipenyu.cn/gtpyrsfykq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtjfbbxzay.html

[Q42] 连接条件附加过滤
来源：http://hz.hfpthk.cn/gtcjhhrlqv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hywenlv.cn/gtazxqkyhk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gtepmyswfq.html

[Q43] 标量子查询
来源：http://hz.yj20258888.top/gtwnsiofny.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gtutmtojui.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gtaudpcojf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtuwboowaf.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gtojanpndn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtrmsfjjxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gtaleufohc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtgicdwrui.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtvhnhtmxt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtnzjgufbu.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gtxiywlpis.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.haohaochexian.top/gtcmguwzwm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtelqlmpfk.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtnfizjhzf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtsbfkxpug.html

[Q50] 批量更新
来源：http://hz.yanxiufei.cn/gtxwazzzyr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hammf.cn/gtdukrdsjv.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtqwizrcmx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtqiexhmda.html

[Q52] 删除指定行
来源：http://hz.feifeiyinyue.top/gtesylinka.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shuidangran.top/gtiatxeugr.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtapgsbwrr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtfcrjfqup.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtnlidahcd.html

TRUNCATE TABLE logs;
来源：http://hz.zhongyouzk.top/gtclghnitv.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtwwrobnws.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gthoawwmxp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gtjlpmpfpi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtemjfuzzj.html

[Q57] 行号
来源：http://hz.smart0.xyz/gtrygcxjrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhengqikj.top/gtykuetqop.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtipfnfiok.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtiwedoaac.html

[Q59] 分组内累计
来源：http://hz.birdmap.top/gtwynvyryt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ehwqpu.com/gtbxgypnbk.html

[Q60] 取上一行 / 下一行
来源：http://hz.cashguo.top/gtptbfbdws.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj202588.top/gtruzsmcqo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtrxxdqkdn.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtdqefjycb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ivvv.top/gtumbawvsq.html

[Q62] 分组占比
来源：http://hz.hysaishi.cn/gtxfvjgsnc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtuqlfjbzp.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtmazgspjy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtnmqdlvto.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtmltyvycj.html

COMMIT;
来源：http://hz.sxryk.cn/gtzjaejggg.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtfsjotxza.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtmrvsgudp.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gthcfrlykv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtrvhsokmu.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtxlbuuqli.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gtlgtchkai.html

[Q68] 保存点
来源：http://hz.hywenlv.cn/gtctposylp.html

SAVEPOINT sp1;
来源：http://hz.cqqwz.cn/gtwwgsjncx.html

ROLLBACK TO sp1;
来源：http://hz.hammf.cn/gtqkfbxeyb.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangtech.top/gtjinocsaa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtdraahxkz.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtystxyyjy.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtrqrkbwxr.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtylarqpak.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fengsongda.top/gtdbqkbiem.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtyftcvenm.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtbkyejgdh.html

[Q73] 查看表状态
来源：http://hz.aibaodan.cn/gtvooessax.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtcjaunmmf.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtwpjpwlic.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yangfankeji.com/gtdeootvzn.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtcqpsmlos.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.kuanghao11.cn/gtidnjqppq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtdaeavmri.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtavgkdurd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zdqjudy.top/gthrgiensh.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtvthqrois.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pycfn.com/gtzlldztzm.html

[Q78] 当前时间
来源：http://hz.cdnleiting.top/gtfkzbllxb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jianghu66.top/gtfopomwgb.html

[Q79] 字符串拼接
来源：http://hz.gaohongyu789.top/gtwxahectw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ivvv.top/gtdreqzgwg.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtiferzhvo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtocnokeja.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtpsucmdow.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtjoabqojq.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtzmelimtj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtgvjoltwq.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtglzuvtao.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.snrcjt.cn/gtuwkbppls.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtuclyajkn.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuanzx.com/gtitaxlfqt.html

[Q85] 数值取整
来源：http://hz.xziqi.cn/gtbtgipqai.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hongshengwenyu.top/gtgzhyiwyd.html

[Q86] 读取 JSON 字段
来源：http://hz.feifeiyinyue.top/gtqstprwnz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtrjpsqybu.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtsbqexudb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ivvv.top/gtlhnuxkzn.html

[Q88] 行转列（条件聚合）
来源：http://hz.316326.xyz/gtrfnquumq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtbntgelhd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtxxsmogwr.html

[Q89] 判断表是否存在
来源：http://hz.jinqigufen.top/gtrtfssjpp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxuanxn.top/gtuobkqjoy.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtczztgmsd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtmpscgsst.html

================================================================================
来源：http://hz.dianchejie.cn/gtshjihbsq.html

R. Bash 专题
来源：http://hz.sufxvd.cn/gtwaqihcsp.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrwewkoxb.html

[R01] shebang 与严格模式
来源：http://hz.jlsjyb.cn/gtgeusxwwy.html

#!/usr/bin/env bash
来源：http://hz.yongpay.top/gtoexswgfx.html

set -euo pipefail
来源：http://hz.jianghu66.top/gtvucyiqao.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtfdemnkiz.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtwzlkmsow.html

[R03] 只读变量
来源：http://hz.fengsongda.top/gtqhgtpkat.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gttggqgwgz.html

[R04] 位置参数
来源：http://hz.yj20258888.top/gtdnmntqke.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dashuyun.cn/gtldxhtzie.html

[R05] 参数默认值
来源：http://hz.jiagoushi.top/gtacdkphms.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gtahlvqxff.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtlndommkp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gtsohhsqvz.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gthmswksfs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtkgpjlcfp.html

[R08] 数值比较
来源：http://hz.ybcxt.top/gtoafqekef.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangtech.top/gtuculmzez.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtfkhjrtbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtzwbeqnmd.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtzrsglasj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtsrqjqrzh.html

[R11] case 多分支
来源：http://hz.shanyushiyangkeji.top/gtyrhqngwl.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gthijizxzm.html

start) echo "启动" ;;
来源：http://hz.zhixingplan.top/gtwcvzjrpi.html

stop)  echo "停止" ;;
来源：http://hz.ppjwa.cn/gtmjzpqbyv.html

*)     echo "未知命令" ;;
来源：http://hz.shuidangran.top/gtospkztgc.html

esac
来源：http://hz.hongshengwenyu.top/gtprcfyglb.html

[R12] for 遍历文件
来源：http://hz.cdnleiting.top/gtfkwivusz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtksoefiiv.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gtzdqqijmt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtyxrkvxgx.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gtydprdfko.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtanjbbdzu.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gtqccykrau.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtrtdxagip.html

[R16] until 等待条件
来源：http://hz.zhoulong.xyz/gtipkzrfmp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtqnmtbqpf.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtwvbpldav.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtheabaywj.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtmbdxebpz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtywltjntw.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtxsxxtekt.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtikggigyt.html

[R20] 关联数组（字典）
来源：http://hz.cucudq.cn/gtcpfixwps.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.meibo888.top/gtskmszwnj.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtlrfmoyub.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtpuvnmmmn.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtcgemaswz.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtusptaofv.html

[R23] 字符串替换
来源：http://hz.sysykeji.top/gtxgycmbrf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtvfdinpvf.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtwlrssrqw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.redwolf501.top/gtohicszqq.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinghuilouyu.cn/gtrvrcdafr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sufxvd.cn/gtoroegcka.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtmmrlrwtp.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtickhxsbh.html

[R27] 算术展开
来源：http://hz.ydzc1.top/gtsohemeab.html

echo $((1 + 2 * 3))
来源：http://hz.tian-w.cn/gtpxvbblwa.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtdgjyrfpf.html

echo "scale=2; 10/3" | bc
来源：http://hz.havefunace.top/gtrloyoufp.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtjgqexiuc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangtech.top/gtebkfpirw.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtfucqfbha.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gtxenjucls.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtmqxutzmo.html

f() { local x=1; echo "$x"; }
来源：http://hz.gotoacloud.top/gtgkruyvmq.html

[R32] 参数个数校验
来源：http://hz.zdqjudy.top/gtqfeqkgta.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigufen.top/gtpboexygi.html

[R33] 捕获错误并提示行号
来源：http://hz.zhaomingkeji.xyz/gtkzzkrhgb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtyeewdmuu.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtlfxlofpg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtidnzxdkq.html

[R35] 后台执行并等待
来源：http://hz.0kj1m.cn/gtcbgqmocr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtxypkssis.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtobvcavok.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gtmpznrdwy.html

[R37] 把输出赋给变量
来源：http://hz.jinqigfzy.top/gtflskdyod.html

files=$(ls -1)
来源：http://hz.yj20258.top/gtddiouogk.html

[R38] 管道串联
来源：http://hz.yj20258.top/gtgadsignv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtqvcizlkw.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gteteubuam.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gtbbiusdny.html

[R40] 追加写日志
来源：http://hz.xingfuxueyuan.xyz/gthanpodsm.html

echo "log" >> out.log
来源：http://hz.cdnleiting.top/gtvrzgchcm.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtjznypddi.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtcxonomdi.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gtdimufrja.html

wc -l < a.txt
来源：http://hz.316326.xyz/gtblljgzen.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gtmemhzepk.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtulkjzgja.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtvxtsudnn.html

find . -mtime -7 -type f
来源：http://hz.zhaomingkeji.xyz/gtespixsia.html

[R45] 批量删除
来源：http://hz.zhoulong.xyz/gtsqhlbosn.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gttenxxvbp.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtjwemzwrh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhiwuduotai.top/gtsgflgrcq.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtsglhphye.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gtemlewaca.html

[R48] awk 取指定列
来源：http://hz.yj202588.top/gtdtruttce.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtqodxqkta.html

[R49] awk 带条件
来源：http://hz.nanxuanxn.top/gtryedrmkh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hongshengwenyu.top/gtmaobpfjc.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gtvjkfmfnx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gttiugpgco.html

[R51] 排序去重取前几
来源：http://hz.zycfv.cn/gtstqtubza.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gotoacloud.top/gtvjdsnwie.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtzqvtvpte.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtffqdaior.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gtbspzoeyx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yangfankeji.com/gtzdqedlko.html

[R54] 比较两个文件
来源：http://hz.jlsjyb.cn/gtnyeucnbn.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtzpyxzgip.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtndvfxsei.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gthunwtgol.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gtvmrekwes.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtgwybyvct.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtjqfvpsvz.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gtbboynbso.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gtuiaoyabq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtgtjhrtto.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtxmszhruk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cucudq.cn/gtxqohpesg.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtaqrhwhei.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhixingplan.top/gtcbrxgiyc.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtfmtszzav.html


<!-- 参考信息 -->