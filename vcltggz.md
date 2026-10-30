代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gsigrpihj.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gwawqhmso.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gqwjxhrmm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/goestzdfb.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gmfirvisf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gumgmqnmy.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gldzfthxx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gurvqlzsa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gbrtnqjak.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gcunknmlj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gxlkjufzh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/ggecapmtd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gjqzsszkn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gankxpxrg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gayjqdhzh.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gopswwmtl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gkzmazqvg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gonmgpcvv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/ghdnbdsjj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/grwiondlw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gukyhzyvd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gbolyucgw.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gpltqxhro.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gplphuabi.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gmsslnsbq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gmtacnfva.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gkooselqy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/grchicsbk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gajvtmnys.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gaxukcboo.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gflklygka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gfsbomash.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gfqwhxopl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/ggskvxrfg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gmztyksei.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gmwpuzluu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gkurydowx.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gwpjxmrfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/getptdswe.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gzihrqmho.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gjgputucy.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/guhrxxgeg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gjhqbvwjk.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gvglhdoxn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/grjgwlwkm.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gakzjqlxv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gviuicfpa.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gualqaeax.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gisyxepcu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/goxryhywy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gdnjxbzqm.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/glpsxwfgt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/goqbekzzt.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gurtjyefx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glmwiwxqh.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/garahfilw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gljyzlmnd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gzbcsfqfg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gdxfeokrr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gaosjhpip.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gugksmlji.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjbryolus.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/ggmsjxdld.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvkwtwz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/grvemfdkn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gprkezkbg.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gtaqdwxue.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gvdngbisa.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gyvlpouir.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gywhqsewe.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gbqdtbtmh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/glsebtmnv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gihhncpmi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gkyyaqxmt.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gxjnnyvnc.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gpdwzdpxw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gitqruhiy.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gftsezpcu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gftacncoq.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gbzckpiyw.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/glvidjgyd.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gqnxcitew.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/grvrgxgbj.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gryoeayky.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjndkkzzv.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gvkehqxxp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gxaannrnd.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gjxtmarsy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gisetnqvr.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gboyipyms.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvelkwpmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gmihlabnf.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gdanpuesz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gwhpeznqf.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gzfsltjrm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gosyzcwpc.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gwooilpvk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gaasfcjci.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/guatvfjkc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gdizagiqx.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/grmaguyue.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gemdindmu.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gdmeoadnw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gvykrzday.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/garkwkkau.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcjvfkunv.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gklctuwaw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnopsdtvz.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gvtcojxmr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsiuphrun.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gwdncldcv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gslwumikg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gkczcphsr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/goqlcxonj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gnpbhdjbw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gejxqlxlv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gglctzadg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gyxorytsm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/glpvcghwi.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gdxaaqisw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gaxyzxsac.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gshcgtohu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gqimmddpt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grhwxixqd.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gsfkxrenc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giysmoror.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gldnyacbh.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gjhhsadua.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/glmpzonju.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gamyshfbi.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gqtowdasa.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gpjuwdqqn.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gmipeevil.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gyspkkzzf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gdwupwjxz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/glvprymhu.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/giumrvkwg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gtwlhrniz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gterkccmu.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/ggfyuzfsc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gfsapfrty.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gpculkzxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/grmvmjulz.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/grpdyhvxe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjjcgeboe.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gkvuhbize.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqfobrsku.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gzzemjdnl.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gjdfdljpw.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ggbhzcqym.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrwozopt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gfitfngvs.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gebuhiwcl.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gwijfjryc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gtqffunra.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/ghvdjtaul.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gbscxzyjt.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gkwvgtzyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ghqdpylwb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/givqnmfrs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gjbpuzinr.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gwwhsbguz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvqhlkxeq.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/ggjmnyawa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gsgqedddf.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gqzibpdfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gmxyrvqgn.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gxnwoiehh.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gottinbun.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gggadlfbr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gtujjdmcv.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gxmfyrrdy.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gmdlucolm.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gdbjauulr.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/ghbqoerrz.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gfhrhwxoy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/godemoyod.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghkxfmpmz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/grzihrvkd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/ghheqrxeh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gcvvhmeuo.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gczhivmcw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gnhnbilid.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gzggcvwnl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gzbgifxcx.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gvlbflwlo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gqsipvjum.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gksviksia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gvjjsheah.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gzcorcgdj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gtaoqhbqc.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gdvhsyjqr.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gfggxhupb.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gdkpnaqry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gdascfoyx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gyipwxpkf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gmfixsdlt.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gamcrhwey.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gqasobikx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gwayqtkgm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gbwuawfbc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gyfbxrxpa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/giwxixzrm.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/giyhjklev.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/guazvzaej.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gsihjfnme.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/ggfzttelf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gsleozzel.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gmyupbxaa.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gorxgfhvl.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gcqblmkze.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/geiisgxat.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gixpkkkdi.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gkplpzymo.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gwgqwufua.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gheewyyzo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gaosgofvd.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gpaocxbnb.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gkuplrogv.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gitkapibp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gitxodecf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/glowlaceb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gthfjfvug.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gvknyzrol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gzeiswhra.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gstjzwjnm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gnhxomejn.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/giidydysk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gdydusjcf.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gsqgaphoi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gkapzpjlo.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gsvcxhtsj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/ghdahugun.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gkbglfxxl.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghtnatglx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gsftwcmkk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gplyokgyj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gdizaomzt.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gzbhbcbga.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gncvmnwdo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gzxqfqdpk.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gbjenuxss.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gnhmkphbn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/ghehrqebr.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gjgzsdeyw.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gapbcvoxi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/grbleevzh.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gybkldtvh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gabiesebl.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/ggfyhelef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gbhevlxaa.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gxctavwyz.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gpkmersrb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gbkxarwxx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/ggalfbqjy.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gwbahuooa.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/glreiydjn.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gniauyrur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gyzjkcfan.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gpcfqjqpt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gphoeycmz.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/giyobghux.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gshhrnncl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/goekzzgom.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gkivbqwdl.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gbcsspeet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gykfmzkxx.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gndgjfpiu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gqletezhp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gskzgfkra.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gwltycqxq.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwpmcnyen.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gyzyeklef.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/grcgotwdn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gjguxpmlu.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gnbouugsg.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gnjqvzyjh.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gcrnyamjw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gbtsktvyt.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gxctkbmjr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gjugprcbb.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gfhkyitmc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gxfeximeh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gbnxmzrew.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gnmahdgsx.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gwbyzrprs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gbbqegxfl.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gpziqjblz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gfeklxpno.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gapgvbvvn.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gvtcvgjfa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gezfggsza.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/grtbcbusl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdialpmpu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyqrcdaox.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gpgataelb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gwfarrkdl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/ghspbpjqv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gtrrykiuh.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gkrigeqip.sHtML


<!-- 参考信息 -->