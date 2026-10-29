代发 wailian999

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/glyjtfapy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gpqpgdcbb.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/givrumnaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gybuzoacq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gtitgqgxd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gntybiqif.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/giubvidba.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gdfjzwgjv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/ghvnqcehg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/grlvmgxge.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gkujqikep.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gomgxznpw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gjblflosb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/grjmjbnit.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gppinhuqg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gtudlkrth.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gjjazxjtn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gzutlqrmd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/grxdhqmzw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gvfugmiar.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/goshlruux.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gmhxwgevu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gtotsnroe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gutfgqdkc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/ghbaupisq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gxbwicwbk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gyzoqiujt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gvsgdkdut.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gyypppher.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/goyhelxeq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gobneftbh.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gfcyzbbsa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdzfbjyfu.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gowrifark.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/glujiehah.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/ggsaguotw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gupvrpaai.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gelbpmomz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ghnbvdfup.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gfokhznao.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gfkqimcfi.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/giddostpn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gtlimttth.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gubzduoyk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gokmiwehb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gkytzeqoa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/grmhofduf.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gkkxpfptn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkgfjvwlo.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gtgheovma.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gcnewwkmr.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gimbzfdyt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gukqjbrwm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gunxfjuft.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gqugyiqfg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gchvojfig.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gkcrkztaz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/goqovyeln.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gwhnymoqi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gyaffyrdu.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/ggcxaijdi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gbpsczmon.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/grudasuin.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gqimaenvf.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gpnkhrhuo.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gsxgdjwui.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/grddinvpd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gitouoipn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gfbykntsh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gpxuvgrnu.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gsnzzvpfm.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gwxguevac.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/ghpldeudi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gpvoggsgt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gjncdapkb.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gyurvsnib.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gzploqruc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gycsetjbh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/ggyoflenx.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/grqtbkldp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/godbsxckr.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gromutddg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gxhxyzxtv.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/ghrbxgwkq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/glezhwvzv.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gchbqqgsv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqscznunb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gpdxtdgty.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/glsoihddd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gxfxhjabk.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/guygytaef.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gkzrauipt.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gztxxwitl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/ggqedxcws.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gpfiemkel.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgbmpql.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gtefmieqx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvhvtekkj.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gyuuvzikk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpiqfnilb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gijrqdgou.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/giexufkqe.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/goytlmiil.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsmnfxljx.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gnrzieoss.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdqnycdvm.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gebsbuiux.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gldqzlkum.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gkjdgrafi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gpsbymgrz.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gpxhezgvd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gigcxhdvq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gphvqluwy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gwguasbzz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghkhzqgyb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjtdnotuu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/guswyajce.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gzshaymdh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gsqopycrt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gunhpliqd.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gjuxpzdgk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvxaztpfu.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gcpiwcfuw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gougyclqf.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/guntcgbwu.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/grajuzeib.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gpczxvkkj.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gsjvpmqra.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gsecdqmzg.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gdjuirjdi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gbueeeotv.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gqwhgwafy.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gsrpegfpw.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gsxhtsrbk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/guznvaigu.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gvrxezjfo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gspnfgain.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gtbwzuuug.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/glhpvohnw.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjvyubmqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gsgkgtaku.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gfwmlqqhm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqgspinlh.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gwjpiwzjf.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ggqjrwmry.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggvmgeupu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gkmxfdhnp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gclztxhjl.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ggbbbgmze.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gzmghcdlo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gfeqbhbya.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/glxfgqhck.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/grhcgevcf.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gzvauxbob.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gcxopehyz.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gnffqhkyh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/givhizyzx.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gkolridko.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gnvfmwkhe.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gqozdptlv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/guffcxscf.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gjndsaago.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gylnkcgcy.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ghwlpwekx.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gsuovyjeh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gncvmyyxz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/govdbhide.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gsbzcimoc.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/glvnysjkn.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gdytptwfz.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gvidrutjf.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gvdwgqgyp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gzfsuqdar.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/glsvxjfpn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gowuruekm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gjydalmti.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gpbitmuhh.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gjxaftbde.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gcxsooorn.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gloyzeius.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/ggdhlnwsz.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gopdvsvko.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/grgeskliy.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmehjpxts.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gaxcousac.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gnwravbqa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gxwfyifpi.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gridlxvxf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gqitkxnnx.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gxltqheqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gjpnxkagc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gvqrypwfb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gcjxkftai.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/givkrwrvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gshcjzuur.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gtrnibrvz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/ghmgisdhm.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gmuyninnu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/ggzenwyso.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gujhmtqph.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gwgtmlgho.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gjhrvtttf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gasspfsuw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gtinbxhfl.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/girbpxfwa.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gjvewrqoa.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gkapttpxq.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gtmksnejb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/grjkvqycd.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/grctmjosc.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxezpbgor.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gqjdgihoa.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gizhyazln.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gwnivwtiy.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ghqlrvdqm.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/ghdshvhka.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gpoqvorqe.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gfetxngsx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gvtqgadvq.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gbnjeyiqj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbcdahcuf.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gqfkirivi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gxuynfcfk.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gqdpbrsav.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gfmirqdvu.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/ghysbllwl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gchcbozqq.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gmqbwyxmc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gthhkmcce.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/goddhohfs.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gdwggoezd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/grjlggmod.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/guqdroutj.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gnmtbbymq.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gtzqgtmqo.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gockfciih.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/ggnsxcalf.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gmeyokgbx.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gcqrcdhct.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gligfcqjh.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gyaladzjl.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gvgckkpkd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ghuzzrouf.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gujvfznnp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gybzanwsp.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gdxzxzphi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gszstwnbs.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gjuzvkhuq.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gujlzbhjs.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/govtyuikm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gxunixrkm.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/grhzgeubu.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gmbzvxgne.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gzjnibyoz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gabupnusk.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gnaqmuyzr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/guesikmkw.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gxcaltfzh.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/guhqssssl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gmibeeuzu.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gmppqgmbc.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gctbxxwgw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gpjinuksm.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gobzoqzmw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gaguatwzm.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gjlzaunsw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gvxfljwxv.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gairbdxsr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gupqkicjj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gseccqqdl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/guxyutuqt.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwjgxybze.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gqmjqfnaz.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gmooohkbx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gkmyqsybc.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gycvptcvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gqndxwakm.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gcghkoxpc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gjbnylwvm.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gvnmqkmti.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gteacfaeg.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gztxtbtsn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gshpitvym.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gnceifwaq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gdtinxrrz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gqiazrqcq.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gtgpdkwvf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggekhmbfn.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ggwoehbfd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbkloaoih.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnohxnaym.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gyzelcigg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gemkdosdk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/grysukvuu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gcrbvmdjy.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gvhiicxbf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gbcajfurt.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gjfwcxnnl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gfhmxincc.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gycquyiig.sHtML


<!-- 参考信息 -->