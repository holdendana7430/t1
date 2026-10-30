代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gytzkcfjc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsszcotcg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gqbuaogug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgjomku.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkzpoopx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbvnnrf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/glfgzhftb.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlpphte.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdoflzif.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcckxktug.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gscjvdjwj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhhqlcoc.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjntkwmkl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzhdmofs.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gyfhqyfkf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gplaffovs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gqokbpoyf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/glxjudftc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsffvnsrj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfavfdybm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaugbcaw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocryykxy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gheuddygk.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/grrsmxbuo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gxhkxxktb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjryakmx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gelecnceh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/giygjbbzz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gawlzadpy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/geemxlxfy.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhveeahq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gebajzsrn.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/grywludnt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gwjunesvy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkgbwvqh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhdptyec.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogrpdov.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjblnmeix.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyosxhbte.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxaflqme.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/giqspxrij.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxheqenk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqabahgop.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxyhcynp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsnhidtl.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtucqwjmy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gusmkhpqe.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gqjdohzbh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdsofxbkq.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gjtimlofa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grokagrci.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyjxyarz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/glddjphju.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkcajms.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzlodwtr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfteftyfu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrijcwwg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gymuxshhv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gthpefjtp.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuuftqah.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcghmfexi.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gperuqhsy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyadgqoth.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gamdlaxzm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybrhdgbr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowgeabuw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdvbermo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gepjfjexi.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmkwvcl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxbcvsgnt.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmbasdgs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzgqoxlg.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmzgsaqxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/ggbfjyyuu.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxusicvsz.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gktckukjq.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvlfjtqm.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnkyyflv.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gpktsggjj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwgcnub.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/ggwqkccbr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvufqiac.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gukaoszbr.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdrqicol.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gohwynixl.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkelxrjss.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvmadalp.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gwvkwefjr.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtetbwyuc.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gcolokiaz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/goycoupsz.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gducsmsmm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveeybpml.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjjpiaam.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gzjnpcofm.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzfiyjkw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gqgkwzfnz.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gknzdaqsy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxyroani.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeaccsrq.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gepvvrbyg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gmyaheqbp.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gltgxjbao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnjdksvl.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqezoihrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gfkhjtgzk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipxsnsx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gigtmsmrz.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlbqskun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gumztpuzv.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwprqgmp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gehevmivh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gucewrdkx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaydkibcs.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gocsqsbyq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gicmyajjt.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gqdaydwye.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbarecwaj.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/grlfmlavq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhnskta.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuqltqjo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnypwhcs.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyoouoofy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gtzktewje.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxdodvqx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxkifxyk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghnwbiiee.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glewtyhum.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/galzhysaq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmdkgrsc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcemrtswb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjommgsqa.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gjyndykty.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnktrylka.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefhtqhjx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcdmsmjy.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gogftyhoq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gadzrgowa.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gipqascta.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtufbseav.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsxrkxcs.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ginaifrdn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/geebzacpl.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllndorrp.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guirfhhfl.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkswqmwtx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpagawawi.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjfwfetbq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjzprtiqm.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gydeikazi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwkiymmk.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotjjqexc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghbduvrnm.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gulcabjwv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfmnbzw.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixjkzcdo.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/grixwiegi.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymvdnggc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyixvjjbr.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/giurqrogj.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gtxcqvsfy.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gewczsdyc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcklddfjv.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfopeafie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvsclspvd.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcwutijq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfehnvjfx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczgxbxql.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gukrjfwfw.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gazdpkugm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcguypxqa.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqdurlmy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgkoxueq.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/grjefpybl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxajbdxdk.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbuasedtp.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gznzabnqj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwxynum.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gihxkmdpd.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzixmryi.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gosbnxnew.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gviitxkqz.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqiyvov.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdrbtnzbh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmoquodr.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gownemtag.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggddwgmbn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gcunoxump.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqeanyviq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdijzaco.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngwuvxp.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/ghikbhemv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/giimimcux.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gplsqcugs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevcnieu.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/glqhacktr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/grgxiothb.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqyuwwowe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtobamgsd.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzyskrrwq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhcowuri.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzsyuyda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggdiymztu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gkvgcpvzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gmcoiktqy.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbvgbfwlf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gealnvpci.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/genqdjktm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gesfrshge.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/glcxdtnbd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvpiiwbs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlbrnxbn.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltyuyhec.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbrqczda.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqncdeqs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gejjyshaa.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gbtqfsyvi.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcqdsplq.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpskxvop.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxazkpem.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gllzwdylj.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicbnxjev.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gropbbvcr.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpowcpmez.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwormpneg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxahcpzt.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwbnuhpwm.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gentatmsi.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/goxabsuff.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gushyowok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrnooyqi.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkmkrulvw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtbhtlypn.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdhbnsr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grxejxtjx.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcbkajpe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gxztwakho.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glqmewbin.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gorwpbzcu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfpggxez.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gkictirxw.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gpcdowbdp.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gykjagace.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/giehxevrl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gkpnvcjmn.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxwwvughx.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwytgpjk.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gzsllzyoa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyzymwvk.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrjhmek.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfjbkwgq.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gnldljang.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/grtwuabni.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/giqxgvnlh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvoxaudf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedrrkhq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gqabtqbwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonkjwkko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyhjyvvr.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqvatya.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxplzfae.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtvdljpw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gnzltgiwa.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gcegtwnyi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/goplofrsn.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gfdoctbim.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvfdowlv.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyhjyypwz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gcpqklbeb.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gchyxtfgn.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grzoitehn.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/givhrnfbs.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhijvdhj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/goyajboeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grcyqcigg.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjentmmox.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gtkvcbrgh.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/grcltcxlq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjmntwty.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gkjzhahfi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsogxwzs.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gfiddvszv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbecnpaaz.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghexjrucl.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gifbhkjng.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gxerjbfzx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhxvcrko.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaobqvmv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gxuxeryqp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govrujddb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gaosrkosk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gvmyftjib.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gzmbsimrn.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmhxohcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godslhazu.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gckvbasum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqugbgcig.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gllebpkrm.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gamedxskx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnqvcvug.sHtML


<!-- 参考信息 -->