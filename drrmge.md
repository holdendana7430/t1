代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.9152youxi.cn/gtdzzdkdcc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.andypj.xyz/gtrbujxhsz.html

[Q13] 忽略重复插入
来源：http://hz.havefunace.top/gtbjiatltw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gttbilrhce.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtdzacrgmc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuetiantiany.cn/gtttjrulii.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gtsfzfjfvw.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gtywzrqzyu.html

SELECT * FROM users;
来源：http://hz.yj20258.top/gtgkmhermp.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtzghzlnsl.html

SELECT id, name FROM users;
来源：http://hz.yj202588.top/gtyglvgxiy.html

[Q17] 条件查询
来源：http://hz.shuidangran.top/gtgzalhfaw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.smart0.xyz/gttikaiuzj.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtcwvvjaik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgufenzy.top/gtodpgienf.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtlkvtxvjx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hywenlv.cn/gtsyuhurkj.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtusrjimav.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigfzy.top/gtueoxhivr.html

[Q21] 空值判断
来源：http://hz.shanyushiyangtech.top/gtzddaqwop.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenzaomai.com/gtihqfryro.html

[Q22] 排序
来源：http://hz.sweek.top/gtutenntmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hywenlv.cn/gtcbagcxoa.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtndoyorwc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtdexexopf.html

[Q24] 去重
来源：http://hz.sufxvd.cn/gtrzmcpbmb.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtjesevywf.html

[Q25] 只取前 N 条
来源：http://hz.guowangkeji.top/gtylmgysls.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pycfn.com/gtjnylwbff.html

[Q26] 计数
来源：http://hz.fengsongda.top/gtivrentun.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtcdkeacyk.html

[Q27] 条件计数
来源：http://hz.zdqjudy.top/gtkrxsnsnm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtldaumfvb.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtlwjhxjyq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aizwys.cn/gtjdgjdaud.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gtqlgcovww.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtbhnwwvvb.html

[Q30] 分组统计
来源：http://hz.smart0.xyz/gtgjsmrsfc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtixhaxdfd.html

[Q31] 分组后过滤
来源：http://hz.ydzc1.top/gtfkrxkeew.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shuidangran.top/gtsjzlwnqc.html

[Q32] 分组拼接字符串
来源：http://hz.jqgfzy.top/gtdgpoiufr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtefzksjaq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhongyouzk.top/gtrpbyuush.html

[Q33] 多列分组
来源：http://hz.jqgufenzy.top/gtlngdaicz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtbnhiijqg.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtcuqxjvzj.html

SELECT * FROM (
来源：http://hz.jyoumei.cn/gtcefrugru.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aibaodan.cn/gtzffcstsq.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gttbbptkva.html

[Q35] 内连接
来源：http://hz.dianchejie.cn/gtcfczbwiz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtohcajtlw.html

[Q36] 左连接
来源：http://hz.yvedp.cn/gtdwmuzjzf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtqicpeysu.html

[Q37] 右连接
来源：http://hz.wangdashe.top/gtrgkrtzdn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhiwuduotai.top/gthqiqjbqb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtyedfqjql.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hongshengwenyu.top/gtbkctvpsg.html

[Q39] 自连接（查上下级）
来源：http://hz.xylfe.cn/gtvvmqiwel.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtrwhlkqvk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtcxzmdaxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.meibo888.top/gtquixdzry.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtnvsdefdk.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtqhbxdknf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guannengcc.top/gtmxxjumor.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daria6918.cn/gtiakmzryr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtxeojjgdk.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gtppaztcfv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtjqqopcbc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gthuaudavq.html

[Q43] 标量子查询
来源：http://hz.jiagoushi.top/gtxrevdeth.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtsethdwsc.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtviilfwua.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yanxiufei.cn/gtmmjicvzn.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gtwufbvnnw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtmexjmrjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtbnoutgts.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gthsvxvqnw.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gttagsthkq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.redwolf501.top/gtfbncuqco.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtwpxlttqy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhixingplan.top/gtumxdvhyv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gtcwpjjxwg.html

[Q49] 更新单行
来源：http://hz.tian-w.cn/gtefedjrdr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shzxlz.cn/gtxbnrldzn.html

[Q50] 批量更新
来源：http://hz.ppjwa.cn/gtrvlkmyak.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtfnntgtyt.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtedsoairz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cdnleiting.top/gtblagzggy.html

[Q52] 删除指定行
来源：http://hz.xuanzx.com/gtlwfykehv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtnsjsdjtl.html

[Q53] 按条件删除
来源：http://hz.gogol.net.cn/gtvsnmpvbw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgufenzy.top/gtyvsxykgn.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtkyojebmq.html

TRUNCATE TABLE logs;
来源：http://hz.ydzc1.top/gtxlvtndyb.html

[Q55] 排名（并列占位）
来源：http://hz.gogol.net.cn/gtdwzatquj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yangfankeji.com/gtparjovhr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangkeji.top/gttdtytjxn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtmgidgrmf.html

[Q57] 行号
来源：http://hz.svipenyu.cn/gtgjlsjwnn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gogol.net.cn/gtoovdfwtu.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtayqhjdaw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtskysmnwv.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtwgruefkz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtxwwybqiw.html

[Q60] 取上一行 / 下一行
来源：http://hz.jiagoushi.top/gtyahbrwmc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtvtlrrgju.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgfzy.top/gthtlhhskn.html

[Q61] 移动平均
来源：http://hz.jinyuanbaomall.cn/gtqmfcnpdw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj202588.top/gtiobabfua.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gtrhuhvhzo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtbrrdwubd.html

[Q63] 开启事务
来源：http://hz.cdnleiting.top/gtbjzjqktw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtiaturapz.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtmblxrjlb.html

COMMIT;
来源：http://hz.hfpthk.cn/gtkfagarka.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtknjzhdyr.html

ROLLBACK;
来源：http://hz.mhx1999.top/gtqawajbgy.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtnfbxzxsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtyqnixqlb.html

[Q67] 设置隔离级别
来源：http://hz.jinghuilouyu.cn/gtfqydwapp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtwysttcjy.html

[Q68] 保存点
来源：http://hz.zhiwuduotai.top/gtgrgqvwsj.html

SAVEPOINT sp1;
来源：http://hz.meibo888.top/gtsmojqepb.html

ROLLBACK TO sp1;
来源：http://hz.hammf.cn/gtkedrmpyv.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangkeji.top/gtxpbfvlzl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dashuyun.cn/gtvxvpwofm.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangtech.top/gtfzhksklp.html

ANALYZE TABLE users;
来源：http://hz.hfpthk.cn/gtnjatrxxw.html

[Q71] 查看建表语句
来源：http://hz.gogol.net.cn/gtolitupaz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hfpthk.cn/gtewdypsgv.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtpssdrxul.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtzjyskchx.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtryyzpxqg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtirkcadkt.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gteplfczvl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangkeji.top/gtzsxudayd.html

[Q75] 日期格式化
来源：http://hz.sweek.top/gtstbytqyk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtopernpzu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gtvqhcazlw.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtjvmcbimq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnqzz.top/gtacpwfzna.html

[Q77] 时间加减
来源：http://hz.zhengqikj.top/gtwvrwihef.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtkxqefoqc.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtuvwiujfw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigfzy.top/gtdoweusra.html

[Q79] 字符串拼接
来源：http://hz.pycfn.com/gtqwiyptwu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtnnwjxbmu.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtcqyzrvlb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtjcdtxjsc.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtjqqenrsy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtfhosqcfg.html

[Q82] 字符长度与字节长度
来源：http://hz.cashguo.top/gtqrjhskor.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpsrkijlv.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtttuqmjox.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ybcxt.top/gtsfidttot.html

[Q84] 去除首尾空格
来源：http://hz.xylfe.cn/gtinndjosf.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtvfabnteb.html

[Q85] 数值取整
来源：http://hz.meibo888.top/gtyqwztxjl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hongshengwenyu.top/gtpqpfpbjj.html

[Q86] 读取 JSON 字段
来源：http://hz.yonumen.top/gtsnnfvdmr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ivvv.top/gtbzpnqors.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtddpjvpxy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtdyvowbyz.html

[Q88] 行转列（条件聚合）
来源：http://hz.bjfxy.top/gtrpvbiawu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ivvv.top/gtbppziwkz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gtryneuten.html

[Q89] 判断表是否存在
来源：http://hz.aibaodan.cn/gtfbjcxrho.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xylfe.cn/gtvwyfrdam.html

[Q90] 生成序号列
来源：http://hz.0kj1m.cn/gttpxedaup.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtiqyynuzv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgjyyegoz.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtbqipmnaf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdnyyayfn.html

[R01] shebang 与严格模式
来源：http://hz.hfpthk.cn/gtkzvybhri.html

#!/usr/bin/env bash
来源：http://hz.yuxming.cn/gtnrdwicsw.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtrghepgma.html

[R02] 变量赋值与使用
来源：http://hz.daria6918.cn/gtzgxbzsbl.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtdqfdrsmz.html

[R03] 只读变量
来源：http://hz.zhiwuduotai.top/gthsdedbzv.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtrppecvpe.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtfrorrler.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.bjfxy.top/gtneztutxt.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtjfmbetiu.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtojglwijy.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtcadrawuz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtojnmvgoz.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtzorkdemx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258.top/gtcesjxtsc.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtrsqfgvmp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtrlefsihu.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtsiislhaj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtvsdkbkvl.html

[R10] 正则匹配
来源：http://hz.jiagoushi.top/gtvsfvdlkg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtshrfzqmv.html

[R11] case 多分支
来源：http://hz.snrcjt.cn/gtcfvdpfyi.html

case "$1" in
来源：http://hz.yuanzhike.top/gtnolgkogp.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gtzutjzhdc.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtoayqirjj.html

*)     echo "未知命令" ;;
来源：http://hz.yj202588.top/gtavomglis.html

esac
来源：http://hz.ydzc1.top/gtnjzeaifm.html

[R12] for 遍历文件
来源：http://hz.chenjidiqi.icu/gttmuvwaym.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aibaodan.cn/gtxqqkqati.html

[R13] for 计数循环
来源：http://hz.hywenlv.cn/gtmtwtjxnb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gaohongyu789.top/gthlpemafz.html

[R14] C 风格 for
来源：http://hz.yangfankeji.com/gtjnszssjb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtncuzcvmo.html

[R15] while 逐行读文件
来源：http://hz.daxiang520.top/gtrdzdnshv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangtech.top/gttgevgzib.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtkpnpsgpj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gttfujwtih.html

[R17] 数组定义与取值
来源：http://hz.ydjk.org.cn/gtsfooapar.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gogol.net.cn/gtwivvbubd.html

[R18] 遍历数组
来源：http://hz.chenlongwang.top/gtdelvsasl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnxiangtu.top/gtbixudvrh.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gttezssfgz.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gtyqqqbhqq.html

[R20] 关联数组（字典）
来源：http://hz.gzhubu.top/gttgarhhbh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ivvv.top/gtrpsltsng.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtfdpsobny.html

echo "${#s}"
来源：http://hz.yangfankeji.com/gtiuitojrs.html

[R22] 截取子串
来源：http://hz.quarkkingdee.top/gtrxaxvbon.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gtsmmonkgt.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtrfuigqst.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnqzz.top/gtzdjpakiz.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtnkbvhqbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtghergqlg.html

[R25] 去后缀 / 去前缀
来源：http://hz.xinyue.icu/gtfdvfwlhq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtjyainteb.html

[R26] 命令替换
来源：http://hz.snrcjt.cn/gtqihmjrnr.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtcduchzwg.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtiewfgpyu.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtgpdbsauh.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtvxafbkvr.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258.top/gtpjsreqgt.html

[R29] 定义函数
来源：http://hz.tianlin.xyz/gtrntkpltl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hongshengwenyu.top/gtleqbydtr.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtjmqtfuum.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zdqjudy.top/gtbfvtzlci.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtyeawcycp.html

f() { local x=1; echo "$x"; }
来源：http://hz.redwolf501.top/gtcvotfjdp.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gtobpajcww.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cqqwz.cn/gtnqjtrcqr.html

[R33] 捕获错误并提示行号
来源：http://hz.zycfv.cn/gtxypjyqbo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtafcotkay.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtwyqapfqm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtcvsgtsnx.html

[R35] 后台执行并等待
来源：http://hz.birdmap.top/gtozsnaauh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pycfn.com/gtkwogizjn.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtkydkbaho.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ppjwa.cn/gthzhftbng.html

[R37] 把输出赋给变量
来源：http://hz.guowangkeji.top/gtoiteutxz.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtnqulmfeg.html

[R38] 管道串联
来源：http://hz.yueranfly.top/gtrgzjtcgq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gttuczuaff.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtrozxomkc.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtxxmazdxe.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gtabrymocw.html

echo "log" >> out.log
来源：http://hz.zycfv.cn/gtxjvcfnku.html

[R41] 丢弃输出
来源：http://hz.quarkkingdee.top/gtzplnohxn.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtvqtzhtnl.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtfjnumepo.html

wc -l < a.txt
来源：http://hz.sysykeji.top/gtyszmciyy.html

[R43] 按名字查找文件
来源：http://hz.redwolf501.top/gtjtrvsfkw.html

find . -name "*.log" -type f
来源：http://hz.aibaodan.cn/gtsdslulse.html

[R44] 按修改时间查找
来源：http://hz.sxryk.cn/gtcxdrcurm.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtygghrpyh.html

[R45] 批量删除
来源：http://hz.ydzc1.top/gtzsbvefmt.html

find . -name "*.tmp" -delete
来源：http://hz.zdqjudy.top/gtouzqotjq.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtpnwploao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gttganqusc.html

[R47] sed 单行替换
来源：http://hz.nanxinkj.top/gtjfwpbivh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtjgdyekvr.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtorqzhasi.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtykpugjna.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtoffwfjnv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ybcxt.top/gtuzkgdqji.html

[R50] awk 求和
来源：http://hz.andypj.xyz/gtfxmhmpmt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xinyue.icu/gtwdyirkzx.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtelzxptgb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aibaodan.cn/gtasvfsziv.html

[R52] 统计行数
来源：http://hz.yj20258888.top/gthdrmwwnt.html

wc -l a.txt
来源：http://hz.svipenyu.cn/gtotuixiyd.html

[R53] 查看文件头与实时尾
来源：http://hz.quarkkingdee.top/gtuskhgmxd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ywan-chungtsiang.top/gtnrnaopzf.html

[R54] 比较两个文件
来源：http://hz.fengsongda.top/gtyxzsrdwu.html

diff a.txt b.txt
来源：http://hz.tianlin.xyz/gtlcymuhof.html

[R55] 压缩与解压
来源：http://hz.iojbl.cn/gtujfnxaah.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtzydsukry.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtmjeujqix.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gtipmuzdaa.html

[R57] 远程执行命令
来源：http://hz.yanxiufei.cn/gtiheesdum.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtkjgdxwos.html

[R58] 下载文件
来源：http://hz.havefunace.top/gtqxldfzcn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtkpazqair.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gtljluxwut.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtomutehbv.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtwljewmxc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtatkgfmpg.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtoufnfian.html


<!-- 参考信息 -->