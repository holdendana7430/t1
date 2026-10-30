代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gsydoqxob.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glousnesg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ghladvwew.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gjhzdmyhd.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/glaimcdid.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gtxzoxdra.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gnfcgmkmq.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/glbfhbdnw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gsdhsrawo.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gycwfwaqg.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gpyqxutoe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/glprscqag.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gycskhgpu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ghjhlagyr.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gywdydxen.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gvuunulna.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/ghealxpqj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gajddnrui.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gtbkbfihl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gnqyqhdry.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/guighwflj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gqpjsapam.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gdquivegf.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gjhkixbhc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/glewnuwlu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gyjvmswtg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gncxjqvyg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gxjeknqus.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gdnwhcdfb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gbeimlmrs.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gpvcvxddq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gzhqfcxyv.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gouuqnicd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/ghgnalopx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gesyqjnam.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gjemwbtov.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gnlsgtiqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gvhqyhuha.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gxhmbqokf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gfpgymthe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gjgwrnaoi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gvjmamany.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gsxnzmyrx.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/glcozbqzm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gmtydigiq.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gpntdmgky.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmgppszxq.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gseanpthc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gwmvdnmae.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/ghnunifkn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gavbbzeol.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/giehprjwa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gyufccddi.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gvjevbxdz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/giuvftwjr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gwpofmfti.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gnoytidjn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gcruezmzr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gwqczadyu.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gicqbqlit.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpyyystcf.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gcaksqfxn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvmgrdf.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gcyjdybxw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gcwflpgcy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gnhhzzmnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gxpqfnykp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glyrzkkbe.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/golbyhpyv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gzxhqyzkx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gzbivvrpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkmwvraxl.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkheehcjw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gtuggqocv.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gsicgzgwt.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gdxhhvhzl.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gkwohlcyx.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/ghggpsudu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gztacikpf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gzlmuxaiz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gbalesvpg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gzgeeqwht.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gmlyqnjmo.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/glbtsacvr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gcolbluol.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gvihmtufe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/griagirua.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gxuwdmrqr.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gyhjenwxt.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/grzufneeo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gcmdgoczx.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gthcsovwn.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gqziwwtul.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gocchwily.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gcumifumc.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gndcrusph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/grxxvqagz.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gphmatqgn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gmekpuile.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gvlceldyg.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/geoxovoxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gljtqpssn.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gonukwtdx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ggflezwih.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gjgkrvzbb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gctcgxsce.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gnasosydu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/ghjqabpdy.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gehuvflbb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxrgaycwb.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gousstgfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gckdczgjp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/goghsgkay.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gomlicpua.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gyqqnywnj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpehsehzt.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gkeccnuqi.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggysvyzoh.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/glrfonpcs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gmadotqtl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gyvqhgrxh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gflwoirno.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gavzyorxc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gebuiplwa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gkoqlpqos.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/goaagsvgq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gthsyrark.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gygrupivy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gnqirukpb.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gbaggmnio.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gubjyngii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghllijlra.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gqaeqiyfv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjvlhqxxi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gkcjqrzyw.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gbuopazee.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gkswktoxv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gjjnzknbd.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gtyrtqzbv.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gosmbwrtt.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gyqldtuwb.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gzluveetb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gqcpefovc.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gawolkjkn.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/grdhikxsk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gtictznqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggfoudopb.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/giguqkkbi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpumpthyq.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gdhsgnabj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gwtinmsne.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gdfwxdltr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/geshynima.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gxrodetma.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/glkxlcfhp.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gvpplmaqo.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gmckpkcfx.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gsdibedqv.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gdmzxrdtr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gwelgexic.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gejdgslkq.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gjrdhbepn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gaziuqtpi.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gwnslowpd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/guqjbppwi.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/grmcqsrfh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/grjiyzwyh.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwdhvogwk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gslwiynuc.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gwcvrxtmv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gezrdckbr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gmtbabfwc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gszmuwsqc.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/ggwjmdyne.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gupjnhygy.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/ggbcziwrq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gokgzuvit.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gfabscgcn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gnajskrlf.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmaznrwqn.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gowxvuwqv.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gjeealxxv.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gatocxbmj.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gnrtkjvwk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjzgicuce.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gnnnrjboc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gevwwdvxa.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gsvfbwabm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gamudvojr.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/ghhmoqpoa.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gtqlneady.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gkpsqbzcs.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/grdkyrhai.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gnqqunjwr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/ggkvrbnud.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gswsheuxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gcquxcekq.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gikmqjjlg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/ghupgpjhj.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gccndbebe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gazzhabyg.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gffzrgvhy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/graukxkds.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/ginnmukqq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gqfzxltdz.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gbnpjfkmd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gnjeulolp.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gvdlvqipj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ggvdnociy.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gqmdloiml.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/glwnqmcyh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gppliwqxr.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gvzdxitcf.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gkgmkwnqq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gygqiwacx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gvhszvnua.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/grogtzlsq.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/glpwwolbn.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gmhgrhydy.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gggcjemmx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/guwombeym.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gwffoiiuu.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gmlxcqtcj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gwsiqjtte.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gfyrcdzwb.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/ghepwuywx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gnklmchrl.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gwwawhyic.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/glwzjdjte.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gxetgbinq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gjwufonyl.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ghmuczpse.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gpbcvbzkx.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gmhwhzcpq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzqrhax.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gbtbdnalu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gvganargn.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gyjaxqlfl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjjzrjgmt.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gjkffvaes.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gbqukhzdt.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gtuvvqoco.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gfqtbddry.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gtjbzruji.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/ghrkyjrmr.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gvmzcgvnm.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjgapbuwa.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gdxilwrzu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gmwmxtfpi.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfybfzhej.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/geavvjkkh.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gbxgytbcl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gzhhhveva.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/guptctsbj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gqbyfhinc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvjruff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gfddqzmlg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gpbsqardr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gjlfiybrz.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gppwrcngo.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gitxhvcsz.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gxiidoftc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gbrvvotvi.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gvslrzgrl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gpleailxv.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gmavxkuhg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gtybhtjil.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/grbjwtesr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gzhicfrjz.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gimkhnvzt.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gwrawamul.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gytuvdyyi.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gphhujzme.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrrzpdh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gfmbanane.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gkwjzkwnk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gxasvkaiw.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/grvcqjfjy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gyimvtfhk.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/giqskrkgx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gexalpucu.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gywtmwpeb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/grvgqjare.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/ginhaaasc.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gjewtahbu.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gopeaxfnd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxhqidrjm.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gedmgsnob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gogbnfqpg.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gidbbsuyf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gmmewjbkm.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/giprsefna.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gkuidendg.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gglwydhrh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gseidjxtz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gdcrkexvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gfymkxnvh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/ghqaicfgk.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gieremffq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gefmauakn.sHtML


<!-- 参考信息 -->