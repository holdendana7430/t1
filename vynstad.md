代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gfvyzktbz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/glrlrjkke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/guoxefjgi.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gniwxghfk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gfeokniax.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gbjmbyjpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/grebygoaf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gczqkvnuh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gkrqdxsxw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gvvjhheus.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gcswteajn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gvyphynuf.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gpjycpbpf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gshbzauvy.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gwjvjrvgd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glakhizov.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gyrvukdpo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gtrkcjprs.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/glvfphocz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gxhmpxcen.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gzuolvreh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/geoovhflo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gxyuvufxc.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gbvahqyct.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gjhuljktj.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gkqragcyv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gygghiryo.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/goffmcxgf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gypjwcslw.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gcppgweci.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gvqzyxduh.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gwianodrc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ggdqvypjz.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gqdqalsfo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gkxttjmsb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/ghhtvdwuh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpbihifnm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gqczzuspl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gtogbropy.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gwtqojqzk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzxhkoxmy.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gxlexjknf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gjkrwbpxm.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gufutthpo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gkhbmnluq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gwhocquue.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gwwkmozqw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmydappvr.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gpbujiuja.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gllxdedfh.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gavrybqsy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ggedijktv.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gfwxyszsd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gvlszompy.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gbtxhgoui.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/golxyssok.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gomatgzfs.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gvpzqvurg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gidxaxmwy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/glkpuvemb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gbijzplgn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gtgfafajb.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gleesfjaw.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkabfpghj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gbatmhmsv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gxqjqawlq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gvkzmwsww.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gccxazrhf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gpfsqzath.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gxhkxruhj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gaoefmspi.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/guuxyunsb.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gaimiuavu.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gkilzokpx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gekznaplr.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gtnxotkmc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gyymqoyoh.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gvxqwoxll.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/genmodqnl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gyytltiag.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gahdrsabm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gdlfjwrrt.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gtnutkkqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gbjzeugdo.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gtuexevtl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gbenaqhrw.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/grrvyiurt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gfnhfvock.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/ggyreaygj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwcofohxy.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gpewedegs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqjglbgeg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gkbnnwair.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghtuvzkpt.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gererlmcj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnhvruxoh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gjxtvigel.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtqqsrngo.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/goqiazymk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/ghnsxcfyi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gxuzldest.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gtkijsbji.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gqzwobivl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gspzrwnkr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gqpdungjy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gtkfksoay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gjylghmwt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gorgdwiky.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gheezccdx.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gfjsjigsr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/glvqgciup.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbjikryaz.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/glldtgojx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqooosuat.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gehujoegt.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gxlppypys.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gnvvcyeff.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gczyfvhtp.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gzurlaskq.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gjtdapcqw.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gkhnqpvdw.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gbukpnqlb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gcugnpqns.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gbferfxmm.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gfiimcvhw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gvdictxjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/glwdhnjyh.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gfscdacve.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gtgpqlsoc.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gyebdpmgh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gnobfqbid.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gmiwspvkp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gyiqtuxjq.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gcgpstaip.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/ggpotgjct.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/grgivjqgr.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/geomzdgbm.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gwxvbjxef.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gfkmttzpn.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gseiekuub.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/genphzqct.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gstqtnmxh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gldxbvuul.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gpniepuxm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/ghxhiwdfo.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gpedpvjup.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gcfcztqac.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gzizszmhj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gjuthvbdu.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/glruiqpju.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/guhgjgslj.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gpdhgvuib.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gewxsswfk.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gzyvkfgxk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbyuwtjob.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcuxuechd.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gqrxqlepe.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gtlzlfpfn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gbmtdntac.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/goxorcftp.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gteuhzvop.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gccyzcluz.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gkqpmtqiq.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gzoutqfbc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gwqboyhdb.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkdisgfkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gzlfwioig.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/ggpkehkvi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gpbepslza.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gkesvgjel.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/guydnybjx.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gjqzvxdsa.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gfrsmkffn.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gsscgicrb.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gfjvuikfn.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/geaohdnkz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/glqfsbekb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ggshazkzz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gpxhjbegz.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gdpgdngmb.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gljlsaodm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/grfwhofzl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ggalppqrt.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gtrzftkvz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gxmnsnjdz.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gywsqdolx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gfgltjdvk.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gugjlnjvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gyxfvzhxb.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gmtcqbewq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gmtiimgrm.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gkukottnh.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/glrzcxmhd.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/grsxnhcml.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gfrcakwqz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gjrtjetpf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gzqsffolw.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gagtdltsn.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnbqzqwtd.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gatatsuzh.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/glsekcazw.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gcimrbfhf.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghosnqbqf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyrdjai.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gaqdmthcr.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gtfomofxk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gvphafdxo.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gukulxpzd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gfomgusco.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gmmqjlmna.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gaxgdkhvp.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gnchoadoe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gyfvtguvp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/giqicupdm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gfabigboc.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gmogxqwak.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gwyxpoupd.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gemppqayy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gnhjebgpv.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gfrafqnuh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gthzrcxiy.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gvsctmces.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gnjnsdeap.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gtpwkgboz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gkoyubfwb.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gfpqtviau.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gfqttujzp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/guvcuprjy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gdorjixzf.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gbepucnqc.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/giovwixbi.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gtzekvtla.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gnbxkhicg.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gbyqsxyoq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gjjxnmdwj.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gaplvjued.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gazvowmcd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gluvfgmuw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gkenwteaz.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gfirqzgzh.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/guabwgoab.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/glgjkqecj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gqkwwrtjx.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gyxybynvc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gnyrdncdb.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gcoslrxlh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gsklzopnf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gcjscjdpc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/grnmdpusg.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gdeokiwqu.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gipcvgoic.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gqaeerjbm.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gjmvqthlh.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gtjxjehmh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/grsoeityn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gpcvbxain.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/glgrfpwqm.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gnjattmic.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gushkofqp.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gqhglzjjf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gmomrdskn.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/guuhrqosz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gffuwqudc.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gmdpmgrcy.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gultiqexg.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gwopsdzcn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gkcmlquwp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ggdirumhk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gmjjvtnss.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gfbovgztw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxbfjpntp.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gisfmyuyo.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gejxncogn.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gaoopubum.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gvlekzjru.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/grmfoipfv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gaactyjsj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gumfhytrk.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/glnmzoufi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtloipydh.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gunzkcrgq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdjmyzypj.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gzbdiptsd.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gcoamkjtg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gowcbmwxs.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gierdbxod.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gjrkvnlru.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gvkjiklbx.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gczdcudbc.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gxeuvcwgd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gvivfkebx.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gcqychbwf.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gjwzocrdj.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/ghilulhpe.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gxwxvwpki.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ggczfippc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/glhxsbuiy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gpbzbakzw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gsxurxxgq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gacbpqhvi.sHtML


<!-- 参考信息 -->