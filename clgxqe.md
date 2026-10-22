代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fdiadync.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rynitwdq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kpuhbrcz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cggdxfnu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2erzjxcvo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vnsginkm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2aeehgijq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2iwnrcoyh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wxiuqqxk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nkqrcytb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hreyslcb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lwvkgdpf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iymzvozc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ygnzrnmy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dlsvyftu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qqpkmhwc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vsiozfmh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qxnaoxfc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2piwowxuw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lobxivye.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kufjpvin.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ckaynoym.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ilegtidn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ptkrpmvv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dtwzxiqf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rxqlidgb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oalcewrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pdfvnebm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zxqismsr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjihdu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tvivoulw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yykhyqrg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2trpbpylz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sksawwno.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bcydgtjd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xakvrsya.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xctgvfrx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2utwmcgci.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lsdganmb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kgmphlgn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sllivhrh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ztvnljhv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zzbuzpxw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pvendoll.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tkvvufit.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2imoulzjn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uypyfuch.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cjhgtxft.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2quzblchs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xxiykete.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hujlyhzj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jpjsiksy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jpcrwxgu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2agvhlwks.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wysrjnuo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pnhxefal.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uuvmcqje.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2safhyxjt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qylgkagd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lsmceoeg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zvqkifww.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ezajytog.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bddqpcia.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2itjxzrmt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jhnbdbky.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pnfnhoiz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zuafaaqp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2usbmwenh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zqzfbqvl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nftalxws.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eujwxeyo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fkzzckfz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jablukbp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vhvyrxhf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kaykzvqr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dtoporag.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntrcakoc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2aatrxlxo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pbtxdxnc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yxjvjkht.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sifbmbkg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cmxuocgx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nkgycpyn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fvjpzhhx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yetpwvne.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vusbospt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgtlkukj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dermzlep.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2krlmuljo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2juiaoqrx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rqfdjwag.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2duqbyppq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tmsitibj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fydwgiwx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fejcseqm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2shnooejb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vjwietap.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gppgqivg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dsrigmid.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2donlednq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qcuigoad.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrvvnepl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2npnpyjfo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdtqvasi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fndzajiq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmhvhroh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cylynwjd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wesvlydt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hljjupml.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2piflwhwp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yxholibd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2sdqsnxwq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xfvgwtao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2npxgppia.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvpimvex.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lpodcdsb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2foacvjsv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wglhxdmj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ymhfocfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izbdobhw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wtqohcpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgkkylsd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kjbygjia.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ssrggqsj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cyjtarxr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2esjsmlao.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zvnkpvsl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmhlkcvw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hkhkdzhx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ejuhrjod.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ijvgfobi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2obkfxvzq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dagmopwm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2edflxubq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dmfnxmjf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lcbyfrsv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jkxubajb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kgjahiuv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qisztkry.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cjqathqi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2utowgtnl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tlkejbly.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mogwjfkn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wgcdrzjl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pynbhoae.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vbptrznm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gixtlgdl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zdeqrfkr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jdczdass.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fbdpdvfo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bkokcfmy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tgztxqqz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vwgzkpew.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mzvtcbvt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzvqzjlo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mvbzkydq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qjwqjmxi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rhodvbea.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2darvmndh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pfnqwqia.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2redptttn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tjzmzaym.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtugtkwm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vdyzychw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2chclsskw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hzpjpzju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gwxzbthp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2evfjpjzg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2atgdvnxu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cukcnnct.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xfimcymq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sxodmstq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2frdrmorl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jyjxmpxz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mokuujim.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jujjthin.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2apaggchc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qpdrboyo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nlzlvezi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xxqtaamp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jnsspexh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tvzawgvm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2smldbbyb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlghzbvt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xowjqume.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2agjxohor.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pgyzqgbl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2sspisnog.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxdyfpix.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nefsywiw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vkmrkmoj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ezmznvkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mbxihart.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2avjvhdst.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fhwmpufc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xvlwhzol.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2obanjqpz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2nprbiaso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sltdznam.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xpznxfgz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gfmcgwfb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mgxrutzh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jrokecbz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gytqstuq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ddenckhj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ktxfgrsr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tasvfjlp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mdrhcoeu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wvmqyvmv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rtppqskw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ruitnxje.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sxsgoxfk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2szodhfok.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2facuegvj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ludfvmjd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2iutlpmku.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cdowfccj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jzjlyhgy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2oyiflyst.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fushjope.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfdmbt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vkhivjxo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nxgmkvie.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hrxnmste.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nqyuezgd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jkuepjrp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ggcenhfj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vtfgkmax.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2biwbbopc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2oygpscdh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uearfztz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tumokqpq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zturivcq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zhkzncxt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bnsjvila.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rwvxhhml.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ampnzenh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cesfptdd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2otaewlnu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wsgttloq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nbkqinal.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtrwsxkp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2algumadt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qckumwhf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2iegjmyft.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jdrvnfoq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ueituuir.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xkwnfala.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vmjyeixj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpcglazf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2daqqykzd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mtbajyzu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kdzphtkv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pteqhgzj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2spwwlewa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zrjdfvzf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nndffgey.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xldyowmh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2egkiwmhf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2txrnykwm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dsrrphyl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2styvfyqm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqvbrpjl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vmdpquvr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2akvqfqzj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hhuxzglc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2eegzpxcm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eedeytws.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2oiofterc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2binjtmvt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kysbpkvp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2djmsqatg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2viunpyye.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ptcfpnnc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xervspqc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vzkwnegi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nbrbdqre.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zgtvguqe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hceuzqah.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wnkvobpt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2glzaajxn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zkzdqpke.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zhzcguji.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nycoqdtv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrkftckf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2djlrvmwh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2prankmcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttikubpo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hnhlxace.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxdctlur.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pgbepvpo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2psqbyopk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rpzqgjvz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2piqiscwd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jjcexrqr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tppczgbb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ytuxjwlk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lttztqjn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qtsltvro.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fptjpibk.html


<!-- 参考信息 -->