代发 wailian999

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gqudkivax.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gobxltbnb.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gagporkpn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gvxjqliqs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gsmklbaqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gtwqjbeio.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gwlklyecr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/ggguqgyij.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gutqscynx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gtybquako.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gaevdbckw.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gbydyojpq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gnyqrnlxl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gmzyregxw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gtwrxtfun.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/glfipzgii.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gpemnewgq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gdtrgskgp.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gstlwmzqv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/grxxqmmpx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gtuomeypc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gntxjjnrv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtuthewhk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gyrtkqixx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gssmmuayd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/glrtdqcuj.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gmphjdyme.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzkxombd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gilkgveiw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmqicnkpz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gzhupsieh.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gdotiotnk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gxeqtotep.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gmvtjdioz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gzqupnhba.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gxafyppox.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gsclukzjp.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/guzddmmud.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gfvxwmvnm.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gzkjhordn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gopzjinai.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gwxjwljyd.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gzzlvnmbk.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gilglmmgz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/grfocgojt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gpzavkmyn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ghlzecbzd.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gpkmrnllh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqukurtrt.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gyrnqqpsd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gljszxzez.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gwmevvpjl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtnpvbjea.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gjrjycffl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gfomigaee.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gesmsrukv.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gnlpxoyuq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjhcvkuud.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gcqpbtcne.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/girzwicch.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gnjfxhkie.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gfhzheaxa.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/ggohrnvve.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gddakoptm.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gkglrofki.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gydmqtfgs.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gprsodjnt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gkjxmjtau.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gzgtqshmu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gosfvgwud.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gdknisfnk.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gpfefzyuu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gjglkuckt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gnvkdehsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gohejxukf.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gjxdgkuzo.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gizojpowx.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gfkxanute.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gssjtpkux.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gvqjgnyer.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfihbajjl.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gkrnzvovh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gajnhipiw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjabxvh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gujmimahl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gifhqithm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/guwxhhjwf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gykubftun.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gmjuulqfu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/grfmamzzf.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gbazuiucg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gdndhyldy.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gkroogese.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/guyvnttoa.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gggxjjasd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/giqieaitd.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gozaqnkcx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxsokyxwj.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gengrzjdb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/geynweclv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gmysyjxwb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsxhhtkey.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gquttxydv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grlssyumx.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gyzrwcbkk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkajdxhfc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gmchcgyrc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ggjetimpk.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gltkrabbk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gkqnppdsx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/glpghzbny.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gkqqakcra.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gttguelng.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/ghzjhmgvy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gswkqdznf.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gnswkclat.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gvsbloioj.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gtobjeljp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gsbvgczrk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gonbgngds.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gobnjpplv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdobnnwkj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gazydtarx.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gdyrhsrgf.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gbhiwgrjn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gibyieour.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gazgrtjim.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjyigwx.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/guzfuqxov.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/ghyuxpbdl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gxzmayxov.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gtkqgvzry.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gxmxghkdk.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gmokkoemf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/glflnplsm.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gftywecgo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gnphmsvvn.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gvmrmdjqn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/glgsrdnbz.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/grydernye.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gqpcxbrcw.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggsqkvsif.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/glkehtccw.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gywlginua.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gvayijmrq.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gyrtfiznh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gnwfesoeb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gurwpnwch.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/ggwzbocmr.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gxwxtggsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gpoipabso.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gfbeuailc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gfalszcam.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/ggiildehl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gcizhczqg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gceqkfujg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gbslevaai.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gjwalofax.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gjjcunwfi.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gjmtugkxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gdvdipril.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gvuesklly.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gekfvwmho.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gsslfkdcd.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gjsmtirdh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gpntxoycj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gxrfsozmh.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/geicecrte.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gcknpbbhb.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gmqkooony.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gdowytpgt.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/grtbcmedn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gmudilexm.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gqfgiqxzn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gfqkukjkz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gxzzugkum.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gwfoswxya.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gpcumrbyk.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gnmsplhue.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gpuktinxb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gesygpguw.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gblunevfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gvwfbuidj.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gmrxeuuyu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gzqkjgfuh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ghnzloezn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gztogwssc.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gtzgcuyoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/ggdrpvhjp.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gaimrvvrb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gwvmfcrnz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gdenfdpzt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gjywlrgwd.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gnyphwbnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gbfgiawhs.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gxngccfrv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gouucwbpc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gvkbqsrcs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gxnxtnnck.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gcyqmifpi.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gerzyxzyd.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gkyrwurax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gqhbyxjkk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gqkcaiknb.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gomowtagp.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gfhabzmro.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gjwrlmnhn.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gtchuvpzu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gbpjqdqib.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/glsxqzfrl.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gipftsnrz.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gduqhrbzh.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/ghwcganjr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gglsvqjgw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gsiziamag.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gknebpjfr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gvtjkwdfx.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gjfohhvkx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gjcbakbvk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gixvidmzw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gidnltmtm.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gmjttcryf.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/guglilije.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/givlenelg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gzkbsoedm.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gakzdjqms.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/glvipqdlv.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gmvmgfsff.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gtdaxmxtu.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gfqndsvny.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvhdufvxg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gbkdjqhoh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/grjougbhp.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gtrkxklca.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gvmmxtoyc.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gelupkoya.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gdguivfok.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gcsxuzzfp.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/grgptzpqc.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gqgpvsfid.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gzpqyekxs.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gvlvvefds.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/guhzfugwd.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gydonnrsm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gdppakezx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gipidkpxe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gpmgacfei.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gppgbhyxq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gymsszdgo.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gsuvbbmhl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gwatyzkgp.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gtloavyep.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/ggudcftmj.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/glmdrbydq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gpumcaych.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/geykdmlxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/ghitnhfsw.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gqedtaqxq.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gjppjffbe.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gbbxgmhjk.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gypkkbdma.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gborwomcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gwwrfbljn.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gxjcagmke.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/ggyidgqrp.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gsrgtbkcg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gexxrqhdj.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gncurywmw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/giijvlbwy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gurtvvpqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gawpyautk.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/godlzovcg.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/giidfarlx.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gdzbwwnyj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gamlymeru.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gntbbkgli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/guiaizmiz.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gjhlzqqdo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gmjllpgok.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gsfdqibwr.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gomgngjei.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gwjbufowb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gtmkyqtch.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/glkvwbkio.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gukdqxxkj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gnjjipgfz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gaqykwiad.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkrowckyd.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gueqqvdlh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gidjuiofo.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gefuedrlb.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gstxqawry.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gkmgmlvjx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpgtewbja.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gnedcuajy.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gyzggiktp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gtkjwugvm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/guwjdtwcz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gsrudzxgh.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gwyhkabpe.sHtML


<!-- 参考信息 -->