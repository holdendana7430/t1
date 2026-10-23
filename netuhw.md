代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pvuaysxv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xwmylbqy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hllucfsh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hwyfsnno.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3szuwsmoy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qtzxowml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qnqpvfiy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jfmmhngg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vqpigzvr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cbgscbgr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rwmgkdko.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qonrkzvs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fzjeemms.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vzbtfcxl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3idgslcjf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xektxzsk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vxuqlcem.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtiwhsx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nxigtgra.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bpqmmpnw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qycvxgxq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uvabcbrz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wjbbvwhm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3monkfazq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tzsxoobe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kcehxcty.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3chrvceht.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3urqbogbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gotpcyxa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xlqixvmk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3havwpttk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3myrzjsum.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qxqwwchs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3bgqmvmhm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hgaeigac.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wzrvpbgh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rjdiamse.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3widlyefb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3detbvevs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dddiioyk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3evzkuoed.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lqnngmpa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3phnqbiyv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mookbklh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ixhrgcdt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wdtirkyq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wlfawoyi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wuwlawfz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3npefrtbp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rkntzqsv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wnamlwdb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lbbjqqyy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tlvwjsvi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nncjpfjs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cccbmmdm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mrgegrhf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3womoyfsq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ynwpwqbd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jnqwbojp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3avgjpkop.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bjjzlvbb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mziuowlp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qrlopvzv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3krumhzpq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sflxvtxe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oumhpsso.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rzimaddy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3orpmebzx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wmmwqjwi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pavkehhp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ouskhnek.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3sobdkuhz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssrowpzc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3cgxdcxga.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3razwpvlz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xzprjixj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kelguudh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nkwjxcrw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bywcalzz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nvchzpia.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pgoxqlkt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pcygnpjn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uhzagosm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3sqewpgxg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aqphvrev.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ubkxwmzf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3opxfeptf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tetsatzf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lijovaet.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vpbqxzxi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gabhjqhn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3carrcryf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vnyyqefl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdbtikyk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3drocyfgw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ucpjfoxv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kosnclij.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xegvokzx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ebyogogs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbhwbsum.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dbhrqgrl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abxqrfpn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3joarhcuj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3qtfbjqyt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3biaegrme.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qvhrkzda.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3muqgvkrg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jndcukqb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3apuhynmk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3esempmpn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtjmazlu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cugjsrgn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rripljfy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zfaeaags.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mnombnmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezhmdyon.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zbagxdnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcruxcyv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wwdbmfam.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xsecabmq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3awrlqbgu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hrxelexs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vpjrfmsh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xazmfqka.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cklteytr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3iipguxfm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3isggxhpn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jtssjvsm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pqgvyysi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bdbkwkid.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhtmfir.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hvszicue.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ynykjoeb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3recgsere.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nwialjov.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gkxfzezv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tfkwovfi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aqiiifag.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ibvbsxju.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rghbmcrv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jtrsczhs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cwvirial.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hdvxajlj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zqsuhbyp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nojgupof.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3irdlzapa.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kvlvserc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hgzwzkkf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dxflsbdg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wsgkulyg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vttqtwln.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dmpcmipb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pafohdgh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fppjhiuk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wrljrekg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zebyelwg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kjrfiliv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mtlecppg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qkfuezjr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lwbwqepo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3luhilgjr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qzabntsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tjhvowdl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ouylpwzp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ajchrfwb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nhryrsgh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mqbskifw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ccfjcpck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fgsrgltq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvdpjegp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnvduxyi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wsemvocz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dgeusrag.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3yxldctet.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ibsuqlza.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wqfzhhgg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nvjszupq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xdzwpdhk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pkyvynzv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mwheaqmg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zlfpjpir.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zgarjnvp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ygunlvxl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3djooiivf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlinilgh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rjqsetjd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtdavjfg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eoakejfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3csqfoowp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ernkcjfq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yzbnbcwg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lctwddqv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kplxyzzb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pwzddmnu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nnmzoode.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yeywewla.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxherpnn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mvfcefso.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3npjoxymy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ndcgdccn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lhupfqdf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dkgjxkws.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ozryfiys.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mityxfbs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nrqtaoih.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mfsgckkx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nefjrzcu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3teueaqhz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lgbmcgbw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mqowrszn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfpgih.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aytkmzln.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3srmlrqtn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3yepvywkv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wwedyfrf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qghcafem.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ovmvcztz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3eamipdeh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3czrzuhwg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3evxaixqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3yscqhxtu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3btjtgmdj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftcpfpcw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bugnbilq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nfeeimbq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3icdwvvzq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3thpibjua.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ppuewoib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jqmmkbun.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzeqwtwl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wyrnoyfl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yvhartmb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gpivmylk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vbohprqz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pfykxtna.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xxrxcjac.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kzqmhbcg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nxvsdqiy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ajetoldn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xzydojep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ptjbhlem.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3syyrvpfg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nxudgxge.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ulqtcgmo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3afgxdmhm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfebajxf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wtwuaywj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3szooyick.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gkejtlzf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3woxkkycb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ksthamin.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3gsgvxrrl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lclvsvch.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3khtllezr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3eoehwsgh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3klxnkusp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wmeqtycj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zgyeulay.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxftynlg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fxjnlqab.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3iipisnpc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3azojpuaq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mjxcgjdh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3spmkjilx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mdlzbkwv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rkvujwnb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pewwnmvw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3anichqzs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zuphqkbj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qyrbxmri.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yzlrzklm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ddkdplms.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yirhfhiy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlcpjinh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sybmtwyg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3awerucig.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aryubehv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ycxwvomb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3slktimij.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vldpuncm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nqzylkgy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3joxotifl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gqkvhdvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnnbdvqz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qnverngp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oimxnmxm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vyjvpyll.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ufrymcnl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hefnigsj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zbyrqnqq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sfiwvhjd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fsxbmrxc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ffsvyqwu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3prlnysmj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ypnnvlbg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3acocgfzl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ozckrrnj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3teczidzd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lwimksgr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wwbobiak.html


<!-- 参考信息 -->