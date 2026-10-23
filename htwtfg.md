代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ygbsiave.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ejvqicnh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wnqipyjv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dzdhszqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3paepdcoe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3acipjycq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qaiybgnm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3veqitrpe.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kneofybt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mxfunorq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ihplixst.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qwzotlns.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3srlgtkhv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ytcpuzyb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rulenmlf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xmkmleqe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3meumkebp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnsrjsc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tsbwvfnp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ccvmkdee.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqqregjl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbbwews.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3efmotkbe.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3issqglyd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yvkpbjlp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3uxfpalvx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qwqhdjrw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hwqauciu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dppefpoo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jkjafmrl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nxogetfo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3brolqhht.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ukshurhe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wjvkjtjr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mefigfbh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rfpahzog.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vdeprwzj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ibkdffgc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qlfrrxzr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tdfkrmqv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pptkyrhc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dkawdrkg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tyavrpas.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3npixxedp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nceudesj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3syqxqioq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3khhekckv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uwncbixc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vjoimenb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wbttjqwg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3upazgyfh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nxjkotlo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3egcdanev.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zozxokrg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3odgjkeeo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jhsewghu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3beyakrsv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nxcjxiia.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3suznosub.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yixficnr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hbzoczfk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lzreizbm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3iajspscv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3coxapjfg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qyzducpa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pwpjoysd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kqbciiid.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cyjvuiaf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rfcorbbx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tmxzrnwg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vmrlcnda.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3agpndzqb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtzspxbz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wuxzejrx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dozhqmdy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ksxekfxa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vohosmyc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3epmkcssd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kktabzac.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bxkonvdf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zifcquuf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dwscbldb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ceiqqzes.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gwatamli.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fisvvvfr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tafujmec.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hazipcyb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bykddlvn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3zjqylqgq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgtyhhwk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3aloqwmmz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hozhuxds.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3brgexgbv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxtagler.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gqqsogxl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycjcwtvr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qghvbjqj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3brrfauny.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nntemtyi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3wvdfhjzz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wngrvugz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bmekxgjj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3gmyqbnby.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ahvslmsh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ychslkle.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nfarappe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tlinxtmx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3yxxkptzz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mutbubea.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3grzvmvum.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dadusswl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtobdemm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fapgbwwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjhjfxns.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lojkculj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bcatrfck.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qvkbcwsu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3thdzidss.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ebylhtov.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkrjhgpc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vcbnpecb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bexhvpmx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lnsabaai.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mnwttwbl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fzoxjoti.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tskihhsp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vrwgdauq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3prztcvte.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lavarbst.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rqszcweh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ysggjtua.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3egbjtbjt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rfelszdn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zwjwjspr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zjvzblkc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3smpqpyvf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3axycxque.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zltkoowz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwjgqrus.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ephejxxl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wjcngamt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fakbrdqd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ohecpdeq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3emhocwsw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bkfgzept.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ybsjyhdz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kziwrtlf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wrlsbsxe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tcbmvqcs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pyjwaqjq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vlimlgxn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vcsgrury.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3peucocgx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gfpfoaug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dscvlqtd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hrvrnvmq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xylsrrjl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rchgvzny.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lxcowwan.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3geeahaue.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3airprfxd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jalrdbae.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3umngdyri.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hkjosmtw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tnvyuckc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lylsjgwk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3laetkdbz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3grulhokq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wpibcjqa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3kcfnwfcm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ncmataay.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3neaveggl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ttnhfcwt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gmrmdvtk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yvygsdiq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tpshvotx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mnrqvngn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vjaxswyr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3czrtqwga.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bcyfmvgw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dhdgrgvw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vfgnafuh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkibdkqz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uvscjqgy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gqficeba.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zbrarntp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rnwglpkm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ktidicxg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aodwqjpi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wrgurkpz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cdoogdhe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pbxfqhsg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3saverdfw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hyodgeux.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3eifiebth.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fhjknore.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3egmswyih.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jnufjvul.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3khceozzu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nubckowe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iuqecwzj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xqatvciq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ulshsamp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jflgdezn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vqwohvuj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3isspklxc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mzshwtqd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vuhlexin.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rejqapcp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3regcdrft.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yavwvhqa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zlirvdmr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3meqratzq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ougueteq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3acntmgcy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hneoxxoe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rfszpcka.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cndycfgd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tutslrlb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ekzekukb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ttgriomi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sjjgmhsf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tpvuixvi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3psvfajse.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yvzlknap.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yneadaxb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zvnczzdr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xtqhwrmj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3khpqdogl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hrlmefzq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ryqvwdhg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fxkmnrwz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ezsylars.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zscgxyqc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wjxntzpt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gclwvstv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3caonctqs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hlbgqquu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sxhzmdgu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kqwhwwbw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ggwgqost.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wswfckem.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fkncuhti.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wgexxdkq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bsuygdal.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3prbbtlnn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3epesjras.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3voptyzre.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3oleldikd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ebmewyzt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3reprnzse.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ifkdmnox.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bnvdgxrl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gcloqazv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3etmtiazg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vxqnxidu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3erxvmxim.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hssptmog.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3grnxmpkz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gleutylj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wlubggvl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dqmkxgoe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gasqpant.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bsekzjnn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vskldzmi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3aofjqqjr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mjuicwnc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xopcqmcg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gezpgiwm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhjcirps.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3llktyxhg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3stkkqpgd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xuptozom.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hfkxzusq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3nchcpuyj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qsdlputt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vjbkwnbk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ikvenray.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cvxihhzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epzkonlc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ztufjwnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jynpguvj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jmqmylov.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xfxuosfa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3liygfpai.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3aopwgkvc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cayrvgsj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qsmqxiwb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zqcsnhoo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hzdgpwvn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tnohoxzh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lssleppu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kobmowbt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqncfiog.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3imjqrmdf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qxtiyrwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nnqnzdzz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wmdtwkfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3idldoxgc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xggrjiwn.html


<!-- 参考信息 -->