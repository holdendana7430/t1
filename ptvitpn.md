代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gqzhnbyhg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/ggghhqmug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gxssqpvou.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gyddeqpwv.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gifykiunm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/geoglujsg.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gqabyiqnj.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gfwasgbvw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gwocqpesw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gitufkxzw.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gegrpxslz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gwsxooapy.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/geldcopxa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpeqjrtjm.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gprsfqmhh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gcpaqdtbw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/ggqhecmll.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gfeuzgreb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gsqmevonf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gfwjurmyu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gwgscrmix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/guwhkabjr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/glwbqsvtu.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gfjhultzl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/giwwumkti.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gtjbbxeoo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gzmizuogq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gtzxqbklp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gfojvypmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gskmyuyoy.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gnxufghvl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gyzaozuoj.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gjfobpcqd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/ghifrfivc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gijiglrpc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gpfreiijr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gmfurmurr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/geqfzodjo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/ggrmvxzpv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gyfvdslpx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gnahmjhzf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/ggiarkazp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gxzwjawsr.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gvirqssqi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gkzafcoxl.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gsgnhqshi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gaosxtalj.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gftzacrty.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gvujsaeyb.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/grfhwtwkh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gppvbdauz.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/geccjpzxw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gksaymrur.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/glljvmvvi.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/ggxeuzyht.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gdpopiwph.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gltlwrhag.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/ggkkcstef.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gotjitwyr.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gvkzmglrm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtaldapyd.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gwyisjghu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfwdbbxht.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gormbsaoh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grczmhvrq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gszxtpvxx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/genbytazm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gricshzir.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gnnjzowqw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmxoaemag.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gfixtctcn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkdpqygky.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/guxplfrqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gsybtargd.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/goetnkecg.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gjkpirzvq.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gymuvduun.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gwqwyhjej.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gpjbhvvks.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gpkqoafpj.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gecaqdyiw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gkkzkbtvq.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/ggymuhodp.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gxwwlzupp.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gefjcpzuq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/ghfqifbro.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/garamygpz.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/guvopfxzg.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gnwxstnzs.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gygjmcpnu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/ginmdbipe.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gjrjsinlv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzlszsvri.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gttqhoyzo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gdhflrhrn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gfdfsanvt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gffzsslzd.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghmrjvxtx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gaxhoyypk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gblxqmgnf.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gcghoaugx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gcbknrsvx.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gudpupbbl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gygbzacmf.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gehpivgvm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gdvylmufc.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gjzqvfthu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gcwkahqtq.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gltgcrwmg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtxjzzggq.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gwsrudsys.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gnziubdal.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gopidfkbf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaanowtgb.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ggpzlsobg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsifnhdgl.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gdsypxlkn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/guvqwgily.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gjtnxrilx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gogqlwqeg.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/giblqsluc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gqhxeqtst.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gopqvjfwh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gwnlvawzp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gmrfmrvib.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gpazumkaz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gobhibfnr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/guvvnbxwv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gtgrccyiy.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gkvqkrepj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gnocnzwyv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdxedffrx.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gxawwfyrr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqxwwkwue.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ggwbnqxli.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gzgzegggr.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gzwrbgqad.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/ggbyanbvg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gjaopwpuc.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gnxfebnsx.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gcotojavk.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gqwnmngct.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gvnozdsmh.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/grwjlysnr.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/ghsfuocbv.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gfpmccagz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gjgofccha.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/ghivoarya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gvhwykcyb.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gslllqeuq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gskgxedff.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gsuwhslkf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gduewtiho.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gptgddadz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwltsfjlt.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gwcetaaoy.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gwocaujox.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkpucbtpy.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gsynoqwcy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/geemdpbqq.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gwtopxlhf.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gbmudthyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gweamfzrc.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gqeeaooei.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwgirzozw.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gaqfpdidm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gijsvybuc.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjogazmpf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gemnfihfm.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/guazecryn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/ggoigtlvn.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gghbfgham.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gzyabmkre.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gkjkfajlv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/goxnxtlwd.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmkzjmyuz.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gjxgsidno.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/ggwspowaw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnyeykn.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcselawtl.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gddwzwwxv.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gztupjpow.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gmdfjbwja.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdvmofxob.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/ggigdkxuy.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ggldoqtkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gsjkwrfbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/geragcbdj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gyhqatswm.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gyzahalgr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/ggmzarqir.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlnqwmq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/ggltjdclv.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gptuupgwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/glgflagbk.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gfqchraog.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gaysiexoe.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gubmawtvx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gdiijijrk.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gqzpygizk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvuvhhmu.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gfskdvsaj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gpirjhidp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gmxyluisx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gwpnczsnn.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gzmimxzio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gelosaqea.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gtdhyubtm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gjjjgdodx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gqkqhjgwl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gxfpflqsz.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gqhfrkkst.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gvcnkudbq.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gmsuskuio.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gjcwoedhd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gdwfqyezs.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gbvtkigve.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gdcxyskyt.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gpeztlqcp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/girsyhspg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyejeghpg.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gwcujkyhc.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gtvnjupsa.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/guescblvb.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gpvftvqtp.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gbmxbfcde.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gktvsujmv.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gthpiwxkf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gxjtvctzt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gxepahasz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/giopsukrb.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gzkcasnmv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnnublcyj.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gmuxiudra.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbggawzzp.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gpdqgowuu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/guggcvqng.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gdbokzxnb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghrlxeexh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gwstvbsgb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gncxlshbv.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/grdgzzzdy.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glvjcunam.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gzotuabse.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gqanqipfl.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gsvyhebqx.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gtmyojprg.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gtpmuaecn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gbkanrmji.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gnchtqqoj.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkwfztm.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gkfnmekkn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gdfcbzjon.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/glgkijskm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/geimmfnrj.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gxobkbvpb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gjghqpssl.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gvdfibpcg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gkklpfmne.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gdloqjizi.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/ghxkjnibf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gsmhbesed.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gwamnvhuw.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gcksvifiu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/grqunacbk.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gvacbqclb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gqqpjzuiq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gjqidbmhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gzclltooa.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/ggxiuscxp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/guliyhmkr.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/geeqkhpxg.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gjiuerpbe.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gtutefqwd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gezceuspx.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/glqxkxyts.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghakkbmdx.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggleuypci.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gcfnoxwfz.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvojpvlyl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gqkturume.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gbijwlpnm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/guvntexbd.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gejhyddvv.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gukinneux.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gysbammrw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gzsvwhmqg.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gkdyokgfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gzhjzhkrd.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gvfoyunsl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gxprzjdfm.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gfypnillh.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gxrsckemb.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gushsnpzw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gsyfuzzpt.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gjkwrxpyf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/geihubigc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gapgdhgqh.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gdquajyth.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmlkffalc.sHtML


<!-- 参考信息 -->