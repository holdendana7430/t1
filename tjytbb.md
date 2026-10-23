代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bjyhhfzm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ihakqzgo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kfjowqaw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sdnjsdwb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pxsjpmhi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3awhdjtsr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gocfdptq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ianbzxnb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3prijkvxq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3koyacmqb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3spckhyjj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vmfibgxt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yhahoskr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bndtxsrs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mvvqhqkh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mwpgtoaf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tccmxtsh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bqkhhpav.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xunotjjn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3raqwxgnj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kqcdsfzv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sqysyjgj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gdrnymyo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yhgrsimr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eecjylzf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rlfecnxq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vvehbytd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3czdwsvep.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kfarcent.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vauhyqjk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3viishbwq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3crqqcdkh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3moccxgkp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3stzyyyik.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wvgqcygw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rgsvnljw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ilhdwgrq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3igebuiku.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pfxmlnev.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rxbpcowk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btyrjuwg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3woxlucqh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dqvbguhq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jvtegxrq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hzgwpnjw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kcvzcsxy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ooiyzqik.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uzcsuczs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nflmcrvl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ryarakgs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qzakmccw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yrzjxpys.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jynfcnll.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bmkdzcvw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hjrhwueh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mdjjtytq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tfaeqrhl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ylltnzox.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3aapydmbo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3csweqpcv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fycjnmym.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yjebtmnr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sqofzjeh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qrdbiudj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lscbtkka.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3esrpvqpa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3apinqpar.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kqadfdok.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qcunsozq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3srobtadc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vwmxlbsa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3udnceuib.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3npnmbxkz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jbmbrlbi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3emwpaiuy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ndhilxui.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3whhccqnx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dxlnxjvx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rmzobgad.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3skmonsss.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bawqqqbp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vzkfnjbj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hwxiwsqi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ospfbpue.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kjrcfhfu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vtjmdrzj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zkichrcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wcjdczjo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wvwktuxl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xquggmhv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zxbylmws.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mswhttlv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ktpwgkka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkpkzjuh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iqceswme.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlukaehv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hnalbzyt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbdciuzx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bfdukcst.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zdmhzxeh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lvigfzkc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uxpzsucg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3svlrqojp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fdhalveu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ahbzaorv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yuqbrzmu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wgrjhddm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ftdfequq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vvibokng.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bgwxzzhn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vijpxnho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxceqxvw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bwhwjfep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgtpmccz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bsqesrfl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hcfqpdzz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vaduiyei.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yrifjejy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zoutjiwz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3igabxesm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3badlsdaa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jdekxfnh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pvlflndn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vjqtawmq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqyrkpes.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vozqfxys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dcdsdori.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kimwmhnl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rdlutrvp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wzmpiyhu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3phdtlpcv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtsabyqu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qmkxefej.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3sihrutmb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rabaaqad.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vghgtcty.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wnuhzelo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3curiiqfo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ueucueao.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3czyrlcyq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xkskkapi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nhmgzftw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iledznai.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dgblebsz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rpmvqtid.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dknrtxer.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcxbrikv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3emlomyhd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rorkigga.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nnytniij.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qroditjn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hsweqpqj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sstpicux.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ydvloexg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ygtbitvv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pvrxbkyd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tinwgeep.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zqyovupl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3orbhmboz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qwulafqi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iwejgnty.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dgrixcuk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qyvxiqdb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bgdkcxqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dodblrqd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bsiddyso.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ujiqcrel.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sxarhldl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3whwqxkgb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nzygltwa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lirskywo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qialsgea.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3potrrrli.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zfqfcbxx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lucmwiis.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3umnfdisn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nylrlzba.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yhogzepq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tsljpxwa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jtevtvti.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vuqweblz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ntrfzcai.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ekvckwey.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wspquktk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zelhrgiv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zzrzmufh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rnelphvg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zohyxvqg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bnibbusq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cdfjnlmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3anejdjqx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3uwmwxmil.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eobfwojh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3verdxkcr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mtnwbmzh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3auhblvec.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3okbgnzrp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bmokyovs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kyyikhuv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nsyzmser.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bhwemmlj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xjsbifeq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lfloieaz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdmglnsk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qkwhblxu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vuxcntrq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wnemgzbh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hjdzzoum.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fmxyahgx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nyaavdkp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3smilbtaz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fcaznbgh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yuhcjblr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qpsrzgmm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hwsffpso.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rinjfozw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wxrpziti.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lpeayety.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ydncvzwj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xcuucugc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pbeaweak.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gwtvuxlv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmvoldrd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lmqrcpab.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xwnwabwu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3btbghnry.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3gashuhuk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tzgxsojr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wsbhlwtn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3chlfjvxf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3csghudkl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3swaygxoh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bjlbayur.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ovmdtrze.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3prcbzasy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mdwgboou.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3glxefgru.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xhsrqdxd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cowcxvdt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3npemwixc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gtfpqlpu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3inijoqmr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mibvxtcm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kobndspf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mfkrdiwf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yiqkmvrc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vjcyxxuj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kvzgehkd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3akqrummk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bszjsngo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xvjlnfqr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tcnljblu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vhdhprrh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3quyttaio.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvgsebkt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cvwgdoax.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ypwhojzs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qeexqrpi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hoslesdv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bwlkouhk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zjvfgcht.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fxzinxfe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gvappdro.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yxbeywjj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mkbwvcay.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hyplrpdh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cbufmnpv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgoxhqjs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zxwupyxk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3grjmmqlo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vwgwoifv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lmxzgtox.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3enpyzbrj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eibeveop.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vszlerch.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zmbnyubg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mskcqpdl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3oqpwkfhk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bdgqnghz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xekgjcfr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ehscbxpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raqmcwhq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3epqpdiew.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3giihyuco.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ppziihel.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hoohwqbt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mfccdtmv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bitsmxwm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3khvxqfog.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bqwcardk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3habswgnc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yeyeiajr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fxibslkq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3suotabxs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3owrbkvuc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wtixpiko.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bpeyswso.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kiigurms.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jubxzjfa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lbwlnjal.html


<!-- 参考信息 -->