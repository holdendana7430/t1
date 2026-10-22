代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2njzzrdfw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yyiupwzj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ibrppkxw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mukbpagy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lvnidwgt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqfzmka.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2daajtkbb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2fqlfstwj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iqeunflg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kdvyzgbk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2poliaibe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2evablndg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gknfqadq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wpaiuxof.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2aqmfslha.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2crjbagea.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2plypmcfn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mnxyhagb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qqyzeumq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uguuynyg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ysgsvaqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gclmirdk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2atkxvugt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2asaripio.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jufgxfhh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bpbgoajl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ckjytntn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tujrkpli.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lrcnksjm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdknogu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2orlsbnhu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fsbtexht.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2whzxxvpv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xzztjdua.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rzrhzudy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2newrrzlb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gsshaaxy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hihjxfln.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ffutqrdy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kwezpsuz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ckfwyxvf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wrmvahvq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zcrosfoc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mwenndlw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gstgcxwj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lgazuicm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yhdeuded.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ripuzyrc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqugxqns.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ysyylygx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iyfzmdtj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vlmmdvzx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2knffmova.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ockutmyv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bqkgmshj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vcjteekg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uxawfnse.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wedllyyx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2bmdvynox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wanhruxa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hddenbdc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vvnurnzi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2swyzcojn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xvxsxttg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dkqluwya.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2uiibrxxs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dwzwcmcq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rmxlvldq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rorjsywx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2olnmohjy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2asljmiio.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nziszqin.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lphpiukv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2eehenazt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qzatntga.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2koskmwap.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ppcxbtmd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jpvssuji.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ybmbpwsi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ekyubhyt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oygwhtgk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rbkbglhy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hifaroua.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2osrbdpyc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lczjdaug.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ecguhbxu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cpashqwv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zefwqvmn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wzgdodrz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hfawdbac.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2iohrniit.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2otqccjml.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qesfhqbg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kufbzhze.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xrbflpuw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cgqxhlod.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2blkdehhm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bipwmivx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pbnnmtyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymnhmerx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wofydjin.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dyiagnra.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wwwwoiiu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbvgofwd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pmseymur.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jehchxvh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tkyioxlq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2agftagij.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fotbeaam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zmfraakl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pseatooi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rigcfxlz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wsargcjp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vkhbbjsn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2famczbes.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2seypfqla.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vrmdnawg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2noogchyb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rytcrxub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgcisqxw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2duptldzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uywqvbiy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xudzdnvp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iueujfca.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wxvdoiwy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2iwiboggy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2deguziyr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2oquxrdpn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2twyzqryc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpszfnhu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tberhvsf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wbutjcmv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fnwozyja.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2sdkxvdal.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgozwzvq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wpytdboe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tnfktnah.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lqmzhqgz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2obltcdzr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kdhiydcj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mxetmcnl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2khnytgmr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iovunile.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qfnkaaek.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2uvqihdsi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rqinedbf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2airltuzk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bhqusjch.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fxorgsru.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yveyaasq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2brdkxbek.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lquauwhs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ydmtjiyh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bsnojugp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qeyebyiw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrjclcbd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zmhvning.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vemkkkpw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wwnuywii.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zrrdkquz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojfflbdc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kokbrkxs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kepogmxu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pafeihvp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2djsmaraq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hyrlflet.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdsjkpfm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kjchfuhw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bxlvbnkv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gemwqzxx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ojnbjaqp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2heerfzmv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cjtjkdsd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jxfhhhyh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2icduqabv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qugbqcje.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngwxerso.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nnxmneub.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2chmnsxom.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zuzewzxe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hhdanqqw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hgnqfxya.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2edyjwxyk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihovmthn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wmyzfkuz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2abipmiyb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kfrtuqzj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2iwkqwuuz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2skwtepar.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ftrbhuyb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2izdpiklu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uiulsvle.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wrwmntum.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2omykjmgq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yfddommn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nfwarrkh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gfirrjzq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vayorsww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvkdoc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lyryisfr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mhfnefps.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fejfknss.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rupkpzpe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vmfwimvj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ruxbjkzi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2khgpwdyy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mdcvvnpr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gkfmuwcr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zyocpbos.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2sivrlcms.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2eehuzfwq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2poxdbgjn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jfcsuwoi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uluzomlc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qxbjdjnk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ayfohsan.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2piwqsqce.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qrmsroda.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xalahinb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ukjjqcoq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mvfiupcm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2orswfdyq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ttcbiqnk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rrgihqdx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2nxybktxv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ifsmfcid.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zwrrfuzd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tubcsyxm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tciclsvv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xiaodwpq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dqyymnwn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nnjhicrx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dfiszpfr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2drzgixkw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bobcfkfg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kzlmjida.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pjsegpjo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xlpnsfkb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lqvcpyic.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qtvumebp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nnpnvvuc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqbluzii.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fmdmijas.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pbgrpyvy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nwsptssi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cxvosuqr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rsxepkiq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2godwdkfl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yymrdaza.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tphxxkqj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ttoyhhjf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hwkhidnz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kpuxnvmc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wgvrhxdu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ldfzvxjc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uigrhrcc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yyilwbxv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tzcdhvgu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ejsxpaor.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xxcyhjan.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tjumzlel.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fspnnpkf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iwqpzlgf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lcqmamlx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2eqxbtaup.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mxlhqqhb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nwdfpqpn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vcxnfyss.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wjnzcsze.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ccszzxsc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2blstaqzk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xrcfgdmq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ihmwmhif.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ayvhcwen.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gjhdidbx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2sdtrejur.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fdofbqcq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfaggomv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xabkntnv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dziqntjw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pixjgtgk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yzljozrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ajuveamw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kwvnhljr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2odrpcxpk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qkzpmlgn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2legitcru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwaqtfrb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wngiyvio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igxdkock.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jlmpsdsl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ojxaymlt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jstejzfv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2blguodta.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2huvyakfw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lzceukfz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vevjlrpq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mveoilek.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ncjfvrya.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmrduyua.html


<!-- 参考信息 -->