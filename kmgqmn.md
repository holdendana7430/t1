代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uudsjrrg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2sudcmdzg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ditqjlyz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ibffftgr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tiiglefa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tlcymrle.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iemnrrht.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fbyqxdde.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2pexgybus.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vnjbxzyb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cuydnpvs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2otndcjvb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vfeujspt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nvsjuzpu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ysfklmkg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qdqpdalu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lgpmlxoz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mxbhsdjw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2trelvtee.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hpbcnnlk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hnnqzyql.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hvotvycm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rebenoae.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyawjblw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zcucxbzz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cqpgwpff.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pjaywmud.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2buarywtf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bogdqsig.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jhfftczl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gtcgeqgj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fwstlrzy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fkrcbyhm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2skpsvxzz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vpkvsign.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xxekfehn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ffgwjxum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtzbemp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mbbcheit.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2sbvxutli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qbzlvnfr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kicgljxu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ktoasexp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pxyboqfx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ujvqwsph.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tpswnjny.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2izzpheul.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rlzyaxdq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xyblpdah.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bhzwpkfg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2holzuohu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2exqvijwr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hdotcspy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2urwmeccs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jowjhnri.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ungwgczj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qrrywrmk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2cnxbhnhh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2msevywrw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ylnzcgve.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mcqqhycm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jlieenjx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2biglqmhz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwqkiyhl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jaozuubf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dhemjbqh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cljgbadh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nllrdkag.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fslqsups.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ycqaqasz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kjdkfnmr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2pkfxcyln.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wgetblof.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fbmrgjgc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sthnxvqx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2puuisiov.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mmjkgnkc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ahlnforj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2eqgmnzui.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fhmdnzxd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2odwmszhg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2huojtgyh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2udsfzlhs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2axykppqg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2myhbmavz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2thmuaqqz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2txrtqnwg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uiozgzdm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tushmuov.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qseidfrz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pzxxkkvy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2codrhbmk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2savqwgbx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xjorsgam.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dstrrgfi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zyfgzxvu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mdwszsap.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlfeaal.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hepufufc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fsxgtzjg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lzvhjdwo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mnollzny.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jhgxenmi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wtxiayse.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tqcuuzmm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzantyum.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aoooxkkl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmlpzsts.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rjuobyiz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpijunaa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wxsnbrbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqkfdvkz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hgxwxoto.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2akubbyap.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yzjlrytw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qktywvrb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rrmwjczg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cutxxesq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pdptkjpb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2whtwfvbg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nopcxlev.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cjjkkmws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbfmmser.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dlqorile.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xclxkkko.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kfmrjzkq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pklhaehp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqpjovxk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2laoipubl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clakyrlf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tdbjpkwh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fjdycoju.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xtefvbxh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vzlpleaw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yvscktsq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2juicxael.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mgermfrp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hiysxfqu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zzuybiox.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ewisjlpw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxpfvgqu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lalbtwhs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jqvryxsz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwzxjiny.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zzfloxaj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2bndoojkn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2enimghfp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ymkdfmkq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2drorqnfm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cphuskpb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kysaubfm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rxvzmuri.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ycavbvmq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jfpujosu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jmubfdqg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zviggzcp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gpsjrrli.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyztuwpg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tihuteqx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjwjgpqv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvdpzsqx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pkpsbnov.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tpzrbxye.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bforxrsl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2irlolejc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cyvlrqkh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ehbkcebe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rkeirxmm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sknwahzg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vvvqsbmz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2phnagmkx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aeakfsle.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eblcmcpl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mdznpigh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2griashqv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2skfajsrg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2asytdkgu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lislbsqu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwjukfme.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wfugzoay.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ytllvgwo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cnwwoanq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2leoszpwy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ayzasjjy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fpdrwwxv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkfclrfx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hbjjjxrp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rkzlofqv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cndsmabs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mzptkyeg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iwljogyn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2eieydgii.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xpyuawxi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2aeevefqv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ixnwwcbh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cbramhqa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkxixryo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kcbsdeke.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qnkamngi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2upvvbvpr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tsejpljy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qvxytxmt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hsmyrrdh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zlyidbxx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rczwjskk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hcqimpma.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2soyiwogs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fhrsreoi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vzkmbzpa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lsoamukw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hjzyyxhi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bucuuqdt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ylodduzx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hwcczapf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vovgasln.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qlnynzob.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pivjxddo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2iqvntptd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fweqtopa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljdpxalx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rtjiynoi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2livcnszz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hvcjzewh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rdxxhxxr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mgacockk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pkwwftad.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ervqlvls.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pkbkeptj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vjndbrne.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zxebtjbc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eovmppmm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uaidwyzx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yykgzvig.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kxaqquft.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrwlksit.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hcnrptat.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ieyqldyu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cfsirhuo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lhinsjwk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iltyvbzg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2oqtfapir.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ckqblmjc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyfsqtai.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2oqvjxvok.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rsnqrsbw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oxehkmjo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gfqemvkq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ihzodpxf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tsxvbaqu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mbplrntu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2idspkxbm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oybvfgtp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uvifujha.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iwvejyjw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vojcfbzr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tuvzugni.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cweyrwax.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyyfuavh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bwhnnete.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jyocjbse.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yesfsqtd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cjvgfxjj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vhelhesy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sfzqjoag.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cubcukgr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ubjmwmlb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nckyjbkn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2amjydawy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pqoizvxi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2irtxcrke.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyirgmck.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ndkubnzh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dawkcmyq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wmbqufqe.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ledxruxy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lchsfwkb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eezscafy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2pcyblqbt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sjmzbogb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rygohgid.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kphtojxv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tlrokwuz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zzpwztxo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhcugxag.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vieiafhh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pczqfgkf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2eochmcmr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sytbrkqk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kpjvtcyw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lbuyivyu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ovuvvywh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ckkyzjze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ytioakaa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vtgepsyd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tzmqnexe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozhiffsm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wxhrhgkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaekvqwy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cpkcqfqy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cwsuoyuq.html


<!-- 参考信息 -->