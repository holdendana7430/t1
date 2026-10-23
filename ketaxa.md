代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3prpupccy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3snkruhga.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3snxwwynt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xilcbprw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zyrvrehv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kofviffv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pajgtbic.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lgqdchqy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gxdbwbma.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jltifkux.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3leripoqi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uwaytjdv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tnkbkjbh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tabrcsap.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3izplrpyx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3upvubmpd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jsmjhadj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gylxrtpx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3whsxjhad.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vknmyilz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lenbmpgk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3sjcohxda.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xrmgaxmj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3aflnorpk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3klbhxrsn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3thnlutsu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nhcfbhtw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pdwfcoyu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xkucrmoc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3znhechuh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3txsexvbx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ulrjvjno.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ooafklnd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bdtowfap.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ujkunwbt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zlpjfdov.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pugqhron.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yqrghfyw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ugvvwcjo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qneejlvs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fnvtrksm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dwmmpshd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wqvwimft.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tieprnax.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vowqqtea.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tdzyaqwd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fbegrcws.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3moixdubx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tkdtlopo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3akaecsyh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ysypbzkm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mpoiovie.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3srxepuip.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yyihiosd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nfobifne.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wpudgoew.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rlrjfzxm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zonpikwg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dkazqlxc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wyjvbnnb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ciyeldie.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3uutkypxx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fumzmusp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nhbpnxrb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hxdlzkvc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3egbogwww.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xwkziplz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3diwpofry.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rwfrbspf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ujyznpzj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nnxsozyr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ykwuwltt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tsyvfkaa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dftsuuam.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lbrjmiik.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3puujcobn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hgapting.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3agfwbnep.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3iielgknr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3lnaxjnlx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wtgwkeyg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xnxarzhx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qxwdsney.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ykjwpgug.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gtpdtziu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vpqonaru.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kqyhstzh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wyeufptj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3npdcphvc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kdhmverl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hievypcq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bzdsprwm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjvqdajk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fxqdtkhh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ghuharur.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hhnpndtr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qtyrvhtm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvzysgse.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nkijelaj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kfpzbbqj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cqbrfsxj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qbwptqsg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3utylwnjv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vymhoflx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uugftuti.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mosypqrk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xdinuzpg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jaldglfi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3onkkhtzj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnvlgplx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ltnanvoe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bljwwuxd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mddayygy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyxoervb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gwhsucvx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gaqwgupu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gyfuluyz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtfvgpye.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ncnudwlc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rfuffvlg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hpnrjacx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dwolorux.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vyvzvfsl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pqegrbzp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3amljxjdu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vubreuxb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3elesbqyc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3iaqzppjy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oltajpxk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hutgcuqk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kyeweixw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luhxszic.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iufdoswe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbyfwfiu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jijcdmhg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kvvvaave.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fmvlgqtm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yzmsdgxe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hanvhmyf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vrwtyyrh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mekwagxx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3heiwrsvs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3agpstacv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ckuikiqw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfvdfniu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vvpymixx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bgxfimuf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tehjlgib.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3efdgfhij.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bqeefban.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fudffsfn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tnoeruuc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iluyfhne.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mycmlcoj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cjlguiby.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cvnkxxti.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ysttqvhx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fubtecnt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3avbnrdmb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bdtanhod.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vfssrhri.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3okrgcobk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ivbpmawv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sccmnyoo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jpifeunj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xwywrcrw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aqxatltz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lgkhunyc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xtlixfgg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qgmawkxy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3evntblxd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rabfyolh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3lfpibdrn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xumdmxwl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3efvmsdco.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qxmtfjnf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rlajhlmq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ywtzntip.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fvrswmoz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wkmygayk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3amooseek.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jqyqtzqv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujtimlas.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iaurnnkp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3updnkfwr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iszgxzdz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jnodiwvt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fgksxcpt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3otwxfgyz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3patpmjvl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tiuooord.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fhcywzsq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kbwjndvo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pxbaveus.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vpjzwcwt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rubyscky.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dbhnqwkk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dlgswysf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lbmbkaul.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uovzfire.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tsjwsdzt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yerhxtci.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3exxmiudb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jbbcmpsh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ciyihwes.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fkzcvioe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3grmcuqeb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ouwsdwzj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ryfjdkdm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3laicfbfh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3liyryoqe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvlhahuf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3euimxjwk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3beoatwfl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wxnepvtw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ynkedkwo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xewpulgn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cyarvswd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uchpksim.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zgtmlivz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bswwrqgn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3acewjazc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fygxvjqh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ksflhazh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oskiorwj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yqclepxf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vwcqowuw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fareqfzd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tepinaku.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bwhoyfro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gjjgmcui.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3asrgtqqg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3epeckgbl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ocggcjlm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3maitrsrp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mnpszffu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rvfvaiwu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rmnoknvc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbmltgvh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ppgnveyz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zaxqsggt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qvvjyqpw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rdpbjoxf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rqjrqjym.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3oiveiprb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3csyjwfce.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ljllqlji.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vekcxyjq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3eapbylwt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jdocgvxr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ehmcrvty.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sjhnhwgn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3sgoshwck.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbizloeb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sddwhrlv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rgsrlafp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3pgsyxyob.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3babwujfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mwliaaep.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pdqxpeua.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lhbzmdco.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tfzskmek.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hqwmpqyn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xzdqfjmv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rqgjpdbq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3fvzgvrwz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rthwxexb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hlyurdze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lvszkleg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aujbglsp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ewdcpdsm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3epnaydhr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hitlcuvt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yfnhxnyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jprtnpdh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tvbaokfk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nkaqxpdq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3travggeb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tcqcqsah.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekdmjjnj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fcmaqjdx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3slnhxaok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zetqczfc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mjcncety.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yzubetjb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3msmcvmew.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxzabmsn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3trvnzzrp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3forexkwa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3utshmyvn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3armjyjyf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kxikdhnr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wnkmipve.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xonopnmr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mugyeoyr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vfnhtrvy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mjjyddyn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3iylhzcbo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3filxsdgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghxyvorm.html


<!-- 参考信息 -->