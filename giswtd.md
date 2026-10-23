代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3avhwslkj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nhitcxqy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vrnkdtpd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dsivxvqu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3umqmqbgd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ogilqtub.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xovjtvaz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3hanextcd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3amwzpsbp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3effzjcwy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3emkxpvin.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rnxdzewv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3keugecjm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hghgesha.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3obnjvspt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zxwkznut.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3eehwliel.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nyojgkfz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3aqkiqkaa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zncgedpc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3spuqwfsv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3guwgcati.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rnqmrzca.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3abcbjbzk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ahayxubs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xpgqpuxa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aczutahq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vfoewhmq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bsspjrsy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mmihvlip.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kdyhakze.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3eifpaivq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gbxpzkzd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ughbagnt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3swmipnih.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dhjycblc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ruczaaau.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gkbdxjny.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zyqpgqdd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dxkyfkoq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3svdlamny.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3oyigfysc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3oucdidis.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wwmlxqxn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vbrvlitr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gkshfwun.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jrxobjyt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ujigusuh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtqzufqb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ixhayygg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ysoxvvyv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sltmnznb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3czcoqnoq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3refinhxi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pironytp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jhmqjvid.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3sjmgqttk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rtspheap.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qgqzombq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xlhlwyrz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mevlccdi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3oqyljzex.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3frdulejg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3estfihyd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cdqddwlq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pgciaerj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3obtzmnxh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wjgojcxb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hbnfzqni.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zhbawrgy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ufqyguyn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zueyyjvy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3yacdcsyt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3mqflezyp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3srzjgrsd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vedwpkjg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxzyztrr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vohukoxe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mqyxfoov.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kpfefnrp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ftabyhqf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lflruyli.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hqdjzcyt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rwpnuzbj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wuaqtici.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ketbrfen.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bxyxassn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3iyfvriqj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3byeflady.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3komtvftl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vhamdcoe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vebvfjqz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3alyhelqd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sltrbwqe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kutyghby.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zhimlida.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3svcxtwga.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3huxanwac.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rkveprpj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hppiyden.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3uswupqfd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vdwnbqup.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3difxdvvy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flwuglsk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tdjobsvv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcritfav.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3czaxzumb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lumcxesp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3djrjamlh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vgloapbc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3aiqhgsep.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lihsxiil.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3khteoavl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ibzsjqls.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sgycmzaa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gjuckosw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3puoshgvz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3bicihylp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bcdtkozc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfvfvchp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pprixvii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pscmgsti.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vtbemiav.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zrxwinjx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tegpkbcg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mpumjzye.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zougmofx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mtqjlpfz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vgpdpblz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zobdaxku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jltagfwv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dpjjqnam.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qsazkrwu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mjqkjorr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3khpurwkr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jumptpiv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3shynvauc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mcayyger.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rrzqbysd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tfexzsmy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3unluuaif.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xlgoptdy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3axotetlb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dpwxxcqk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dcaubteu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kwhrozkg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nmtbmpdk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qkxirymr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hjbleboh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3iznajwsu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dhqonbbl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3porgnfpj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jtyckpia.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hauxpwlh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hshabqak.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jupfgtiv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cebvzqxn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3icglvilo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gubiaxvy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qpykhsnk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nthyqxmp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yuupepyf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zlotvhnf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3egsdfcfm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlkjalam.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eywutjnm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cjqhqpzk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iqkrqsuf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zjzvaasm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vysdhzer.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3llokqoca.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3grgnvuce.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rvnttsqu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3taalhzjq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jdarojzn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3purfllau.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3smyzoioc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qklnufsp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hiytkmzq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3oywwchnr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jkxqessb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3paawutiw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ejogvxzp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqykmoma.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qmmltpcs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jwltfvwr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vwwvsiju.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nsaomsyi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hucyofgz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3byjbptpg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kclmhxya.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3azasfhhq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fbilejva.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tksjbqhp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zwhagaws.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vrmedauc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ikfpacqb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oxmircxp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cjzmajnt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fabakgfo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3oywcewlv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wojjpbiq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jeskkgak.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3svhrqgvh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hbmulgww.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3subguwck.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bumtpywe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3utsvvmzn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3otdwfuqg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rzdbsaje.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ikdiness.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nuomqnyk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ammddotv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3blyxaqxj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fjjyalvz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ogdmwihj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iowljqah.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3joriibni.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yzvfreos.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pqtulwqn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xumsagyz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dcjeyuun.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3asfxifdp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3krfxffeh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3axdakqqw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3leaqnbbw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qbudsnvb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rudlllou.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qcgmwngx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kyceojkd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3otwzepgc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3unbksrqm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lozmxmxb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kxfipcuu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kqpcffua.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pmvwkcoj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fnuxwxpa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wlqkxpgn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3koglwnyv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bwllpran.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iwyrexgi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yksutivd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zbmigekk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jealdwzx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lanlxnzd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ilvukdse.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yujzbdom.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fudorzfn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lhnsnvlv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nmjhszbx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fltxqjew.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3poeohift.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3epwsbnza.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3woqnbpyp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3yxruemmg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sifmowsy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qzttguvn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dzbavntk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ishqqvrj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3opmyzkww.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dwaodwmn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3owaiqqwo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qxrbesbb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3slsxzhrv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3guwjnsmx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hhtrjnpw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3buwlftlr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zctzyjnz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tylvqugb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wkocfewq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bmhypgcw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ftjxsmno.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3djbtemzr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lvfhsljl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tionqrjd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eemykszw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3buqprnkk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cautyvxo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3njfzsbmi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qgmfxrih.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3aizvhxdk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tneeczio.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lsvexclj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ybpivqan.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vnzqiyjp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ppkjdfnu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dqtgqzmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwelveyc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kreksgef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnxeozll.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dbmbxzjs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yiccuzlx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kobhkqnw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vmfgnjpm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3slvqdfgc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gepcozdf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zjaasiky.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3poniqsqe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qpsydzgl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nkshmvwi.html


<!-- 参考信息 -->