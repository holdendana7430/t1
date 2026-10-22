代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wpkyfabc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mdgerdua.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hrtgbsiz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2auckocis.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2meqnddjs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bbdbvzco.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2szkdgepe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ngkqspei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gdzzxjzh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zrsxogqt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gwgizilj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kgaxqzzp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yfxpaanl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bafenlnu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mhjkzvcl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gofoknqh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pziqmhfy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yjtrqkmr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gpptsulr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xgwtimpd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sqrwhkua.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yromwwcl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jlphedsa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2acyfhigk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2axenagkk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jsfubfgw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ladoscbk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bczgihfz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dfmhcueo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2futnebrw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uyswwoub.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ihlvepzy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvethmxm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ovtiwfcm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ehhhmicu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2menjubsw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2svejpmqn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2egjkltop.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hyzinjbb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wmvgxrss.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uvoxiuby.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2sjuwxhwv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mgrvyqys.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mailrecq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xovbhctz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tbwlwoaq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dgxvdtfb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rwzhsyuh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jddyiyxi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bcwgcttz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hspfpiux.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ndalpheh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ozkgifbg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jmysgcdw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bzcqcuhl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqedisx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nuxnezpd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oavifsna.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dddordsa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xkjicpbd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cbqplnod.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2czgxjhyq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2osqodktp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vvrffbyc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xvlhdnhc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2midxgawj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rjxvfwxp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dlmgmwjl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mpolewsl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2uecqssbo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xcsauelh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eyhgfzgl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rkqrdkxv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2iqcufzhj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mqqeudoc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uaryrqyf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yzkhkgbo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bbyvttdb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ewqqyofl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2btnsqthg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxekyzfo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fgxyfftc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2otzpxqan.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jifgiwkn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zzemlxjz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mgwtnkfg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eqlehloz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zzkflfex.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fyfehuyr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qpnyjvst.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2naevqkkw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hiflfxwz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ufmvesqa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2abhqoftb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tgvgtnbq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tmnhbfzh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2lbfqpgdv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2agabweqw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ulghsvzt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjfeqltw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2luinmkxx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qqfsyteq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hrhjegpd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwdixqka.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uiphdjpi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afqflsso.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yfsvkufu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rmaimxqy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hbknseew.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ufoqesxv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vqmcbqnz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jevevrxf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hopnlmxw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vgxjstai.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzyuezid.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zrgorsqt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dovmrwmw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2eybcsmzc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2otcbapml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjskirpu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2akjqsipz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zeheyais.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gccndpqe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vsdnxtbw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xsuoinbm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nyhekddq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mnfbsthj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2auzcadgw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2eoboujym.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gtxvynxc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pkzmmqbi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sabpsrml.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2trqdoyem.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gpmzrdzb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttcmxuof.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkjzqxhp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yfnkkxut.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ywtzubjf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gbimhmig.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vtujuzes.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zptbvcyu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mbgjujyl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jbhicmsb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2letwegxc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dggzdznc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pvqsckal.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gzeqsvww.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lbnxmgea.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yjgkyuqf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjpldbdn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zcrlzmhs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dgqsvayz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vbnagndy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tmkvjxrz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzzktrin.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jlvlelju.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2spqoguje.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qcmmhxbw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hpecaseq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tbtgwvee.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdfkinde.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cbppafwy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sbpnbwsf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2avvwzdjr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hvxcatua.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qvafnsbs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2smmxoscv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vyoabapa.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rdzyhtyg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ybneamdg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tibqimog.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nstyimfj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2dtbschpf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cmsysvno.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mwhudxre.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vebybefa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uhffplog.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vuvodckm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ipqmhdbb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zkchjiwn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2figxxzft.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yvftwczj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lzlejgeh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tdcbtblc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhmiwazl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xnqznmyo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dwrfvhjo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jamiksuy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2eqldbgmy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rijrhztj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ezysaadb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cilxofnl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nixdbkrc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zkxfjeqv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2apywmmab.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pkolznzt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dpqdqjlt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hpzdxdlj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ohizxpjv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dssbldcp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2soeyvfqo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vlotjpkw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ujwtlito.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2anepllco.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rvpxbecc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jdvmqavk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nkmzbpfd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ptgcpqnf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vjzhuuyp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lrzdbesn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqwzfdpi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hienozjs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2staotigp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ineuefnb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hoaxlnlv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bfstebhv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bwlbjeod.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ocofymlr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2djugawwb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jbtdzxuh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mxqdptwn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kncnydwf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xatbzlrt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rtkbsiqw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pnixlzzm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pidkneks.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wpvqxwzs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lejtlgle.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bimuxvhc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2rksjxhyy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okikurxt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rcszigjq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2swezyixu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ilqqxvdp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uitmazuq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jazmeuzh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2efzwgruf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ezpwqpdd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xvlqthep.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2abystmpg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2optwofmf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdqxvmhq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bopjamrr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jyxiitcq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xcvunjpj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvxacldv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rdcjmctr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ltvftuah.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2owzximav.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fhwjfgeb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ypcyuhyz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ymbifoiw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mwvxfide.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hsnsrwof.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kevvhijq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iycqrzfk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zbtuuhho.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2unmwkqbg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mqvnxciw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2odmvyzsg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uccukpwl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2eaxanzcm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yrcqkbyz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nilankvg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2egmpngji.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wyzebgpm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mfgkpkua.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pgdrzzrf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qfxtbyoe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2aaskxdes.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uxxqcicz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tcsefmaa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2igyalnyw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wdaeeryl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ivyqpojd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hvmrkgcs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kmyuiral.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yloiyzgi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qjzcbnps.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gizvscap.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2eqlzorok.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2moojaede.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2axfuzqdu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gencelec.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2crslikzt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mwubodkh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mdfpwjye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtbromdr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tbaqjjzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfwcyjxn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jgbxgvfu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yuufwzku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uewiqcuk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pshxfrmn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kkyrdijk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jxohcmcz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dfnlipuw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ccvzaedz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qdedcbax.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dzivvxqh.html


<!-- 参考信息 -->