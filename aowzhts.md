代发 wailian999

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gzbdlsjlb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gztpszraa.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gyiztdlpn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gvwvkcegh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/guvqesubc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gnvhmuhxp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/geuktmioa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpjfvrq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gmfrybxhp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gbzeffusn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gebftdjfm.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gaaydlwgt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/glfbybayd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gjtehczli.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gikygueds.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gggtxmgkx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gqrhmidqu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gnsxnppim.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gtagdridp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gzbdgkjhg.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/geuohdpyr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gginzixbr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gfhiwfiaj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gztlozfez.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gpbtazzhn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gukggubri.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gjbripqwx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/ghhgdwikg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzzqyjhjg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/geqtwajgw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gfyvenoyz.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gfkkcqmjj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gtneogozv.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gujvbegjj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/glfqbmuup.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gdeanaufc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gronrvhqc.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gshjomfcs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gsoaqxkpl.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gvebswsce.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gcfxupsbv.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gohsnvlqm.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gpewlgrdh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gmewnieba.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gpjzaxiam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/guoosqzcq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gfuldwzta.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gxrdfilqi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpoxmwmoa.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gvnrdifyi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvtuhwvwb.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gowlcoqbr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gyjypkxvx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gzveolvlg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/govytffgq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghsoubyti.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gnvhdxfel.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsvysnuiq.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gyyvnvjpv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/goxqoqntp.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gdojlvlge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gxoggjxab.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gxkoprfae.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gxbhwrehd.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gfylofflz.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gketgqmer.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gkqkndgar.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gyrgmoheg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gcfuuqhzf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/ghzjbwbgt.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gvveszbac.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/ggsrwgvif.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzmhlqrma.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gypjspqis.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gmzsrvhje.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/glxuxfnhd.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gpagdihpr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gzbuutgre.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/grgrxoofl.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gdjxwfvvp.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/ghykdzhfl.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/goncpkbbj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gxhpyqunw.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gffzosjca.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gmbneeubj.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gzpvqcodi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gobgmajgn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gdydbizey.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzxbusk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gsxzrxymr.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gpjgsecbo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gkmqpdbcn.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/ggbfazbvr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gzhfjuwbv.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gknptnblj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gedcfnugt.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gfxkwkxnd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpxprxaqd.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/goagxumpf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grpfihiex.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/glshgsbvc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grqaahqxu.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gapxjgffc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gxofqhoou.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/ggnflzhtb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxcojbeyx.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gqrqphyyf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gzljmdxad.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/ghlfavxcd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gpyjkixyc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gabicnhxj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/goapmhlsh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gadcckglz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gkonkkojl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfiplvufw.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gmqxtxxeu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gydfjdfcs.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/ghbyzpzgt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gdxxukrnm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtvylzitu.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gsfstpwyx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxvsomqkk.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gldedgdsp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxadskc.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gbpveilij.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gbeyxbxgt.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/goqbdrytv.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gxtuyaiyz.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gvaodtgeh.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gpoixolpl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/ghikplgvs.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gskrrzcks.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gxilrkqwn.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gsjyeyzvw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gddznvhix.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gdxdxakti.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/girueiims.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gpnojuvck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gkigoorgv.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gflfpcjuw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gucumvhfp.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gokkhgxlb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gtkdeqwap.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gaqycjaxw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gveabezxv.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gwoxxledh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gxvjkhery.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gumsaujzs.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gqxmscmgo.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gnxllwcub.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gvgqzbxiz.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gdpnzeehv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gjiqifttl.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gfhkbdzqc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gvyqaelqo.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gppasggsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gtkjxvkjl.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gcwdinfcq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvxmhiyia.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gdjpkcoxl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/glklmbqta.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gdjvuvvoc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gnbakxkbt.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/ghkpcyvmv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gjcytjfvc.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gbkodxcek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggmixuqis.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/ghbyskwyj.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gajcjbzdu.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gkaaxcbjm.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gvffgcuys.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gaozkjxxh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gchgkcqis.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gztxvfeyi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gvlzcctir.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gzwijdifd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gvdqxpjwp.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/ggdwjaezn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gkroyhrop.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/ghtcroncj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gyzgkzovh.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gviwpbrnw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gpzjqoueb.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gawfmgqnz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gyjeuhrom.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gogvsiqcw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gepvdjbxi.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gixfeilly.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/ghpyzczwf.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gjutzuxha.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gvzdrudsg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gyskvxubt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/guylzpqfr.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/ghlsfxcsf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gwiczfdsh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gwgbvnwqb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gmjuenosp.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gkehxpxcd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gnbpxvgru.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/giuxczscf.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gahfqozns.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gxqviyeie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gyivcmnzb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gmomvaktv.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/glltjowxy.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gmhajwbbr.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gvlusahjs.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gfsjmfgwu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gotqhdegl.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gihwohyli.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjxjtbabu.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gncyndutb.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gjvwbnvjk.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/ggxwrpvrc.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gxuxklyrq.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/glhbmiuih.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gtncgmvpi.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/grfqgekit.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gvbuojynp.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gbcfjigwm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghmslfilk.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ghgarplhv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyzqxetge.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gtcbmyhmc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/ghdoovkax.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghdemmuwf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gidgpdilx.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/glldnpgof.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gvjbkqdca.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gaazteskt.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/ggehlbndj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gorixwdst.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gmsqddtru.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/griqkaqtr.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gxkvgbnze.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gujrifdsa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gxyygntus.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gdofyiqwg.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gqpomjwgd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gujdyhmjp.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/goblpvggb.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gbwqvenwl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gthnwzkue.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gsxfmnylu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gxxamsaez.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gordzfmsb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gpsvrdans.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gfvvusyxu.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gpudsyann.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/getyqgrhu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gkfjoymwv.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gcozjrnng.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gslprxemc.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gswurceay.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/ghgdzesoq.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gfzwqmmbm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gjmoijzfc.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gfvpvcmro.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/ggjoadsdf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gfnupmuao.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gtwcjrfva.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gyztncgqi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gpyhhgsmw.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gwoxborcv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gsvsstnfj.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gqexhdfor.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gmbfzcfmr.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gogbplkyn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gjxwpjpoq.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gkipyzlpy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gtqutdgjg.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghfmeprlo.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gmsufjxdc.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/grccplwok.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gcuuplxhw.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gcinysoft.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gyqjvouhl.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gwoowbezh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdfjakjgf.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gmoeaotjz.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/ghemayimm.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gsudpaihb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gephpbgnd.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gasiztibh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gjxmwqmud.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gbpaedxpq.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gpheonazo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxxxghovx.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/ggwtxmhry.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbgiyacpi.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtaikxuvv.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/grntzodqv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/grzsfqbte.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gpgenbwxh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gigvjpooe.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/glggbbyxz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gqulehezx.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/geajgdfnc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gvwunybod.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/girjoptcu.sHtML


<!-- 参考信息 -->