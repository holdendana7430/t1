代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3krwsxfba.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rsytnyry.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ycyxsvxe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mfblxgpd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ryoiwfad.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vszklpwh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zupseqvz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oufmlblx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cvkbxmbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uxivkseu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rvknyxtf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kbyreklj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mazdxnty.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3izzqfrmv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gqbikbgm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3noplwoir.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3aibcgzyo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vqwwnsgy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3enntfzno.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ofdylglp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ttunkprs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3chxpdhte.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ihyvzwok.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rhqczyhe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ovleambv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3farpucfa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rlachldb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fmhcjjqb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gyhgtnqv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dzjidhhz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3szbfsxdp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bqcrtllw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gunzteab.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3iohlozop.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nfgstpuy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qmkbaupe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kokliwdn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xeocbnmn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dlwudsyx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vqinkbne.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3buryyiqd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qdwneqjm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3maarrdwp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qunzoddr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3phuwqikb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jjdcoqxt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kcjwkqgq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3psvplwfc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wrgeceww.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sumnhyhh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3goqltkkh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gxqydjil.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xpmdxfhc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3udpcxcvs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rstqoobb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mipbqeyl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3iyxkxzlv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3enjmvofs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ipugldhq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3avnnulqk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yafifbhp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hccunwxx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3focujwzm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sqdhnuws.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bqphffbz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dwrwafwz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ledwcyrm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3aslrdyid.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pdrdrbrj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sqphztlq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3oefustkl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fejobmkl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjtyjyvv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lwzlfqct.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nfuyekgp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hoizdako.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hdnjchas.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kfjfxbmq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vjmjwycf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3olzweykr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nvagjmuj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tjsqjzem.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hzbhyqbg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3owdbsagu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pbndovuo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wazwvgox.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pcyzoily.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vccyorbq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pqhksxry.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brcbtlup.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rnueytau.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3binndwqm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zmbvdqri.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shsnzxoj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkupensw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmbcdycg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cziezyir.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iqhtpzvo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bfozzfyq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xacxxcbn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3deytojcx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kcdyjvvd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3orjhogsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3pdtcodon.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vtwhdqdh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kwnzskop.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xojmhqfr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lwcvxgyb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gknlwsht.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nsdjnnrd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dswfxkho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoqwxboh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sygvewdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heqhkeah.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xzjtsgdj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3twuqezvy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3asuxiwbb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qgpymtgc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hzrwbnst.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwdvxzrn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gjhjjhnp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yavkrqlq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3baltfupd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lphrffcl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3olyiclri.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3swiwwfuj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sjlztctc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3mjvxwici.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rxygtvft.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ozciqeap.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3beiutgmc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3boiviuup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cbukunbf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3enxlgvin.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3deydkwye.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpdkhs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3aywtbmxr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3egkxyaas.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yxipuild.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bqyatoel.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nhyeysnk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3szewankg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dkttjgev.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrbzcczg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vogqvius.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cuoaapxx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3povjecaf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nwdycpnq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zpmxklln.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aovcvojy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ijntxsyw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3adenfdhf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3drhnnazr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yoyxxwfa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mjptdqat.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3urhetspk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3msxlczch.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3spukcrlj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkacmbsh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3exqlkzao.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mtxytsez.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3luzopdjw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3icvpqpxq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rldklhgd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gvuazbtb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3txolhdbd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjlzjjui.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pftgpzci.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jwzcucqp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3optdoyaw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3akimmylf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3hmxllkbp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wxsbtwck.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kcmkryde.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gfsfnyba.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lwfjcbnq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxloahfr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qbdlcnev.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3czjnmpay.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3bbgynguy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rxuhnlzm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qtdyqrrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tftmdftc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yiyhxfmp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ngigqpav.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zmfnqjyv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3effpzphy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fcvagqqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zdiznbtr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rnmdzoqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tkwgrwax.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fcptzgxh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghqnjlbz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3anyqcyfv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3keeqmjid.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ivptuzrn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xnqfetoj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ssafgyhr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ctoopuak.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ymlkqwtt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ckylvrny.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zmxpzgna.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sruxcmqt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwlanozn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3spimjfzz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3duhdsttw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3abfihcje.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qaqzwgyg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iofhaydi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rdldmfqy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ocegewui.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pzghfeke.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbowiymy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3krrwlmaw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pgbizchc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nvvozuuc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lljxdbua.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hciotqvb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3megkyrwq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pyenilue.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3owcpttwh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rncefvpx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hwpwiirq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3knudarfz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yatkisrg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdngouns.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bzsixoac.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3douxxrex.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3bljxqxkx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bufbcfyv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rabyifoz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mbookwcd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kdsgfxxm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xrgtzqgb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sqcrdkwm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zaazcwyr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fwhqptbe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lsebkjco.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hjtcxzkt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hglivhdd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3togkobub.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwomwtfz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gurxqdvr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qolyculj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ilvrzzmd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gqycocal.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwqrxie.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cjxtfwai.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qimriklr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3knbspuya.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3iqwpeljr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fufplrae.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tllwgpvc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cqsbwvbx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbzcfsbh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fkyxflpc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ooiubzrx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3plsiqnis.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3yomlfdwr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3emiczucp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3obcmjmva.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nqgwfgzv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rkyhxftm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lbvqshpw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tqahukcq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zdupvsav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cudolieg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3reqhmtsh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kywmsahf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtsgzsbg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pemjmyst.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxklul.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xmolaqjp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3onoyuddk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dtvqxaue.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vtynfkwa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3eastcslj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wogswdqi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3liowvaxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plapesfz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nfcpknqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzflusdb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xzqkycda.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3tytfzwgo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykwlzvpo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nueasgls.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oslsilsg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mjykoxvx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3thumvpxv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sjwodbqu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rdcvnbml.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ripufvrd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tbqkljyt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3evftugxf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kvokwwsf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qbttsnaw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yyzcapyj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nbshihaj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gpapomdb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gnsbzadf.html


<!-- 参考信息 -->