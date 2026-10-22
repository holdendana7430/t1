代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rolhtzix.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2sgtkrosq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2npselfvj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2suogtcsy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mechbcea.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fttjqaoz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2evgnohqx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bhopgvte.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kkabprbr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hwlyhbbh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qtquyapa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2czaeuyiv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hbmihlff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dbggipwe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2esytyikt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xlopicil.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xecakbfo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vtmateld.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbwoxilj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2omefjzjk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pnwgiebq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2azxhopms.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2imidmaeq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rzwhmhgn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nrzqvjxz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vhnjjlkv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bsxmvdck.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tfaznpwe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2esjveosr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vgiqcvef.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xrupoojq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2muzutubt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mocafnib.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nficwmwm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqzhwey.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fgprbjql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yxtyslat.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ehdxcdxe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rqcumgzl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2txpwfsfi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2slmjhswt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vbxebzkv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gehgtcpw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hfyrjmig.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sbuuiiam.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2suqmnuue.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qttfmjwi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jelgfskk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2apwnyfid.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fvqtmcrz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lpksgftq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yxkhmncm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2huzdclqj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wcachahj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ucsecymw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ndicylge.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wdrgzcny.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zcpeokvu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zdmdbxxe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hvpqqloo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2uwgcajvb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2flzppeqg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sglpxvns.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pjsmehis.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2viqmrusn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bbxlhpps.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vznrfldy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wxhdwibp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufqaiysb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2flcpdqps.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rzvucwxx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2enrgxtoo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nlzxmniw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2icvziaak.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mefdvdpu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lndgnclr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fxaxwplh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fpeglvmy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dgqxlsqt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2brqfbfdt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ihfigyzr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ukhmzufg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nrzkblub.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zrwowlis.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hfuhwbzd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2xyugzmhn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ulypjgpz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2uafefuyj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mhzqibje.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yyqwcdfs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fjoxntqm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vohokxir.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qrfcanrj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2riooftgv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2twscohzr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xtwcqfga.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2dyhvgbai.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xyqkejlo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ufwzrlhl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hguauehd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xzobwbvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2szzxpurm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2padqedyi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ptqxiwbe.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eyeqrcmo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2eudciqmh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iizqgval.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2edirtazu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mctbiklp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xaklmcus.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2awbofgvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vilglgbr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ywyvupbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbkarrrj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2crjsnlnl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pdugufuz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2blasuuga.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dyoyrahy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hsmtneau.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zarykesb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zjaivzkp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2daknpbhb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fpnknnvd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gqqunayd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2moyjxehf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uddovovs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhwkwnxk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkutvcno.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bsaalsgs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lgeukbus.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ecthjeeh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynnedppp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2thfezqpo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yteqkful.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ggzshipw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vqxcbnyv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fpeasvmt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mjumxyth.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2exutesif.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gmrdpyeu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2iboupvhi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cjvcuksm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2apeyyoyd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cyxkbhsi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jztowyxu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uuspvbqn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqmtpugi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2scxleeam.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2aqbemlct.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wobevrcn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tqmcvwsg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nqxcbeqf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qprqjogl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ggwjvjtj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzfasoft.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rwmrnvyg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eugrqwaf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yhsxtolt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cgzenjxh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2thdsoccc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wkuxloqz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yhdnfgsa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ieicusao.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kmbkibum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2atkcmnqk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xjviuetu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qkgkfkbe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qpuvyryf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kzkpauaq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2uzmkwwio.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yhoxwrez.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cemciuzn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lmpdifvk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2azkzripr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ykrwjcsb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ceemvcqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2egjrqzci.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2slizajhs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sxttbkpv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2quiapflg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pdhmbirh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gifdhffc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnnpapek.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ijbwclfs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hhvkuodu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xvyyppco.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2urvsdnfv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2llofjgqb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pldtkwzc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2gkqxkjwe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gbguajxk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hgedvnld.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdzwvphj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vpkpobei.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2buapipgs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yffoaanc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gfesjwru.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lynbtryy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hcgxggss.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hxmauwhc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nyknndwp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qdklunue.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pfnlmnky.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qresfibl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xvvgppwm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cvdntadg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sizjzflt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bfjruomh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pmrwnfgf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fzefyfpe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fcgxnlwf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2infzyoqk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wkyiolyw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iusxvjbu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ayepgcbn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qxnzcopk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2egpodiek.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yratirre.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cfxxxzwc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gnvhpbek.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vonfiuyy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2asdxaebh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ktoyyevq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mbmkxzxn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fyyxlsdn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2awulcvcc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ybrchalf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cueanxoi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cgxlqvpe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vbplnnpd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hcjrdzyk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ubnsypdp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2resihdat.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2anleiyls.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jbnfmcdq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dfkbgeba.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bqjpkatk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ghblulqy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xgtrdech.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2codogdvu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kdxfnsah.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pueilvjw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aiulvxde.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gsfxiozv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2oxhsonth.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kazzxuha.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tyiiujdw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uusmmufh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hjtvzswg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2citgjmou.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2asdtkkoe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2znbtblnm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gwmlxbmq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2edzkgool.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ohqfvyav.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cjdgcezs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2urksabnk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pjyrscqp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bimlbrez.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fevkwozi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xljukhuu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2knhwbytp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cxuexble.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ywbbfhej.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tfpcronn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2slsylgaw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2arswysfg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vnvkmteh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mvacdmvq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2unkvkzhy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fqaakobr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2utoqxizi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rqvpjbbx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cscugltd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ffprkdby.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xcotneey.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2czcerpsy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ouqpbklb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2byxndpmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdiappqx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ojghuhnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gziqetln.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ivprcbbu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2czcfzoib.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yhppxeuq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lcxnsyrl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pkfxfprv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xjlhearw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2klmnjvuf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zvuxztus.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pwlfouoe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2znihuqnj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2igjhjxmv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2stnqpgav.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2slnitpnr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zgbbqija.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jyeoloxr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qplgimtw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wmnssqmq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ymbqnfup.html


<!-- 参考信息 -->