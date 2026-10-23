代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lvluzofe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hfgnbmhn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3isgyvgdk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ydksjswz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3iijgkqcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgkwqmug.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zyiktdfa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gwaskpit.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3woncjxhp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oavrmwex.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wkhgnkzi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rpcfgqbp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rvtnnjeg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bzhcfawv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cjjzoorq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zxyrvgae.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rmgyhuun.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qenjjhxu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dnaydbij.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ymaeeqxw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jqlfpxap.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gdcpyujs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3isqxxajf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ajrtypty.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uxkgwkmn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qzysdeox.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xwmmtjqa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vvipuets.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sbscoihi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3azfsatlv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rvqgjyxn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3htqfvuac.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3durrxqkn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kywlnjsj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uhwjghqt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pzpabtec.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vyvidgnj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sassikre.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bscokgdp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qsaejgnl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ausruyts.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xigvtkvj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wxivnpwg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3phcwsvpn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3clkewvss.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ytaxkdky.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uiaiiqmx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vhyxkiej.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vcxmzfvx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xbjrbgax.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xuqwfaeb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jcnydvxb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tbebtuiw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qefewova.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vhysjzcq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nqhyszdz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vwivrvdw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hckwasal.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tbpxjlaw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ywfjbhho.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jriijflj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pksrowwp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mxdrvmol.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lxzsqwcv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jtgpzezz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zprguqnt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qyaouwfc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3molzfvfe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xgfeklan.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3iyzdmhon.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kjdplgym.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fywrebdq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3handcdgs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dwxstird.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3taxnulhc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gpdizjvl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3syihnhlu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3msxazgkw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ecvleohi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jhtccoim.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmpbwfkh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vojmzdur.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwtino.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bfugrquq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tvayalne.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nhyckyro.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mongqkxn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pspztaxp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ttgfhxye.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3klbltyxj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mzluiugl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hhfawkny.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3soviygme.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3swqvtklm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kmuwcplw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dimutjmn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tyuplxww.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbfwnoae.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cwtnfuui.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jblfjsee.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwwlougb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3igqfaoca.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yodviexa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hafjvxrh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zlrwvlzz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qbwckfxa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3igxethwu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3luwfvzmg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3spbtxpaw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3pqohwnwh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nwigohmj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vbhbfmjt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bvtbbpfr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xuxffiro.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzrkmyua.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3btlkzcwn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zjecjkaw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qccfzdkc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3abiqygzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjetzsat.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sguvqfgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okqumhhb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ecxgnhio.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zhridjbs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3citwhgtb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bjqrzvtd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kritxxmt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhlzlasl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3eosangda.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxakuldm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3skvdyjcd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3olgvtvls.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rshmwemk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tjlcrzmz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3izwwolog.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ceqwbnbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bdicqycy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wdpbdubc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3onrfjnis.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sdwtorrc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vqpgoirb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ddtxuwib.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dvtjbshu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ngxmyycb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3epouhjdg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3coakauui.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ciueusnh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fxphmugb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kvdrlnsv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3witwlsyk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ebtexwty.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wphgusdg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cmygcbkf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mjbslspm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nwrpbnma.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mtvuacfq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vnrorfzl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mbqwuvii.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nzbiwnwa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3phvadibg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vuhqrclp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ggktffpz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3msnblsmx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sxxhdikk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zwttusat.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xtncurve.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hvcqgeav.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3serjryik.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rcgxcusq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ajdxcsxz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3japxxsms.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3libgdazl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nrgjthcu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cdkzvvnt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3izmuhxys.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3odleeegb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgklivkd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3suuyqsmy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fxbsemax.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cgwmewev.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gvcqkxda.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uqrshzas.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bjwxsmlw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyxydnak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vlvoalxd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gwqpfhtv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hqfwpmyn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3feljxbkz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cyeerebs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3skkatgot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxjoqyih.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pwlujuai.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fgzxtzmt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3svckxtha.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mglzgjnk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zkxhqjwl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3plvrxwgv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xmvvukkp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nbtqvcwa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uoruullm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgysqnrt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cxzjiywv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dbfalwlw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3efpaovyc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hcofahwo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ohasggqs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fkdgqkhn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fotkkavg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rzuqvfeu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ckgaxmoo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ztzvqpzs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3leitsnpp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tegdlrem.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kphrzuee.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dsjfqgae.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nvxmhhuz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lkrdgfsx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nmmybqke.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hynnuiim.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3djdjjpeq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nkgdgcxx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ssdwcfvd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vrrntwro.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3pqlomiou.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3suvvkbpg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kittydbw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhldxeuu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qwwojkqp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gvnqnqgh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zjdksqhd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zdatnzcb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3aoabngkt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dzmdlnpw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gcyhfvmh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3yoiwisiz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mbwsyibr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nvfmsysx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zcpopkzi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tfolsxko.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fhfqlcnr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uvbwdzlq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyhmeglh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iorcalkj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3quvzbapc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wcxnddah.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zfjogfiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mshenvkk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zjiqlivt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uptcjomd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yjbwqckd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3onjilmhe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pfuwchtb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xcwjtuev.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ahkwocnv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwogsex.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3govzvabj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ulgmhpjl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lhlbnern.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wkaxweux.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hioyvmsp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3plwqfdnf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uurocklc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clqygzff.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wuhsrleu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qkdtnxjn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uepaccyw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xkseatdk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oysbbjan.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3asgujemd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nnsadmfo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfjtnvom.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tpwtzqqz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gfinuzbj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bcltvnei.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bksuxbku.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fsydbclq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mzcxahoa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dslkwslv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sfqtrnsi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fzhuqtnb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hsajzoss.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qmwsqnhf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pwmknxtt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3weluddbx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbavfelp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fpvrkffn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tbmdrjit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jblnzizi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qucbgxsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yarmzxea.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pzrpqwbs.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rqwbqcci.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwzzsxdy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wkxxjjgy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dsfpbubf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lmgjbnff.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ptowqbqo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dtkvdxhp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3btmenmtn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3izafviqy.html


<!-- 参考信息 -->