代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hzfbmeul.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zbflsxch.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gsrcoxab.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3evtdrmmk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lrfogdng.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oqmhaxgo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zpdrpxfp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3udhzyojd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rxrafhho.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bspihmxv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3oxtzujrm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yyaywoej.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qfjcqbtw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ysnwzekn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lpvvgfyf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tkkeorpb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wefcrrmt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3amadghbe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wvspofna.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3akqxmior.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yrnlyvla.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fexsoejo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zofgdeos.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uukekfga.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3eibgkylp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nistweul.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pwwpbghk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vnwqtlkm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3azcfsbvd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iouabnvg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3irygkpdh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iyoregbj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cyevnjhq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fzgjqqbs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dqdndiix.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dhjmeber.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fqjonavx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3llhpymsn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jiwsvuwq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3egmrsdfb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ufovatbt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pofpplfr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tmgjxpme.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3aovyqjsp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ygqbzyag.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkhqnb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gcpykmew.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3frokdmps.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hpbwimxb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3cchrlmif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pnkfgkwx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yswcfvvt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkxuxdxf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yzptdbus.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nkdmgyzn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qdvtbhxb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3emqvndkq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3iuxkjohz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zyptcjry.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nazbvpig.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dtjrovsk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zbluvobq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ohdobqvw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3myxgzfoq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ceitpqax.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bviorfxt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qvusiiuz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yhnadbpr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3takxdpau.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xbhxufrs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3utwepkfp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dfngpuxk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dldcrsiq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ghehkuao.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kfyorguh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mgwpcfgx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ctwjofud.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vcagywmr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mazzlyml.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jbnqjejr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3thxwlcyh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3azqeuezz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3igduuuou.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zcljkcko.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pyvwyozi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3snyzwkes.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xkybuekj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fyuhffzc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3dhhalzmi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dtjrfzla.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iqnnlubb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pneiurfw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3huhkaxjb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3yocujasi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fbvgrjvh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3huzpxirz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tvmdjubv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ehbmkwad.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fzzwkaou.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ubuyvafh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vsbfwvfq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zizqdfkv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ajxaoqmb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pvhdiuey.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lrztyudv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3snhonlsn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ramvdmaj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsngmxev.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3txopbhdv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dpdfjzcp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3swazcmsg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nzctxkpb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jybamewu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ynskjvlc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rsowlxal.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hhyvchpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kapxtlms.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jythpjqs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtxxvkjh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3notjwxtc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pfddiwjr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3exscuvbm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tyfwlgwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuygehbk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cpezxkmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzntpitk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jcotdsjc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pubbonpa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uciihgps.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zpylqgxy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3leebnqto.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nukhazgi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3suhrtirn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3azllkage.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ejzzoxuz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pwpxrawg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tlpcqxym.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tzaruhks.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmagdoid.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pajemqpy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3amprbulx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ksulbasz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3drutknys.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gfcyboeu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3onpnpgiw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gcbjcjhn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xjwsukds.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hdeurbcc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qjjrzfyg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bajrvvdh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3brqavyvz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3knpftwnr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qkdxdbzv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3eoiwafsl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kxksucqe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nhddlnsg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ypftmpir.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3obmbukcy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gfhvkiyn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhvemsmc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mxbuuckd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rblbqtfg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dsjnuies.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wnlxuavg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zoqglwkr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qitavdki.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyzscoii.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jycjimbo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wtbrldsb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vhoxtame.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xtdodyly.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvqtqqno.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pmixrvuc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fvntedyz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pyzetrvn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ewzalbzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rnipujfr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3azzogwmt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3czieozts.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3uxxqyyva.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bncqeszs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pfhhrapg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ggtibygj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ncyfpwfs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mexpqezi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xaqmohev.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fwksbllf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3neaqabto.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mgybknvo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wcsvxpje.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ybzmvblh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3begdygri.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gikqocim.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tdlzfrof.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iyukxroc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3snzsgxgf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fiolqvxq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3etuklgiq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cxyspuft.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vzenkebv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3llgthutr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tvvpmptp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3oxfpzpqo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jzokpesf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ozlxmlxl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hzzjbzdx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3urjcygtg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3akdjglgj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dtdyawvb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3akmcqwqm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ccnucokt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ftqusmme.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pfrknmar.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fjnsqkmk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hvfwzbpg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrqqyshy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3etvwatkt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pscimwrr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3yzbepuba.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ikelhvia.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pfkcmifd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3afjscpvw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3twvdlsyc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fjokrtvt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hgbdeclm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nxmewwdp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxmhveer.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wrfgtezf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mzuqpeno.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tuauzhfo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njjeienq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3szpymvwa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pqnpowxf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yghmkzde.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fofexhyl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3eqquutyf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wcxufvua.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xduhohje.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njfvetoj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ucdgimby.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jblwraed.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xbofvxzd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xdnqtgnf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zjvhmhgw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fglkbfuq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mkkiiaij.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vzfcphat.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cjayxtkx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cfuijied.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qaxeoswa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3reukirow.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wczquxwr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lxgcmxnx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zmpkhxcf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3opmxbbvf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mjdkhthf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kfeqlnil.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rpxapycb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmmnshb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qkutdcnx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3eaqjlvgd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hmsrtzej.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ozvjxzqn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yosfcmuv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vgnpgeou.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3atfbswip.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ubpdeikv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mlwicmuf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3voadreaj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rwkerudp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qmxkuwxs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ewsfmpyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wkifpgxa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rfiqcdrm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3teobmtao.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cwfrapoz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3owvsfhsb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ynuxshcn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oydtnkki.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3znorznwj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bwfphrav.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xakxrgzf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bscwetfy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xhunkuwj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3swfpcgxm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qvpokafh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jfohkvaz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oroznktq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mzauuqui.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3beiyrmll.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pemqjosl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzxdkugx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tpuqtetd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcgulqba.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dskmmimr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3demnrjpj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3atjjmfzl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3muszbntx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3beaiysgx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dvytziyq.html


<!-- 参考信息 -->