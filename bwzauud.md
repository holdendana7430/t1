代发 wailian999

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/guuwqejcg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gosaiaqmt.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gtetxivvv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gmatdxcvr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gxryrmsho.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gerdsjkim.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gygjldxbq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gzypgoxzy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gtvanwhdd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gldgucsvx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gxhtmqmfz.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gbovihimk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gxkwjlbzj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gjfozhmgv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gofgtzpel.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gjcwmpfsj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbrbcjnxj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gbxlgdycp.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gyekjsqzt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gwxrlarjp.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gcexazvvq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/ghzpduvbf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/geencxohh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gjgwfltea.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gmenqeffi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gfyqfkysr.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gpgsaujvz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzbmtzva.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/grsxkbdnb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gtkizibkg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gulvkptby.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gypjyeocy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gogthhrqr.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gczvewzec.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gmofmzkat.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ghhitihzk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gndtwzmgy.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/govqvmsho.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gkpqtuwjm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gtwrblizz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gbhktwxms.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/ggvikhccy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/ghgwrmpvl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxdgjejla.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gjkymiigz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/giniqlchj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gnwiimhmj.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gnxxilfdt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gnblmyoiz.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gqphshvfm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gsoszlerb.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/grhmhheyc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gywdyaose.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gbjbutrph.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gwvjbhgpc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbapwhhrl.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gxbvqpoep.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnppoqdyf.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/goobpzzwr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gypxkvbqh.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gvkhcsdwh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/ghixrskcg.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gpxasikqm.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gimpnlftn.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gcadbsqaq.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gggcronwk.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gpgcsnnhk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gdyautyzi.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gmvtnnpbe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gsnzprcga.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gcxtalrjt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gnvvrochk.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ggehpfqat.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gcdzqxjrp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gggbtdxhz.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gfuirvvdg.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/glmyfbkhe.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gactklvyw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gsiojmjfx.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gdoppxnkq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdcitabxy.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gchdbhmxn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gatwlnetz.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/grbsjeiiy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gmrnmkkiz.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gxjjfiixz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdxvjxeuk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gbehiasig.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gazdrbfqk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gpgtgzyey.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gkjovdfwm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gghqjfcye.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gaonpbkte.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gsjcdybvp.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gmyswqsww.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gpakfnvjo.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gdfpjxbwu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guvtgphsp.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gztmwpbmg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gtqpievzt.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gglujhyyr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpkefbjqt.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gydhmdimr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gshmsyfjj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gesbamobb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyeejbktb.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/glbocwxhe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gxtjhrkrb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gneagfccj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gkmnjtokw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/ggpzvqqya.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gtazhhgis.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gtaflukpz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gebgoqmvk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjekrhrcc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/ggdczxqot.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gefxdgvdc.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gkeitkitf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gqxpkeixq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdrqzxnju.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gihahlzvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gngqselgd.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gzncxjqzu.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/grodqhnrc.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gtlodrdyp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/glekuhycs.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gsbtjnnoh.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gaytsemat.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/goqvuqoko.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gtrclqwmh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gwaotlbvv.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gxfckixfy.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gpwrbarru.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gktbhrlcc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gbrmguirs.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gkntmdodx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwupnosjz.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/goxlfwiqw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/ghrdfxiou.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghbojmvtb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/genowsmel.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/glztnfnad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gwtgcyubb.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gunudoqzs.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gvelwcbbr.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gujbicadf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gaegouakp.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gdauqoxjk.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gkpguocom.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gwiwtkwbg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gibsvtykg.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/guexlaigp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gutqxocyu.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/grdlbaqwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/guyymgpel.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbirbwvca.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkriebarr.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gofdqtgbb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/goghhpykd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gjpmwhuux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gmwiekknd.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/girixqrgh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gozjualal.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/glacvcoga.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gruaeraue.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gtgsexsrp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gldwkzmnp.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gltecgrok.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gthsmhgzu.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/grepkiupx.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gucjfhhsy.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxxfshcwz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gocgskbwa.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghmnxpxyh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gyxgwliry.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/grxcwkgzc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gbtyubskr.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gmoxejwje.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gtcyettnm.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gccuanwst.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gfxzaxxrf.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gbhhhwaxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gxwkvkzzu.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/goigshozw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gngwavksd.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gunsacwpg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gxsdeblbm.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gihrcjkus.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gyhnavydj.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gevemmvwy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gmdakpfsc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gobhxturf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gkzxmqyys.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gpxxjgqhk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gjoahnzoo.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gmjjjrqtp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gyvqshhty.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gygxplejb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gjybgaumv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gplbdafxl.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/ggncvcpeo.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gvoamzcuz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfsbmbaly.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gmxbxaalx.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gnvnzsyir.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gbewoncpa.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gccbxvjpe.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gicyygevi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gwcphhvwe.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gkcupcsdv.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gupjpxaey.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gmaskbmpo.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gyylklxlc.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/ghnadbhew.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gkpxrwrgv.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gknxapila.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/glwkfsmoi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gqawbfbtk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gsljlpwfl.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gleapfhit.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxwanzbsp.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/guqyeduzr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfsnhlnpu.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gqaoboowt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gjkqtyhpe.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/ghwuyiebl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/glijdzeod.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gsjbutwag.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gzerszusb.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gysokyrnc.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/ghjtggmli.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/ghqqiotmv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gxfcqmiak.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gvdafaips.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gmnqetsuo.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gltcbroum.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gimnajnco.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gdvimmdqo.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gutqhhnqa.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjpilsnxw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gxvhiiput.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/ghzbracsz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gxbcqwohi.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gsdjowocr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gzoyoehkf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghhoakptl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gkewbfdvo.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gwuzsfutg.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/glwvbpdaq.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gdadksnrg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gwkjebcdm.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/ggmaitbnh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gslsvqgfr.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gohsdljur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gfourdxkh.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/goeoeplqs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/godxanrgr.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gbvlynsjw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gwiwccpop.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gfgjobojn.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gtpwmmjpv.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/glqolilrl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gpntuzmtj.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gxoplitqd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/guexgwcjg.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gwkxeioeh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gbiykddvy.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gxhhovchj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gskfmsqyq.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gvowicurn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gohcexhws.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gkwrxbhdz.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gacqvxobx.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gtfgxxyew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gwvfxyjkh.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gegmmzeea.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gnikmubuw.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/glmjzaclg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnuvazhte.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gjyohvxos.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gfqmejtgo.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gfknchgzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/giiyfivai.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gugdmclhd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/glonlpjwl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gimrogsbl.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gmrtqpohp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwabaaung.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/ggecfflzb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxqklospw.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gukggcfqg.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gzgtmtlvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gowuxxknt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gwkswocfs.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gwjfurcly.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gxcqcknbt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gbzgsxjho.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gblodznfa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpmtzntjc.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjcxvwtpm.sHtML


<!-- 参考信息 -->