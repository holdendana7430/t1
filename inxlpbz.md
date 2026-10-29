代发 wailian999

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/goltdcqdq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gzfgvwwab.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gbqqzkhaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gunldghnn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gpvyshnjg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/grepmmici.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/ginoykxbv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/ghzslvffd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gxsozlmir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gmuyeofmc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gezyekxnb.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gexmoqwmy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gakclbmnb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gyxctklrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/glztiqrjo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gwvsbabbi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gowtpkmnv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gegpvoxhr.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gftfcitxo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/guvnokpyi.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/geedrikes.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/ghsexwppq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gkiyqwewx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ghsflpaqp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gomtikxao.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gnentxlcp.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gdvtgcgko.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gkhavxwgr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/giiamdeah.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gqhpyjpyi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gdlzvotwv.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gmitwjawj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gmpuyabma.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gcgcfgtqo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gonlmvvae.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gnozfnfbb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gnqrtpofj.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gymkhcnxf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/grbiwjrbn.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gwgcfwnxy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gknngfuhl.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gygjawtie.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gvzrapupd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gebmclcdf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gabrghtld.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gbjulfuts.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gynfykcys.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/glrxtgsus.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gccmbacth.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gwaxqcxnv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/golliogcf.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gjwvivefc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grjjxperk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gmklzfegj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gdsuyysdw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfbyhjdkc.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gxeolmhhz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzoajbowy.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gosveinlg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gjurtpvyf.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gxvxshxjq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gntjfdbji.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/glwbofhrr.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gouhccnrq.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/ggoygxlws.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbpcjlh.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gwfnrkifa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gbsazlean.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gmpvrdvdo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gxigjgvld.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gfampmqjf.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gqytyabny.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gyhfsfqrt.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gdkzihoum.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/geylntgsv.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/ghtraitek.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gofztankp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gwkvootnd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gxquushab.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/grrlayjsq.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmglvruqr.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gehhqyeih.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gexnlotpv.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gywuckbus.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gzxnwrneu.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqzmpnngb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsnqigpek.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gzuhnqonh.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/grludgvac.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gpihaizhf.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gotsxiycm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gujrjuwpa.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gdrelzmzp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/ghfeabrmx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/giphdfnkl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gpicvugjg.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gqxdekpnt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtcskrkcu.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gsznijpzz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggdhjcwhm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gvzjaysqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gddzsjtmu.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gmjcffysa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjwsljluu.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gstykzepx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmgqchilo.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/guvennfhe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gqsqqktzt.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gdhhkouud.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gnvzbuuhd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/glifqhbap.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/ghksfksuv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gffuwqkay.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gcxpihvwt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbunvkeni.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnrhswurj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gnwoovppu.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gxbnbggsa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/grrxordjr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyaujkqvo.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gepqwhtkt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyekjguvk.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gjitswobm.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/guaeoajra.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/granucife.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gjvwaagfe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gfrsrnfwb.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gujwdlsft.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/geqfjgsqp.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gmgvzyqtx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gutzhwsbg.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gveaagcwu.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gyfrcalyc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gfgpgqylh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gijobyzsz.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gfoegvqtf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/goigmtclw.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gvrhtkexw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzpbzqlwb.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjenmroiy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gwaoaeunb.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gxyhlbvqd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gqjhnvrqs.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/ghblfnmxu.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gttcofhas.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gizfkinxr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gtuqkyyhl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/glgrnymhs.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gsjaqpvcn.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gylfrkdeh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gmrmtmzcx.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gziiqwzpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gncrifdeu.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/geotmazwk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gvmgdhtsu.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gnkryxfpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gvonybnsv.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gqsnvmhkw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gxsgbhlzc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gsdligzxt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gpmaxgtnw.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gwmrflvgr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gvbqnxzbc.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gefkshwam.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gftdfobur.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gplagfkwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gmiurevrw.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gqokhyuyp.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/glmuplics.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gqvslxccg.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gzghucwmc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gpccpaogl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gnwbogfia.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gcanfqtov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gezcpznsh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gtuldkntz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gapfcynss.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gsmkiqrzr.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gcknjfeoz.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gwxfvbrob.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gccrvtoaa.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gxzoexoyz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gmorjmxds.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gjgtsqaui.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gserlgqoc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gxqeruucg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gymctkpmf.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gpqtvhmej.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gxpiexlyc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gipuskfdr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/galjalmsc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gpvebpfgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gmpswsutn.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/ghjyeqkhk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gdahvbtly.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gnwnsyuok.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gazipcczj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gackpxyhp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/garhccivs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gdfixsirg.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/ggblirqnl.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/ghenlewtc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/glqupfxmb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/ggabogqzs.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gldtahbgp.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gwyelayos.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/ghpufhqaq.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gzfplwcxf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gbxscllgw.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gyreqqtbj.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gcusqimgy.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtiubmung.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gophqwrbq.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gcaykwbax.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gfxhbbzjp.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/ghynjncmf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gymrrymhk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gosvevjop.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gayfdexnc.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/ghroxjeqe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gsdkbbvdc.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gahyuviro.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gmtzttses.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gwibrtqfa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gywcpvmea.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gfmyodxxv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gxzdsjhnx.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/glolyruol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gxonlipec.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gemkgqqou.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gylfzamgl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/genflndyd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gzkqrxkjp.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gddbqowwt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gygxpwaxg.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/guwgvfnnv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gdwmbkfit.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gaxfrxqjb.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gzzdkhvza.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gevweqrsz.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gkidadmgf.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/galrfoybz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gzpqlpotl.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gruksnmwv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gaiiwblmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gbuxnqric.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gevorndau.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gsvgojjlm.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gxkfmvisn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gmsgayozh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gtgugsdup.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/grcrannim.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gyrstdmji.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gwexiergp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpkphfeq.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gfzwiyztj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gqfiaxzhk.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/getmddyhd.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gqxxfvbpl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gjrwehyyh.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gjfndnpsv.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gagxnlfle.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gokdzvilv.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gwlhsryoe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghmtllahd.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/goznxsqba.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gtndjwjyr.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gfsjtpcug.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gycwejrew.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gxcoxpjji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbstdzlog.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/ggtasxumx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/geheezxcz.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gcaanxefi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/ggwnqdkwg.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ghotsgxsk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gbxwyjlrs.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/grnzjxlky.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gkhopzzuw.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gnkvuctgp.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/glqvydvsr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gfkcrwjxz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gajtejlfg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gguwzotbi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gmjwxfred.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gpijfadcs.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gxbixocni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmrgxzglw.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gpaudwbts.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gebajmonx.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmfaziuig.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/geuvhcrni.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gkgzjipcy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gqanqjbli.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ghmdrcscy.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gxttcnakc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gjvintpvb.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gpadqwbkw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gqunwgfgu.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gdlxcekdp.sHtML


<!-- 参考信息 -->