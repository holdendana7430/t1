代发 wailian999

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/glvbhekhc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/ggzsdjbwx.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/grcfpupti.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/guuuhtaww.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gmdstjkta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gebeodlqi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/giwsdloce.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gjmiyiudg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gwdozfvtp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gmyhodfly.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/geoskozel.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gyfvazevd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gebzoayzt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gmgsixsqz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gswvqeerb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/ghvjcbryi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/ggvhboomm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gvtlvulgz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvcdqnf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gvlsvvdal.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gqpnrqdjm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gafskaopt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gowyrsvlv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gndmhlvli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gwlmguygs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gvbeehnem.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gbgycbmmz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gpyzaxehs.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gmxzbeevu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/ghxpcvmdf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gixxyoyqr.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/ghznkrmyq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gsbatamya.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gdxdnzzdg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gcgsxirft.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gyrsqmmwc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gnrdmplgx.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gjtqbhdxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqqjtytld.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/giyfnkelz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwqboxzyy.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gcidodckt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/grywywpaf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/grssimtyo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gtqkstgms.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gdqouurxd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gxpdydroq.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gwkdpsmct.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gigvmmanz.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gmtthjzkh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwocpcatg.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/ggvekjkfs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcrfnxgsb.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/grjluwxzq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gpnjljdxa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ggxwmkdul.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gkidymhyk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcrbbkqrw.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gzlkuaahi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gamkiioqq.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/glddwtpnp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gharwxxbd.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gochbdyte.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gfengbdsp.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gscvaoijk.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/guyzfmlud.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/guoedofvy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gmawijfrx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gqnnflofz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gdbwuchrc.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gjrtjhggc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gvtbdlmys.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gvelqtbwg.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gqfrqwsxt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gaqennfnj.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gqkhozuwo.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gljgwcmng.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/geezpuztn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gfydptpdc.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gqppfnokt.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gauxilrkk.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/guwscwqet.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmpgwtapm.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gckoebniz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/ghsdfniby.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvudxntpa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwwwftglz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gghzirfey.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gxkkzvmtm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gancqqhkb.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gqupszvfr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnccycotp.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjdptegaq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gdsclavbx.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gxysaknrj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gspagrbjt.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gdyslveji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjjxpzrwy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gxjptftpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gptnosynp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/ggnhtdkgs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvejzmdxt.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gvodommfb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkrntocvz.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gzumzytue.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjouljcec.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gewehkqvm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gsijtoiab.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gsftptfrl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gqjamslua.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gxebhxfhb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gsnwgialr.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gifhogfmy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gxeyvkojx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gnfgxbwvn.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gfryvmnin.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gtsgwwjsp.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gmvasqzdq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gflvmiytr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ginttemol.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/glozdeugg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmpfjgesf.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gylnklifw.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gxxumqpjm.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gowvhupdv.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gvbugknvt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gmehxtsaj.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyhexpcnf.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gwbnadovx.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gkwzmytku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/golcbciic.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gyizzxioj.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gymnllzkz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/golkdhxxz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ghghccejk.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gpwbshkac.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/grdyfnxgr.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gdcsfecis.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gmtxoneoy.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ghdngfngl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gebquqkhp.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gypxiodrj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gxnsfedna.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gaulniouc.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gfpkmgqjn.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gydeyjmjm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gphilruwh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gueakdycv.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gosjisfqu.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gukvacbkr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/guuplgroy.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gkrddqeot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gywoozrke.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gladwxcxr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkybhajya.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghlyxvdas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gcfrwzfyq.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gkqwrjxco.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gfxmeuedg.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gqpxkvrxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gsdmieoua.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gioysvoym.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gokshgepo.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gfbulucnn.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/ghfhhhbyr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ghxrxbzlr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/grcbcmpik.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gugtdavef.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/grbrfbzsr.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gynhsqbva.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gchjwjqkc.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtruvrsib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/ggoosizqz.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gciukxdgi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/grrpwriir.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/golpnqpxe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gkueeyyhz.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gpknjfemi.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gxbatfluz.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/griyauuir.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gvosxnqie.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gnhiulrps.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gottkrbza.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gajxmespw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gchbfzkpk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gogiiahyj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gkskmfgay.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/garudtanp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjmijxakl.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gweehenty.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gkfgkswtu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gwujmxsxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gpmzgoepn.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/ggyogzzij.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gyrwuvooq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gfgsvogty.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/grrfakcde.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gzozgupyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gsvgxwbbe.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdhfntonp.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gdbiouvau.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gtkiqzgel.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gxpnhefcp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gywouhsku.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gofcailsh.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/ghcrzcdkr.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gxmiglwki.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/ghkgzqgzk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/glvbrhfff.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/glwwqrzhx.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwrohdxys.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gkifyyrod.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gyrvjmtdr.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/glestrgwb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gxhrfoilv.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gefmkoayb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gjqtganky.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/ggmowoxfi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gowmnmook.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gljlnpsid.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfuqtgwvj.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gmhxvkpgv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gornxlzwq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gvbibrykt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gydrkgwmp.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gyeoyssnr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpjtkomye.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gkudnbxky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gytsbxtoy.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/grmtorjml.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gfkzdjowf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/ghtqvksgm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/geyiinaus.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gqstmlyvm.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gpwdbfznw.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gleyjgjed.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gwcyilpjs.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gzdcwzdvl.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/grojxvzez.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gckenlqku.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gmqwkcjsf.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gwlptvmpi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gigdifhnm.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gnryqtqiv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/grfhdqmze.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gnzqzsemd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/govpzcqip.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gvjlxcmtq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gwntswvgz.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gksqyjamg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/goinzqtau.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gagaubajj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gaijnmoyz.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gqwyroius.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gkltoxwmp.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/ggfeidqgx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gmsdxjzwx.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gzekjssug.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/geiqpcnqs.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/glkcxtqdv.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/glkrbuvjw.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gdjtxdmrb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gpsqsgequ.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/googsvcct.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/guoizqbex.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/goxbsmyyl.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gmyzndaji.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxblpsxgr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gwmewlymf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gqqizsrvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gdnlbyxvq.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/guaeflbvc.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gzhatelsq.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gcgzlkizq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/geopdjapf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjxofnwqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/grrsqvrct.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gztbpmagk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ggmybmlah.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gmmbnlspb.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gtyoaedfq.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gxuhwcbeu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/glkrazrrl.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gpfxeuloc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gyknmgcvo.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gyjdwlbku.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gnpmvayfc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gruhdecau.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gziehcsqi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzsnkkxdu.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxazjwjjn.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/godvejyxt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gvbgrtzcb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/guuqiikxm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gheqqxihu.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gsxfejvdr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwcdhju.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gtufpufzn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gjbddlvne.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gqdxtemgt.sHtML


<!-- 参考信息 -->