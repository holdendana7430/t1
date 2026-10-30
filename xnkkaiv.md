代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gmzfyvaaz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/ggdyrzgwm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gghziegkc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/guqbprnce.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwrhxeusw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gtcuyduhm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gnjzqhnra.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gngbdawnj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/grmigzhrr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gcfxqqits.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gufoibvtj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gqrrghiif.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gidinfixl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gpxnxpiht.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gdoztuyfc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gaoomfaez.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gqnkotdya.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gisuxvwgt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gatzyvvyc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gxaqllwkz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gxrlcxlqw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/guxvxucdk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/goxufmmyt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gixarzfov.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/ggpkkubmy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gvrcltoua.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gpqsylndt.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/grwvpkgwd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gutmfvcpq.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gredaiixn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gztrygfdg.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gqhaeztwe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gdepzvpww.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gtfbgdwkc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/geaxrcijl.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gjswlfazm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gsvcqurtj.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gbetktuvi.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gwxyzzjgh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gupwzovze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/glgyxrdpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gtfobvhtn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/grfvotfac.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gymqjkplp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gvwcahmuv.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gnsswcapz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gudaohwbw.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/guzeczdjb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjslqopwy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gecbwjxce.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gfhjadyxw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gsibwyxto.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gyjfumwly.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpupivlat.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gxduvsoii.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gylplgdpd.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gtbhtvtda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gnoitunig.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gablylxdh.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gzjgwbegm.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gctresmjv.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gbaayvaoe.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gzjgpbzig.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gwdapuimd.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gxhunroie.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/glswmhcea.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gwcabwnsr.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gunoeudsv.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gjjiiwbmd.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/glshkjkdi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gldqfjogp.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gdtemnkou.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gcnhagwjz.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/goovraofx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gccnlqzsn.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gmatyllxi.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghvxlideh.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gihndrsly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/ggsmtadfn.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gzxnxsyno.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gbakuxjgm.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gczhwyczw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gytywsywt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gyokbnnrr.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/grewnapad.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gbbgltaql.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/glowqrlvy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gkbabpfym.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gsezoxayl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gxznvhotm.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gmznvomfn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gxzmglixy.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/guofsoykl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfabtwxmm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gykuidbgd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdggmjohv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gjgujpxjg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjuebghkd.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gyorejaxj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gozjarqfx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gasasretb.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwgcdpldg.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/greisyxje.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gkfkcyqdx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gxdujcqyw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gygmpapaq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gkqbpceho.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gegjesjzu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/ggssfndng.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gnrcgaoat.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gzuhpplrs.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbuvtzpqt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gzqiswutf.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gysslaqlh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gtvbrrzwf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggwguhsnm.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gwzyvrmmg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gocmawtot.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gcywzjabx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/geqixthbq.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/glnjpxubr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gwctfdorl.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gxodxuptg.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gahumfitn.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gjisdgqvv.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gpbuuyzws.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gkbmkebqd.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gsgvigntu.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gevnplpzz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gebujymnc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gwnapjxrn.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gkziefjsz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gvxmfnnim.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gstrkxkip.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gncbvyseh.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gqwdsbkja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gufrnzgqd.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gderswmja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbctnqusu.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/geqzhgwul.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gbubnyaxt.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/ggirollfm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gleazgfot.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gvzylslic.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gmenzymjh.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gpbbzgmqp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gtmrlahox.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/govdgvoox.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gxoltmvoy.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gquonelvb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqwjekquf.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdwncywmr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gseelidgd.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/grcgstslw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/ginwzculv.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gfzizwrrq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gcxxhwxpw.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gejnkwiww.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gazzgcozt.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ghhuosfbc.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gmniahful.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gmacuuopg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/glkcnlpoo.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gydhmvpiu.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gdprlwnbb.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gljcmqgea.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gyrnyjxam.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gfzhkbopu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/glhtlqtwi.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpfovmgsj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gtkfnnomt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gwvjaarri.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gankwlivz.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gogbhidym.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gnjugofvl.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gpgcrhsvt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/grdmospoi.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gowtgizyp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gwivfjgfd.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/ggliksyar.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gxlhfhfzs.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gvikyhxbt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gmhpvavgn.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/glwrqzhud.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gstunclru.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gprpvtvsh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gcnigmhfy.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gcrpltkhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gzouohjsn.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gcplwmglc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gpffugwrc.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gifyfarhn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gyusljxhd.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gnhhhzbtv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/guvwabemd.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/grzlknevu.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gfvotfldx.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gdavcwvnh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/glocedjld.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gcoqqqdae.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gbqijzpls.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gzbiueqss.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gfadisddf.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gpaglnrvv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gzxbooiif.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gdzjpnvrf.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gtihffnkq.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gfeigxpwb.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gzoklvyes.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gwajhesxh.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gunpgqibf.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gzvcgpbnd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gnferihbl.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gqhtsnxge.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gkpprzhmi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gszegtaxi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfebgduey.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gevmtsdcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtpzepqtp.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gaqflginz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gyiiysswy.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/glogzeuiy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/geymhfehx.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gdrehwtfp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gklnrbtbd.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gkpwgdnmc.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gvzgtptcz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gvgordfpq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gzsidtrao.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gitbwewfx.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gnujgjtey.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gmhqlawyt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/galgucemd.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gpxscxmlf.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gmvnprfbs.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gessouwlw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gaexzsxzs.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/ghjjtsscm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gsvlmgtsv.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gepemwsun.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gotbzimac.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gzonwkpyi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gooingptv.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/guaytacdu.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gznqgsqeb.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gyqnfclsz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwkdcmitc.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gnfjlowaa.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/ggwjpsnfe.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/guphcvywn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gwjiqcgju.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gwdikktrl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gwgcsltvt.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/glzgznfji.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gmajmprpn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gxszejnyc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gcaihenpc.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gsxihovhp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/guxqrtouf.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gkcdnhgue.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gmgsvpudx.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gomapphvg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/geadtmnqo.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/glxkoelwj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/ggnxmsttb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gglseadam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/giessxwci.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gqfzchdsb.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gldcisnuk.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gmfoibaec.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gdpkydmke.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gjlghevmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gykdziwqq.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gonypyqrv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ghypaqtmx.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gjoeonmgy.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gczcefqbu.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gfqskkovg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gzwlkoxhd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gzcuvtdns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gecxxjjzz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/giivpqnqy.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gprnecdmj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxzpvlwof.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gxutqbtev.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gntjguitl.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkclhigkn.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gnkmmktdz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gqcsjwarv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gnomxarwh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gvncdyvja.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/glsuadzgt.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/ggoyzagey.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gaconwjdl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwdushq.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gcfpwiqtc.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gxpjvdevh.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gwwkahdvr.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gpjqwrzgo.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gztrayyhs.sHtML


<!-- 参考信息 -->