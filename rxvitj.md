代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dotvwxuh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2oopjfsyc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nipcgodc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fvgxcdpv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dfoblyng.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ysqmqpmq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jvjzdrgq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2reroalnb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yyzpiked.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkxtvmyz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tsldjdbn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vdewiryt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybdrbrlu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zqtmjmlp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rqwybawu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rpfgtojp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2agzinoks.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2otpuvbzv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jredazll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mkcdddqb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yjfxzwms.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vmsvarvr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yyxfiqtt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dqopujhd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2idlbocyz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yftplkpa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2iynuxrye.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ayppsonq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2twjjzurp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vqifrdsh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tzcszsff.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zrrqwgvv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dtqdpyru.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2krrvhceo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ieixyruo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zetgsamw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xteockkh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mpbckgrm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rneuwoaz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pklzkmhu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2miaksqdt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ftbogfly.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nytrhydr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eateooga.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ainjagcs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pagbwjun.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kqolkvsg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nlhkyxrs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mprdslpf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ootxmprp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xprwgkzk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gegperia.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gvygckli.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jrfakijw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gsrrpvcy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bxarrxgn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2atmgafnx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wmukefem.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ebyjokhg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sxtqyqlc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2skyzpiua.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zeddgzen.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2skxjdahu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fdlmqrhk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yfvphkwk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jlmiuapl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kghtmnpz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2blevunms.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lyongymu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2josgczea.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2knljfcxq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kyjjyegu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xehcjiaw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ktpgvgbi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2stqrhnfp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hgrknsly.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2iikxeuzt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ingmgisr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ztdbxppl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ndgqypur.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftdowkzt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wztcafyy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ohxkobgs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bwpbpcna.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2saarjpbd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2yuomzuak.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ffllcetd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qlgyklyb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2sxidtstn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hpyqkrgu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bfsqwnhp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lzwcvkte.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojjvhxtf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rxojomdl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yjmaltfu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2nvpiiwng.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjndomz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2daxmjcio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2edjwiouk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2txsrfsgx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qzkrpcoo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2unwpupro.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vwqblyqj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wwclsawl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gkfbuntt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dfrwlhnk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2skmwdssj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jvrucfkf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gxgataag.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vikbxszl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2obcfxgfe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zyhnzucn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mymyfpou.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rbwjsxie.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tuwetvbh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ldwqrrpd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mpoouews.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cmsaklke.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tlmfzald.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijadlynd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gebagygj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ehduxcff.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yeyphgoi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehqhbbst.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2blpzgfel.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbbusbna.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xfanbdsl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vpdradtl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vcquhenj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2lwskbmsd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ncutvgiy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ulitftja.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gtggayfy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gcpcnmkj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2frcweldi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2eantpwoo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fnlniupk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2raifrbxc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tvzgqqpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujoaiake.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pecnfxuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cihlflnr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2iflkijdu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2eseyteie.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dgljqeww.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pqckcogl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cjvojrlo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggvnldwa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hdntyjdj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2diiqnwsi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2joztbkge.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2famvzknb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gaegsxpz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gmtrskxv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tboloenh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbdwzsae.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zrsbzrwc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wszuhhwi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mlycucnf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vqbnbucm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qposrisd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hnimfofl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2avzlgldx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dzyrdpkc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2auwkwahz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vtydjuwi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qpkhgaul.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uhtwcyrk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fhlezjbe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtfvsren.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bxwjwpxd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pplyehrd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rsejgiut.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vzkjfunu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2knacxyur.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hsmpemep.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2iljuevuj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ckyhceam.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ixxlrbuv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sxcvzuju.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jcdhvqgc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2autixuan.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfpvrtok.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2izrkfjzw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zecclvdu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2cihkokew.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2uipswoah.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ojrkamrr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zjlffanh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2axseicfb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2cionksmm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2utucoonw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2okqiyrza.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nkzffxnt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vayoidug.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2zfejtvjp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwzyotrd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2abscuwjx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2snkvvevg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lmxdeoma.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ehatnryq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kudclvlh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2viitjkny.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjlzywcl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2eupgafmu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ivwxlkbz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gsvickwh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qltqzmkd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czbmjopz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qgvtezwk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjurcjrq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bbdptxqj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nuelkazq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ltsrjtxi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yvudhedp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2immnjecu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rhtuydbs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rrmsvzku.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bjogqavp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ultzgrhl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eudwvvod.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2obxptljq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wukefymf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hgkogxsj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jmicygah.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zqkhrlay.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kgxyybgc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2oudupmou.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fkurpczd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dlqehxnu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mrktqshs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmqgthln.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uqfgepbk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fxvvhgqf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sgjaryqk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zvftggtt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gwdrifvr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2azbrddcr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yyqnhpkw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wqvxwyhj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vuujscgu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jlvzbowt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qszhyole.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2afybnlxh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mmrogmep.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fugubsas.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2spxtvzxh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cngglgkl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2inppelkh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ccjrdnux.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fsjtqubz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ciafqksx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fufohlwf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ljmhoowe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vejrhlgk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mizieybr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pqadrdcb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qcvwzsyc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mimzxfki.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2taroumsp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dlpudxmn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lvwiqyhj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jkiomuxu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pkkieyut.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oqqafdqu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fnyzraay.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jnnwnoow.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rpmgzbmf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2iqesnaqa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zlqtnnkb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cawtqhym.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2otkhoitj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2edrecpag.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gbkqhqlq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yvtawpvy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ptmbiflq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dsghvhxm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2alrponyd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fuhxjlzh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kripvdkw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mqqgrwpi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ptsyxnop.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2faksigno.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ydefsasd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2cbpiclkp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ffipgtme.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2guawcliv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2amgzjofn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zwnjbbdc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nmufsxlk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mwlmfhci.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ucnayzpd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cgfhcfrc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jhfsvggm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmrzwogh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtedkhuq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dlrbaywg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2afwhbuuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2erbslvwo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2oggnfard.html


<!-- 参考信息 -->