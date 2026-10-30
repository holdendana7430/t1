代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuafqoay.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxtccrhn.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gwwtsiena.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gvhwcptdj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/giqqpipfm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbsxhnym.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbtmahtj.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxyjzdba.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpbmqvdz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gfhyvsjkh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gdbsavxbg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbinrmjhf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwrqascs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvwtppge.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gorykgqko.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkeonyr.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gfepsajjy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbizegdqz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqahhqmxs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipzouqnu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjqdlepjc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gazkzdqtw.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzgioinm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkjaohhv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gedgtazmg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvulkdac.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxujecgzm.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gycbwtrnx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdohmzgo.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gvflhtozg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfuojvu.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gsndpnyam.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gijygyqdk.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gmsabuaul.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsffpiujp.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gqdbydxfb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gcsrcnava.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gtzmhjfqa.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/grdfmpozx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkclqzajp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/grtcmnqxb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhvzleci.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuckamne.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gotosodzr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyaunmxvd.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcqloajm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gztaotemo.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/glbavylbl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtgguskz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/goxmldhsl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gdscltcva.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaepvbmc.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gyclozvsj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gajvguygu.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gfyhzibed.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoxuviiu.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxucdwlv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrpspjcx.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlmlwpzo.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gkqphwthf.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnsnmqwly.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvirmfmq.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghezjlext.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gappowmvr.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpvmfpwc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gtoykjbww.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gawuiszng.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdslklyrv.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmrrjgobg.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gmetpuocy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gqxwywqrf.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gvjupgzjt.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnrzohlel.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqnghnjc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gwxvlnpoo.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gmsxfkjmv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmsankyn.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/givveyuzd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/grschqmus.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcmhtmti.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/ghlferqpd.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiblmxng.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvtesomn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrydotau.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxvkxyko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdhwrsuc.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gwshbklca.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/ggrpoojxw.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcvnvrmjw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvocktwi.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpsjttip.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gpanlyqng.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhitcrso.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyqvdpbnz.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsvqppsy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmngkwwbo.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gqleborpu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrckkmkf.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgdnmhlq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxytzsjzz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvihqmwu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grdvkuzcg.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gavlkckqc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebzopmiy.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gslrdfztg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gtsmhtzgd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjlkzwsu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/grkkvvnxg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/glsgehjds.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gbiwpqhrk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gemexfjkj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyuggxtu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyegmrusk.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkobrpryb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzxhojpb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqzbgrixg.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gartukfee.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvmqrfazh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwqurucw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtefabjbe.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gwitqhwgf.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/goyfrsqjg.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/givplrmoi.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjtfpdzah.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/ggvulzaxw.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeugodmd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gynphkvpv.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gyfbnwuks.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guojjjwrs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvoicmtb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeohttmv.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjvwquaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsbvuvzys.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdjazfur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goqkmepdt.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqvizjzf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoirpwjp.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpcwzdfpa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuemvlim.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhxpphwk.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gxclynfrg.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmzeqovy.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmyxbeagj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guygjerke.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/ghhqoztgi.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzuzmuiq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybfowmkc.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gaskjycqm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwknyeqy.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/grgkmzeyx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/goerisjlt.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzofqst.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtocliqtg.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghihjsmkk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gowkddkof.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgdkphjx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzjxmsron.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gkfphzfbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnpecmgkc.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goybhjwtv.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjepxcrgz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwfxiwhy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbonmgzdu.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtiiburp.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gibtazeyf.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gmqtrrbzn.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsqnvavtr.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmbjjkwi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzqqhsnsi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genjzyryg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuowniuc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/graqmppzh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gardjgwpy.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggevpbfiv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gfgeozwqb.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golarjrev.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gigryaqqa.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gjwhaijkq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/govbxuysr.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gctxkjyus.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gexkmchmm.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gastbghvv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfnjctvq.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkenonxt.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghceyrpev.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfybihxa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gilfdrllh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gbjecgbep.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gibxldzed.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gomimjdzo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gbntpdtqi.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gidnzzbje.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkfwzxdx.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxrlrprua.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gvolirrwl.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpemyfpe.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajoyrahr.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkolaqvg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gltpghqwx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gumqeqfdi.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/glhvmuyui.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/graxtegmd.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gyoqejzke.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnaprjtr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpzkjvyq.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gapdtsmek.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwnowjfjc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiyvrabn.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggymrlxoq.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gibqtdrfl.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwjsmroje.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gqndgyknj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzwrkhme.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeywulky.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/ghfmukosx.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/geaqfoyiq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlapkhba.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/glfulaxmf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfmdxgirf.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuphwlsv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/greynvkcu.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzbnqwkcj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghrmxmfyi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjyhxfgd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwtnpzcw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmchlhvo.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggkvofqbw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gmqocaelo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwhaaixtg.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glwydtkts.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goknffwhd.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/groqexeai.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gzwmupuvs.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghgbxjsms.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gfnuisfer.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/givoonuwi.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgyrifhf.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqptgnjf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/guqzcbxvl.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpclptszl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsngcwivk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfaxtnjf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/geisanpnb.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gqumkcyet.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gxayyydxr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtztcyjh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/grcnpcspu.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbngvcfc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gvjioxxel.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrgycnsx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlnnmbjr.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grtaecvsd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gogvhawtt.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/grpihbkjb.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxjixkrn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gygaohurl.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/goqlzmoyo.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gqompgncb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gznethuap.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gdvbgahpt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gajysnwpk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoioblob.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkfpweqv.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggotxfrap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnysmsvp.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gkhwsydpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqsqthsp.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifduumx.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjoixwsh.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gznfwchdx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvimhbal.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvcdjdky.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokvokixk.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqcjqpoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/guhmybiyw.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godebjhwp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgivlxk.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvuvpkle.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuufgyxc.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gnxownvjv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gaunnqjbm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggvxhgxrv.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gigaixfvr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gadulgjae.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gysofiekl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzveycrxl.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvlpjasf.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyghknmm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/glfrvycqn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzwudmk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtysrjhe.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gvydcxuyn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquoefoci.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gveiucgfe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeexoopg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaazhbwh.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtjueqtr.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grfbuyyfc.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/giwhcujoz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcnnfour.sHtML


<!-- 参考信息 -->