代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gbxoxwqcz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gvcofkgdf.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gqjtmguna.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gsdabihmd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gkuvlniep.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/goufmobxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhbrlop.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/ggndvjlil.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gszlyjldk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/ggxmwuyfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/guhmdzsbc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gpuckbnlb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gsyssbovy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwfngwk.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/geeafipyg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gtybatwpx.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/glckzborf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/ghxcnzjux.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/grzytuwhv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gghmfquqy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gfltfunkg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvuheiniy.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gkspzfzqm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gfwdggbus.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwlglegzf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/ggeyjrkka.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gnxgaaesh.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gtjzjfcmi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/grzdjclez.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gstpppnyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gihgxnkyw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gbobnrdir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gvkdegycl.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gsveitqzo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grhamsyle.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gwbxbbeac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/guagyylbj.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gflyhaaax.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gfbpjsvxc.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gwnygltok.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/glvttwsaa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gjxaqahxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gilrrxndv.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/giwekrmfr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghlezazfy.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gyhbzywgs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqzbslrif.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/glvjfeumo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdbzuwntt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gocoptoju.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gipvbtkkk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxjmmucnf.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gecsqxgdz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvaxdcdgf.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gvwbgtzgh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghvpdrshf.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/goyhlpwus.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gsnzwrwpf.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gdqntpegw.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gcojyaewf.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gkinoyhll.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/giqwzgqzo.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/girrqwvwi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/godaedinh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/giwghgcad.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gdttxvggk.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gjdodlvtd.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gkfydjpdn.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gjwtrthgm.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/guovvntmk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gjowviezh.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/ggxjpgvxt.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gilifdesg.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/ghgsflwaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gwimuqzct.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/grpaxfcau.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvirglepx.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/givjkabuv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gdtbouiup.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gsowntgzj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ghuvxcbou.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gqevqlyvv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpyniufva.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/goavydktq.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/glepxxfuq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/grmgtpnek.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/griuoqvpu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gtianwukt.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gxxfwrgpc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gjurbzutn.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gpticmjzy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gkwkvrhoq.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/geizcpsoc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkaaotfej.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ghgmfkhxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gozsflnxp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/ghhmzjydk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqkqkvqph.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gvonltxuy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giakcbhmr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gkfbrflne.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/goqnwrurr.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gwsknhmvj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gajycpjqc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gyvobuzfg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gwhdbnuxe.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gydgefiba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gykfqoaqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gevvacuum.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gnljxonvi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gjgrxoige.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gflkeueiu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/grkkpetof.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gfppzgcxu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gifnsrqlt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxsmpktdc.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gagcirvik.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxwdjarls.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/glmtmomck.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gpjlqjrpl.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gzjmkjdun.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/glexqsvay.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gcwmhaizx.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/giorhhuxb.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gjuybsret.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gpyzzmkdi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gzmozwzjd.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gqpuqhpae.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gkwxingfi.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gklwbenfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gvhdmpxbp.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gxwpjqtsn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gkxlkaqhb.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/ghryixxbs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gxsmqcohv.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gqhahaahe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/glivxqkew.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gphfyzyik.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/guwpbctya.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gmglsbide.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/grrooejnb.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gxofoxtgu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjtzeiuwg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/grbwtjuwn.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gfqfydfnh.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gpntqxhdu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gonsjbkhk.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/ggzyeftuz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gxeogckvt.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gkutfsmob.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/giygreeeq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ghstsktbp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gelxkyfhh.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gsrufhjvk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gkarrehjs.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gnrdyvlzv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gempvofqp.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gvtwbwqpq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gfexjflln.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gajazglav.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gamkydcyp.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gybqaflyr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gflvjhmwx.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gneiwluje.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gcbchbdfe.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gkgwkengh.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gvwbmgmet.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gwazvfrzt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gqcrhvfeh.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gypzhhkjt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gppojjund.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gnxtypnnv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gzshzfqza.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gmhwexrno.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/grmmcyqcp.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gsuvpiqso.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gdpzbokan.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gpgaeivio.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gbqqtmwxq.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gamlzysid.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpfauupav.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gssbnxjgf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gfxydprup.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gzxxcsgzi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gkmahtvlo.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gnuyzqcie.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjkhwdtqf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gowsvahwm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gcxkcsisi.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gfkptnqpg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gzzapdjjo.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gtixmbjta.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gdflpzayp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gxnovqdft.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/graufvaoe.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gkroayacx.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gjxzfgwhu.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gmvxdsvyl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gpftxbfvl.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gzbjkhjyv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gdysqtwcq.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gxowiwfih.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gragxvgpm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gllutligk.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtpanpfuk.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gnuduaecx.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnzueafxk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gcxhgjrvo.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gdjsifovp.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gognbvmye.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grersxcqs.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gasanayyu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/ggtceffnj.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/glsbalxiz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gnbgfpjpq.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gialfyofg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggohsfjft.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gqujndtqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqqsgozvz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/geyicnjvn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gcbdymifm.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gobipezeo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gecvsepfi.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/grwkqhghu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gxlggkbwa.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gamxrzlim.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtmixytat.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/grpmyozlv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gxaqlavhm.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gldwjuedi.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gfdeabzlx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gmaftipvi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/givclptrw.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjowefvlb.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gofrybklx.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gqmlzlvmv.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gwxhmiwbh.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gmrnkzxle.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gnvxqfhvr.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gqrwkqlsj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gyoaedwnn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gkdskfglg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gfatvuhje.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gmymqwpdv.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/giwbumbpp.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/ginilhxns.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gbycmnktw.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gyyogfews.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gbhdaalkw.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gntcybaie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gdyhyijzj.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gpvxtrywc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gxnrklhms.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gbfqpyuff.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gkrbepqrl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gstbvisir.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/ghwqxdnrh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gdufqexxt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gqabkdozo.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gillvyoik.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gbdxfznom.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/ghozhajyz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gskxdeore.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghcnwdmra.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gbqfvdsck.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gwzcjelmx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gncldkzkm.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gtyefsvxj.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/glksdoram.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/grtibudxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gzoqffyjj.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gcclfqulo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbmzeein.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/ghsudlfqa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ggmjivjtf.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gjooyjecx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gibftuafu.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gsuuviogw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gqotzfpxx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gctjnoylp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/ghdnyvegg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/ggudzthtg.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/govdylvkl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gepwcmvcd.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/giqqumuvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtpkciwri.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjayudwww.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gxlzuavvs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gacmfithf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gmflozqsm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gxptsmidr.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/ghdxnncox.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gnfvgswol.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gwteawswf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/glwdlqkml.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrjinjk.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gvvuuazme.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ginichnie.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gltnarfwo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ghmioblnw.sHtML


<!-- 参考信息 -->