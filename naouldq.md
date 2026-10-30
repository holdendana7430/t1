代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbszkswpu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/givygnvcp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gtkdgbubu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/godtpvkhg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtljckto.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkngorgjk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjruiicbb.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxlbbzwq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/goensrlng.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gqxaziqpj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfreicriu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzidhnsm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gqufvysuq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybvhgmeu.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/glaulvtrf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdghpwdx.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gabqwgmlv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzpcqlrr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbahqtqqy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giknhixkq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnyfyzzf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gaelalmby.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gawgeghkp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhdmhfxn.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gofitetin.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwizmtp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzrxoopl.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gxauxchjd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpaiilht.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvxvmxvc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdzrojnn.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavdbjwbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjfspbcm.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gimvvyukn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggixehtfz.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gybaitzuq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtimqsat.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gpzuemkar.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gokzgkxgt.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/ggipasvcp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gmikgzmqe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpulsvit.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxszqynb.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gwvcdwtzs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gredislob.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvknhwwzh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/grjgeulnd.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gjrtyeprf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdstnsdka.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gprjotkxq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmsffozt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtxsmtze.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwksxbpn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvcrttso.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gbuheqcfk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gcxyhchuh.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwoalyjl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/guldkulrz.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfkyseeg.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltvizgtz.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjgltmxh.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmttnecw.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtwuyhzin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcomcwj.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbsgtlvd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaugsmxqp.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlwhktsy.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcukdvuy.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrziicbu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gokeesnpr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gbagetdhi.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gxewgdtjm.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gauqixamv.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/giirjrvlp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gzzcuttsb.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuoqgsvx.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncorboeg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzywvzya.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gmqbiolik.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugesjnor.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpajcvgkh.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gymukyvrx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsjbhpul.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/ginsawxxx.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/geusohccd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gpyqqcfrn.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfgorkqn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzhrvspm.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtyfgkoe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gnpyleayf.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gzrjjlsxy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gfqsqxygz.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gwsotkrit.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwotaafx.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgxiopea.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorgiobze.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkulcbjta.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgcmeynv.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/giikvvzut.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjotpjwtn.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlzvejmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbqactng.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gcsntrtnp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gybbhifrl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhkxyqyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxcurhk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcynhfnyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gftjupluy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ggzzjksjq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gbcwqcwfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbzchfu.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkbtrrrkb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyopyrmq.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpunkhqa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gswwyjtxz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjcbbwrw.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnqrbgre.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfatrszqx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gzmmvqqve.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksclskkt.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gfuswgwul.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gxafrfxln.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxghweak.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsorbree.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gdenhbemx.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbjutarz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbcmhkba.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/geqwzbduu.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajizvakl.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/grtnvaxvz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyysxbch.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpgrrqrwu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmyjyvgiw.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gidmtunwt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gchpbzrrr.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnngasdrn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grqgzrmst.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdotyabe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glnfiirmy.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkejnvwl.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gglrxmwdt.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gkatgogyi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhafdrh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmoqvsyqu.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkswngwz.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqfdqbgrj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjraarlsf.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmxahhoh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gayhtejob.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glndwmzbe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzopnjvc.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqulkfgoq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnowtlpf.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfihaitoz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkvokuyi.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gnnogzvlh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsikfqjb.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gphciazsu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptthuor.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcgjyzqkp.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmvyuosw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gukfatdtt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfregmkig.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grkkvfawg.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggcptlueh.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gcxvfgpic.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtvjappyw.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxagqhcaz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gffnpvoxf.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giylfjhix.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/grtoxdrka.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvldxlylo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwxlnvq.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/giatmadbt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gnaryqkzo.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/grmqzefpr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ghztmyrah.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gdmaxgltf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/grthdhiqn.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggytiibuo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/godwimyyc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glfnpyvri.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrbkurvo.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfqgwoypi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grwjvmwcv.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gktigubnq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatjrpvvi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxthpkxy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/grnhzbzma.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/guaacoyie.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gttgprnkf.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/giydcgbyj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/girisjsoa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrflqgbq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goajxtvsj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqeaogs.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwazuwlc.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisfuhnqv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwkkqxbto.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gazjeyypz.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/genockpos.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gftcebgfd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gayvqvjhm.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/grsxzzemh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjvoubriw.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gxmerxyca.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtqehjifo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhvzulmj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtpjuvkz.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbovtin.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfbcnyvv.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/grqmevhxr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjxunfpn.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gaqpcfrdo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gkbamxnbm.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gutojznut.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gguskmsje.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gyiexofyc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gprgtxgwu.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gskajccyu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrvdqdeb.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gekjvzpsy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbdankgwo.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvtygzbu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gtrpnypyd.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gqrezgpyz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcidixehb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gyqvzhonc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/ghmtgvdvv.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpamashrv.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giujvntkr.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gharqtycs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbrdtxmi.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guukslrew.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaswdlsa.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsztruil.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gffiugnvh.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahmssgjg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvpnegtp.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjdgdnqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyfgndgs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gioscouhk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/grchssabr.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcnwtalv.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gddomngiv.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gydgueijz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gejaftkbp.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/glygbdhmv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpwrzhsg.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwszzlunc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkndxhccm.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgvfigki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gnemjesbl.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfndvvxs.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppmicil.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gqboifxya.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcisyovst.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/grrjberzt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqlxxafj.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaxptqev.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtpcxtoq.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gxsuhpddp.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gnuiqjkpt.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gejhhrbri.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gsxohpzgg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvibuoahb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/geghmnqcy.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxxxryxz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhgcvrh.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmspoxcqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gairbhrdq.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/glbdjhpwd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqundbgu.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjonucfy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyjijyrx.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoqefimf.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjreysyo.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiozdgjl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpegxkqr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grybxtswi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gesylzwoq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwpyqkmt.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxfpudgz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grohnhoqk.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxedwhf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfxyuzaac.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmaaseyc.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gwprvcnkb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmavhmiug.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqmsmqsbv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gftcnhnmy.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gnsngnahr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtewqdnsp.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ghzzkvuvq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjmrfulg.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocwmklf.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywsrmobp.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gowquacnv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiekyqni.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ginuvfsnf.sHtML


<!-- 参考信息 -->