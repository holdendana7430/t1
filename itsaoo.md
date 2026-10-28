代发 wailian999

SELECT * FROM users;
来源：http://hz.hysaishi.cn/gtyahhnnsp.html

[Q16] 查询指定列
来源：http://hz.gogol.net.cn/gtyypinwce.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gtkosbwfqb.html

[Q17] 条件查询
来源：http://hz.sufxvd.cn/gtwyngqdqm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuanzx.com/gtcwhfmvrl.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtimnvaabr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhiwuduotai.top/gtsjekcotk.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtmbrkokdj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtxampliui.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtjidiiuje.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hammf.cn/gtufzubatg.html

[Q21] 空值判断
来源：http://hz.pengpengdd.cyou/gtvrwhtvlt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtoebqagwa.html

[Q22] 排序
来源：http://hz.cdnleiting.top/gtuagwzedl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtdqcsynci.html

[Q23] 分页
来源：http://hz.hnxiangtu.top/gtnnoyobzp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtjhtocppv.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gtbslkjqmk.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtshcwizqs.html

[Q25] 只取前 N 条
来源：http://hz.havefunace.top/gtwayapuoh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gtnndylsxv.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtujsprifn.html

SELECT COUNT(*) FROM users;
来源：http://hz.hongshengwenyu.top/gtljgqfzlt.html

[Q27] 条件计数
来源：http://hz.meibo888.top/gtwpjfeora.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yangfankeji.com/gtrzsjsaqw.html

[Q28] 求和与平均
来源：http://hz.jqgufenzy.top/gttzbpwddk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhiwuduotai.top/gtrijnhntl.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtzrbsxbhy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gtmbuqzbbx.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gtqmdwdcxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtowzgwlys.html

[Q31] 分组后过滤
来源：http://hz.gzhubu.top/gtwfwgzwbs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtsksqpdnk.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtcqjbxqzq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtbtoshpmo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hongshengwenyu.top/gtbbcquiar.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtefqnxwrv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtsgcsywin.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtiwsyafip.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtughnvfzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nwbrower.top/gtmcajomdi.html

) t WHERE rn = 1;
来源：http://hz.cashguo.top/gtyavikiaf.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtchwhrmhs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtofeswwhv.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtnznhpkvs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtklhlphkh.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtzjxwfnax.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zycfv.cn/gtbvbaxzeu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guannengcc.top/gtamttaivg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhixingplan.top/gtatkcvwia.html

[Q39] 自连接（查上下级）
来源：http://hz.shzxlz.cn/gtsmqflbqd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nwbrower.top/gtufycegxf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtoeegfjyf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtukvotgdw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gtpuzltfrk.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtqudzsxpu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gtcegzzsfg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.havefunace.top/gtskotmmkv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuxming.cn/gtnakswpew.html

[Q42] 连接条件附加过滤
来源：http://hz.316326.xyz/gtzpespkhk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jlsjyb.cn/gtsvjnhepz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxinkj.top/gtlapivyus.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtumaqamxc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jianghu66.top/gtzxnvraix.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gtdmptnbyk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtsabsmsmq.html

[Q45] EXISTS 判断存在
来源：http://hz.havefunace.top/gtwejkzndc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtqhyydmxq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xylfe.cn/gtnhhlojou.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtpyjqcjpd.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtctnuzfra.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangshuangyany.cn/gtyueyjfqa.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtplyuhgrc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtiiyzbivv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.vqdsnc.cn/gtiifcvofy.html

[Q49] 更新单行
来源：http://hz.hnqzz.top/gtfttguduk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtzmhiehvi.html

[Q50] 批量更新
来源：http://hz.yuxming.cn/gtbdgdjmej.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtcdqeahpu.html

[Q51] 用子查询更新
来源：http://hz.tanke756.top/gtgiuhxklh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtsyjkuaxr.html

[Q52] 删除指定行
来源：http://hz.shuidangran.top/gtdeaymaoj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtbvfywhcy.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtpwarxbcm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtcvemckaw.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtwrreglpl.html

TRUNCATE TABLE logs;
来源：http://hz.wangdashe.top/gtfqpxacce.html

[Q55] 排名（并列占位）
来源：http://hz.zhixingplan.top/gtbpsqwcpn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daxiang520.top/gtitgnkslm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtbjnypyrv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtmyjquxyg.html

[Q57] 行号
来源：http://hz.jinghuilouyu.cn/gtscatrdiy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gtjlpgzptg.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gthtuqsypu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtwahdbpks.html

[Q59] 分组内累计
来源：http://hz.daria6918.cn/gtwembgpbj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ivvv.top/gtujqlajli.html

[Q60] 取上一行 / 下一行
来源：http://hz.cqqwz.cn/gtmgbhpjmp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dianchejie.cn/gtidlmwoxu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.52xcode.cn/gtenhrfyol.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtmdsrgwnq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtpdtqzszn.html

[Q62] 分组占比
来源：http://hz.316326.xyz/gtgmyspukl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtkbmeeeyi.html

[Q63] 开启事务
来源：http://hz.pycfn.com/gtbrojaroa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtcgblgvjc.html

[Q64] 提交事务
来源：http://hz.redwolf501.top/gtcguvdvja.html

COMMIT;
来源：http://hz.wangshuangyany.cn/gtpkeqaged.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtiequubmo.html

ROLLBACK;
来源：http://hz.shuidangran.top/gthsexrdzx.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtofwnskkl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gttkvkqchv.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gtwqoybdxr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtbcrbequx.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtcdwopmsp.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gthsolfvxl.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtyifaapav.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtwoudvwoz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.guowangkeji.top/gtuglghgrs.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtoshwfipt.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtydgeckqv.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtupzkyoox.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jqgfzy.top/gttscjsahx.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtgkrvzjgk.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gtjcbgqukk.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtgoydzurx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.birdmap.top/gtjauvcrql.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtqujnmbxb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydzc1.top/gtbjnawzjk.html

[Q75] 日期格式化
来源：http://hz.yangfankeji.com/gtooxzihpk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtjwwwktgc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yanxiufei.cn/gtmynwnhze.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtpspttyxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.vqdsnc.cn/gtimiqpjbv.html

[Q77] 时间加减
来源：http://hz.zhixingplan.top/gtbrrqydha.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shzxlz.cn/gthkxnijju.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtqvzmjegj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtpsbllimg.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtmjgbexxm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtzgonlxrg.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtvwnuxlgv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtictptoxl.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtphfibaoz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtdueycghz.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gtexprluno.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shzxlz.cn/gtjzyuwvom.html

[Q83] 大小写转换
来源：http://hz.jinqigufen.top/gtziioihfi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gttlcrvnuz.html

[Q84] 去除首尾空格
来源：http://hz.nwbrower.top/gtzojzlokn.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtkjsoevsf.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtqylakoln.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.havefunace.top/gtwkzgguor.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtfhsdmdtm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.birdmap.top/gtcoohsgnn.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gtbimqlmij.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtaqnrsqwt.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtorkkdegs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtvafkfjso.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yueranfly.top/gtzrqggejn.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gtdyyzfhaf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtekspchdq.html

[Q90] 生成序号列
来源：http://hz.cdnleiting.top/gtkrbzafck.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nwbrower.top/gtelhqcdmy.html

================================================================================
来源：http://hz.daria6918.cn/gtksgeemyv.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtwvtaaafa.html

================================================================================
来源：http://hz.guannengcc.top/gtokjphnwr.html

[R01] shebang 与严格模式
来源：http://hz.aizwys.cn/gtwnmjacft.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtzxmxwwwq.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtsybjwxaf.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gttmkvwbas.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtpeiwxjwo.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtlbdwnmsu.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtqzfsrzcy.html

[R04] 位置参数
来源：http://hz.yuxming.cn/gtlhauyqoa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guannengcc.top/gtgfkmzjzn.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gtyyznjele.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gthkapgxiu.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtnxeothgi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtgrrtjtoe.html

[R07] if 判断文件
来源：http://hz.chenzaomai.com/gtvsydlfxr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gtvdlgfzgm.html

[R08] 数值比较
来源：http://hz.52xcode.cn/gtmqhivhvb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhaomingkeji.xyz/gtvcjjucxt.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtepodzcbq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuxming.cn/gtbrdiyozk.html

[R10] 正则匹配
来源：http://hz.jinghuilouyu.cn/gtioopzsoe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtjjaviirm.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtrzzcnffv.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtihzgdanc.html

start) echo "启动" ;;
来源：http://hz.havefunace.top/gtpwtfkizw.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtankcspyt.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtfzbuifmp.html

esac
来源：http://hz.gzhubu.top/gtlwdoxijp.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gttaxrzmai.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtvcqkudpy.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtkhdawjeo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.svipenyu.cn/gtqkacnhsp.html

[R14] C 风格 for
来源：http://hz.havefunace.top/gtruxqzfcq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtcqeyvxti.html

[R15] while 逐行读文件
来源：http://hz.zhongyouzk.top/gtcxapjppq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.snrcjt.cn/gthamknipe.html

[R16] until 等待条件
来源：http://hz.cucudq.cn/gtqzwabzox.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtvikjmner.html

[R17] 数组定义与取值
来源：http://hz.cucudq.cn/gtmhzpfjle.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtgvvtxwkk.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtnwpljbfc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gthhhwmvzi.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtmoclysjr.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangkeji.top/gtcnuixykp.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtlgpskdkh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinyuanbaomall.cn/gtfegucszs.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gthmcadesb.html

echo "${#s}"
来源：http://hz.cqqwz.cn/gtxrwrnytk.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtrzsnoilx.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtbvqlpkwz.html

[R23] 字符串替换
来源：http://hz.cqqwz.cn/gtmojufepv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtxyzuqmod.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtcsmyhqws.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gtogbjmpax.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtrwwqgeal.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtfuutlzqz.html

[R26] 命令替换
来源：http://hz.xuetiantiany.cn/gtxcxyagpa.html

now=$(date +%F); echo "$now"
来源：http://hz.shuidangran.top/gteuivwguq.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtigniqale.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtyhdkivtt.html

[R28] 浮点运算
来源：http://hz.tianlin.xyz/gtwlznsccr.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gtoxczxidr.html

[R29] 定义函数
来源：http://hz.daxiang520.top/gtznhbxxmf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sweek.top/gtwlihzdpp.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtdzypxael.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtwllvrajg.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtixueizdi.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtxgkbpxpt.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gtzaagxyxv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gthacztqey.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtvnjfzgxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgfzy.top/gtiurpulgc.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtgfnihcjl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtozxhqtdk.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gteobjoobi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.redwolf501.top/gtajeuasyk.html

[R36] 并发执行多个任务
来源：http://hz.ydjk.org.cn/gtnsicrviw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jianghu66.top/gturfimhha.html

[R37] 把输出赋给变量
来源：http://hz.ydjk.org.cn/gtpgbhjwam.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gtnirjqkxr.html

[R38] 管道串联
来源：http://hz.hnxiangtu.top/gtytgrvlqk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhoulong.xyz/gtptksxeca.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxinkj.top/gtjqaaabtb.html

cmd > out.log 2>&1
来源：http://hz.meibo888.top/gtvbsthehb.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtqhvpxeem.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtfknibadz.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gttjzdfgon.html

cmd >/dev/null 2>&1
来源：http://hz.hfpthk.cn/gtsotdccmu.html

[R42] 输入重定向
来源：http://hz.vqdsnc.cn/gtovygyhei.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gttoopmfmj.html

[R43] 按名字查找文件
来源：http://hz.yj20258.top/gtadngampc.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtdygepzkf.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gthrmbnuuf.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gteaukfmlc.html

[R45] 批量删除
来源：http://hz.ivvv.top/gtpirecqwk.html

find . -name "*.tmp" -delete
来源：http://hz.tanke756.top/gtdviwzslg.html

[R46] 递归替换文件内容
来源：http://hz.haohaochexian.top/gtburgnuwu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.feifeiyinyue.top/gthfvdhgaf.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtqzgwutxq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtmwfnqlhe.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtqqurjtnh.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtsvqaqszv.html

[R49] awk 带条件
来源：http://hz.zdqjudy.top/gtdnogvtiu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtodsstpaz.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtmroerpcl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yongpay.top/gtrvziwznd.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtcurxloij.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtidrnuppr.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtrwmmtcac.html

wc -l a.txt
来源：http://hz.meibo888.top/gtdhzbyxww.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtqfafddol.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.havefunace.top/gtbacuupuc.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtbhndbxcs.html

diff a.txt b.txt
来源：http://hz.redwolf501.top/gtgzcdobeb.html

[R55] 压缩与解压
来源：http://hz.svipenyu.cn/gtjktkjkpw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tian-w.cn/gtmuimtbcf.html

[R56] 远程拷贝
来源：http://hz.xylfe.cn/gtjrjierbd.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtjgfedemr.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gtukjstfsi.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtcxqtvmun.html

[R58] 下载文件
来源：http://hz.zhaomingkeji.xyz/gtjlazxlkv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtvqcxnild.html

[R59] 发 POST JSON
来源：http://hz.nwbrower.top/gtfdiyyneo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenlongwang.top/gtmqyozolc.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtqphindjz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj20258888.top/gtdmyqaitp.html

[R61] 磁盘占用
来源：http://hz.bjfxy.top/gtwofwxwbl.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtgvknhxmo.html

[R62] 找最占空间的文件
来源：http://hz.sufxvd.cn/gtigwkexvw.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gttkbiyeft.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gteomamerq.html

free -h;  ps aux | grep nginx
来源：http://hz.52xcode.cn/gtwmbnilbx.html

[R64] 结束进程
来源：http://hz.xinyue.icu/gtmxeedrfn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtvsbwgheg.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gttfwkoiyk.html


<!-- 参考信息 -->